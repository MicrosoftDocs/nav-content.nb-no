---
title: Gjennomgang - Mottak og plassering i grunnleggende lageroppsett
description: "I [!INCLUDE[d365fin](includes/d365fin_md.md)] kan de inngående prosessene for mottak og plassering utføres på fire måter ved hjelp av forskjellige funksjoner avhengig av kompleksitetsnivået til lageret."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 0a540f5813ed67ee62e43390d6d11b7c3a137f13
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="walkthrough-receiving-and-putting-away-in-basic-warehouse-configurations"></a>Gjennomgang: Mottak og plassering i grunnleggende lageroppsett
I [!INCLUDE[d365fin](includes/d365fin_md.md)] kan de inngående prosessene for mottak og plassering utføres på fire måter ved hjelp av forskjellige funksjoner avhengig av kompleksitetsnivået til lageret.  

|Prinsipp|Inngående prosess|Hyller|Mottak|Plassering|Kompleksitetsnivå (se [Designdetaljer: Lageroppsett](design-details-warehouse-setup.md))|  
|------------|---------------------|----------|--------------|----------------|--------------------------------------------------------------------------------------------------------------------|  
|A|Bokføre mottak og plassering fra ordrelinjen|X|||2|  
|B|Bokføre mottak og plassering fra et lagerplasseringsdokument|||X|3|  
|L|Bokføre mottak og plassering fra et lagermottaksdokument||X||4/5/6|  
|D|Bokføre mottak fra et lagermottaksdokument og bokføre plassering fra et lagerplasseringsdokument||X|X|4/5/6|  

Hvis du vil ha mer informasjon, kan du se [Designdetaljer: Inngående lagerflyt](design-details-inbound-warehouse-flow.md).  

Følgende gjennomgangen demonstrerer metoden B i forrige tabell.  

## <a name="about-this-walkthrough"></a>Denne gjennomgangen  
I genkle lageroppsett hvor lokasjonen er definert til å kreve plasseringsbehandling, men ikke mottaksbehandling, bruker du vinduet **Lagerplassering** til å registrere og bokføre plasserings- og mottaksopplysninger for de inngående kildedokumentene. Det inngående kildedokument kan være en bestilling, en ordreretur, en inngående overføringsordre eller en produksjonsordre med avgang som er klar til plassering.

> [!NOTE]
> Selv om innstillingene kalles **Plukk nødv.** og **Plassering nødv.**, kan du bokføre mottak og leveringer direkte fra kildedokumenter for firma på lokasjoner der du velger disse avmerkingsboksene.  

Denne gjennomgangen viser følgende oppgaver.  

-   Definere SØLV-plassering for lagerplasseringer.  
-   Definere SØLV-plassering for hyllehåndtering.  
-   Definere en standardhylle for varen LS-81. (LS-75 er allerede er satt opp i CRONUS.)  
-   Opprette en bestilling for leverandør 10000 for 40 høyttalere.  
-   Verifiserer at plasseringshyllene er forhåndsinnstilt i oppsettet.  
-   Frigir bestillingen for lagerhåndtering.  
-   Opprette en lagerplassering basert på et frigitt kildedokument.  
-   Verifiserer at plasseringshyllene er arvet fra bestillingen.  
-   Registrerer lagerflyttingen til lageret og bokfører samtidig mottaket for kildebestillingen.  

## <a name="roles"></a>Roller  
Denne gjennomgangen viser oppgaver som utføres av følgende brukerroller:  

-   Lagerleder  
-   Innkjøper  
-   Lagermedarbeider  

## <a name="prerequisites"></a>Forutsetninger  
For å fullføre denne gjennomgangen må du gjøre følgende:  

-   Installere CRONUS Norge AS.  
-   Gjør deg til lageransatt på lokasjonen SØLV ved å følge disse trinnene:  

    1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Lageransatte**, og velg deretter den relaterte koblingen.  
    2.  Velg feltet **Bruker-ID**, og velg din egen brukerkonto i **Brukere**-vinduet.  
    3.  Skriv inn SØLV i feltet **Lokasjonskode**.  
    4.  Velg **Standard**- feltet.  

## <a name="story"></a>Hovedscenario  
Ellen, lagerlederen hos CRONUS International Ltd., oppretter en bestilling for 10 enheter av varen LS-75 og 30 enheter av varen LS-81 fra leverandør 10000 som skal leveres til SILVER-lageret. Når leveringen ankommer til lageret, plasserer lagermedarbeideren John varene i standardhyller definert for varene. Når John bokfører plasseringen, bokføres varene som mottatt på lageret og tilgjengelig for salg eller andre behov.  

## <a name="setting-up-the-location"></a>Definere plassering  
 Oppsettet av vinduet **Lokasjonskort** definerer selskapets lagerflyter.  

### <a name="to-set-up-the-location"></a>Slik definerer du lokasjonen:  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Lokasjoner**, og velg deretter den relaterte koblingen.  
2.  Åpne lokasjonskortet SØLV.  
3.  Merk av for **Plassering nødv.**.  

    Fortsett med å sette opp en standardhylle for de to varenumrene for å kontrollere hvor de er plassert.  

4.  Velg handlingen **Hyller**.  
5.  Merk den første raden, hylle S-01-0001, og velg **Innhold**.  

    Legg merke til at i **Hylleinnhold**-vinduet er varen LS-75 allerede definert som innhold i hyllen S-01-0001.  

6.  Velg handlingen **Ny**.  
7.  Velg feltene **Fast** og **Standard**.  
8.  Angi LS-81 i feltet **Varenr.**.  

## <a name="creating-the-purchase-order"></a>Opprette bestillingen  
Bestillinger er den vanligste typen inngående kildedokument.  

### <a name="to-create-the-purchase-order"></a>Slik oppretter du bestillingen:  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bestillinger**, og velg deretter den relaterte koblingen.  
2.  Velg handlingen **Ny**.  
3.  Opprett en bestilling for leverandør 10000 på arbeidsdatoen (23. januar) med følgende bestillingslinjer.  

    |Vare|Lokasjonskode|Hyllekode|Antall|  
    |----------|-------------------|--------------|--------------|  
    |LS_75|SØLV|S-01-0001|10|  
    |LS-81|SØLV|S-01-0001|30|  

    > [!NOTE]  
    >  Hyllekoden angis automatisk i samsvar med oppsettet du utførte i delen Definere plassering.  

    Fortsett med å varsle lageret om at bestillingen er klar for håndtering av lageret når leveringen ankommer.  

4.  Velg handlingen **Frigi**.  

    Leveringen av høyttalere fra leverandør 10000 er ankommet på SØLV-lageret, og John fortsetter med å plassere dem.  

## <a name="receiving-and-putting-the-items-away"></a>Mottak og plassering av varer  
I vinduet **Lagerplassering** kan du håndtere alle inngående lageraktiviteter for et bestemt kildedokument, for eksempel en bestilling.  

### <a name="to-receive-and-put-the-items-away"></a>Slik mottar og plasserer du varene:  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Lagerplasseringer**, og velg deretter den relaterte koblingen.  
2.  Velg handlingen **Ny**.  
3.  Velg feltet **Kildedokument**, og velg deretter **Bestilling**.  
4.  Velg feltet **Kildenr.**, velg linjen for kjøp fra leverandør 10000, og velg deretter **OK**-knappen.  

    På fanebladet **Handlinger** i gruppen **Funksjoner** velger du eventuelt **Hent kildedokument**, og deretter velger du bestillingen.  

5.  Velg handlingen **Autoutfyll ant som skal håndt**.  

    Du kan også skrive inn 10 og 30 i de to lagerplasseringslinjene i feltet **Ant. som skal håndt.**.  

6.  Velg **Bokfør**-handlingen, velg **Motta og fakturer**, og velg deretter **OK**-knappen.  

    40 høyttalere er nå registrert som plassert i hyllen S-01-0001, og det opprettes en positiv varepost som gjenspeiler det bokførte kjøpsmottaket.  

## <a name="see-also"></a>Se også  
 [Plassere varer med lagerplasseringer](warehouse-how-to-put-items-away-with-inventory-put-aways.md)   
 [Opprette grunnleggende lagre med operasjonsområder](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md)   
 [Flytte komponenter til et operasjonsområde i enkle lageroppsett](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)   
 [Plukke for produksjon eller montering](warehouse-how-to-pick-for-production.md)   
 [Flytte varer ad hoc i enkle lageroppsett](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md)   
 [Designdetaljer: Inngående lagerflyt](design-details-inbound-warehouse-flow.md)   
 [Gjennomgang av forretningsprosesser](walkthrough-business-process-walkthroughs.md)  
 [Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

