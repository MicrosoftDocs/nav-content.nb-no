---
title: "Designdetaljer - Håndtere gjenbestillingsprinsipper"
description: "Oversikt over oppgaver for å definere en gjenbestillingspolicy ved forsyningsplanlegging."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 281f87c446ef95cf3e8bbe119184d2202699f4df
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="design-details-handling-reordering-policies"></a><span data-ttu-id="92704-103">Designdetaljer: Håndtere gjenbestillingsprinsipper</span><span class="sxs-lookup"><span data-stu-id="92704-103">Design Details: Handling Reordering Policies</span></span>
<span data-ttu-id="92704-104">Det må angis et gjenbestillingsprinsipp for at en vare skal kunne delta i forsyningsplanlegging.</span><span class="sxs-lookup"><span data-stu-id="92704-104">For an item to participate in supply planning, a reorder policy must be defined.</span></span> <span data-ttu-id="92704-105">Det finnes fire gjenbestillingsprinsipper:</span><span class="sxs-lookup"><span data-stu-id="92704-105">The following four reordering policies exist:</span></span>  
  
* <span data-ttu-id="92704-106">Fast gjenbest.ant.</span><span class="sxs-lookup"><span data-stu-id="92704-106">Fixed Reorder Qty.</span></span>  
* <span data-ttu-id="92704-107">Maks.ant.</span><span class="sxs-lookup"><span data-stu-id="92704-107">Maximum Qty.</span></span>  
* <span data-ttu-id="92704-108">Bestilling</span><span class="sxs-lookup"><span data-stu-id="92704-108">Order</span></span>  
* <span data-ttu-id="92704-109">Parti for parti</span><span class="sxs-lookup"><span data-stu-id="92704-109">Lot-for-Lot</span></span>  
  
<span data-ttu-id="92704-110">Prinsippene Fast gjenbest.ant., og Maks.ant. som er relatert til lagerplanlegging.</span><span class="sxs-lookup"><span data-stu-id="92704-110">Fixed Reorder Qty. and Maximum Qty. policies relate to inventory planning.</span></span> <span data-ttu-id="92704-111">Selv om lagerplanlegging teknisk sett er enklere enn fremgangsmåten for balansering, må disse policyene eksistere sammen med trinnvise balansering av forsynings- og ordresporing.</span><span class="sxs-lookup"><span data-stu-id="92704-111">Although inventory planning is technically simpler than the balancing procedure, these policies must coexist with the step-by-step balancing of supply and order tracking.</span></span> <span data-ttu-id="92704-112">For å styre integrasjonen mellom dem og gi innsikt i planleggingslogikken som er involvert, finnes det strenge regler som bestemmer hvordan gjenbestillingsprinsipper skal håndteres.</span><span class="sxs-lookup"><span data-stu-id="92704-112">To control the integration between the two, and to provide visibility into the involved planning logic, strict principles govern how reordering policies are handled.</span></span>  
  
## <a name="in-this-section"></a><span data-ttu-id="92704-113">I denne delen</span><span class="sxs-lookup"><span data-stu-id="92704-113">In This Section</span></span>  
[<span data-ttu-id="92704-114">Designdetaljer: Rollen til gjenbestillingspunktet</span><span class="sxs-lookup"><span data-stu-id="92704-114">Design Details: The Role of the Reorder Point</span></span>](design-details-the-role-of-the-reorder-point.md)  
[<span data-ttu-id="92704-115">Designdetaljer: Overvåke forventet lagernivå og gjenbestillingspunkt</span><span class="sxs-lookup"><span data-stu-id="92704-115">Design Details: Monitoring the Projected Inventory Level and the Reorder Point</span></span>](design-details-monitoring-the-projected-inventory-level-and-the-reorder-point.md)  
[<span data-ttu-id="92704-116">Designdetaljer: Rollen til tidsperioden</span><span class="sxs-lookup"><span data-stu-id="92704-116">Design Details: The Role of the Time Bucket</span></span>](design-details-the-role-of-the-time-bucket.md)  
[<span data-ttu-id="92704-117">Designdetaljer: Holde seg under overflytnivået</span><span class="sxs-lookup"><span data-stu-id="92704-117">Design Details: Staying under the Overflow Level</span></span>](design-details-staying-under-the-overflow-level.md)  
[<span data-ttu-id="92704-118">Designdetaljer: Håndtere forventet negativ lagerbeholdning</span><span class="sxs-lookup"><span data-stu-id="92704-118">Design Details: Handling Projected Negative Inventory</span></span>](design-details-handling-projected-negative-inventory.md)  
[<span data-ttu-id="92704-119">Designdetaljer: Gjenbestillingsprinsipper</span><span class="sxs-lookup"><span data-stu-id="92704-119">Design Details: Reordering Policies</span></span>](design-details-reordering-policies.md)  
  
## <a name="see-also"></a><span data-ttu-id="92704-120">Se også</span><span class="sxs-lookup"><span data-stu-id="92704-120">See Also</span></span>  
<span data-ttu-id="92704-121">[Designdetaljer: Planleggingsparametere](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="92704-121">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="92704-122">[Designdetaljer: Tabell for planleggingstilordning](design-details-planning-assignment-table.md) </span><span class="sxs-lookup"><span data-stu-id="92704-122">[Design Details: Planning Assignment Table](design-details-planning-assignment-table.md) </span></span>  
<span data-ttu-id="92704-123">[Designdetaljer: Sentrale begreper for planleggingssystemet](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="92704-123">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
<span data-ttu-id="92704-124">[Designdetaljer: Balansere behov og forsyning](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="92704-124">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
[<span data-ttu-id="92704-125">Designdetaljer: Forsyningsplanlegging</span><span class="sxs-lookup"><span data-stu-id="92704-125">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
