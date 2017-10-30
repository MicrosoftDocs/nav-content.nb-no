---
title: Opprette hylleinnhold
description: Etter at du har definert hyllene, kan du definere hylleinnholdet. Du kan med andre ord definere hvilke varer du vil lagre i en gitt hylle, og angi regler som skal styre fylling av hyllen med en bestemt vare.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2fe2b29ff5c374d7b40f18bddfde4c66ce032e18
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-bin-contents"></a>Opprette hylleinnhold
Etter at du har definert hyllene, kan du definere hylleinnholdet. Du kan med andre ord definere hvilke varer du vil lagre i en gitt hylle, og angi regler som skal styre fylling av hyllen med en bestemt vare. Du kan gjøre dette manuelt i **Hylleinnhold**-vinduet eller automatisk med **Opprett hylleinnholdforslag**-vinduet.

## <a name="to-create-bin-content-manually"></a>Slik oppretter du hylleinnhold manuelt:  
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Lokasjoner**, og velg deretter den relaterte koblingen.  
2.  Velg lokasjonen der du vil opprette hylleinnhold, og velg deretter **Hyller**-handlingen.  
3.  Velg hyllen der du vil opprette innhold, og velg deretter **Innhold**-handlingen.  
4.  For hver vare du vil lagre i hyllen, fyller du ut en linje i vinduet **Hylleinnhold** med den passende informasjonen. Noen av feltene er allerede fylt ut med informasjon om hyllen.  
5.  Først fyller du ut feltet **Varenr.**, og deretter, hvis du bruker lagerstyring, fyller du ut de andre nødvendige feltene, for eksempel feltene **Enhetskode**, **Maks. ant.** og **Min.antall**.  

Velg feltet **Fast** om nødvendig. Hvis hyllen skal brukes som standardhylle for varen, velger du feltet **Standard hyllevalg**.  

Hvis du bruker lagerstyring og har angitt riktig størrelsesinformasjon om hver vares målenhet på varekortet kontrollere det maksimumsantallet du angir i vinduet **Hylleinnhold**, mot hyllens fysiske kapasitet. Minimums- og maksimumsantallene brukes når det beregnes etterfylling av hyller og plasseringsforslag.  

Hvis du velger feltet **Fast**, gir du varen fast plass i hyllen, som betyr at [!INCLUDE[d365fin](includes/d365fin_md.md)] vil prøve å legge denne varen i hyllen hvis det er plass til den, og det vil beholde posten som gir varen fast plass i hyllen, selv om antallet i hyllen er 0. Andre varer kan legges i hyllen, selv om en bestemt vare har fast plass der. Andre varer kan plasseres på hyllen, selv om en bestemt vare er fast i hyllen.  

> [!NOTE]  
>  Du kan sette opp flere hylleinnhold samtidig i vinduet **Hylleinnholdopprett. - forslag**.  

## <a name="to-create-bin-content-with-a-worksheet"></a>Slik oppretter du hylleinnhold med et forslag:  
Når du har opprettet hyllene, kan du opprette det hylleinnholdet du ønsker for hver hylle i opprettingsforslaget for hylleinnhold.

1.  Velg ikonet ![Søk etter en side eller rapport](media/ui-search/search_small.png "Ikonet Søk etter en side eller rapport"), angi **Hylleinnholdopprett. - forslag**, og velg deretter den relaterte koblingen.  
2.  I feltet **Navn** i forslagshodet velger forslaget for lokasjonen der du vil opprette hylleinnholdet.  
3.  I feltet **Hyllekode** velger du koden for hyllen som du vil definere hylleinnhold for.   

    Hvis du bruker lagerstyring i denne lokasjonen, fylles feltene som er relatert til den bestemte hyllen, som for eksempel **Hylletype**, **Lagerklassekode** og **Hylleprioritering** automatisk ut. Dette er informasjon du trenger når du skal definere hylleinnholdet.  
4.  Velg varen du vil tilordne til hyllen, og fyll ut feltene som gjelder for hylleinnholdet. Hvis du bruker lagerstyring og vil bruke funksjonen **Beregn etterfylling av hylle**, fyller du ut feltene **Maks. ant.** og **Min. antall**.  

    Hvis du vil angi denne hyllen som den foretrukne hyllen, selv om hylleantallet er **0** og alle andre plasseringskriterier er like, velger du **Fast**-feltet.  
5.  Gjenta trinn 3 til og 4 for hver vare du vil tilordne til en hylle.  
6.  Velg handlingen **Skriv ut** for å forhåndsvise og skrive ut hylleinnholdet du har oppgitt i forslaget. Fortsett å arbeide med hylleinnholdet til du er fornøyd.  
7.  Når du er klar, velger du **Opprett hylleinnhold**-handlingen.  

I dette forslaget kan du arbeide med flere hylleinnholdslinjer for flere hyller og dermed få god oversikt over hva du legger i ulike hyller i en gitt sone, passasje eller reol.  

## <a name="see-also"></a>Se også
[Beregne etterfylling av hylle](warehouse-how-to-calculate-bin-replenishment.md)    
[Lagerstyring](warehouse-manage-warehouse.md)  
[Lager](inventory-manage-inventory.md)  
[Definere lagerstyring](warehouse-setup-warehouse.md)     
[Monteringsstyring](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyring](design-details-warehouse-management.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

