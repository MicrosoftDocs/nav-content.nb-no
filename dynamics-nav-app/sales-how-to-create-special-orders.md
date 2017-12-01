---
title: Opprette spesialbestillinger
description: "Du kan opprette en spesialbestilling for en bestemt katalogvare som skal leveres til en bestemt kunde. Leverandøren din leverer varen til lageret ditt, og du kan deretter sende bare denne varen videre til kunden eller sammen med andre varer i en annen ordre."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 596b9a5638e551a8165429308a68a4c8dddb6a06
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-create-special-orders"></a><span data-ttu-id="f5d99-104">Opprette spesialbestillinger</span><span class="sxs-lookup"><span data-stu-id="f5d99-104">How to: Create Special Orders</span></span>
<span data-ttu-id="f5d99-105">Du kan opprette en spesialbestilling for en bestemt katalogvare som skal leveres til en bestemt kunde.</span><span class="sxs-lookup"><span data-stu-id="f5d99-105">You can create a special order for a specific nonstock item to be shipped to a specific customer.</span></span> <span data-ttu-id="f5d99-106">Leverandøren din leverer varen til lageret ditt, og du kan deretter sende bare denne varen videre til kunden eller sammen med andre varer i en annen ordre.</span><span class="sxs-lookup"><span data-stu-id="f5d99-106">Your vendor ships the item to your warehouse and you can then ship the item on to your customer either independently or together with other items on another order.</span></span>  

<span data-ttu-id="f5d99-107">Spesialbestillinger betyr at bestillingen og ordren er knyttet til hverandre for å sikre at den bestemte katalogvaren plukkes og leveres til kunden.</span><span class="sxs-lookup"><span data-stu-id="f5d99-107">Special orders imply that the purchase and sales order are linked to ensure that the specific nonstock item is picked and delivered to the customer.</span></span>  

<span data-ttu-id="f5d99-108">Før du kan bruke denne funksjonen, må du først konfigurere kunden, leverandøren og de varekortene som kreves for ordren.</span><span class="sxs-lookup"><span data-stu-id="f5d99-108">Before you can use this feature, you must first set up the customer, vendor, and item cards necessary for the order.</span></span>  

## <a name="to-create-a-special-order"></a><span data-ttu-id="f5d99-109">Slik oppretter du en spesialbestilling</span><span class="sxs-lookup"><span data-stu-id="f5d99-109">To create a special order</span></span>  
1.  <span data-ttu-id="f5d99-110">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Ordre**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="f5d99-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Order**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f5d99-111">Velg handlingen **Ny**.</span><span class="sxs-lookup"><span data-stu-id="f5d99-111">Choose the **New** action.</span></span> <span data-ttu-id="f5d99-112">Opprett og fyll ut en  ordre for varen.</span><span class="sxs-lookup"><span data-stu-id="f5d99-112">Create and fill in a  sales order for the item.</span></span> <span data-ttu-id="f5d99-113">Hvis du vil ha mer informasjon, kan du se [Selge produkter](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="f5d99-113">For more information, see [How to: Sell Products](sales-how-sell-products.md).</span></span>
3.  <span data-ttu-id="f5d99-114">På hurtigfanen **Linjer** fyller du inn salgslinjen.</span><span class="sxs-lookup"><span data-stu-id="f5d99-114">On the **Lines** FastTab, fill in the sales line.</span></span> <span data-ttu-id="f5d99-115">Velg en kjøpskode som **Spesialbestilling**-feltet er valgt for, i **Kjøpskode**-feltet.</span><span class="sxs-lookup"><span data-stu-id="f5d99-115">In the **Purchasing Code** field, select a purchasing code that has the **Special Order** field selected.</span></span>

    <span data-ttu-id="f5d99-116">Du må nå opprette en bestilling fra et bestillingsforslag.</span><span class="sxs-lookup"><span data-stu-id="f5d99-116">You must now create a purchase order from a requisition worksheet.</span></span>  
4. <span data-ttu-id="f5d99-117">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bestillingsforslag**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="f5d99-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Requisition Worksheet**, and then choose the related link.</span></span>  
5. <span data-ttu-id="f5d99-118">Velg **Spesialbestilling**-handlingen, og velg deretter **Hent ordre**-handlingen.</span><span class="sxs-lookup"><span data-stu-id="f5d99-118">Choose the **Special Order** action, and then choose the **Get Sales Orders** action.</span></span>  
6.  <span data-ttu-id="f5d99-119">Vis resultater der **Bilagsnr.** er ordrenummeret, i **Hent ordrer**-vinduet.</span><span class="sxs-lookup"><span data-stu-id="f5d99-119">In the **Get Sales Orders** window, show results where the **Document No.** is the sales order number.</span></span> <span data-ttu-id="f5d99-120">Velg **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="f5d99-120">Choose the **OK** button.</span></span> <span data-ttu-id="f5d99-121">Det opprettes en bestillingsforslagslinje for varen.</span><span class="sxs-lookup"><span data-stu-id="f5d99-121">A requisition worksheet line is created for the item.</span></span>  
7.  <span data-ttu-id="f5d99-122">På bestillingsforslagslinjen velger du **Ny** i feltet **Handlingsmelding**.</span><span class="sxs-lookup"><span data-stu-id="f5d99-122">On the requisition worksheet line, in the **Action Message** field, select **New**.</span></span>  
8.  <span data-ttu-id="f5d99-123">I **Best. forslag**-vinduet velger du handlingen **Utfør handlingsmelding**.</span><span class="sxs-lookup"><span data-stu-id="f5d99-123">In the **Req. Worksheet** window, choose the **Carry Out Action Message** action.</span></span> <span data-ttu-id="f5d99-124">Vinduet **Utfør handlingsmeld. - forslag** åpnes.</span><span class="sxs-lookup"><span data-stu-id="f5d99-124">The **Carry Out Action Msg. - Req.** window opens.</span></span> <span data-ttu-id="f5d99-125">Velg **OK**.</span><span class="sxs-lookup"><span data-stu-id="f5d99-125">Choose the **OK** button.</span></span>  

    <span data-ttu-id="f5d99-126">Det vises en melding om at bestillingene er opprettet.</span><span class="sxs-lookup"><span data-stu-id="f5d99-126">A message appears telling you that the purchase orders have been created.</span></span> <span data-ttu-id="f5d99-127">Velg **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="f5d99-127">Choost the **OK** button.</span></span>  

<span data-ttu-id="f5d99-128">En bestilling som er opprettet som en spesialbestilling for en salgsordre, blir respektert av planleggingssystemet som balanserer behov og forsyning.</span><span class="sxs-lookup"><span data-stu-id="f5d99-128">A purchase order created as a special order for a sales order is respected by the planning system as it balances demand and supply.</span></span> <span data-ttu-id="f5d99-129">Det vil si at bestillingen (tilbud) forblir koblet til ordren (etterspørsel), selv om den aktuelle bestillingen ville kunnet forsyne et annet tidligere behov.</span><span class="sxs-lookup"><span data-stu-id="f5d99-129">That is, the purchase order (supply) remains linked to the sales order (demand), even if that purchase order could supply another earlier demand.</span></span> <span data-ttu-id="f5d99-130">Hvis du vil ha mer informasjon, se [Designdetaljer: Gjenbestillingsprinsipper](design-details-reservation-order-tracking-and-action-messaging.md).</span><span class="sxs-lookup"><span data-stu-id="f5d99-130">For more information, see [Design Details: Reordering Policies](design-details-reservation-order-tracking-and-action-messaging.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="f5d99-131">Du kan ikke bruke funksjonen for spesialbestilling hvis varen allerede er reservert.</span><span class="sxs-lookup"><span data-stu-id="f5d99-131">You cannot use the special order functionality if the item is already reserved.</span></span> <span data-ttu-id="f5d99-132">For varer som selges på spesialbestilling, må du derfor passe på at feltet **Reserver** på varekortet ikke er satt til **Alltid**.</span><span class="sxs-lookup"><span data-stu-id="f5d99-132">Therefore, for items that are sold on special orders, make sure the **Reserve** field on the item card is not set to **Always**.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f5d99-133">Se også</span><span class="sxs-lookup"><span data-stu-id="f5d99-133">See Also</span></span>  
[<span data-ttu-id="f5d99-134">Arbeide med katalogvarer</span><span class="sxs-lookup"><span data-stu-id="f5d99-134">How to: Work with Nonstock Items</span></span>](inventory-how-work-nonstock-items.md)  
[<span data-ttu-id="f5d99-135">Salg</span><span class="sxs-lookup"><span data-stu-id="f5d99-135">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="f5d99-136">[Foreta direkte leveringer](sales-how-drop-shipment.md) </span><span class="sxs-lookup"><span data-stu-id="f5d99-136">[How to: Make Drop Shipments](sales-how-drop-shipment.md) </span></span>  
[<span data-ttu-id="f5d99-137">Designdetaljer: Gjenbestillingsprinsipper</span><span class="sxs-lookup"><span data-stu-id="f5d99-137">Design Details: Reordering Policies</span></span>](design-details-reservation-order-tracking-and-action-messaging.md)  
<span data-ttu-id="f5d99-138">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f5d99-138">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

