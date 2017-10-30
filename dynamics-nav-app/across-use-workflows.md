---
title: Bruke arbeidsflyter
description: "Du kan definere og bruke arbeidsflyter som kobler forretningsprosessoppgaver som utføres av forskjellige brukere. Systemoppgaver, for eksempel automatisk bokføring, kan tas med som trinn i arbeidsflyter, før eller etterfulgt av brukeroppgaver. Å be om og gi godkjenning til å opprette nye oppføringer er typiske arbeidsflyttrinn."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 0032a2018feee31b1eed52bb41d1ab916c47a912
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="using-workflows"></a><span data-ttu-id="4ac5e-105">Bruke arbeidsflyter</span><span class="sxs-lookup"><span data-stu-id="4ac5e-105">Using Workflows</span></span>
<span data-ttu-id="4ac5e-106">Du kan definere og bruke arbeidsflyter som kobler forretningsprosessoppgaver som utføres av forskjellige brukere.</span><span class="sxs-lookup"><span data-stu-id="4ac5e-106">You can set up and use workflows that connect business-process tasks performed by different users.</span></span> <span data-ttu-id="4ac5e-107">Systemoppgaver, for eksempel automatisk bokføring, kan tas med som trinn i arbeidsflyter, før eller etterfulgt av brukeroppgaver.</span><span class="sxs-lookup"><span data-stu-id="4ac5e-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span></span> <span data-ttu-id="4ac5e-108">Å be om og gi godkjenning til å opprette nye oppføringer er typiske arbeidsflyttrinn.</span><span class="sxs-lookup"><span data-stu-id="4ac5e-108">Requesting and granting approval to create new records are typical workflow steps.</span></span>  

 <span data-ttu-id="4ac5e-109">Før du kan begynne å bruke arbeidsflyter, må du konfigurere brukere av arbeidsflyt, opprette arbeidsflytene, potensielt med foranstilt tilpasset kode, og angi hvordan brukere mottar varsler.</span><span class="sxs-lookup"><span data-stu-id="4ac5e-109">Before you can begin to use workflows, you must set up workflow users, create the workflows, potentially preceded by code customization and specify how users receive notifications.</span></span> <span data-ttu-id="4ac5e-110">Hvis du vil ha mer informasjon, kan du se [Konfigurere arbeidsflyter](across-set-up-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="4ac5e-110">For more information, see [Setting Up Workflows](across-set-up-workflows.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="4ac5e-111">Vanlige arbeidsflyttrinn er om brukere som ber om godkjenning av oppgaver og godkjennere som godkjenner eller avviser forespørsler om godkjenning.</span><span class="sxs-lookup"><span data-stu-id="4ac5e-111">Typical workflow steps are about users who request approval of tasks and approvers accepting or rejecting approval requests.</span></span> <span data-ttu-id="4ac5e-112">Mange emner om hvordan du bruker arbeidsflyter, refererer derfor til godkjenninger.</span><span class="sxs-lookup"><span data-stu-id="4ac5e-112">Therefore, many topics about how to use workflows refer to approvals.</span></span>  

 <span data-ttu-id="4ac5e-113">Tabellen nedenfor beskriver en sekvens av oppgaver, og har koblinger til emnene som beskriver dem.</span><span class="sxs-lookup"><span data-stu-id="4ac5e-113">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>  

|<span data-ttu-id="4ac5e-114">**Hvis du vil**</span><span class="sxs-lookup"><span data-stu-id="4ac5e-114">**To**</span></span>|<span data-ttu-id="4ac5e-115">**Se**</span><span class="sxs-lookup"><span data-stu-id="4ac5e-115">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="4ac5e-116">Angi at en arbeidsflyt skal starte når den første innpunkthendelsen oppstår.</span><span class="sxs-lookup"><span data-stu-id="4ac5e-116">Set a workflow to start when the first entry-point event occurs.</span></span>|[<span data-ttu-id="4ac5e-117">Aktivere arbeidsflyter</span><span class="sxs-lookup"><span data-stu-id="4ac5e-117">How to: Enable Workflows</span></span>](across-how-to-enable-workflows.md)|  
|<span data-ttu-id="4ac5e-118">Be om godkjenning for en oppgave, som godkjenner, godkjenn, avvis eller deleger godkjenning, og send eller vis godkjenningsmeldinger.</span><span class="sxs-lookup"><span data-stu-id="4ac5e-118">Request approval of a task, as an approver, accept, decline, or delegate approvals, and send or view approval notifications.</span></span>|[<span data-ttu-id="4ac5e-119">Bruke arbeidsflyter for godkjenning</span><span class="sxs-lookup"><span data-stu-id="4ac5e-119">How to: Use Approval Workflows</span></span>](across-how-use-approval-workflows.md)|  
|<span data-ttu-id="4ac5e-120">Opprett trinn i arbeidsflyten som forhindrer at en bestemt oppføringstype brukes før en bestemt hendelse inntreffer, for eksempel at oppføringen er godkjent.</span><span class="sxs-lookup"><span data-stu-id="4ac5e-120">Create workflow steps that restrict a certain record type from being used before a certain event occurs, for example that the record is approved.</span></span>|[<span data-ttu-id="4ac5e-121">Begrense og tillate bruk av en post</span><span class="sxs-lookup"><span data-stu-id="4ac5e-121">How to: Restrict and Allow Usage of a Record</span></span>](across-how-to-restrict-and-allow-usage-of-a-record.md)|  
|<span data-ttu-id="4ac5e-122">Vise forekomster av arbeidsflyttrinn med statusen Fullført.</span><span class="sxs-lookup"><span data-stu-id="4ac5e-122">View workflow step instances of status Completed.</span></span>|[<span data-ttu-id="4ac5e-123">Vise arkiverte forekomster av arbeidsflyttrinn</span><span class="sxs-lookup"><span data-stu-id="4ac5e-123">How to: View Archived Workflow Step Instances</span></span>](across-how-to-view-archived-workflow-step-instances.md)|  
|<span data-ttu-id="4ac5e-124">Slette en arbeidsflyt du er sikker på ikke lenger vil bli brukt.</span><span class="sxs-lookup"><span data-stu-id="4ac5e-124">Delete a workflow that you are sure will no longer be used.</span></span>|[<span data-ttu-id="4ac5e-125">Slette arbeidsflyter</span><span class="sxs-lookup"><span data-stu-id="4ac5e-125">How to: Delete Workflows</span></span>](across-how-to-delete-workflows.md)|  

## <a name="see-also"></a><span data-ttu-id="4ac5e-126">Se også</span><span class="sxs-lookup"><span data-stu-id="4ac5e-126">See Also</span></span>  
<span data-ttu-id="4ac5e-127">[Konfigurere arbeidsflyter](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="4ac5e-127">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
<span data-ttu-id="4ac5e-128">[Arbeidsflyt](across-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="4ac5e-128">[Workflow](across-workflow.md) </span></span>  
<span data-ttu-id="4ac5e-129">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4ac5e-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

