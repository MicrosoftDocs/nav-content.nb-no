---
title: "Hvorfor er siden låst fra tilpassing?"
description: "Forklarer hvorfor du kan ikke tilpasse en side og hva du kan gjøre for å låse den opp slik at du kan tilpasse den."
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: personalization locked, cannot personalize page
ms.date: 09/07/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b365d14c199d36abebcae0b3ac86340fd59cf8ef
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="why-is-the-page-is-locked-from-personalizing"></a>Hvorfor er siden låst fra tilpassing?
Hvis det er et låseikon i banneret **Tilpassing** når du åpner en side (som vist), betyr dette at du er hindret fra å foreta flere tilpasningsendringer av siden i [!INCLUDE[nav_web](includes/nav_web_md.md)].

![Tilpassingslås](media/personalization-locked.png "Tilpassingslås")

Det kan være to årsaker til dette:
1.  Hittil har du bare brukt [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] til å tilpasse siden.

2. Du har brukt [!INCLUDE[nav_web](includes/nav_web_md.md)] til å tilpasse siden før, men det er gjort ved hjelp av [!INCLUDE[nav2017](includes/nav2017.md)] eller en tidligere versjon.   

Hvis du vil fortsette med å tilpasse siden ved hjelp av [!INCLUDE[nav_web](includes/nav_web_md.md)], velger du låseikonet, og deretter klikker du **Lås opp**.

## <a name="what-happens-when-you-unlock-the-page"></a>Hva skjer når du låser opp siden
Hvis du velger å låse opp siden, nullstilles den gjeldende tilpasningen av siden i [!INCLUDE[nav_web](includes/nav_web_md.md)], noe som betyr at siden vil gå tilbake til det opprinnelige oppsettet, og du må starte fra begynnelsen.

I [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] forblir siden slik den var før, og den vil ikke bli påvirket av de nye endringene i [!INCLUDE[nav_web](includes/nav_web_md.md)]. Tilpasningen i [!INCLUDE[nav_web](includes/nav_web_md.md)] og [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] blir atskilt, slik at du nå har en tilpasset versjon i hver klient. 

Senere vil du tilpasse siden i de to klientene separat. Derfor kan siden potensielt se forskjellig ut mellom de to.

## <a name="see-also"></a>Se også
[Oversikt over tilpasning](ui-personalization-overview.md)  
[Arbeide med tilpasning mellom Dynamics NAV Windows- og webklienten](ui-personalization-overview.md#PersonalizationWinWeb)  
[Tilpasse arbeidsområdet ved hjelp av webklienten](ui-personalization-user.md)  
[Tilpasse arbeidsområdet ved hjelp av Windows-klienten](ui-personalization-windows-client.md)  
[Administrere tilpasning](ui-personalization-manage.md)  
[Arbeide med [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-work-product.md)  
[Endre rollesenteret](change-role.md)  

