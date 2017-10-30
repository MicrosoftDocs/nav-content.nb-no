---
title: Administrere tilpasning som Administrator
description: "Lær hvordan du kan tilpasse brukergrensesnittet slik at det passer til din arbeidsmåte."
documentationcenter: 
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: e3d088c35efca4d62b7db1f0d44d5ef2958317d4
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="managing-personalization-as-an-administrator"></a>Administrere tilpasning som Administrator
Brukere kan tilpasse arbeidsområdet etter egne behov. Som administrator kan du kontrollere og håndtere tilpasning ved å deaktivere muligheten for brukerne til å tilpasse sider og fjerne en hvilken som helst sidetilpasning som brukere har utført.

## <a name="disable-personalization-for-a-profile"></a>Deaktivere tilpasning for en profil
Du kan hindre alle brukere som tilhører en bestemt profil, fra å tilpasse sine sider.
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Profiler**, og velg deretter den relaterte koblingen.
2.  Velg profilen i listen som du vil endre.
3.  Merk av for **Deaktiver tilpasning**, og velg deretter **OK**.

## <a name="clear-user-personalizations"></a>Fjerne brukertilpasninger

Hvis du fjerner sidetilpasninger, endres siden tilbake til det opprinnelige oppsettet før eventuelle tilpasninger ble utført. Du kan slette tilpasninger brukere har gjort med sider, på to måter: ved hjelp av siden **Slett brukertilpasning** og ved hjelp av siden **Brukertilpasningskort**.

### <a name="clear-user-personalizations-by-using-the-delete-user-personalization-page"></a>Slette brukertilpasninger ved hjelp av siden Slett brukertilpasning

Siden **Slett brukertilpasning** gir deg muligheten til å slette tilpasning basert på per side, per bruker.

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Slett brukertilpasning**, og velg deretter den relaterte koblingen.

    Siden viser alle sidene som er tilpasset, og brukerne de tilhører.

    >[!NOTE]
    > En hake i kolonnen **Gammel tilpassing** angir at tilpasningen er utført bare ved hjelp av [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] og/eller den er utført i [!INCLUDE[nav_web_md](includes/nav_web_md.md)] før [!INCLUDE[navnow_md](includes/navnow_md.md)]. Brukere som prøver å tilpasse disse sidene ved hjelp av [!INCLUDE[nav_web_md](includes/nav_web_md.md)], er låst fra å gjøre dette med mindre de ønsker å låse opp siden. Hvis du vil ha mer informasjon, se [Hvorfor en side er låst fra tilpassing](ui-personalization-locked.md). Hvis du vil ha mer informasjon om tilpasning mellom [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] og [!INCLUDE[nav_web_md](includes/nav_web_md.md)], kan du se [Arbeide med tilpasning mellom Dynamics NAV Windows- og webklienten](ui-personalization-overview.md#PersonalizationWinWeb).

2. Velg posten du vil slette, og velg deretter handlingen **Slett**.

    Brukeren vil se endringene neste gang vedkommende logger på.

### <a name="clear-user-personalizations-by-using-the-user-personalization-card-page"></a>Slette brukertilpasninger ved hjelp av siden Brukertilpasningskort

Siden **Brukertilpasningskort** gir deg muligheten til å slette tilpasningen på alle sider for en bestemt bruker. Dette krever skrivetilgang til tabellen 2000000072 **profil**.

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Brukertilpasning**, og velg deretter den relaterte koblingen.

    Siden **Brukertilpasning** viser alle brukerne som kan ha tilpassede sider. Hvis du ikke finner en bruker i listen, betyr det at de ikke har tilpassede sider.

2. Velg brukeren fra listen, og velg deretter handlingen **Rediger**.

3.  I kategorien **Handlinger** velger du **Fjern tilpassede sider**.

    Brukeren vil se endringene neste gang vedkommende logger på.

## <a name="see-also"></a>Se også
[Oversikt over tilpasning](ui-personalization-overview.md)  
[Tilpasse arbeidsområdet](ui-personalization-user.md)  
[Arbeide med [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-work-product.md)  
[Endre rollesenteret](change-role.md)  
