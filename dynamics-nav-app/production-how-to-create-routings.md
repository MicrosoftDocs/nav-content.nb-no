---
title: Opprette ruter
description: "En rute inneholder hoveddata som gjenspeiler prosesskravene for en gitt produsert vare. Når en produksjonsordre opprettes for denne varen, styrer varens rute planleggingen av operasjoner som vist i vinduet **Prod.ordrerute** under produksjonsordren."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 49cce1f32f1d66dc17c0d9758937541ef1baaae7
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-routings"></a>Opprette ruter
Produksjonsselskaper bruker ruter til å visualisere og dirigere produksjonsprosessen.

Ruten danner grunnlaget for prosessplanlegging, kapasitetsplaner, planlage tildelinger av materialbehov og diverse produksjonsdokumenter.  

Som for produksjonsstykklister tilordnes rutene til den ferdige produksjonsvaren. En rute inneholder hoveddata som gjenspeiler prosesskravene for en gitt produsert vare. Når en produksjonsordre opprettes for denne varen, styrer varens rute planleggingen av operasjoner som vist i vinduet **Prod.ordrerute** under produksjonsordren.  

Før du kan definere en rute, må følgende være på plass:  

- Varekort er opprettet for overordnede varer som inngår i produksjonen. Hvis du vil ha mer informasjon, kan du se [Registrere nye varer](inventory-how-register-new-items.md).
- Produksjonsressurser er definert. Hvis du vil ha mer informasjon, kan du se [Konfigurere arbeidssentre og produksjonsressurser](production-how-to-set-up-work-and-machine-centers.md).

## <a name="to-create-a-routing"></a>Slik oppretter du en rute  
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Ruter**, og velg deretter den relaterte koblingen.  
2.  Velg handlingen **Ny**.  
3. Fyll ut feltene etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  Velg **Seriell** i **Type**-feltet for å beregne produksjonsruten i henhold til verdien i **Operasjonsnr.**-feltet .   
    Velg **Parallell** for å beregne operasjonene i henhold til verdien i feltet **Neste operasjonsnr.** .  
5.  Hvis du vil kunne redigere ruten, setter du **Status**-feltet til **Ny** eller **Under utvikling**. Hvis du vil aktivere den, setter du **Status**-feltet til **Sertifisert**.  

    Fortsett med å fylle ut rutelinjene.
6.  I feltet **Operasjonsnr.** registrerer du nummeret for den første operasjonen, for eksempel  **10**.  
7.  Angi hvilken ressurstype som brukes, i **Type**-feltet, for eksempel **Arbeidssenter**.  
8.  I **Nr.** -feltet velger du ressursen som skal brukes, eller skriv den inn i feltet.  
9.  I feltet **Rutekoblingskode** registrerer du en kode for å koble komponenten til en bestemt operasjon. Hvis du vil ha mer informasjon, kan du se delen "Slik oppretter du rutekoblinger".
10.  I feltene **Operasjonstid** og **Oppstillingstid** registrerer du tiden det tar å utføre operasjonen.  

    > [!NOTE]  
    >  Oppstillingstiden beregnes per produksjonsordre, mens operasjonstiden beregnes per produserte vare.  

11.  Angi hvor mange enheter av den valgte ressursen skal brukes til å utføre operasjonen, i feltet **Samtidige kapasiteter**. To personer som for eksempel er tildelt til én pakkeoperasjon, halverer operasjonstiden.  
12.  Fortsett med å fylle ut linjer for alle operasjonene som kreves for å produsere den aktuelle varen.  
13.  Hvis du vil kopiere linjer fra en eksisterende rute, velger du **Kopier rute** for å velge eksisterende linjer.  
14. Godkjenn ruten.  
15. Nå kan du knytte den nye ruten til kortet for den aktuelle produksjonsvaren ved å fylle ut feltet **Rutenr.** Hvis du vil ha mer informasjon, kan du se [Registrere nye varer](inventory-how-register-new-items.md).  

> [!NOTE]  
>  Husk også å beregne varens standardkost fra **Vare**-kortet: Velg **Produksjon**, velg **Beregn standardkost**, og velg deretter **Alle nivåer**.  

## <a name="to-create-routing-links"></a>Slik oppretter du rutekoblinger
Du kan opprette rutekoblinger til å koble komponenter til bestemte operasjoner for å kunne beholde forbindelsen selv om produksjonsstykklisten eller ruten endres. Det blir også enklere med trekk av komponenter i siste liten, nærmere bestemt når den spesifikke koblingsoperasjonen starter, og ikke når hele produksjonsordren frigis. Hvis du vil ha mer informasjon, kan du se [Lagertrekke komponenter i henhold til operasjonsavgang](production-how-to-flush-components-according-to-operation-output.md).  

En annen viktig fordel er at koblede komponenter og operasjoner vises i en logisk prosesstruktur når du bruker **Produksjonskladd**-vinduet til bokføring av avgang og forbruk.  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Ruter**, og velg deretter den relaterte koblingen.  
2.  Åpne ruten som inneholder operasjonene du vil koble.  

    Kontroller at rutestatus er **Under utvikling**.  

3.  På den aktuelle rutelinjen, i **Rutekoblingskode**-feltet, velger du en kode.  
4.  Legg deretter til forskjellige rutekoblingskoder i andre operasjoner i ruten, hvis det er relevant.  

    > [!NOTE]  
    >  Du bør ikke bruke samme rutekoblingskode i forskjellige operasjoner i en rute fordi du kan komme til å koble en komponent til to forskjellige operasjoner ved en feil, slik at den blir brukt to ganger.  
    >   
    >  Det kan være hensiktsmessig å navngi rutekoblingskoden etter operasjonen for å sikre at rutekoblingen er operasjonsspesifikk.

5.  Sett rutestatusen til **Sertifisert**.  

    Rutekoblingskoder tilordnes nå til operasjoner. Deretter må du opprette den faktiske koblingen ved å tilordne de samme kodene til bestemte komponenter i den aktuelle produksjonsstykklisten.  

6.  Åpne **produksjonsstykklisten** som inneholder komponentene du vil koble til operasjonene ovenfor. Hvis du vil ha mer informasjon, kan du se [Opprette produksjonsstykklister](production-how-to-create-production-boms.md).
7.  Kontroller at stykklistestatus er **Under utvikling**.  
8.  På den aktuelle produksjonsstykklistelinjen, i **Rutekoblingskode**-feltet, velger du koden du nettopp har tilordnet til den aktuelle operasjonen.  
9. Legg deretter til rutekoblingskoder i andre komponenter i henhold til de unike operasjonene de brukes i.  
10. Sett statusen for produksjonsstykklisten til **Sertifisert**.  

    > [!NOTE]  
    >  Hvis du vil aktivere rutekoblingene for en eksisterende produksjonsordre, må du først fornye produksjonsordren. Hvis du vil ha mer informasjon, kan du se [Opprette produksjonsordrer](production-how-to-create-production-orders.md).  

De valgte komponentene kobles nå til de valgte operasjonene når du oppretter eller fornyer produksjonsordren ved hjelp av den aktuelle produksjonsstykklisten og ruten. Dette vises i vinduet **Prod.ordrekomponenter** under produksjonsordren, og her kan du også fjerne og legge til de definerte rutekoblingskodene når som helst.

## <a name="to-assign-personnel-tools-and-quality-measures-to-routing-operations"></a>Slik tilordner du personellet, verktøyene og kvalitetsmålene til ruteoperasjoner.
Hvis du trenger personell med kvalifikasjoner, spesialkunnskap eller spesiell godkjenning for en operasjon, kan du tilordne dette personellet til operasjonen. Du kan dessuten tilordne verktøy og kvalitetskrav til operasjonen. Denne fremgangsmåten beskriver hvordan du tilordner personell. Fremgangsmåten er de samme som for andre typer informasjon om operasjoner.

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Ruter**, og velg deretter den relaterte koblingen.  
2.  Åpne den aktuelle ruten.  
3.  På hurtigfanen **Linjer** velger du linjen du vil behandle, og velg deretter **Personell**.  
4.  Fyll ut feltene i **Rutepersonell**-vinduet.  
5.  Velg **OK**-knappen for å avslutte vinduet. De angitte verdiene kopieres og tilordnes operasjonen.    

## <a name="to-create-a-new-versions-of-a-routing"></a>Slik oppretter du en ny versjon av en rute  
Med versjonsprinsippet kan du håndtere flere versjoner av en rute. Strukturen i ruteversjonen tilsvarer strukturen i ruten som består av ruteversjonshodet og ruteversjonslinjene. Hovedforskjellen defineres av startdatoen.  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Ruter**, og velg deretter den relaterte koblingen.  
2.  Velg ruten som skal kopieres, og velg deretter **Versjoner**-handlingen.  
3. I vinduet **Ruteversjoner** velger du handlingen **Ny**.
4. Fyll ut feltene etter behov.
5.  I feltet **Versjonskode** angir du versjonens unike identifikasjon. Alle kombinasjoner av tall og bokstaver er tillatt.  

    Den nye versjonen får automatisk statusen **Ny**.  
6.  Hvis du vil opprette operasjonslinjene, velger du den første tomme linjen, og deretter fyller du ut feltet **Operasjonsnr.** i henhold til rekkefølgen på operasjonene.

    Operasjonslinjene sorteres i stigende rekkefølge etter operasjonsnummer. Vi anbefaler at du velger passende trinnbredde slik at du kan gjøre endringer senere. Feltet **Neste operasjonsnr.** refererer til den etterfølgende operasjonen. Nummeret på operasjonen kan angis direkte.

7. Når ruteversjonen er fullført, kan du angi **Status**-feltet til **Sertifisert**.

Tidsgyldigheten for versjonen angis i feltet **Startdato**.  

## <a name="see-also"></a>Se også  
[Opprette produksjonsstykklister](production-how-to-create-production-boms.md)  
[Definere produksjon](production-configure-production-processes.md)  
[Produksjon](production-manage-manufacturing.md)    
[Planlegging](production-planning.md)   
[Lager](inventory-manage-inventory.md)  
[Innkjøp](purchasing-manage-purchasing.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

