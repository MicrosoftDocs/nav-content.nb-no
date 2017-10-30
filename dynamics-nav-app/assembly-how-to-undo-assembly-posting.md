---
title: "Angre monteringsbokføring"
description: "Noen ganger kan det hende at du må angre en bokført monteringsordre, for eksempel når ordren ble bokført med feil som må rettes opp, eller fordi den ikke skulle vært bokført i utgangspunktet og må rulles tilbake."
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
ms.openlocfilehash: 3ba93dd182aa1591f5d24398d4b749942d38bb4b
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-undo-assembly-posting"></a>Angre monteringsbokføring
Noen ganger kan det hende at du må angre en bokført monteringsordre, for eksempel når ordren ble bokført med feil som må rettes opp, eller fordi den ikke skulle vært bokført i utgangspunktet og må rulles tilbake.

Når du angrer en bokført monteringsordre, blir det opprettet et sett med korreksjonsvareposter for å reversere de opprinnelige postene. Hver positive avgangspost for monteringsvaren tilbakeføres ved en negativ avgangspost. Hver negative forbrukspost for en monteringskomponent tilbakeføres ved en positiv forbrukspost. Utligning av fast kostnad opprettes automatisk mellom korrigerende og originale poster for å sikre nøyaktig tilbakeføring av kostnad.  

Når du angrer en fullstendig bokført monteringsordre, kan du velge å opprette monteringsordren på nytt til opprinnelig tilstand, for eksempel for å foreta korrigeringer før du bokfører den på nytt. Du kan også velge ikke å opprette monteringsordren på nytt.  

Når du angrer en delvis bokført monteringsordre, vil alle berørte antallsfelt, for eksempel feltene **Montert antall**, **Forbrukt antall** og **Restantall**, bli gjenopprettet til verdiene de hadde før den aktuelle bokføringen.  

Hvis du vil opprette på nytt eller gjenopprette monteringsordrer, må følgende betingelser være oppfylt for monteringsvaren som hadde avgang i den opprinnelige bokføringen:  

-   Den må fortsatt være på lager, det vil si ikke solgt eller på annen måte forbrukt gjennom utgående transaksjoner.  
-   Det må ikke være reservert.  
-   Den må finnes i hyllen som den ble lagt i.  

I tillegg kan eksisterende monteringsordrer bare gjenopprettes hvis antallet linjer og rekkefølgen til linjene i den opprinnelige rekkefølgen ikke endres.  

> [!TIP]  
>  Du kan løse konflikter som skyldes linjeendringer, ved å tilbakestille endringene på de aktuelle linjene manuelt, før du angrer den tilknyttede bokførte monteringsordren. Du kan også bokføre monteringsordren fullstendig og deretter velge å opprette den på nytt når du angrer bokføringen.  

Fremgangsmåten nedenfor beskriver hvordan du angrer bokførte monteringsordrer der varene ble montert til lager. Hvis du vil angre bokførte monteringsordrer der varene ble montert til en ordre, må du bruke **Angre levering**-funksjon på den bokførte følgeseddelen som er relatert til den bokførte monteringsordren. Hvis du vil ha mer informasjon, kan du se [Tilbakeføre bokføringer](finance-how-reverse-journal-posting.md). Angring av bokførte monteringsorder skjer automatisk på samme måte som beskrevet i dette emnet.  

## <a name="to-undo-posting-of-an-assembly-order"></a>Slik angrer du bokføringen av en monteringsordre:  
1.  Hvis du vil angre en fullstendig eller delvis bokført monteringsordre, kan du velge ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bokførte monteringsordrer** og velge den relaterte koblingen.  

    Vinduet **Bokførte monteringsordrer** åpnes med én eller flere bokførte monteringsordrer som er bokført fra den aktuelle monteringsordren. Hver delvise bokføring oppretter en separat bokført monteringsordre.  
2.  Åpne den bokførte monteringsordren du vil angre, og velg deretter **Angre montering**.  

    Hvis den bokførte monteringsordren du vil angre, er relatert til en fullstendig bokført monteringsordre som nå er slettet, har du muligheten til å opprette den på nytt, vanligvis fordi du gjerne vil behandle den på nytt.  
3.  Hvis du vil opprette monteringsordren på nytt, klikker du **Ja**. Hvis du vil angre bokføringen uten å opprette den relaterte monteringsordren på nytt, klikker du **Nei**.  

Feltet **Tilbakeført** i monteringsordrehodet endres til **Ja**. Monteringsordrebokføringen tilbakeføres nå, og du kan fortsette å behandle hele monteringsordren hvis du velger å opprette den på nytt eller åpne monteringsordrerekkefølgen som du har gjenopprettet til opprinnelig tilstand.  

> [!NOTE]  
>  Hvis du vil gjenopprette antallene fra flere delvise bokføringer i en monteringsordre, må du angre alle aktuelle bokførte monteringsordrer ved å følge trinn 1 til 3 ovenfor for hver bokførte monteringsordre.  

## <a name="see-also"></a>Se også  
[Monteringsstyring](assembly-assemble-items.md)  
[Tilbakeføre bokføringer](finance-how-reverse-journal-posting.md)  
[Behandle ordrereturer eller annulleringer](sales-how-process-sales-returns-cancellations.md)    
[Arbeide med stykklister](inventory-how-work-BOMs.md)  
[Lager](inventory-manage-inventory.md)  
[Designdetaljer: Lagerstyring](design-details-warehouse-management.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

