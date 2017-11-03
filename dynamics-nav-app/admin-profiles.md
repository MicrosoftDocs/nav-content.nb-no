---
title: Administrere profiler og rollesentre
description: "Lær hvordan du administrerer brukere og rollesentre i Dynamics NAV."
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: profiles, roles, role centers, user roles
ms.date: 09/01/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: a657c409c9cd361a505f1fd61dbb5254b25c5144
ms.contentlocale: nb-no
ms.lasthandoff: 10/26/2017

---
# <a name="managing-profiles-and-role-centers"></a>Administrere profiler og rollesentre
Profiler er samlinger av [!INCLUDE[navnow_md](includes/navnow_md.md)]-brukere som deler samme rollesenter. Et rollesenter er en side der du kan plassere forskjellige deler. Hver del er en beholder som kan være vert for andre sider eller forhåndsdefinerte systemdeler, for eksempel en Outlook-del eller deler for å legge til oppgaver, varslinger eller notater.  

## <a name="about-profiles-and-role-centers"></a>Om profiler og rollesentre
Du bruker profiler til å knytte brukere til forhåndsdefinerte rollesentre. Et rollesenter er en hjemmeside for alle brukere av en profil som er konfigurert til å gjenspeile oppgavene og prioritetene til brukere av profilen. Rollesenteret for ordrebehandler er for eksempel konfigurert slik at det gjenspeiler oppgavene og prioritetene til en ordrebehandler. Et rollesenter gir deg enkel tilgang til informasjon som brukerne trenger for å kunne daglige arbeidsoppgaver. Rollesenteret bestemmer for eksempel bunkene eller flisen som vises når brukere logger på, og koblingene fra navigasjonssiden.

Profilen som brukes vises i hodet for hovedinnholdsområdet i rollesenteret. En administrator kan deretter tilpasse dette rollesenteret for å dekke behovene til en bestemt rolle i et bestemt firma. Rollesenteret for ordrebehandler kan deretter tilpasset ytterligere på en enkelt datamaskin for å dekke behovene til en person som utfører jobben som en ordrebehandler. Denne personen kan tilpasse rollesenteret ved å lagre spørringer, legge til filtre og legge til eller fjerne felt.

Profiler og rollesentre tilpasses til rollene og ansvarsområdene i organisasjonen. [!INCLUDE[navnow_md](includes/navnow_md.md)] inneholder et sett med standardprofiler, og hver av dem svarer til og er tilknyttet et rollesenter. Administratorer kan redigere eksisterende profiler eller opprette nye.  

> [!NOTE]  
>  Profiler er ikke eksplisitt knyttet til rollene og tillatelsene som utgjør sikkerhetssystemet, men profilbrukere må ha tillatelser som er tilpasset deres roller i sikkerhetssystemet. Hvis du vil ha mer informasjon, kan du se [Security in the Role Tailored Environment](http://go.microsoft.com/fwlink?LinkId=147633) i MSDN-biblioteket.

## <a name="to-create-a-profile"></a>Slik oppretter du en profil
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Profiler**, og velg deretter den relaterte koblingen.  

2.  Velg **Ny**for å åpne **Nytt profilkort**-vinduet.  

3.  Skriv inn et navn som beskriver den tiltenkte rollen for brukeren, i **Profil-ID**-feltet.  

4.  I **Beskrivelse**-feltet angir du en beskrivelse av profil-IDen, for eksempel **Ordrebehandler**.  

5.  Sett **Rollesenter-ID**-felttet til rollesenteret du vil tilordne til profilen.  

6.  Hvis du vil gjøre dette rollesenteret til standard for profilen, merker du av for **Standard rollesenter**.  

7.  Velg **OK**. .  

Fremgangsmåten for å endre en eksisterende profil er det samme, bortsett fra at du velger en eksisterende profil på Profiler-siden i stedet for å velge handlingen **Ny**.  


##<a name="copying-a-profile"></a>Kopiere en profil:
Du kan spare tid ved å kopiere en profil hvis du vil bruke lignende innstillinger på en profil, og du bare vil endre noen innstillinger.

1.  Åpne profilen du vil kopiere, og velg deretter **Kopier profil**.

2.  I **Ny profil-ID**-feltet skriver du inn et navn for profilen du vil kopiere.

3.  Sett feltet **Nytt profilomfang** til ett av følgende:

    - **System** slik at den nye profilen blir tilgjengelig for alle leietakerdatabaser som bruker programmet.
    - **Leier** slik at den nye profilen blir tilgjengelig kun for den gjeldende leietakerdatabasen.
4. Når du er ferdig, velger du **OK**-knappen.

## <a name="ExportImportProfile"></a>Eksportere og importere profiler

Du kan eksportere og importere profiler som XML-filer til og fra en [!INCLUDE[d365fin](includes/d365fin_md.md)]-database. Du kan spare tid ved å eksportere og importere en profil når du konfigurerer brukergrensesnittet fordi du kan bruke en eksisterende profilkonfigurasjon i stedet for å konfigurere en profil på nytt. Hvis du har en profil som er konfigurert i en [!INCLUDE[d365fin](includes/d365fin_md.md)]-database, og du vil bruke på hele eller deler av det samme profil oppsettet i en annen database, kan du eksportere profilen til en XML-fil. Deretter kan du importere XML-filen for profilen til den andre databasen.

-   Hvis du vil eksportere en profil, åpner du Søk etter og så **Eksporter profiler**-siden. Så velger du profilene fra oversikten og deretter **Eksporter**. Lagre XML-filen på datamaskinen eller i nettverket.

-   Hvis du vil importere en profil, åpner du Søk etter og så **Importer profiler**-siden. Så finner du frem til XML-filen og deretter velger du **OK**-knappen.

    > [!NOTE]  
    >  Du kan ikke importere en profil som allerede finnes i databasen, selv om XML-filen har et annet navn eller annet innhold. Du må slette den eksisterende profilen før du kan importere den nye profilen.



## <a name="see-also"></a>Se også  
[Administrere brukere og tillatelser](ui-how-users-permissions.md)  
[Tilpasse brukergrensesnittet](ui-customizing-overview.md)   
<!--[Security Overview](../Security%20Overview.md)-->

