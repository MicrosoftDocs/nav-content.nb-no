---
title: Planlegge lagerflyttinger i forslag
description: Planlegge flyttinger i forslaget ved hjelp av en funksjon for etterfylling av hyller eller ved manuell planlegging av linjene du vil opprette som flytteinstruksjoner.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: fcf44a681e597df1bd50e94e851810fa00656a96
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-plan-warehouse-movements-in-worksheets"></a>Planlegge lagerflyttinger i forslag
Planlegge flyttinger i forslaget ved hjelp av en funksjon for etterfylling av hyller eller ved manuell planlegging av linjene du vil opprette som flytteinstruksjoner.  

## <a name="to-calculate-a-replenishment-movement"></a>Slik beregner du en etterfyllingsflytting  
Etter hvert som lageret leverer varer til kundene, vil hyllene med de høyeste hylleprioriteringene inneholde færre og færre varer. For å fylle opp disse hyllene med varer fra andre hyller, kjører du funksjonen **Beregn etterfylling av hylle** i vinduet **Flytteforslag**.

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Flytteforslag**, og velg deretter den relaterte koblingen.  
2.  Velg handlingen **Beregn etterfylling av hyller**.  

    [!INCLUDE[d365fin](includes/d365fin_md.md)] oppretter linjer som angir nøyaktig hvordan du skal flytte varer fra hyller med lav prioritering til hyller med høy prioritering.  

    > [!NOTE]  
    >  En flytting blir foreslått i henhold til FEFO når du aktiverer funksjonen **Opprett flytting**, hvis følgende betingelser er oppfylt for en vare:  
    >   
    >  -   Varen har en utløpsdato.  
    > -   Avmerkingsboksen **Plukk i henhold til FEFO** på lokasjonskortet er merket av.  
    > -   Avmerkingsboksen **Hylle obligatorisk** på lokasjonskortet er merket av.  
    > -   Feltene **Fra sone** og **Fra hylle** er tomme.  

    Hvis du vil ha mer informasjon, kan du se [Plukking etter FEFO](warehouse-picking-by-fefo.md).  

3.  Se gjennom linjene og endre dem hvis det er nødvendig, eller slett noen av dem hvis det ikke er nok tid til å utføre alle.  
4.  Velg handlingen **Opprett flytting** for å lage en lagerinstruksjon som de lageransatte kan bruke.  

## <a name="to-move-the-entire-contents-of-one-or-more-bins-by-using-the-get-bin-content-function"></a>Slik flytter du hele innholdet i én eller flere hyller med funksjonen Hent hylleinnhold  
Du kan også bruke flytteforslaget til å planlegge andre flyttinger av beholdning i lageret. Du kan for eksempel bruke denne handlingen når du vil plassere varer i en hylle for kvalitetskontroll, og deretter opprette en flytting for å lage instruksjoner for en ansatt.  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Flytteforslag**, og velg deretter den relaterte koblingen.  
2.  Velg **Hent hylleinnhold**-handlingen. Bruk forespørselsvinduet til å filtrere hyller og varer som du vil skal vises på flytteforslagslinjene.  
3.  Fyll ut de aktuelle feltene i vinduet for forespørsel om kjørsel. Hvis du for eksempel vil se hylleinnholdet i alle hyllene i en bestemt sone i lokasjonen, fyller du ut **Sonekode**-feltet. Hvis du vil hente linjer for hver hylle som inneholder en bestemt vare, fyller du ut **Varenr.**-feltet.  

    > [!NOTE]  
    >  Du kan ikke manuelt flytte varer til eller fra en hylle av hylletypen RECEIVE, fordi varer som er i en slik hylle må registreres som plassert før de blir en del av det tilgjengelige lageret.  

4.  Hvis du skal hente mange linjer, velger du **Sorter** for å velge en sorteringsmetode for å definere rekkefølgen av linjene i forslaget og deretter velger du **OK**.  

    > [!NOTE]  
    >  Flyttingslinjer hentes i henhold til FEFO når du aktiverer funksjonen **Hent hylleinnhold**, hvis følgende betingelser er oppfylt for en vare:  
    >   
    >  -   Varen har en utløpsdato.  
    > -   Avmerkingsboksen **Plukk i henhold til FEFO** på lokasjonskortet er merket av.  
    > -   Avmerkingsboksen **Hylle obligatorisk** på lokasjonskortet er merket av.  
    > -   Feltene **Fra sone** og **Fra hylle** er tomme.  

5.  Fyll ut noen av de hentede linjene for å utføre endringene du vil utføre. For hver vare som skal flyttes, må du fylle ut feltene **Varenr.**, **Fra hylle-kode**, **Til hylle-kode** og **Antall**.  
6.  Slett de uferdige linjene som du brukte til informasjon.  
7.  Når flytteforslagslinjene nøyaktig gjenspeiler hvordan flyttehandlingen skal utføres av den lageransatte, velger du handlingen **Opprett flytting** for å opprette instruksjonene for den ansatte.  

## <a name="see-also"></a>Se også  
[Lagerstyring](warehouse-manage-warehouse.md)  
[Lager](inventory-manage-inventory.md)  
[Definere lagerstyring](warehouse-setup-warehouse.md)     
[Monteringsstyring](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyring](design-details-warehouse-management.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

