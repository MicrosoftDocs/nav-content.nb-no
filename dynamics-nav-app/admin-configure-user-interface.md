---
title: Konfigurere brukergrensesnittet (Grensesnittet) for brukere
description: "Konfigurer som administrator firmaets standard brukergrensesnitt ved å tilpasse sideoppsett for forskjellige brukerprofiler i firmaet."
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize pages, configure user interface, customize UI
ms.date: 07/01/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7ba3d45a856eb38fe99fc5012b4e2f2d8609f9ce
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="configuring-the-user-interface-ui-for-users"></a>Konfigurere brukergrensesnittet (Grensesnittet) for brukere
Konfigurer som administrator firmaets standard brukergrensesnitt ved å tilpasse oppsett for forskjellige brukerprofiler i firmaet. Hvis du vil utføre dette arbeidet, må du være administrator med SUPER-tillatelsessettet. I tillegg må det konfigureres profiler, og de aktuelle brukerne må tilordnes dem. Hvis du vil ha mer informasjon, se [Administrere brukere, profiler og rollesentre ](admin-users-profiles-roles.md).  
  
Du konfigurerer brukergrensesnittet for flere brukere ved å tilpasse sider for en bestemt profil som brukerne tilordnes til. Dette gjør du ved å bruke [!INCLUDE[nav_windows](includes/nav_windows_md.md)], og tilpasse på samme måte som enkeltbrukere tilpasser egne arbeidsområder, det vil si ved hjelp av **Tilpass**-funksjonen. Forskjellen er at du åpner [!INCLUDE[nav_windows](includes/nav_windows_md.md)]i konfigurasjonsmodus. Vanlige tilpasninger omfatter handlinger du vil ha med på båndet, plassering av felt på hurtigfaner eller i faktabokser og menyelementer du vil ha med i navigasjonsruten. 

> [!TIP]  
>  En rask måte å implementere konfigurasjoner av brukergrensesnitt for en profil er i tilfelle du allerede har en konfigurert profil i en annen [!INCLUDE[d365fin](includes/d365fin_md.md)]-database. Du kan eksportere gjeldende profil, og deretter importere den til gjeldende database. Hvis du vil ha mer informasjon, se [Eksportere og importere profiler ](admin-profiles.md#ExportImportProfile).  
  
## <a name="general-information"></a>Generell informasjon
Vurder følgende informasjon før du begynner å konfigurere grensesnittet:
-   Før du begynner å konfigurere grensesnittet kan programmet konfigureres til å vise og skjule brukergrensesnittelementer (for eksempel felt, hurtigfaner og faktabokser) basert på lisensen eller tillatelser. Hvis du vil ha mer informasjon om hvordan du kan gjøre det, kan du se [Fjerne elementer fra brukergrensesnittet i henhold til tillatelser](https://msdn.microsoft.com/en-us/dynamics-nav/removing-elements-from-the-user-interface-according-to-permissions)

    Hvis du vil se virkningen av alternativet Fjerne elementer i brukergrensesnittet, kan du logge på som en testbruker med tillatelsessettet for profilen du konfigurerer. Årsaken er at du som systemansvarlig har SUPER-tillatelsessettet, og du kan derfor ikke se og teste det resulterende brukergrensesnittet når du er logget på din egen konto.    
-   Når du endrer grensesnittilkonfigurasjonen for en side som en bruker har tilpasset, blir brukerens grensesnittilpasning bevart og ikke skrevet over av den nye sidekonfigurasjonen. Når du annullerer konfigurasjonen i brukergrensesnittet på en side som en bruker senere har tilpasset, annulleres ikke brukerens tilpassing i brukergrensesnittet.
-   Det eneste tilfellet der grensesnittkonfigurasjonen skriver over grensesnittilpasningen, er når et grensesnittelement fjernes av konfigurasjonen. Hvis administrator for eksempel fjerner et felt som brukeren har gitt nytt navn eller flyttet, fjernes feltet likevel fra brukerens brukergrensesnitt.
-   Du kan registrere grensesnitkonfigurasjoner på den samme siden basert på ulike tilgangspunkt til siden. Vinduet **Ordrer** kan for eksempel tilpasses slik at det ser annerledes ut når det åpnes fra vinduet **Kundekort** enn når det åpnes fra rollesenteret **Ordrebehandler**. Punktet der du går til siden som skal tilpasses, registreres i denne bestemte sidetilpasningen. Derfor kan det være flere tilpassede sideoppføringer i databasen, som du kan se i vinduet **Slett profilkonfigurasjon**.  
-   I motsetning til når brukere endrer størrelsen på vinduer eller bredden på kolonner på sin egen datamaskin, lagres ikke slike grunnleggende endringer du gjør under konfigurasjonen av grensesnittet for en profil, i profilen, og de er ikke tilgjengelige for brukere som er tilordnet til profilen. Grunnleggende visningsendringer er PC-spesifikke.   

## <a name="configure-a-profile-with-the-includenavwindowsincludesnavwindowsmdmd-in-configuration-mode"></a>Konfigurer en profil med [!INCLUDE[nav_windows](includes/nav_windows_md.md)] i konfigurasjonsmodus
1.  Åpne en kommando, og skriv inn følgende kommando for å bytte til installasjonsmappen av [!INCLUDE[nav_windows](includes/nav_windows_md.md)]. Eksempel:  
  
    ```  
    cd C:\Program Files\(x86)\Microsoft Dynamics NAV\110\RoleTailored Client  
    ```  
  
2.  Skriv inn følgende kommando for å starte [!INCLUDE[nav_windows](includes/nav_windows_md.md)] i konfigurasjonsmodus for en bestemt profil:  
  
    ```  
    Microsoft.Dynamics.Nav.Client.exe -configure -profile:"profileid"  
    ```  
  
     Erstatt **profil-ID** med navnet på profilen du vil konfigurere.  
  
     Hvis du for eksempel vil konfigurere profilen Regnskapssjef, bruker du denne kommandoen:  
  
    ```  
    Microsoft.Dynamics.Nav.Client.exe -configure -profile:"Accounting Manager"  
    ``` 

3. Du kan nå begynne å konfigurere Grensesnittet, som du gjør på samme måte som når enkeltbrukere tilpasser sine egne arbeidsområder. Hvis du vil ha mer informasjon, se [Tilpasse arbeidsområdet i [!INCLUDE[nav_windows](includes/nav_windows_md.md)]](ui-personalization-windows-client.md). 

## <a name="cancel-ui-configuration"></a>Avbryte konfigurasjon i brukergrensesnittet
Du kan annullere grensesnittilpasninger du har gjort som konfigurasjon for en profil, på tre måter:  
  
-   Avbryt alle tilpassinger i brukergrensesnittet som du har gjort for en profil, ved hjelp av knappen **Fjern konfigurerte sider** i vinduet **Profilkort**.  
  
-   Avbryte tilpassing i brukergrensesnitt som du har gjort for bestemte sider for en profil, ved å slette rader i vinduet **Slett profilkonfigurasjon**.  
  
-   Avbryte tilpassing i brukergrensesnitt som du har gjort for et bestemt område i brukergrensesnittet for en bestemt side for en profil, ved hjelp av knappen **Gjenopprett standarder** i vinduet **Tilpass**.  
  
### <a name="general-information"></a>Generell informasjon  
-   Brukere kan tilpasse sine egne brukergrensesnittet når de er logget på sine egne konti. Når du annullerer grensesnittkonfigurasjonen på en side som en bruker siden har tilpasset, annulleres ikke brukerens grensesnittilpasning. Når du utfører en ny konfigurasjon i brukergrensesnittet på en side som en bruker har tilpasset, blir brukerens tilpassing i brukergrensesnittet bevart og blir ikke overskrevet av den nye sidekonfigurasjonen.  

    Det eneste tilfellet der grensesnittkonfigurasjonen skriver over grensesnittilpasningen, er når et grensesnittelement fjernes av konfigurasjonen. Hvis administrator for eksempel fjerner et felt som brukeren har gitt nytt navn eller flyttet, fjernes feltet likevel fra brukerens brukergrensesnitt.  
  
-   I vinduet **Slett brukertilpasning** og med **Gjenopprett standarder** i vinduet **Tilpass**, kan brukere avbryte tilpassing i brukergrensesnittet som de har gjort for sider under sine egne brukerpålogging. Når de gjør dette, tilbakestilles oppsettet for disse sidene til grensesnittilpasninger som systemansvarlig har konfigurert for profilen. Hvis profilen ikke er konfigurert, vil oppsettet for brukerens sider bli tilbakestilt til standard profilkonfigurasjon. Du finner mer informasjon om hvordan brukere avbryter tilpasningen i [Annullere tilpasning](ui-personalization-windows-client.md#CancelPersonalization).
  
### <a name="to-cancel-all-ui-customization-that-you-have-made-for-a-profile"></a>Slik annullerer du alle grensesnittilpasninger du har gjort for en profil:  
  
1.  Skriv inn **Profiler** i **Søk**-boksen, og velg deretter den relaterte koblingen.  
  
2.  Velg profilen du vil annullere alle grensesnittilpasningene for, og velg deretter **Rediger** under **Behandle** i fanebladet **Hjem**.  
  
3.  Velg **Fjern konfigurerte sider** **Funksjoner**-gruppen i kategorien **Handlinger** i vinduet **Profilkort**.  
  
> [!NOTE]  
>  Alle tilpassinger i brukergrensesnitt for profilen, både de som ble installert med programmet og endringer som er gjort av administrator, blir avbrutt. Ingen sideoppsett som er spesifikke for profilen forblir i databasen.  
  
### <a name="to-cancel-ui-customization-that-you-have-made-for-specific-page-for-a-profile"></a>Slik annullerer du grensesnittilpasning du har gjort på en bestemt side for en profil:  
  
1.  Skriv inn **Slett profilkonfigurasjon** i **Søk**-boksen, og velg deretter den tilknyttede koblingen.  
  
2.  Velg settet med profil/side du vil annullere grensesnittilpasningen for, og velg deretter **Slett** under **Behandle** i fanebladet **Hjem**.  
  
    > [!IMPORTANT]  
    >  Hvis du har konfigurert forskjellige tilpassinger i brukergrensesnitt på samme side som er basert på forskjellige navigeringsbaner til siden, vil hver enkelt side vises i vinduet **Slett profilkonfigurasjon** med den samme informasjonen. Det finnes ikke informasjon som kan identifisere hvilken rad som er knyttet til hvilken navigasjonsbane. Derfor må du enten slette rader enkeltvis og deretter kontrollere siden visuelt, eller du kan slette alle radene med grensesnittilpasninger for profilen/siden.
    >    
    >  Alle tilpasninger i brukergrensesnittet for siden for profilen som du har gjort i installasjon eller etter at du brukte sist knappen **Slett profilkonfigurasjon**, blir avbrutt. Sideoppsettet tilbakestilles til standardoppsettet for sideobjektet.  
  
### <a name="to-cancel-ui-customization-that-you-have-made-for-a-specific-ui-area-for-a-specific-page-for-a-profile"></a>Slik annullerer du grensesnittilpasning du har gjort i et bestemt grensesnittområde på en bestemt side for en profil:  
  
Du kan annullere endringer har gjort i individuelle grensesnittområder, for eksempel et bånd, ved å bruke knappen **Gjenopprett standarder** i **Tilpass**-vinduet. Du kan også angre alle endringer i brukergrensesnittet som du har gjort for en profil, ved hjelp av vinduet **Slett profilkonfigurasjon**.  
  
Grensesnittilpasningen for profilen i det bestemte grensesnittområdet på den bestemte siden annulleres. Oppsettet for grensesnittområdet på siden tilbakestilles til standardkonfigurasjonen, som ble laget av systemansvarlig eller installert med programmet.  
  
## <a name="see-also"></a>Se også  
[Tilpasse [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-customizing-overview.md)   
