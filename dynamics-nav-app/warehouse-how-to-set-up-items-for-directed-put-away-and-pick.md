---
title: Definere varer og lokasjoner for lagerstyring
description: "Når du definerer en lagerlokasjon til å bruke lagerstyring, får du tilgjengelig en ny funksjonalitet som hjelper deg å styre lageret mest mulig effektivt."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 6ec7065cb2d633ea18c586c6369487052464a482
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-items-and-locations-for-directed-put-away-and-pick"></a>Definere varer og lokasjoner for lagerstyring
Når du definerer en lagerlokasjon til å bruke lagerstyring, får du tilgjengelig en ny funksjonalitet som hjelper deg å styre lageret mest mulig effektivt. For å kunne utnytte denne funksjonaliteten fullt ut må du angi tilleggsopplysninger om varene, noe som i neste omgang hjelper å utføre de nødvendige beregningene for å foreslå de mest effektive og praktiske måtene å utføre lageraktiviteter på. Hvis du vil ha mer informasjon, kan du se [Designdetaljer: Lagerstyringsoppsett](design-details-warehouse-setup.md).

## <a name="to-set-up-an-item-for-directed-put-away-and-pick"></a>Slik definerer du varer for lagerstyring  
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Varer**, og velg deretter den relaterte koblingen.  
2.  Åpne kortet for varen du vil definere for lagerstyring.
3. På hurtigfanen **Lager** på varekortet fyller du ut feltene for å definere hvordan varene skal håndteres i lageret.  
4.  Velg handlingen **Enheter**.
5. I **Enheter**-vinduet fyller du ut feltene for å definere de forskjellige enhetene som kan brukes i varetransaksjoner, inkludert høyde, bredde, lengde, kubikkinnhold og vekt for enhetene.
6. Velg **Hylleinnhold**-handlingen.
7. I **Hylleinnhold**-vinduet kan du definere lokasjonen og hyllen som varen skal tilordnes til. Feltet **Standard** brukes ikke når lokasjonen er definert til å bruke lagerstyring.  

## <a name="to-activate-directed-put-away-and-pick-functionality"></a>Slik aktiverer du funksjonalitet for bruk av lagerstyring:  
Lagerstyring gir deg tilgang til avanserte lageroppsettsfunksjoner som forbedrer effektiviteten og datapåliteligheten. Hvis du skal bruke denne funksjonaliteten, må du først definere et antall parametere for lagerlokasjonen.  

Hvis du vil bruke lagerstyring, må du aktivere funksjonaliteten på lokasjonskortet.    
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Lokasjoner**, og velg deretter den relaterte koblingen.  
2.  Velg lokasjonen der du vil bruke lagerstyring, og velg deretter handlingen **Rediger**.  
3.  På hurtigfanen **Lager** merker du av for **Bruk Lagerstyring**.  

Du trenger ikke å fylle ut noen andre felt på lokasjonskortet før senere i oppsettprosessen.  

> [!NOTE]  
>  Du kan ikke definere lageret som skal bruke hyller når lokasjonen har åpne vareposter.  

Neste trinn er å definere hvilken hylletype du vil bruke. Hvis du vil ha mer informasjon, kan du se [Definere hylletyper](warehouse-how-to-set-up-bin-types.md). Hylletypen definerer hvordan en gitt hylle skal brukes i behandlingen av flyten gjennom lageret. Du kan tilordne en hylletype til både en sone og en hylle.  

Du kan også definere lagerklassekoder hvis lageret har varer som trenger ulike lagringsforhold. Lagerklassekoder brukes når det blir foreslått vareplassering i hyller. Du tilordner lagerklassekoder til produktgrupper, som deretter blir tilordnet til varer og lagerføringsenheter eller soner og hyller som innfrir lagringsforholdene som kreves av lagerklassekodene.  

Du er nå klar til å sette opp sonene, hvis du vil bruke soner i lageret. Hvis du bruker soner, vil det redusere antall felt du må fylle ut når du setter opp hyllene, fordi hyller som er opprettet med soner, arver flere egenskaper fra sonen. Sonene kan gjøre det enklere for nye eller midlertidig ansatte å orientere seg i lageret. Merk at flyt kontrolleres av hyller, det er derfor mulig å operere med hyller og bare én sone.  

## <a name="to-set-up-a-zone-in-your-warehouse"></a>Slik setter du opp en sone i lageret  
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Lokasjoner**, og velg deretter den relaterte koblingen.  
2.  Velg lokasjonen der du vil sette opp en sone, og åpne lokasjonskortet og velg deretter **Soner**-handlingen.  
3.  I vinduet **Soner** fyller du ut feltene etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

Når du endrer en soneparameter, vil alle hyllene som opprettes i den aktuelle sonen etter endringen ha de nye egenskapene, men de opprinnelige hyllene endres ikke.  

> [!NOTE]  
>  Hvis du ikke vil bruke soner, må du likevel opprette én sonekode som er udefinert, bortsett fra koden.  

Neste trinn i oppsettet av lageret er å definere hyller. Se [Definere lokasjoner slik at de bruker hyller](warehouse-how-to-set-up-locations-to-use-bins.md) for å få mer informasjon.  

I tillegg må du opprette plasseringsmaler og opptellingsperioder. Hvis du vil ha mer informasjon, kan du se [Definere plasseringsmaler](warehouse-how-to-set-up-put-away-templates.md).  

## <a name="see-also"></a>Se også  
[Lagerstyring](warehouse-manage-warehouse.md)  
[Lager](inventory-manage-inventory.md)  
[Definere lagerstyring](warehouse-setup-warehouse.md)     
[Monteringsstyring](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyring](design-details-warehouse-management.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

