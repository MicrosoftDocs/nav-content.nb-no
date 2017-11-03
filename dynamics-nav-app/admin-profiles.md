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
# <a name="managing-profiles-and-role-centers"></a><span data-ttu-id="d3876-103">Administrere profiler og rollesentre</span><span class="sxs-lookup"><span data-stu-id="d3876-103">Managing Profiles and Role Centers</span></span>
<span data-ttu-id="d3876-104">Profiler er samlinger av [!INCLUDE[navnow_md](includes/navnow_md.md)]-brukere som deler samme rollesenter.</span><span class="sxs-lookup"><span data-stu-id="d3876-104">Profiles are collections of [!INCLUDE[navnow_md](includes/navnow_md.md)] users who share the same Role Center.</span></span> <span data-ttu-id="d3876-105">Et rollesenter er en side der du kan plassere forskjellige deler.</span><span class="sxs-lookup"><span data-stu-id="d3876-105">A Role Center is a type of page on which you can place different parts.</span></span> <span data-ttu-id="d3876-106">Hver del er en beholder som kan være vert for andre sider eller forhåndsdefinerte systemdeler, for eksempel en Outlook-del eller deler for å legge til oppgaver, varslinger eller notater.</span><span class="sxs-lookup"><span data-stu-id="d3876-106">Each part is a container in which you can host other pages or pre-defined system parts, such as an Outlook part or parts for adding tasks, notifications, or notes.</span></span>  

## <a name="about-profiles-and-role-centers"></a><span data-ttu-id="d3876-107">Om profiler og rollesentre</span><span class="sxs-lookup"><span data-stu-id="d3876-107">About profiles and Role Centers</span></span>
<span data-ttu-id="d3876-108">Du bruker profiler til å knytte brukere til forhåndsdefinerte rollesentre.</span><span class="sxs-lookup"><span data-stu-id="d3876-108">You use profiles to link users to pre-defined Role Centers.</span></span> <span data-ttu-id="d3876-109">Et rollesenter er en hjemmeside for alle brukere av en profil som er konfigurert til å gjenspeile oppgavene og prioritetene til brukere av profilen.</span><span class="sxs-lookup"><span data-stu-id="d3876-109">A Role Center is a home page for all users of a profile, which has been configured to reflect the tasks and priorities of users of the profile.</span></span> <span data-ttu-id="d3876-110">Rollesenteret for ordrebehandler er for eksempel konfigurert slik at det gjenspeiler oppgavene og prioritetene til en ordrebehandler.</span><span class="sxs-lookup"><span data-stu-id="d3876-110">For example, the Order Processor Role Center has been configured to reflect the tasks and priorities of an order processor.</span></span> <span data-ttu-id="d3876-111">Et rollesenter gir deg enkel tilgang til informasjon som brukerne trenger for å kunne daglige arbeidsoppgaver.</span><span class="sxs-lookup"><span data-stu-id="d3876-111">A Role Center provides easy access to information users need to perform their daily work.</span></span> <span data-ttu-id="d3876-112">Rollesenteret bestemmer for eksempel bunkene eller flisen som vises når brukere logger på, og koblingene fra navigasjonssiden.</span><span class="sxs-lookup"><span data-stu-id="d3876-112">For example, the Role Center determines the Cues, or tile, that show when isers first sign in, and the links from the navigation page.</span></span>

<span data-ttu-id="d3876-113">Profilen som brukes vises i hodet for hovedinnholdsområdet i rollesenteret.</span><span class="sxs-lookup"><span data-stu-id="d3876-113">The profile that is used appears in the header of the Role Center’s main content area.</span></span> <span data-ttu-id="d3876-114">En administrator kan deretter tilpasse dette rollesenteret for å dekke behovene til en bestemt rolle i et bestemt firma.</span><span class="sxs-lookup"><span data-stu-id="d3876-114">An administrator can customize this Role Center to meet the needs of a specific role in a specific company.</span></span> <span data-ttu-id="d3876-115">Rollesenteret for ordrebehandler kan deretter tilpasset ytterligere på en enkelt datamaskin for å dekke behovene til en person som utfører jobben som en ordrebehandler.</span><span class="sxs-lookup"><span data-stu-id="d3876-115">The Order Processor Role Center can then be further personalized on a single computer to meet the needs of a person who is carrying out the job as an order processor.</span></span> <span data-ttu-id="d3876-116">Denne personen kan tilpasse rollesenteret ved å lagre spørringer, legge til filtre og legge til eller fjerne felt.</span><span class="sxs-lookup"><span data-stu-id="d3876-116">This person can personalize the Role Center by saving queries, adding filters, and adding or removing fields.</span></span>

<span data-ttu-id="d3876-117">Profiler og rollesentre tilpasses til rollene og ansvarsområdene i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="d3876-117">Profiles and Role Centers align with the roles and responsibilities in your organization.</span></span> [!INCLUDE[navnow_md](includes/navnow_md.md)]<span data-ttu-id="d3876-118"> inneholder et sett med standardprofiler, og hver av dem svarer til og er tilknyttet et rollesenter.</span><span class="sxs-lookup"><span data-stu-id="d3876-118"> provides a set of default profiles, which each correspond to and link to a Role Center.</span></span> <span data-ttu-id="d3876-119">Administratorer kan redigere eksisterende profiler eller opprette nye.</span><span class="sxs-lookup"><span data-stu-id="d3876-119">Administrators can modify existing profiles or create new ones.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="d3876-120">Profiler er ikke eksplisitt knyttet til rollene og tillatelsene som utgjør sikkerhetssystemet, men profilbrukere må ha tillatelser som er tilpasset deres roller i sikkerhetssystemet.</span><span class="sxs-lookup"><span data-stu-id="d3876-120">Profiles are not explicitly linked to the roles and permissions that constitute the security system, but profile users must have permissions that align with their roles in the security system.</span></span> <span data-ttu-id="d3876-121">Hvis du vil ha mer informasjon, kan du se [Security in the Role Tailored Environment](http://go.microsoft.com/fwlink?LinkId=147633) i MSDN-biblioteket.</span><span class="sxs-lookup"><span data-stu-id="d3876-121">For more information, see [Security in the Role Tailored Environment](http://go.microsoft.com/fwlink?LinkId=147633) in the MSDN Library.</span></span>

## <a name="to-create-a-profile"></a><span data-ttu-id="d3876-122">Slik oppretter du en profil</span><span class="sxs-lookup"><span data-stu-id="d3876-122">To create a profile</span></span>
1.  <span data-ttu-id="d3876-123">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Profiler**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="d3876-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Profiles**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="d3876-124">Velg **Ny**for å åpne **Nytt profilkort**-vinduet.</span><span class="sxs-lookup"><span data-stu-id="d3876-124">Choose the **New** action to open the **New Profile Card** window.</span></span>  

3.  <span data-ttu-id="d3876-125">Skriv inn et navn som beskriver den tiltenkte rollen for brukeren, i **Profil-ID**-feltet.</span><span class="sxs-lookup"><span data-stu-id="d3876-125">In the **Profile ID** field, enter a name that describes the intended role of the user.</span></span>  

4.  <span data-ttu-id="d3876-126">I **Beskrivelse**-feltet angir du en beskrivelse av profil-IDen, for eksempel **Ordrebehandler**.</span><span class="sxs-lookup"><span data-stu-id="d3876-126">In the **Description** field, enter a description of the Profile ID, for example, **Order Processor**.</span></span>  

5.  <span data-ttu-id="d3876-127">Sett **Rollesenter-ID**-felttet til rollesenteret du vil tilordne til profilen.</span><span class="sxs-lookup"><span data-stu-id="d3876-127">Set the **Role Center ID** field to the Role Center that you want to assign to the profile.</span></span>  

6.  <span data-ttu-id="d3876-128">Hvis du vil gjøre dette rollesenteret til standard for profilen, merker du av for **Standard rollesenter**.</span><span class="sxs-lookup"><span data-stu-id="d3876-128">To make this Role Center the default for the profile, select the **Default Role Center** check box.</span></span>  

7.  <span data-ttu-id="d3876-129">Velg **OK**.</span><span class="sxs-lookup"><span data-stu-id="d3876-129">Choose the **OK** button.</span></span> <span data-ttu-id="d3876-130">.</span><span class="sxs-lookup"><span data-stu-id="d3876-130">.</span></span>  

<span data-ttu-id="d3876-131">Fremgangsmåten for å endre en eksisterende profil er det samme, bortsett fra at du velger en eksisterende profil på Profiler-siden i stedet for å velge handlingen **Ny**.</span><span class="sxs-lookup"><span data-stu-id="d3876-131">The procedure for modifying an existing profile is the same, except you select an existing profile in the Profiles page instead of choosing the **New** action.</span></span>  


##<a name="copying-a-profile"></a><span data-ttu-id="d3876-132">Kopiere en profil:</span><span class="sxs-lookup"><span data-stu-id="d3876-132">Copying a profile</span></span>
<span data-ttu-id="d3876-133">Du kan spare tid ved å kopiere en profil hvis du vil bruke lignende innstillinger på en profil, og du bare vil endre noen innstillinger.</span><span class="sxs-lookup"><span data-stu-id="d3876-133">Copying a profile can save you time if you want to use similar settings on a profile and you only want to change a few settings.</span></span>

1.  <span data-ttu-id="d3876-134">Åpne profilen du vil kopiere, og velg deretter **Kopier profil**.</span><span class="sxs-lookup"><span data-stu-id="d3876-134">Open the profile that you want to copy, and then choose the **Copy Profile** action.</span></span>

2.  <span data-ttu-id="d3876-135">I **Ny profil-ID**-feltet skriver du inn et navn for profilen du vil kopiere.</span><span class="sxs-lookup"><span data-stu-id="d3876-135">In **New Profile ID** field, enter a name for the profile that you want to copy.</span></span>

3.  <span data-ttu-id="d3876-136">Sett feltet **Nytt profilomfang** til ett av følgende:</span><span class="sxs-lookup"><span data-stu-id="d3876-136">Set the **New Profile Scope** field to one of the following:</span></span>

    - <span data-ttu-id="d3876-137">**System** slik at den nye profilen blir tilgjengelig for alle leietakerdatabaser som bruker programmet.</span><span class="sxs-lookup"><span data-stu-id="d3876-137">**System** to make the new profile available to all tenant databases that use the application.</span></span>
    - <span data-ttu-id="d3876-138">**Leier** slik at den nye profilen blir tilgjengelig kun for den gjeldende leietakerdatabasen.</span><span class="sxs-lookup"><span data-stu-id="d3876-138">**Tenant** to make the new profile available to just the current tenant database.</span></span>
4. <span data-ttu-id="d3876-139">Når du er ferdig, velger du **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="d3876-139">Choose the **OK** buttom when done.</span></span>

## <span data-ttu-id="d3876-140"><a name="ExportImportProfile"></a>Eksportere og importere profiler</span><span class="sxs-lookup"><span data-stu-id="d3876-140"><a name="ExportImportProfile"></a>Exporting and importing profiles</span></span>

<span data-ttu-id="d3876-141">Du kan eksportere og importere profiler som XML-filer til og fra en [!INCLUDE[d365fin](includes/d365fin_md.md)]-database.</span><span class="sxs-lookup"><span data-stu-id="d3876-141">You can export and import profiles as XML files to and from the a [!INCLUDE[d365fin](includes/d365fin_md.md)] database.</span></span> <span data-ttu-id="d3876-142">Du kan spare tid ved å eksportere og importere en profil når du konfigurerer brukergrensesnittet fordi du kan bruke en eksisterende profilkonfigurasjon i stedet for å konfigurere en profil på nytt.</span><span class="sxs-lookup"><span data-stu-id="d3876-142">Exporting and importing a profile can save you time when configuring the user interface because you reuse an existing profile configuration instead of having to configure a profile from scratch.</span></span> <span data-ttu-id="d3876-143">Hvis du har en profil som er konfigurert i en [!INCLUDE[d365fin](includes/d365fin_md.md)]-database, og du vil bruke på hele eller deler av det samme profil oppsettet i en annen database, kan du eksportere profilen til en XML-fil.</span><span class="sxs-lookup"><span data-stu-id="d3876-143">If you have a profile that is configured in a [!INCLUDE[d365fin](includes/d365fin_md.md)] database and you would like to reuse all or some of the same profile configurations in another database, you can export the profile to an XML file.</span></span> <span data-ttu-id="d3876-144">Deretter kan du importere XML-filen for profilen til den andre databasen.</span><span class="sxs-lookup"><span data-stu-id="d3876-144">Then, you can import the profile XML file into the other database.</span></span>

-   <span data-ttu-id="d3876-145">Hvis du vil eksportere en profil, åpner du Søk etter og så **Eksporter profiler**-siden. Så velger du profilene fra oversikten og deretter **Eksporter**.</span><span class="sxs-lookup"><span data-stu-id="d3876-145">To export a profile, open search for and open the **Export Profiles** page, select the profile from the list, and then choose the **Export** action.</span></span> <span data-ttu-id="d3876-146">Lagre XML-filen på datamaskinen eller i nettverket.</span><span class="sxs-lookup"><span data-stu-id="d3876-146">Save the XML file to a location on your computer or network.</span></span>

-   <span data-ttu-id="d3876-147">Hvis du vil importere en profil, åpner du Søk etter og så **Importer profiler**-siden. Så finner du frem til XML-filen og deretter velger du **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="d3876-147">To import a profile, open search for and open the **Import Profiles** page, select the profile XML file, and then choose the **OK** button.</span></span>

    > [!NOTE]  
    >  <span data-ttu-id="d3876-148">Du kan ikke importere en profil som allerede finnes i databasen, selv om XML-filen har et annet navn eller annet innhold.</span><span class="sxs-lookup"><span data-stu-id="d3876-148">You cannot import a profile that already exists in the database, even though the XML file is named differently or has different content.</span></span> <span data-ttu-id="d3876-149">Du må slette den eksisterende profilen før du kan importere den nye profilen.</span><span class="sxs-lookup"><span data-stu-id="d3876-149">You must delete the existing profile before you can import the new profile.</span></span>



## <a name="see-also"></a><span data-ttu-id="d3876-150">Se også</span><span class="sxs-lookup"><span data-stu-id="d3876-150">See Also</span></span>  
[<span data-ttu-id="d3876-151">Administrere brukere og tillatelser</span><span class="sxs-lookup"><span data-stu-id="d3876-151">How to: Manage Users and Permissions</span></span>](ui-how-users-permissions.md)  
[<span data-ttu-id="d3876-152">Tilpasse brukergrensesnittet</span><span class="sxs-lookup"><span data-stu-id="d3876-152">Customizing the User Interface</span></span>](ui-customizing-overview.md)   
<!--[Security Overview](../Security%20Overview.md)-->

