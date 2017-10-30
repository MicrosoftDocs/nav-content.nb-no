---
title: Montere varer
description: "Hvis feltet **Etterfyllingssystem** på varekortet inneholder **Montering**, er standardmetoden for å forsyne varen å montere den fra definerte komponenter og muligens av en definert ressurs."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b7f371c48aa70d2b99ce7b7333b92a63d7764f28
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-assemble-items"></a>Montere varer
Hvis feltet **Etterfyllingssystem** på varekortet inneholder **Montering**, er standardmetoden for å forsyne varen å montere den fra definerte komponenter og muligens av en definert ressurs.  

Komponenter og ressurser som går inn i denne typen monteringsvare må være definert i en monteringsstykkliste. Hvis du vil ha mer informasjon, kan du se [Arbeide med stykklister](inventory-how-work-BOMs.md).  

Monteringsvarer kan settes opp for to ulike monteringsprosesser:  

-   Monter til lager.  
-   Monter til ordre.  

Vanligvis bruker du **Montere til lager** for varer som du vil montere før salg (for eksempel for å forberede til en pakkekampanje) og beholde på lager inntil de bestilles. Disse varene er vanligvis standardvarer, for eksempel pakkede sett som du ikke tilbyr å tilpasse på forespørsel fra kunder.  

Vanligvis bruker du **Montere til ordre** for varer som du ikke vil ha på lager, fordi du planlegger å tilpasse dem etter kundeforespørsler eller fordi du vil minimere lagerføringskostnadene ved å forsyne dem i siste liten. Hvis du vil ha mer informasjon, kan du se [Selge varer som er montert til ordre](assembly-how-to-sell-items-assembled-to-order.md).  

Hvis du vil ha mer informasjon om hvordan du definerer en monteringsvare, se [Forstå montere til ordre og montere til lager](assembly-assemble-to-order-or-assemble-to-stock.md).  

Disse oppsettsalternativene er standardinnstillinger som styrer hvordan salgs- og monteringsordrelinjer behandles til å begynne med. Du kan omgå disse standardene og forsyne monteringsvaren på den mest optimale måten ved behandling av et salg. Hvis du vil ha mer informasjon, se [Selge lagervarer i montere-til-ordre-flyter](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md) og [Selge montere-til-ordre-varer og lagervarer sammen](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md).

> [!NOTE]  
> Monteringskomponenter håndteres på en spesiell måte i enkle lagerkonfigurasjoner. Hvis du vil ha mer informasjon, kan du se delen "Håndtere montere-til-ordre-varer i lagerplukk" i [Plukke varer med lagerplukk](warehouse-how-to-pick-items-with-inventory-picks.md).   

I denne fremgangsmåten oppretter og behandler du en monteringsordre for varer som er montert til lager, det vil si uten en koblet ordre. Trinnene inkluderer start av monteringsordren, håndtering av potensielle problemer med komponenttilgjengelighet og delvis avgangsbokføring av monteringsvarer.

## <a name="to-assemble-an-item"></a>Slik monterer du en vare:  
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Monteringsordrer**, og velg deretter den relaterte koblingen.  
2.  Velg handlingen **Ny**. Vinduet **Ny monteringsvare** åpnes.  
3.  Fyll ut feltene etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  Velg monteringsvaren du vil behandle, i **Varenr.**-feltet. Feltet filtreres slik at det bare viser varer som er definert for montering, noe som betyr at monteringsstykklister er tilordnet varene.  
5.  Angi hvor mange enheter av varen du vil ha montert, i **Antall**-feltet.  

    > [!NOTE]  
    >  Hvis én eller flere komponenter ikke er tilgjengelige for å oppfylle angitt monteringsvareantall på den definerte forfallsdatoen, åpnes vinduet **Montering – tilgjengelighet** automatisk for å gi detaljert informasjon om hvor mange monteringsvarer som kan monteres, basert på komponenttilgjengelighet. Hvis du vil ha mer informasjon, kan du se [Vise tilgjengeligheten av varer](inventory-how-availability-overview.md). Når du lukker vinduet, opprettes monteringsordren med tilgjengelighetsvarsler på de berørte komponentlinjene.  

    Monteringsordrelinjene fylles ut automatisk med innholdet i monteringsstykklisten og linjeantall i henhold til monteringsordrehodet.  

    > [!NOTE]  
    >  Hvis vinduet **Montering – tilgjengelighet** ble åpnet da du fylte ut monteringsordrehodet, inneholder hver påvirkede monteringsordrelinje **Ja** i feltet **Tilgj. advarsel** med en kobling til detaljert tilgjengelighetsinformasjon. Hvis du vil ha mer informasjon, se Kontroller tilgjengelighet. Du kan løse et problem med komponenttilgjengelighet ved å utsette startdatoen, erstatte komponenten med en annen vare eller velge en mulig erstatning, hvis dette er definert.  

6.  Angi hvor mange enheter av monteringsvaren du vil bokføre som avgang neste gang du bokfører monteringsordren, i feltet **Antall å montere**. Dette antallet kan være lavere enn verdien i **Antall**-feltet for å gjenspeile en delvis avgangsbokføring.  

    > [!NOTE]  
    >  For å sikre at komponentforbruksbokføring samsvarer med avgangsbokføring for monteringsvarer justeres antallsfeltene i monteringsvarelinjene automatisk til verdien du angir i feltet **Antall å montere**.  
7.  På monteringsordrelinjer av typen **Vare** eller **Ressurs** angir du i feltet **Antall som skal forbrukes** hvor mange enheter du vil bokføre som forbrukt neste gang du bokfører monteringsordren. Som standard blir forventet antall til forbruk i henhold til monteringsstykklisten og monteringsordrehodeantallet satt inn, men du kan øke eller redusere det, for eksempel for å gjenspeile et overforbruk av komponenter eller at ekstra ressurser ble brukt.  
8.  Når du er klar til å bokføre delvis eller fullstendig, velger du **Bokfør**-handlingen.  

    > [!NOTE]  
    >  Hvis det fortsatt er advarsler på noen av monteringsordrelinjene, blokkeres bokføring. Det vises en melding om hvilke komponenter som ikke er i lageret.  

Etter vellykket bokføring, bokføres monteringsvaren som avgått til lokasjonskoden og den potensielle hyllekoden som er definert i monteringsordren. For manuelt opprettede monteringsordrer kan kan lokasjonen kopieres fra oppsettfeltet **Standardlokasjon for ordrer**. Når det gjelder montere-til-ordre-flyter, kan du kopiere lokasjonskoden fra ordrelinjen.  

## <a name="see-also"></a>Se også
[Monteringsstyring](assembly-assemble-items.md)  
[Arbeide med stykklister](inventory-how-work-BOMs.md)  
[Lager](inventory-manage-inventory.md)  
[Designdetaljer: Lagerstyring](design-details-warehouse-management.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

