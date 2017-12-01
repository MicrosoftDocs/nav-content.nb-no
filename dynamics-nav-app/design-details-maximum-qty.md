---
title: Designdetaljer - Maks.ant.
description: "Maksimumsantall-prinsippet er en måte å opprettholde beholdningen på ved hjelp av et gjenbestillingspunkt."
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
ms.openlocfilehash: 174ca820abd8f9b6942e74d412c8bef6352b64b6
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="design-details-maximum-qty"></a><span data-ttu-id="93918-103">Designdetaljer: Maks.ant.</span><span class="sxs-lookup"><span data-stu-id="93918-103">Design Details: Maximum Qty.</span></span>
<span data-ttu-id="93918-104">Maksimumsantall-prinsippet er en måte å opprettholde beholdningen på ved hjelp av et gjenbestillingspunkt.</span><span class="sxs-lookup"><span data-stu-id="93918-104">The Maximum Quantity policy is a way to maintain inventory using a reorder point.</span></span>  
  
 <span data-ttu-id="93918-105">Alt for prinsippet Fast gjenbest.ant. gjelder også for dette prinsippet.</span><span class="sxs-lookup"><span data-stu-id="93918-105">Everything regarding the Fixed Reorder Qty. policy also applies to this policy.</span></span> <span data-ttu-id="93918-106">Den eneste forskjellen er antallet i forsyningen som foreslås.</span><span class="sxs-lookup"><span data-stu-id="93918-106">The only difference is the quantity of the suggested supply.</span></span> <span data-ttu-id="93918-107">Når du bruker prinsippet om maksimumsantall, defineres gjenbestillingsantallet dynamisk basert på det beregnede beholdningsnivået og varierer derfor vanligvis fra bestilling til bestilling.</span><span class="sxs-lookup"><span data-stu-id="93918-107">When using the maximum quantity policy, the reorder quantity will be defined dynamically based on the projected inventory level and will therefore usually differ from order to order.</span></span>  
  
## <a name="calculated-per-time-bucket"></a><span data-ttu-id="93918-108">Beregnet per tidsperiode</span><span class="sxs-lookup"><span data-stu-id="93918-108">Calculated per Time Bucket</span></span>  
 <span data-ttu-id="93918-109">Gjenbestillingsantallet fastsettes på tidspunktet (slutten av en tidsperiode) der planleggingssystemet oppdager at gjenbestillingspunktet er overskredet.</span><span class="sxs-lookup"><span data-stu-id="93918-109">The reorder quantity is determined at the point of time (the end of a time bucket) when the planning system detects that the reorder point has been crossed.</span></span> <span data-ttu-id="93918-110">Systemet måler nå avstanden fra gjeldende beregnede beholdningsnivået opp til angitt maksimal lagerbeholdning.</span><span class="sxs-lookup"><span data-stu-id="93918-110">At this time, the system measures the gap from the current projected inventory level up to the specified maximum inventory.</span></span> <span data-ttu-id="93918-111">Dette utgjør antallet som må bestilles.</span><span class="sxs-lookup"><span data-stu-id="93918-111">This constitutes the quantity that should be reordered.</span></span> <span data-ttu-id="93918-112">Systemet kontrollerer deretter om forsyning allerede er bestilt et annet sted og kommer til å mottas innen leveringstiden, og i så fall reduseres antallet i den nye forsyningsordren med antallet som allerede er bestilt.</span><span class="sxs-lookup"><span data-stu-id="93918-112">The system then checks if supply has already been ordered elsewhere to be received within the lead time and, if so, reduces the quantity of the new supply order by already ordered quantities.</span></span>  
  
 <span data-ttu-id="93918-113">Systemet sikrer at den beregnede beholdningen minst når gjenbestillingspunktet, i tilfelle brukeren har glemt å angi en maksimumsbeholdning.</span><span class="sxs-lookup"><span data-stu-id="93918-113">The system will ensure that the projected inventory at least reaches the reorder point level – in case the user has forgotten to specify a maximum inventory quantity.</span></span>  
  
## <a name="combines-with-order-modifiers"></a><span data-ttu-id="93918-114">Kombineres med ordremodifikatorer</span><span class="sxs-lookup"><span data-stu-id="93918-114">Combines with Order Modifiers</span></span>  
 <span data-ttu-id="93918-115">Avhengig av oppsettet kan det være best å kombinere prinsippet for maksimumsantall med ordremodifikatorer for å sikre et minimumsordreantall, runde det opp til et heltall innkjøpsenheter, eller dele den inn i flere partier som er definert av maksimumsordreantallet.</span><span class="sxs-lookup"><span data-stu-id="93918-115">Depending on the setup, it may be best to combine the Maximum Quantity policy with order modifiers to ensure a minimum order quantity or round it to an integer number of purchase units of measure, or split it into more lots as defined by the maximum order quantity.</span></span>  
  
## <a name="combines-with-calendars"></a><span data-ttu-id="93918-116">Kombinerer med kalendere</span><span class="sxs-lookup"><span data-stu-id="93918-116">Combines with Calendars</span></span>  
 <span data-ttu-id="93918-117">Før det blir foreslått en ny forsyningsordre for å oppfylle et gjenbestillingspunkt, kontrollerer systemet om ordren er planlagt for en fridag, i henhold til kalendere som er definert i feltet **Hovedkalenderkode** i vinduene **Selskapsopplysninger** og **Lokasjonskort**.</span><span class="sxs-lookup"><span data-stu-id="93918-117">Before suggesting a new supply order to meet a reorder point, the planning system checks if the order is scheduled for a non-working day, according to any calendars that are  defined in the **Base Calendar Code** field in the **Company Information** and **Location Card** windows.</span></span>  
  
 <span data-ttu-id="93918-118">Hvis den planlagte datoen er en fridag, flytter planleggingssystemet ordren fremover til nærmeste arbeidsdato.</span><span class="sxs-lookup"><span data-stu-id="93918-118">If the scheduled date is a non-working day, the planning system moves the order forward to the nearest working date.</span></span> <span data-ttu-id="93918-119">Dette kan resultere i en ordre som oppfyller et gjenbestillingspunkt, men som ikke oppfyller enkelte spesifikke behov.</span><span class="sxs-lookup"><span data-stu-id="93918-119">This may result in an order that meets a reorder point but does not meet some specific demand.</span></span> <span data-ttu-id="93918-120">For slike ubalanserte behov oppretter planleggingssystemet en ekstra forsyning.</span><span class="sxs-lookup"><span data-stu-id="93918-120">For such unbalanced demand, the planning system creates an extra supply.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="93918-121">Se også</span><span class="sxs-lookup"><span data-stu-id="93918-121">See Also</span></span>  
 <span data-ttu-id="93918-122">[Designdetaljer: Gjenbestillingsprinsipper](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="93918-122">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
 <span data-ttu-id="93918-123">[Designdetaljer: Planleggingsparametere](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="93918-123">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
 <span data-ttu-id="93918-124">[Designdetaljer: Håndtere gjenbestillingsprinsipper](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="93918-124">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
 [<span data-ttu-id="93918-125">Designdetaljer: Forsyningsplanlegging</span><span class="sxs-lookup"><span data-stu-id="93918-125">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
