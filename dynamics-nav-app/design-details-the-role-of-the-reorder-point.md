---
title: Designdetaljer - Rollen til gjenbestillingspunktet
description: "Dette emnet belyser viktigheten av å angi et gjenbestillingspunkt, slik at du vet når du må bestille mer."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: desigh, reorder, demand, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 8035a670077e53981e9c366d22bdb20df06d8c1b
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-the-role-of-the-reorder-point"></a><span data-ttu-id="e19e0-103">Designdetaljer: Rollen til gjenbestillingspunktet</span><span class="sxs-lookup"><span data-stu-id="e19e0-103">Design Details: The Role of the Reorder Point</span></span>
<span data-ttu-id="e19e0-104">I tillegg til generell balansering av tilbud og etterspørsel må systemet også overvåke lagernivåer for de berørte varene for å overholde angitte gjenbestillingsprinsipper.</span><span class="sxs-lookup"><span data-stu-id="e19e0-104">In addition to the general balancing of supply and demand, the planning system must also monitor inventory levels for the affected items to respect the defined reordering policies.</span></span>  
  
<span data-ttu-id="e19e0-105">Et gjenbestillingspunkt representerer etterspørselen i løpet av leveringstiden.</span><span class="sxs-lookup"><span data-stu-id="e19e0-105">A reorder point represents demand during lead time.</span></span> <span data-ttu-id="e19e0-106">Når den beregnede beholdningen går under lagernivået som defineres av gjenbestillingspunktet, er det på tide å bestille mer.</span><span class="sxs-lookup"><span data-stu-id="e19e0-106">When the projected inventory passes below the inventory level defined by the reorder point, it is time to order more quantity.</span></span> <span data-ttu-id="e19e0-107">I mellomtiden forventes det at beholdningen gradvis reduseres og kanskje blir null (eller sikkerhetslagernivået) til etterfyllingen kommer.</span><span class="sxs-lookup"><span data-stu-id="e19e0-107">Meanwhile, the inventory is expected to decrease gradually and possibly reach zero (or the safety stock level), until the replenishment arrives.</span></span>  
  
<span data-ttu-id="e19e0-108">Planleggingssystemet vil foreslå en fremoverplanlagt forsyningsordre når den forventede beholdning blir lavere enn gjenbestillingspunktet.</span><span class="sxs-lookup"><span data-stu-id="e19e0-108">Accordingly, the planning system will suggest a forward-scheduled supply order at the point when the projected inventory passes below the reorder point.</span></span>  
  
<span data-ttu-id="e19e0-109">Gjenbestillingspunktet gjenspeiler et bestemt beholdningsnivå.</span><span class="sxs-lookup"><span data-stu-id="e19e0-109">The reorder point reflects a certain inventory level.</span></span> <span data-ttu-id="e19e0-110">Lagernivåer kan imidlertid endre seg betydelig i tidsperioden, og planleggingssystemet må derfor konstant overvåke beregnet disponibel beholdning.</span><span class="sxs-lookup"><span data-stu-id="e19e0-110">However, inventory levels can move significantly during the time bucket and, therefore, the planning system must constantly monitor the projected available inventory.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="e19e0-111">Se også</span><span class="sxs-lookup"><span data-stu-id="e19e0-111">See Also</span></span>  
<span data-ttu-id="e19e0-112">[Designdetaljer: Gjenbestillingsprinsipper](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="e19e0-112">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
<span data-ttu-id="e19e0-113">[Designdetaljer: Planleggingsparametere](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="e19e0-113">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="e19e0-114">[Designdetaljer: Håndtere gjenbestillingsprinsipper](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="e19e0-114">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
[<span data-ttu-id="e19e0-115">Designdetaljer: Forsyningsplanlegging</span><span class="sxs-lookup"><span data-stu-id="e19e0-115">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
