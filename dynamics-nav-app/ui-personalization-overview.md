---
title: "Tilpasse arbeidsområdet - oversikt"
description: "Lær hvordan du kan tilpasse brukergrensesnittet slik at det passer til din arbeidsmåte."
documentationcenter: 
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 04334d3bb50b37b9643b848ca4f59b015f03ad04
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="personalizing-your-workspace---overview"></a>Tilpasse arbeidsområdet - oversikt
Du kan *tilpasse* arbeidsområdet slik at det passer til arbeidet og preferansene ved å endre oppsettet på sider slik at de bare viser informasjon du trenger, der du trenger den. Tilpasningsendringene som du utfører, påvirker bare hva du ser, ikke hva andre brukere ser.

Du kan tilpasse arbeidsområdet ved hjelp av [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] og [!INCLUDE[nav_web_md](includes/nav_web_md.md)]. Tilpasningsendringene du utfører, vises også i [!INCLUDE[nav_phone_md](includes/nav_phone_md.md)] og [!INCLUDE[nav_web_md](includes/nav_phone_md.md)].
  
> [!NOTE]  
> Systemansvarlig i selskapet har kanskje allerede tilpasset brukergrensesnittet til et rollespesifikt oppsett for alle brukere som har samme profil som deg og bruker samme rollesenter. Tilpasninger du utfører i arbeidsområdet, lagres under brukerkontoen din, slik at de skal beholdes selv om en administrator distribuerer et nytt sett med rollespesifikke oppsett i selskapet. Hvis du vil ha mer informasjon, kan du se [Konfigurere brukergrensesnittet](admin-configure-user-interface.md).

## <a name="comparing-personalization-in-the-dynamics-nav-windows-and-web-clients"></a>Sammenligne tilpasning i Dynamics NAV Windows- og webklienter
Du kan tilpasse mange deler av brukergrensesnittet, avhengig av siden, for eksempel hvilke felt eller kolonner som skal vises, og hvor de er plassert, hvilke handlinger som inkluderes i båndet, og så videre. Mange av disse tingene kan du gjøre både i Windows-klienten og webklienten. Tabellen nedenfor inneholder en oversikt over tilpasningsmulighetene i hver klient.

|  Tilpass  ||  Windows-klient  |  Webklient  |
|---------------|-|------------------|--------------|
|Felt i hurtigfaner||||
||Legge til, flytte, fjerne |x|x|
||Vise i skjult overskrift|x||
||Skjule under handlingen **Vis flere felt**|x||
|Lister eller dokumentlinjer ||||
||Legge til, flytte, fjerne kolonner  |x|x|
||Legg til, flytte, fjerne fryst rute  |x|x|
|Faktabokser|||
||Legge til, fjerne|x|x|
||Legg til|x||
||Legge til, flytte, fjerne felt|x|x|
|Bunker||||
||Legge til, fjerne|x|x|
||Legg til |x||
|Diagrammer||||
||Legge til, fjerne|x|x|
||Legg til|x| |
|Bånd og handlinger||x||
|Navigasjonsrute||x||

En annen forskjell er at når du tilpasser ved hjelp av Windows-klienten, kan du ha flere tilpassede versjoner av den samme siden, basert på forskjellige tilgangspunkter til siden. Siden **Ordrer** kan for eksempel tilpasses slik at den ser annerledes ut når den åpnes fra siden **Kundekort** enn når den åpnes fra siden **Rollesenter for ordrebehandler**. Når du tilpasser en side ved å bruke webklienten, finnes det bare én tilpasset versjon per side, slik at endringene vises på siden uansett hvor du åpner den fra.

##  <a name="PersonalizationWinWeb"></a>Arbeide med tilpasning mellom Dynamics NAV Windows- og webklienten
Før du begynner å tilpasse sider, er det viktig å forstå hvordan tilpasningen mellom Windows-klienten og webklienten fungerer. Hvis du bare skal bruke enten Windows-klienten eller webklienten, er ikke denne informasjonen så relevant. Dette er imidlertid viktig hvis du begynner å tilpasse sider ved hjelp av begge klientene, eller når du går fra å bruke Windows-klienten til å bruke webklienten permanent.  

-   Hvis du bruker Windows-klienten til å tilpasse en bestemt side fra begynnelsen, vises også tilpasningsendringene på siden i [!INCLUDE[nav_web_md](includes/nav_web_md.md)].

-   Så lenge du fortsette å bruke Windows-klienten til å tilpasse siden, vil tilpasningsendringer du gjør, også tre i kraft på siden i webklienten.

-   Så snart du begynner å tilpasse siden ved hjelp av webklienten blir imidlertid tilpasningen for denne siden separat mellom de to klientene, og du får en tilpasset versjon for hver klient. I webklienten fjernes de tidligere tilpasningene på siden, noe som betyr at siden går tilbake til det opprinnelige oppsettet, og du starter hovedsakelig med å tilpasse siden fra begynnelsen. De tidligere tilpasningene i Windows-klienten forblir uendret.

- Heretter tilpasser du siden i Windows- og webklienten uavhengig av hverandre, noe som betyr at siden potensielt kan se annerledes i hver klient. Telefon- og nettbrettklientene viser de samme sidetilpasningene som webklienten.  

> [!Tip]  
>Hvis du åpner siden **Slett brukertilpasning**, vises alle sider som er tilpasset av hver bruker. Kolonnen **Gammel tilpassing** angir om tilpasningen ble utført i Windows-klienten eller webklienten. Hvis det er en hake i kolonnen, ble tilpasningen utført i Windows-klienten (eller i webklienten før [!INCLUDE[navnow_md](includes/navnow_md.md)]).

## <a name="see-also"></a>Se også
[Tilpasse arbeidsområdet i Dynamics NAV Windows-klienten](ui-personalization-windows-client.md)  
[Tilpasse arbeidsområdet i Dynamics NAV webklienten](ui-personalization-user.md)  
[Administrere tilpasning](ui-personalization-manage.md)  
[Tilpasse Dynamics NAV](ui-customizing-overview.md)  

