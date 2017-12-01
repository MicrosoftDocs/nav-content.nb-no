---
title: Opprette en ordre som er koblet til en bestilling for en direkte levering
description: "Beskriver hvordan du oppretter en ordre som er koblet til en bestilling, for å sikre levering direkte fra leverandøren til kunden."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct shipment
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 6be69a96ad6df401b3fedf5e0b81df870a1eedfc
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-make-drop-shipments"></a><span data-ttu-id="8b3dc-103">Foreta direkte leveringer</span><span class="sxs-lookup"><span data-stu-id="8b3dc-103">How to: Make Drop Shipments</span></span>
<span data-ttu-id="8b3dc-104">En direkte levering er levering av varer fra en av leverandørene dine, direkte til en av kundene dine.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-104">A drop shipment is the shipment of items from one of your vendors directly to one of your customers.</span></span>

<span data-ttu-id="8b3dc-105">Når en ordre merkes for direkte levering, og du oppretter en bestilling som angir kunden i **Salg til kundenr.**-feltet,</span><span class="sxs-lookup"><span data-stu-id="8b3dc-105">When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Sell-to Customer No.**</span></span> <span data-ttu-id="8b3dc-106">kan du koble de to dokumentene og dermed be leverandøren levere direkte til kunden.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-106">field, you can link the two documents and thereby instruct the vendor to ship directly to the customer.</span></span>

## <a name="to-create-a-sales-order-for-drop-shipment"></a><span data-ttu-id="8b3dc-107">Slik oppretter du en ordre med direkte levering:</span><span class="sxs-lookup"><span data-stu-id="8b3dc-107">To create a sales order for drop shipment</span></span>
<span data-ttu-id="8b3dc-108">Hvis du vil klargjøre en direkte levering, kan du opprette en ordre for en vare som vanlig, bortsett fra at du må vise på salgslinjen at salget krever direkte levering.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-108">To prepare a drop shipment, you create a sales order for an item as normal, except you must indicate on the sales line that the sale requires drop shipment.</span></span>

1. <span data-ttu-id="8b3dc-109">Opprett en ordre for en vare.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-109">Create a sales order for an item.</span></span> <span data-ttu-id="8b3dc-110">Hvis du vil ha mer informasjon, kan du se [Selge produkter](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="8b3dc-110">For more information, see [How to: Sell Products](sales-how-sell-products.md).</span></span>
2. <span data-ttu-id="8b3dc-111">På ordrelinjen for direkte levering, merker du av for **Direkte levering**.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-111">On the sales order line for the drop shipment, select the **Drop Shipment** check box.</span></span> <span data-ttu-id="8b3dc-112">Bruk funksjonen **Velg kolonner** hvis feltet ikke er synlig.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-112">Use the **Choose Columns** function if the field is not visible.</span></span> <span data-ttu-id="8b3dc-113">Hvis du vil ha mer informasjon, kan du se [Brukertilpasning](ui-user-personalization.md).</span><span class="sxs-lookup"><span data-stu-id="8b3dc-113">For more information, see [User Personalization](ui-user-personalization.md).</span></span>

## <a name="to-create-the-purchase-order-for-drop-shipment"></a><span data-ttu-id="8b3dc-114">Slik oppretter du bestillingen med direkte levering:</span><span class="sxs-lookup"><span data-stu-id="8b3dc-114">To create the purchase order for drop shipment</span></span>
<span data-ttu-id="8b3dc-115">Hvis du vil klargjøre en direkte levering for varen som skal selges, oppretter du en bestilling som vanlig, bortsett fra at du må angi på bestillingen at den må leveres til kunden, ikke til deg selv.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-115">To prepare a drop shipment for the item to be sold, you create a purchase order as normal, except you must indicate on the purchase order that it must be shipped to your customer, not to yourself.</span></span>

1. <span data-ttu-id="8b3dc-116">Opprett en bestilling.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-116">Create a purchase order.</span></span> <span data-ttu-id="8b3dc-117">Ikke fyll ut noen felt på linjene.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-117">Do not fill any fields on the lines.</span></span> <span data-ttu-id="8b3dc-118">Hvis du vil ha mer informasjon, kan du se [Registrere kjøp](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="8b3dc-118">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
2. <span data-ttu-id="8b3dc-119">I feltet **Salg til-kundenr.**</span><span class="sxs-lookup"><span data-stu-id="8b3dc-119">In the **Sell-to Customer No.**</span></span> <span data-ttu-id="8b3dc-120">velger du kunden som du selger til.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-120">field, select the customer that you are selling to.</span></span>
3. <span data-ttu-id="8b3dc-121">Velg **Direkte levering**-handlingen, og velg deretter **Hent ordre**-handlingen.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-121">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span></span>
4. <span data-ttu-id="8b3dc-122">I **Salgsliste**-vinduet merker du ordren som du har forberedt i "Slik oppretter du en ordre med direkte levering".</span><span class="sxs-lookup"><span data-stu-id="8b3dc-122">In the **Sales List** window, select the sales order that you prepared in the "To create a sales order for drop shipment" section.</span></span>
5. <span data-ttu-id="8b3dc-123">Velg **OK**.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-123">Choose the **OK** button.</span></span>

<span data-ttu-id="8b3dc-124">Linjeinformasjonen fra ordren settes inn på bestillingslinjene.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-124">The line information from the sales order is inserted on the purchase order line(s).</span></span>

<span data-ttu-id="8b3dc-125">Nå kan du angi at leverandøren skal levere varene til kunden, for eksempel, ved å sende bestillingen på e-post som en PDF-fil.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-125">You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.</span></span>     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a><span data-ttu-id="8b3dc-126">Slik viser du den tilknyttede bestillingen fra ordren:</span><span class="sxs-lookup"><span data-stu-id="8b3dc-126">To view the linked purchase order from the sales order</span></span>
* <span data-ttu-id="8b3dc-127">Velg ordrelinjen med direkte levering, velg **Ordre**-handlingen, velg **Direkte levering**-handlingen, og velg deretter **Bestilling**-handlingen.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-127">Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.</span></span>

## <a name="to-post-a-drop-shipment"></a><span data-ttu-id="8b3dc-128">Bokføre en direkte levering</span><span class="sxs-lookup"><span data-stu-id="8b3dc-128">To post a drop shipment</span></span>
<span data-ttu-id="8b3dc-129">Når leverandøren har levert varene, kan du bokføre ordren som levert.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-129">After the vendor ships the items, you can post the sales order as shipped.</span></span> <span data-ttu-id="8b3dc-130">Du kan også bokføre bestillingen, men bare med **Motta**-alternativet til ordren er fakturert.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-130">You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.</span></span>

1. <span data-ttu-id="8b3dc-131">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Ordrer**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-131">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="8b3dc-132">Åpne ordren som du laget i "Slik oppretter du en ordre med direkte levering".</span><span class="sxs-lookup"><span data-stu-id="8b3dc-132">Open the sales order that you created in the "To create a sales order for a drop shipment" section.</span></span>
3. <span data-ttu-id="8b3dc-133">I **Levere (antall)**-feltet angir du hvor mye av ordreantallet som skal leveres, hele eller deler av ordreantallet.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-133">In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.</span></span>
4. <span data-ttu-id="8b3dc-134">Velg handlingen **Bokfør** eller **Bokfør og send**.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-134">Choose the **Post** or **Post and Send** action.</span></span>
5. <span data-ttu-id="8b3dc-135">Velg **Levere** hvis du vil fakturere senere, eller **Levere og fakturere** hvis du vil fakturere med en gang.</span><span class="sxs-lookup"><span data-stu-id="8b3dc-135">Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.</span></span>

## <a name="see-also"></a><span data-ttu-id="8b3dc-136">Se også</span><span class="sxs-lookup"><span data-stu-id="8b3dc-136">See Also</span></span>
<span data-ttu-id="8b3dc-137">[Opprette spesialbestillinger](sales-how-to-create-special-orders.md)|</span><span class="sxs-lookup"><span data-stu-id="8b3dc-137">[How to: Create Special Orders](sales-how-to-create-special-orders.md)|</span></span>  
[<span data-ttu-id="8b3dc-138">Selge produkter</span><span class="sxs-lookup"><span data-stu-id="8b3dc-138">How to: Sell Products</span></span>](sales-how-sell-products.md)  
[<span data-ttu-id="8b3dc-139">Registrere kjøp</span><span class="sxs-lookup"><span data-stu-id="8b3dc-139">How to: Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="8b3dc-140">Salg</span><span class="sxs-lookup"><span data-stu-id="8b3dc-140">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="8b3dc-141">Lager</span><span class="sxs-lookup"><span data-stu-id="8b3dc-141">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="8b3dc-142">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8b3dc-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

