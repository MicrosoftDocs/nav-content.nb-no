---
title: Designdetaljer - Avstemming med konti i Finans
description: "Dette emnet beskriver avstemming mot Finans når du bokfører lagertransaksjoner, for eksempel følgesedler, produksjonsavgang eller nedjusteringer."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, reconciliation, general ledger, inventory
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: e962cdb35e9267f4b320073c018256153463d492
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-reconciliation-with-the-general-ledger"></a>Designdetaljer: Avstemming med konti i Finans
Når du bokfører lagertransaksjoner, for eksempel følgesedler, produksjonsavgang eller nedjusteringer, registreres endringene i antall og verdi på lageret i henholdsvis varepostene og verdipostene. Det neste trinnet i denne fremgangsmåten er å bokføre lagerverdier i lagerkontiene i Finans.  

Det er to måter å avstemme lagerposten med Finans på:  

* Manuelt, ved å kjøre kjørselen **Bokfør lagerkost i Finans**.  
* Automatisk, hver gang du bokfører en lagertransaksjon.  

## <a name="post-inventory-cost-to-gl-batch-job"></a>Kjørselen Bokfør lagerkost i Finans  
Når du kjører kjørselen **Bokfør lagerkost i Finans**, opprettes finansposter basert på verdiposter. Du kan summere finansposter for hver verdipost eller opprette finansposter for hver kombinasjon av bokføringsdato, lokasjonskode, lagerbokføringsgruppe, firmabokføringsgruppe og varebokføringsgruppe.  

Bokføringsdatoene for finanspostene settes til bokføringsdatoen for den tilsvarende verdiposten, unntatt når verdiposten er i en lukket regnskapsperiode. I slike tilfeller blir verdiposten hoppet over, og du må endre i finansoppsettet eller brukeroppsett for å aktivere bokføring i datointervallet.  

Når du kjører kjørselen **Bokfør lagerkost i Finans**, får du kanskje feil på grunn av manglende oppsett eller inkompatibelt dimensjonsoppsett. Hvis det oppstår feil i dimensjonsoppsettet, overstyrer kjørselen disse feilene og bruker dimensjonene til verdiposten. Når det gjelder andre feil, bokfører ikke kjørselen verdipostene, og det vises en oversikt over dem på slutten av rapporten i en del med overskriften **Poster som er hoppet over**. Hvis du vil bokføre disse postene, må du først rette feilene. Hvis du vil ha en oversikt over feil før du kjører den satsvise jobben, kan du kjøre rapporten **Bokfør lagerkost i Finans - test**. Denne rapporten viser en oversikt over alle feilene som oppstår under en kontrollbokføring. Du kan rette feilene og deretter kjøre kjørselen for lagerkost uten å hoppe over noen poster.  

## <a name="automatic-cost-posting"></a>Automatisk kostbokføring  
Du kan konfigurere kostbokføring i finans slik at den kjører automatisk når du bokfører en lagertransaksjon, ved å merke av for **Automatisk kostbokføring** i **Lageroppsett**-vinduet. Bokføringsdatoen for finansposten er den samme som bokføringsdatoen for vareposten.  

## <a name="account-types"></a>Kontotyper  
Under avstemming bokføres lagerverdier i lagerkontoen i balansen. Den samme beløpet, men med motsatt fortegn, bokføres på den aktuelle motkontoen. Motkontoen er vanligvis en resultatregnskapskonto. Når du imidlertid bokfører direktekostnader knyttet til forbruk eller avgang, er motkontoen en balansekonto. Typen varepost og verdipost fastsetter hvilken finanskonto det skal bokføres i.  

Posttypen angir hvilken finanskonto det skal bokføres i. Dette fastsettes enten av fortegnet til antallet i vareposten eller det verdisatte antallet i vareposten siden antallene alltid har samme fortegn. En salgspost med et positivt antall beskriver for eksempel en lagerreduksjon forårsaket av et salg, og en salgspost med et negativt antall beskriver en lagerøkning forårsaket av en ordreretur.  

### <a name="example"></a>Eksempel  
Følgende eksempel viser en sykkelkjede som produseres fra ledd som kjøpes. Dette eksemplet viser hvordan de ulike finanskontotypene brukes i et typisk scenario.  

Det er merket av for **Bokf. av forventet kost i Finans** i **Lageroppsett**-vinduet, og følgende oppsett er definert.  

Tabellen nedenfor viser hvordan leddet er definert på varekortet.  

|Oppsettfelt|Verdi|  
|-----------------|-----------|  
|**Lagermetode**|Standard|  
|**Kostpris (standard)**|NOK 1,00|  
|**Sats for indirekte kostnader**|NOK 0,02|  

Tabellen nedenfor viser hvordan kjeden er definert på varekortet.  

|Oppsettfelt|Verdi|  
|-----------------|-----------|  
|**Lagermetode**|Standard|  
|**Kostpris (standard)**|NOK 150,00|  
|**Sats for indirekte kostnader**|NOK 25,00|  

Tabellen nedenfor viser hvordan arbeidssenteret er definert på arbeidssenterkortet.  

|Oppsettfelt|Verdi|  
|-----------------|-----------|  
|**Direkte enhetskost**|NOK 2,00|  
|**Indirekte kostprosent**|10|  

##### <a name="scenario"></a>Scenario  
1. Brukeren kjøper 150 ledd og bokfører bestillingen som mottatt. (Kjøp)  
2. Brukeren bokfører bestillingen som fakturert. Dermed opprettes et beløp for indirekte kostnader på NOK 3,00 som skal tildeles, og et avviksbeløp på NOK 18,00. (Kjøp)  

    1. De midlertidige kontiene fjernes. (Kjøp)  
    2. Den direkte kostnaden bokføres. (Kjøp)  
    3. Den indirekte kosten beregnes og bokføres. (Kjøp)  
    4. Kjøpsavviket beregnes og bokføres (bare for standardkostnadsvarer). (Kjøp)  
3. Brukeren selger én kjede og bokfører ordren som levert. (Salg)  
4. Brukeren bokfører ordren som fakturert. (Salg)  

    1. De midlertidige kontiene fjernes. (Salg)  
    2. Solgte varers kost (VAREFORBRUK) blir bokført. (Salg)  

        ![Resultater av salgsbokføring til Finanskonti](media/design_details_inventory_costing_3_gl_posting_sales.png "design_details_inventory_costing_3_GL_posting_sales")  
5. Brukeren bokfører forbruk av 150 ledd, som er antallet ledd som brukes til å produsere én kjede. (Forbruk, Materiale)  

    ![Resultater av materialbokføring til Finanskonti](media/design_details_inventory_costing_3_gl_posting_material.png "design_details_inventory_costing_3_GL_posting_material")  
6. Arbeidssenteret brukte 60 minutter på å produsere kjeden. Brukeren bokfører konverteringskostnaden. (Forbruk, Kapasitet)  

    1. De direkte kostnadene bokføres. (Forbruk, Kapasitet)  
    2. De indirekte kostnadene beregnes og bokføres. (Forbruk, Kapasitet)  

        ![Resultater av kapasitetsbokføring til Finanskonti](media/design_details_inventory_costing_3_gl_posting_capacity.png "design_details_inventory_costing_3_GL_posting_capacity")  
7. Brukeren bokfører den forventede kostnaden for én kjede. (Avgang)  
8. Brukeren fullfører produksjonsordren og kjører kjørselen **Juster kostverdi - vareposter**. (Avgang)  

    1. De midlertidige kontiene fjernes. (Avgang)  
    2. Den direkte kostnaden overføres fra VIA-kontoen til lagerkontoen. (Avgang)  
    3. Den indirekte kosten (indirekte kostnader) overføres fra kontoen for indirekte kost til lagerkontoen. (Avgang)  
    4. Dette resulterer i et avviksbeløp på NOK 157,00. Avvik beregnes bare for varer med standard kostpris. (Avgang)  

        ![Resultater av avgangsbokføring til Finanskonti](media/design_details_inventory_costing_3_gl_posting_output.png "design_details_inventory_costing_3_GL_posting_output")  

        > [!NOTE]  
        >  For enkelhets skyld vises bare én avvikskonto. Det finnes i virkeligheten fem forskjellige kontoer:  
        >   
        >  * Materialavvik  
        >  * Kapasitetsavvik  
        >  * Avvik for indirekte kapasitetskost  
        >  * Underleveranseavvik  
        >  * Avvik i indirekte produksjonskostnader  

9. Brukeren revaluerer kjeden fra NOK 150,00 til NOK 140,00. (Justering/revaluering/avrunding/overføring)  

    ![Resultater av justeringsbokføring til Finanskonti](media/design_details_inventory_costing_3_gl_posting_adjustment.png "design_details_inventory_costing_3_GL_posting_adjustment")  

Hvis du vil ha mer informasjon om relasjonen mellom kontotyper og ulike typer verdier, kan du se [Designdetaljer: Konti i Finans](design-details-accounts-in-the-general-ledger.md).  

## <a name="see-also"></a>Se også  
[Designdetaljer: Kostberegning for beholdning](design-details-inventory-costing.md)   
[Designdetaljer: Bokføre forventet kost](design-details-expected-cost-posting.md)   
[Designdetaljer: Kostjustering](design-details-cost-adjustment.md)
[Administrere lagerkostnader](finance-manage-inventory-costs.md)  
[Finans](finance.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

