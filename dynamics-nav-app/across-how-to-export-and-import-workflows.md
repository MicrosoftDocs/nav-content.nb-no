---
title: Importere og eksportere arbeidsflyter
description: "For å overføre arbeidsflyter til andre [!INCLUDE[d365fin](includes/d365fin_md.md)]-databaser, for eksempel for å spare tid når du oppretter nye arbeidsflyter, kan du eksportere og importere arbeidsflyter."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7ce7c6bd83efaacaed53f5d5ca5c2eb1521c0e6e
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-export-and-import-workflows"></a><span data-ttu-id="6430d-103">Importere og eksportere arbeidsflyter</span><span class="sxs-lookup"><span data-stu-id="6430d-103">How to: Export and Import Workflows</span></span>
<span data-ttu-id="6430d-104">For å overføre arbeidsflyter til andre [!INCLUDE[d365fin](includes/d365fin_md.md)]-databaser, for eksempel for å spare tid når du oppretter nye arbeidsflyter, kan du eksportere og importere arbeidsflyter.</span><span class="sxs-lookup"><span data-stu-id="6430d-104">To transfer workflows to other [!INCLUDE[d365fin](includes/d365fin_md.md)] databases, for example to save time when creating new workflows, you can export and import workflows.</span></span>  

 <span data-ttu-id="6430d-105">En annen måte å raskt opprette arbeidsflyter på er å opprette arbeidsflyter fra arbeidsflytmaler.</span><span class="sxs-lookup"><span data-stu-id="6430d-105">Another way to quickly create workflows is to create workflows from workflow templates.</span></span> <span data-ttu-id="6430d-106">Hvis du vil ha mer informasjon, kan du se [Opprette arbeidsflyter fra arbeidsflytmaler](across-how-to-create-workflows-from-workflow-templates.md).</span><span class="sxs-lookup"><span data-stu-id="6430d-106">For more information, see [How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span></span>  

 <span data-ttu-id="6430d-107">I **Arbeidsflyt**-vinduet oppretter du en arbeidsflyt ved å føre opp de involverte trinnene på linjene.</span><span class="sxs-lookup"><span data-stu-id="6430d-107">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="6430d-108">Hvert trinn består av en arbeidsflythendelse, endret av hendelsesbetingelsene, og et arbeidsflytsvar, endret av svaralternativer.</span><span class="sxs-lookup"><span data-stu-id="6430d-108">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="6430d-109">Du definerer arbeidsflyttrinn ved å fylle ut felt på arbeidsflytlinjer fra faste lister over verdier for hendelse og svar som representerer scenarier som støttes av programkoden.</span><span class="sxs-lookup"><span data-stu-id="6430d-109">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="6430d-110">Hvis du vil ha mer informasjon, kan du se [Opprette arbeidsflyter](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="6430d-110">For more information, see [How to: Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-export-a-workflow"></a><span data-ttu-id="6430d-111">Slik eksporterer du en arbeidsflyt</span><span class="sxs-lookup"><span data-stu-id="6430d-111">To export a workflow</span></span>  
1.  <span data-ttu-id="6430d-112">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Arbeidsflyter**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="6430d-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6430d-113">Velg en arbeidsflyt, og velg deretter **Eksporter til fil**.</span><span class="sxs-lookup"><span data-stu-id="6430d-113">Select a workflow, and then choose the **Export to File** action.</span></span>  
3.  <span data-ttu-id="6430d-114">Klikk **Lagre** i vinduet **Eksporter fil**.</span><span class="sxs-lookup"><span data-stu-id="6430d-114">In the **Export File** window, choose the **Save** button.</span></span>  
4.  <span data-ttu-id="6430d-115">I **Eksport**-vinduet velger du en filplassering, og deretter velger du **Lagre**-knappen.</span><span class="sxs-lookup"><span data-stu-id="6430d-115">In the **Export** window, select a file location, and then choose the **Save** button.</span></span>  

## <a name="to-import-a-workflow"></a><span data-ttu-id="6430d-116">Slik importerer du en arbeidsflyt</span><span class="sxs-lookup"><span data-stu-id="6430d-116">To import a workflow</span></span>  
1.  <span data-ttu-id="6430d-117">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Arbeidsflyter**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="6430d-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6430d-118">Velg handlingen **Importer fra fil**.</span><span class="sxs-lookup"><span data-stu-id="6430d-118">Choose the **Import from File** action.</span></span>  
3.  <span data-ttu-id="6430d-119">I **Import**-vinduet velger du XML-filen som inneholder arbeidsflyten, og deretter velger du **Åpne**-knappen.</span><span class="sxs-lookup"><span data-stu-id="6430d-119">In the **Import** window, choose the XML file that contains the workflow, and then choose the **Open** button.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="6430d-120">Hvis arbeidsflytkoden allerede finnes i databasen, overskrives arbeidsflyttrinnene med trinnene i den importerte arbeidsflyten.</span><span class="sxs-lookup"><span data-stu-id="6430d-120">If the workflow code already exists in the database, the workflow steps will be overwritten with the steps in the imported workflow.</span></span>  

## <a name="see-also"></a><span data-ttu-id="6430d-121">Se også</span><span class="sxs-lookup"><span data-stu-id="6430d-121">See Also</span></span>  
 <span data-ttu-id="6430d-122">[Opprette arbeidsflyter](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="6430d-122">[How to: Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="6430d-123">[Opprette arbeidsflyter fra arbeidsflytmaler](across-how-to-create-workflows-from-workflow-templates.md) </span><span class="sxs-lookup"><span data-stu-id="6430d-123">[How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md) </span></span>  
 <span data-ttu-id="6430d-124">[Vise arkiverte forekomster av arbeidsflyttrinn](across-how-to-view-archived-workflow-step-instances.md) </span><span class="sxs-lookup"><span data-stu-id="6430d-124">[How to: View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span></span>  
 <span data-ttu-id="6430d-125">[Slette arbeidsflyter](across-how-to-delete-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="6430d-125">[How to: Delete Workflows](across-how-to-delete-workflows.md) </span></span>  
 <span data-ttu-id="6430d-126">[Gjennomgang: Definere og bruke en arbeidsflyt for kjøpsgodkjenning](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="6430d-126">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 <span data-ttu-id="6430d-127">[Konfigurere arbeidsflyter](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="6430d-127">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
 <span data-ttu-id="6430d-128">[Bruke arbeidsflyter](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="6430d-128">[Using Workflows](across-use-workflows.md) </span></span>  
 [<span data-ttu-id="6430d-129">Arbeidsflyt</span><span class="sxs-lookup"><span data-stu-id="6430d-129">Workflow</span></span>](across-workflow.md)   

