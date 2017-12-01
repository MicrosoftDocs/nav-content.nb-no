---
title: Administrative oppgaver i Dynamics NAV
description: "Enkelte oppgaver i [!INCLUDE[d365fin](includes/d365fin_md.MD)] krever sentral administrasjon og oppsett. Se hva de er, og finn ut hva som må gjøres."
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 3ddb647d28a4065be248a265316b38e8d37d28c2
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="setup-and-administration-in-dynamics-nav"></a><span data-ttu-id="8f5ad-104">Oppsett og administrasjon i Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="8f5ad-104">Setup and Administration in Dynamics NAV</span></span>
<span data-ttu-id="8f5ad-105">Sentrale administrasjonsoppgaver utføres vanligvis av én rolle i selskapet.</span><span class="sxs-lookup"><span data-stu-id="8f5ad-105">Central administration tasks are usually performed by one role in the company.</span></span> <span data-ttu-id="8f5ad-106">Omfanget av disse oppgavene kan avhenge av selskapets størrelse og administrators jobbansvar.</span><span class="sxs-lookup"><span data-stu-id="8f5ad-106">The scope of these tasks can depend on the company's size and the administrator's job responsibilities.</span></span> <span data-ttu-id="8f5ad-107">Disse oppgavene kan omfatte administrasjon av databasesynkronisering for jobb- og e-postkøer, oppsett av brukere, tilpassing av brukergrensesnittet og administrasjon av krypteringsnøkler.</span><span class="sxs-lookup"><span data-stu-id="8f5ad-107">These tasks can include managing database synchronization of job and email queues, setting up users, customizing the user interface, and managing encryption keys.</span></span>  

<span data-ttu-id="8f5ad-108">Det å angi riktige oppsettverdier for begynnelsen av er viktig for suksessen til all ny forretningsprogramvare.</span><span class="sxs-lookup"><span data-stu-id="8f5ad-108">Entering the correct setup values from the start is important to the success of any new business software.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="8f5ad-109"> inkluderer flere oppsettveiledninger som hjelper deg med å konfigurere kjernedata.</span><span class="sxs-lookup"><span data-stu-id="8f5ad-109"> includes a number of setup guides that help you set up core data.</span></span> <span data-ttu-id="8f5ad-110">Hvis du vil ha mer informasjon, kan du se [Definere Dynamics NAV](setup.md).</span><span class="sxs-lookup"><span data-stu-id="8f5ad-110">For more information, see [Setting Up Dynamics NAV](setup.md).</span></span>

<!--Whether you use [!INCLUDE[rim](../../includes/rim_md.md)] to implement setup values or you manually enter them in the new company, you can support your setup decisions with some general recommendations for selected setup fields that are known to potentially cause the solution to be inefficient if defined incorrectly.-->  

<span data-ttu-id="8f5ad-111">En superbruker eller en administrator kan opprette et rammeverk for datautveksling slik at brukere kan eksportere og importere data i bank- og lønnsfiler, for eksempel for forskjellige bankstyringsprosesser.</span><span class="sxs-lookup"><span data-stu-id="8f5ad-111">A super user or an administrator can set up the Data Exchange Framework to enable users to export and import data in bank and payroll files, for example for various cash management processes.</span></span>  

<span data-ttu-id="8f5ad-112">Tabellen nedenfor beskriver en sekvens av oppgaver, og har koblinger til emnene som beskriver dem.</span><span class="sxs-lookup"><span data-stu-id="8f5ad-112">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="8f5ad-113">**Hvis du vil**</span><span class="sxs-lookup"><span data-stu-id="8f5ad-113">**To**</span></span>|<span data-ttu-id="8f5ad-114">**Se**</span><span class="sxs-lookup"><span data-stu-id="8f5ad-114">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="8f5ad-115">Legg til brukere, behandle tillatelser og tilgang til data, tilordne roller.</span><span class="sxs-lookup"><span data-stu-id="8f5ad-115">Add users, manage permissions and access to data, assign roles.</span></span>|[<span data-ttu-id="8f5ad-116">Brukere, profiler og rollesentre i Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="8f5ad-116">Users, Profiles, and Role Centers in Dynamics NAV</span></span>](admin-users-profiles-roles.md)|  
|<span data-ttu-id="8f5ad-117">Spore alle direkte endringer som brukere gjør i data i databasen, for å finne ut hvor feil og dataendringer oppstår.</span><span class="sxs-lookup"><span data-stu-id="8f5ad-117">Track all direct modifications that users make to data in the database to identify the origin of errors and data changes.</span></span>|[<span data-ttu-id="8f5ad-118">Logge endringer i Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="8f5ad-118">Logging Changes in Dynamics NAV</span></span>](across-log-changes.md)|  
|<span data-ttu-id="8f5ad-119">Støtt opp om oppsettsbeslutningene dine med anbefalinger for valgte felt som er kjent for å kunne forårsake at løsningen blir ineffektiv hvis feilaktig satt opp.</span><span class="sxs-lookup"><span data-stu-id="8f5ad-119">Support your setup decisions with recommendations for selected fields that are known to potentially cause the solution to be inefficient if set up incorrectly</span></span>|[<span data-ttu-id="8f5ad-120">Konfigurere komplekse moduler ved å bruke anbefalte fremgangsmåter</span><span class="sxs-lookup"><span data-stu-id="8f5ad-120">Set Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)|  
|<span data-ttu-id="8f5ad-121">Vis sider, kodeenheter og spørringer som web-tjenester.</span><span class="sxs-lookup"><span data-stu-id="8f5ad-121">Expose pages, codeunits, and queries as web services.</span></span>|[<span data-ttu-id="8f5ad-122">Publisere en webtjeneste</span><span class="sxs-lookup"><span data-stu-id="8f5ad-122">How to: Publish a Web Service</span></span>](across-how-publish-web-service.md)|  
|<span data-ttu-id="8f5ad-123">Definer en SMTP-server for å aktivere e-kommunikasjon inn og ut av Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="8f5ad-123">Set up an SMTP server to enable e-mail communication in and out of Dynamics NAV</span></span>| [<span data-ttu-id="8f5ad-124">Konfigurere e-post manuelt eller bruke assistert oppsett</span><span class="sxs-lookup"><span data-stu-id="8f5ad-124">How to: Set Up Email Manually or Using the Assisted Setup</span></span>](madeira-how-setup-email.md)|  
|<span data-ttu-id="8f5ad-125">Legge inn enkeltstående eller gjentakende forespørsler om å kjøre rapporter eller kodeenheter.</span><span class="sxs-lookup"><span data-stu-id="8f5ad-125">Enter single or recurring requests to run reports or codeunits.</span></span>|[<span data-ttu-id="8f5ad-126">Bruke jobbkøer til å planlegge oppgaver</span><span class="sxs-lookup"><span data-stu-id="8f5ad-126">Use Job Queues to Schedule Tasks</span></span>](admin-job-queues-schedule-tasks.md)|  
|<span data-ttu-id="8f5ad-127">Administrere, slette eller komprimere dokumenter</span><span class="sxs-lookup"><span data-stu-id="8f5ad-127">Manage, delete, or compress documents</span></span>|[<span data-ttu-id="8f5ad-128">Administrere dokumenter</span><span class="sxs-lookup"><span data-stu-id="8f5ad-128">Manage Documents</span></span>](admin-manage-documents.md)|  

## <a name="see-also"></a><span data-ttu-id="8f5ad-129">Se også</span><span class="sxs-lookup"><span data-stu-id="8f5ad-129">See Also</span></span>
[<span data-ttu-id="8f5ad-130">Oversikt over forretningsfunksjoner</span><span class="sxs-lookup"><span data-stu-id="8f5ad-130">Overview of Business Functionality</span></span>](madeira-business-functionality.md)  
[<span data-ttu-id="8f5ad-131">Generelle forretningsfunksjoner</span><span class="sxs-lookup"><span data-stu-id="8f5ad-131">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="8f5ad-132">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8f5ad-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="8f5ad-133">[Velkommen til [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="8f5ad-133">[Welcome to [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span></span>  

