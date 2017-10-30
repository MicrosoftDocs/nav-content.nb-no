---
title: Spore relasjoner mellom behov og forsyning
description: "Fra ethvert forsynings- eller behovsdokument i det såkalte ordrenettverket kan du spore ordrebehovet (sporet antall), prognosen, rammebestillingen eller planleggingsparameteren (ikke-sporet antall) som har forårsaket den aktuelle planleggingslinjen."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: acf030ab57c9251671900b1262dd8441c241c185
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-track-relations-between-demand-and-supply"></a><span data-ttu-id="65528-103">Spore relasjoner mellom behov og forsyning</span><span class="sxs-lookup"><span data-stu-id="65528-103">How to: Track Relations Between Demand and Supply</span></span>
<span data-ttu-id="65528-104">Fra ethvert forsynings- eller behovsdokument i det såkalte ordrenettverket kan du spore ordrebehovet (sporet antall), prognosen, rammebestillingen eller planleggingsparameteren (ikke-sporet antall) som har forårsaket den aktuelle planleggingslinjen.</span><span class="sxs-lookup"><span data-stu-id="65528-104">From any supply or demand document in the so-called order network, you can track the order demand (tracked quantity), forecast, blanket sales order, or planning parameter (untracked quantity) that has given rise to the planning line in question.</span></span>

<span data-ttu-id="65528-105">Planleggingsforslagene gir også støtteinformasjon for planlegging for ikke-ordreenheter for å hjelpe planleggeren med å opprette en optimal forsyningsplan.</span><span class="sxs-lookup"><span data-stu-id="65528-105">The planning worksheets also offers supporting planning information about non-order entities to help the planner obtain an optimal supply plan.</span></span> <span data-ttu-id="65528-106">Hvis du vil ha mer informasjon, kan du se delen Ikke-sporet planleggingselement.</span><span class="sxs-lookup"><span data-stu-id="65528-106">For more information, see the "Untracked Planning Elements" section.</span></span>

## <a name="to-track-linked-items"></a><span data-ttu-id="65528-107">Spore tilknyttede varer</span><span class="sxs-lookup"><span data-stu-id="65528-107">To track linked items</span></span>
<span data-ttu-id="65528-108">Sporing viser hvordan ordrer, produksjonsordrer og bestillinger er knyttet til produksjonsordrer gjennom planleggings- og reservasjonssystemer.</span><span class="sxs-lookup"><span data-stu-id="65528-108">Order tracking shows how sales orders, production orders, and purchase orders are related to the manufacturing order through the planning and reservation systems.</span></span>

<span data-ttu-id="65528-109">Nedenfor beskrives hvordan du kan spore tilknyttede varer på en fast planlagt produksjonsordre.</span><span class="sxs-lookup"><span data-stu-id="65528-109">The following describes how to track linked items on a firm planned production order.</span></span> <span data-ttu-id="65528-110">Fremgangsmåten er lik for alle andre ordretyper og fra planleggingsforslagslinjer.</span><span class="sxs-lookup"><span data-stu-id="65528-110">The steps are similar for all other order types, and from planning worksheet lines.</span></span>

1. <span data-ttu-id="65528-111">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Fast planlagte prod.ordre**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="65528-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Order**, and then choose the related link.</span></span>
2. <span data-ttu-id="65528-112">Åpne den aktuelle fast planlagte produksjonsordren fra oversikten.</span><span class="sxs-lookup"><span data-stu-id="65528-112">Open the relevant firm planned production order from the list.</span></span>
3. <span data-ttu-id="65528-113">På hurtigfanen **Linjer** velger du **Funksjoner**-handlingen og deretter **Sporing**.</span><span class="sxs-lookup"><span data-stu-id="65528-113">On the **Lines** FastTab, choose the **Functions** action, and then choose the **Order Tracking** action.</span></span>

<span data-ttu-id="65528-114">Linjene i **Sporing**-vinduet viser hvilke dokumenter som er knyttet til den aktuelle produksjonsordrelinjen.</span><span class="sxs-lookup"><span data-stu-id="65528-114">The lines in the **Order Tracking** display the documents that are related to the current production order line.</span></span>

## <a name="untracked-planning-elements"></a><span data-ttu-id="65528-115">Ikke-sporede planleggingselementer</span><span class="sxs-lookup"><span data-stu-id="65528-115">Untracked Planning Elements</span></span>
<span data-ttu-id="65528-116">Vinduet **Ikke-sporede planleggingselementer** åpnes når du velger feltet **Ikke-sporet antall** i vinduet **Ordreplanlegging**.</span><span class="sxs-lookup"><span data-stu-id="65528-116">The **Untracked Planning Elements** window opens when you choose the **Untracked Qty.** field in the **order Planning** window.</span></span> <span data-ttu-id="65528-117">Det har to formål:</span><span class="sxs-lookup"><span data-stu-id="65528-117">It serves two purposes:</span></span>

1. <span data-ttu-id="65528-118">Inneholde informasjon om ikke-sporede antall som vises når brukeren slår opp ikke-sporede antall fra Sporing-vinduet.</span><span class="sxs-lookup"><span data-stu-id="65528-118">To hold information about untracked quantities displayed when the user looks up from the Order Tracking window to see untracked quantities.</span></span>
2. <span data-ttu-id="65528-119">Inneholde advarsler som vises når brukeren klikker et **advarselsikon** i vinduet **Planleggingsforslag**.</span><span class="sxs-lookup"><span data-stu-id="65528-119">To hold warning messages displayed when the user chooses the **Warning** icon in the **Planning Worksheet** window.</span></span>

<span data-ttu-id="65528-120">Vinduet inneholder poster som gjør rede for et ikke-sporet overskuddsantall i ordresporingsnettverket.</span><span class="sxs-lookup"><span data-stu-id="65528-120">The window contains entries which account for an untracked surplus quantity in order tracking network.</span></span> <span data-ttu-id="65528-121">Disse postene genereres under planleggingskjøringen og forklarer hvor det ikke-sporede overskuddsantallet på sporingslinjene kommer fra.</span><span class="sxs-lookup"><span data-stu-id="65528-121">These entries are generated during the planning run and explain where the untracked surplus quantity in the order tracking lines came from.</span></span> <span data-ttu-id="65528-122">Dette ikke-sporede overskuddet kan komme fra:</span><span class="sxs-lookup"><span data-stu-id="65528-122">This untracked surplus can come from:</span></span>

- <span data-ttu-id="65528-123">Produksjonsprognose</span><span class="sxs-lookup"><span data-stu-id="65528-123">Production forecast</span></span>
- <span data-ttu-id="65528-124">Rammeordrer</span><span class="sxs-lookup"><span data-stu-id="65528-124">Blanket orders</span></span>
- <span data-ttu-id="65528-125">Sikkerhetslagerantall</span><span class="sxs-lookup"><span data-stu-id="65528-125">Safety stock quantity</span></span>
- <span data-ttu-id="65528-126">Gjenbestillingspunkt</span><span class="sxs-lookup"><span data-stu-id="65528-126">Reorder point</span></span>
- <span data-ttu-id="65528-127">Maks. beholdning</span><span class="sxs-lookup"><span data-stu-id="65528-127">Maximum inventory</span></span>
- <span data-ttu-id="65528-128">Gjenbestillingsantall</span><span class="sxs-lookup"><span data-stu-id="65528-128">Reorder quantity</span></span>
- <span data-ttu-id="65528-129">Maks. bestillingsantall</span><span class="sxs-lookup"><span data-stu-id="65528-129">Maximum order quantity</span></span>
- <span data-ttu-id="65528-130">Min. bestillingsantall</span><span class="sxs-lookup"><span data-stu-id="65528-130">Minimum order quantity</span></span>
- <span data-ttu-id="65528-131">Bestillingsfaktor</span><span class="sxs-lookup"><span data-stu-id="65528-131">Order multiple</span></span>
- <span data-ttu-id="65528-132">Avdemping (% av partistr.)</span><span class="sxs-lookup"><span data-stu-id="65528-132">Dampener (% of lot size)</span></span>

## <a name="see-also"></a><span data-ttu-id="65528-133">Se også</span><span class="sxs-lookup"><span data-stu-id="65528-133">See Also</span></span>  
<span data-ttu-id="65528-134">[Planlegging](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="65528-134">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="65528-135">Definere produksjon</span><span class="sxs-lookup"><span data-stu-id="65528-135">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="65528-136">[Produksjon](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="65528-136">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="65528-137">Lager</span><span class="sxs-lookup"><span data-stu-id="65528-137">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="65528-138">Innkjøp</span><span class="sxs-lookup"><span data-stu-id="65528-138">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="65528-139">Designdetaljer: Reservasjon, sporing og handlingsmeldinger</span><span class="sxs-lookup"><span data-stu-id="65528-139">Design Details: Reservation, Tracking, and Action Messaging</span></span>](design-details-reservation-order-tracking-and-action-messaging.md)  
<span data-ttu-id="65528-140">[Designdetaljer: Forsyningsplanlegging](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="65528-140">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
[<span data-ttu-id="65528-141">Anbefalte fremgangsmåter for oppsett: Forsyningsplanlegging</span><span class="sxs-lookup"><span data-stu-id="65528-141">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
<span data-ttu-id="65528-142">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="65528-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

