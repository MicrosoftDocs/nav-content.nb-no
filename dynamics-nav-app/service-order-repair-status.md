---
title: Definere statuser for serviceordrer og reparasjoner
description: "Du må definere ni alternativer for reparasjonsstatus som identifiserer fremdriften av reparasjon og vedlikehold på servicevarer i serviceordrer."
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
ms.openlocfilehash: d7dbc4cfc06d4c74476a04512bd368a0ab26f837
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-statuses-for-service-orders-and-repairs"></a><span data-ttu-id="a203c-103">Definere statuser for serviceordrer og reparasjoner</span><span class="sxs-lookup"><span data-stu-id="a203c-103">How to: Set Up Statuses for Service Orders and Repairs</span></span>
<span data-ttu-id="a203c-104">Du må definere ni alternativer for reparasjonsstatus som identifiserer fremdriften av reparasjon og vedlikehold på servicevarer i serviceordrer.</span><span class="sxs-lookup"><span data-stu-id="a203c-104">You must set up repair status options that identify the progress of repair and maintenance of service items in service orders.</span></span> <span data-ttu-id="a203c-105">Du må definerer minst ni alternativer for reparasjonsstatus som identifiserer situasjoner eller handlinger som er iverksatt under vedlikehold av servicevarer.</span><span class="sxs-lookup"><span data-stu-id="a203c-105">You must set up at least nine repair status options that identify situations or actions taken when servicing service items.</span></span>  

<span data-ttu-id="a203c-106">Du kan angi prioritetsnivå for alternativene for serviceordrestatus.</span><span class="sxs-lookup"><span data-stu-id="a203c-106">You can set the priority level for service order status options.</span></span> <span data-ttu-id="a203c-107">De fire prioritetene er Høy, Middels høy, Middels lav og Lav.</span><span class="sxs-lookup"><span data-stu-id="a203c-107">There four priorities are High, Medium High, Medium Low, and Low.</span></span>  
  
<span data-ttu-id="a203c-108">Når du endrer reparasjonsstatusen til en servicevare i en serviceordre, oppdateres serviceordrestatusen.</span><span class="sxs-lookup"><span data-stu-id="a203c-108">When you change the repair status of a service item in a service order, the service order status is updated.</span></span> <span data-ttu-id="a203c-109">Reparasjonsstatusen til hver enkelt servicevare er knyttet til serviceordrestatusen.</span><span class="sxs-lookup"><span data-stu-id="a203c-109">The repair status of each service item is linked to the service order status.</span></span> <span data-ttu-id="a203c-110">Hvis servicevarene er koblet til to eller flere alternativer for serviceordrestatus, velges serviceordrestatusen med høyest prioritet.</span><span class="sxs-lookup"><span data-stu-id="a203c-110">If the service items are linked to two or more service order status options, the service order status with the highest priority is selected.</span></span>  

## <a name="to-set-up-a-repair-status"></a><span data-ttu-id="a203c-111">Slik definerer du reparasjonsstatus</span><span class="sxs-lookup"><span data-stu-id="a203c-111">To set up a repair status</span></span>  
1. <span data-ttu-id="a203c-112">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Reparasjonsstatus**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="a203c-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Repair Status**, and then choose the related link.</span></span> <span data-ttu-id="a203c-113">2.</span><span class="sxs-lookup"><span data-stu-id="a203c-113">2.</span></span> <span data-ttu-id="a203c-114">Opprett en ny reparasjonsstatus.</span><span class="sxs-lookup"><span data-stu-id="a203c-114">Create a new repair status.</span></span>  
3. <span data-ttu-id="a203c-115">Fyll ut feltene **Kode** og **Beskrivelse**.</span><span class="sxs-lookup"><span data-stu-id="a203c-115">Fill in the **Code** and **Description** fields.</span></span>  
4. <span data-ttu-id="a203c-116">I **Serviceordrestatus**-feltet velger du ordrestatusen å knytte reparasjonsstatusen til.</span><span class="sxs-lookup"><span data-stu-id="a203c-116">In the **Service Order Status** field, choose the order status to link the repair status to.</span></span> <span data-ttu-id="a203c-117">**Prioritet**-feltet viser prioriteten til serviceordrestatusen du har valgt.</span><span class="sxs-lookup"><span data-stu-id="a203c-117">The **Priority** field displays the priority of the service order status you have chosen.</span></span>  
5. <span data-ttu-id="a203c-118">Velg en reparasjonsstatus.</span><span class="sxs-lookup"><span data-stu-id="a203c-118">Choose a repair status.</span></span> <span data-ttu-id="a203c-119">Du kan bare velge én.</span><span class="sxs-lookup"><span data-stu-id="a203c-119">You can choose only one.</span></span>  
6. <span data-ttu-id="a203c-120">Velg feltet **Bokføring tillatt** hvis du vil kunne bokføre serviceordrer som omfatter servicevarer, med reparasjonsstatusen.</span><span class="sxs-lookup"><span data-stu-id="a203c-120">To be able to post service orders, including service items, with this repair status, choose the **Posting Allowed** field.</span></span>  
7. <span data-ttu-id="a203c-121">Merk av for **I kø-status tillatt** for å tillate manuell endring av alternativet for serviceordrestatusen til alternativet **I kø** i serviceordrer som omfatter servicevarer med denne reparasjonsstatusen.</span><span class="sxs-lookup"><span data-stu-id="a203c-121">To be able to manually change the service order status option to **Pending** in service orders including service items with this repair status, choose the **Pending Status Allowed** check box.</span></span>  
8. <span data-ttu-id="a203c-122">Merk av for **I arbeid-status tillatt**, **Ferdig-status tillatt**og **Avvent-status tillatt**på samme måte.</span><span class="sxs-lookup"><span data-stu-id="a203c-122">Choose the **In Process Status Allowed**, **Finished Status Allowed**, and **On Hold Status Allowed** check boxes in the same way.</span></span>
  
## <a name="to-set-up-service-status-priorities"></a><span data-ttu-id="a203c-123">Slik definerer du servicestatusprioritet</span><span class="sxs-lookup"><span data-stu-id="a203c-123">To set up service status priorities</span></span>  
1. <span data-ttu-id="a203c-124">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Serviceordrestatus**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="a203c-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Order Status**, and then choose the related link.</span></span>  
2. <span data-ttu-id="a203c-125">Velg serviceordrestatusen du vil angi en prioritet for.</span><span class="sxs-lookup"><span data-stu-id="a203c-125">Select the service order status you want to set a priority for.</span></span>  
3. <span data-ttu-id="a203c-126">I feltet **Prioritet** velger du prioriteten du vil ha for denne serviceordrestatusen.</span><span class="sxs-lookup"><span data-stu-id="a203c-126">In the **Priority** field, choose the priority you want for this service order status.</span></span> <span data-ttu-id="a203c-127">Gjenta dette trinnet for hver status.</span><span class="sxs-lookup"><span data-stu-id="a203c-127">Repeat this step for each status.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="a203c-128">Se også</span><span class="sxs-lookup"><span data-stu-id="a203c-128">See Also</span></span>  
[<span data-ttu-id="a203c-129">Forstå serviceordre- og reparasjonsstatus</span><span class="sxs-lookup"><span data-stu-id="a203c-129">Understanding Service Order Status and Repair Status</span></span>]()  
[<span data-ttu-id="a203c-130">Konfigurere servicehåndtering</span><span class="sxs-lookup"><span data-stu-id="a203c-130">Setting Up Service Management</span></span>](service-setup-service.md)  

