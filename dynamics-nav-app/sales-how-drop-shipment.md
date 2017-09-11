---
title: Foreta direkte leveringer
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: a726c8c24d8f843b33b4df4d85ad2b5eab3790e7
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-make-drop-shipments"></a><span data-ttu-id="4991f-102">Foreta direkte leveringer</span><span class="sxs-lookup"><span data-stu-id="4991f-102">How to: Make Drop Shipments</span></span>
<span data-ttu-id="4991f-103">En direkte levering er levering av varer fra en av leverandørene dine, direkte til en av kundene dine.</span><span class="sxs-lookup"><span data-stu-id="4991f-103">A drop shipment is the shipment of items from one of your vendors directly to one of your customers.</span></span>

<span data-ttu-id="4991f-104">Når en ordre merkes for direkte levering, og du oppretter en bestilling som angir kunden i **Salg til kundenr.**-feltet,</span><span class="sxs-lookup"><span data-stu-id="4991f-104">When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Sell-to Customer No.**</span></span> <span data-ttu-id="4991f-105">kan du koble de to dokumentene og dermed be leverandøren levere direkte til kunden.</span><span class="sxs-lookup"><span data-stu-id="4991f-105">field, then you can link the two documents and thereby instruct the vendor to ship directly to the customer.</span></span>

## <a name="to-create-a-sales-order-for-drop-shipment"></a><span data-ttu-id="4991f-106">Slik oppretter du en ordre med direkte levering:</span><span class="sxs-lookup"><span data-stu-id="4991f-106">To create a sales order for drop shipment</span></span>
<span data-ttu-id="4991f-107">Hvis du vil klargjøre en direkte levering, kan du opprette en ordre for en vare som vanlig, bortsett fra at du må vise på salgslinjen at salget krever direkte levering.</span><span class="sxs-lookup"><span data-stu-id="4991f-107">To prepare a drop shipment, you create a sales order for an item as normal, except you must indicate on the sales line that the sale requires drop shipment.</span></span>

1. <span data-ttu-id="4991f-108">Opprett en ordre for en vare.</span><span class="sxs-lookup"><span data-stu-id="4991f-108">Create a sales order for an item.</span></span> <span data-ttu-id="4991f-109">Hvis du vil ha mer informasjon, kan du se [Selge produkter](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="4991f-109">For more information, see [How to: Sell Products](sales-how-sell-products.md).</span></span>
2. <span data-ttu-id="4991f-110">På ordrelinjen for varen for direkte levering, merker du av for **Direkte levering**.</span><span class="sxs-lookup"><span data-stu-id="4991f-110">On the sales order line for the drop-shipment item, select the **Drop Shipment** check box.</span></span>

## <a name="to-create-the-purchase-order-for-drop-shipment"></a><span data-ttu-id="4991f-111">Slik oppretter du bestillingen med direkte levering:</span><span class="sxs-lookup"><span data-stu-id="4991f-111">To create the purchase order for drop shipment</span></span>
<span data-ttu-id="4991f-112">Hvis du vil klargjøre en direkte levering for varen som skal selges, oppretter du en bestilling som vanlig, bortsett fra at du må angi på bestillingen at den må leveres til kunden, ikke til deg selv.</span><span class="sxs-lookup"><span data-stu-id="4991f-112">To prepare a drop shipment for the item to be sold, you create a purchase order as normal, except you must indicate on the purchase order that it must be shipped to your customer, not to yourself.</span></span>

1. <span data-ttu-id="4991f-113">Opprett en bestilling.</span><span class="sxs-lookup"><span data-stu-id="4991f-113">Create a purchase order.</span></span> <span data-ttu-id="4991f-114">Ikke fyll ut noen felt på linjene.</span><span class="sxs-lookup"><span data-stu-id="4991f-114">Do not fill any fields on the lines.</span></span> <span data-ttu-id="4991f-115">Hvis du vil ha mer informasjon, kan du se [Registrere kjøp](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="4991f-115">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
2. <span data-ttu-id="4991f-116">I feltet **Salg til-kundenr.**</span><span class="sxs-lookup"><span data-stu-id="4991f-116">In the **Sell-to Customer No.**</span></span> <span data-ttu-id="4991f-117">velger du kunden som du selger til.</span><span class="sxs-lookup"><span data-stu-id="4991f-117">field, select the customer that you are selling to.</span></span>
3. <span data-ttu-id="4991f-118">Velg **Direkte levering**-handlingen, og velg deretter **Hent ordre**-handlingen.</span><span class="sxs-lookup"><span data-stu-id="4991f-118">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span></span>
4. <span data-ttu-id="4991f-119">I **Salgsliste**-vinduet merker du ordren som du har forberedt i "Slik oppretter du en ordre med direkte levering".</span><span class="sxs-lookup"><span data-stu-id="4991f-119">In the **Sales List** window, select the sales order that you prepared in the "To create a sales order for drop shipment" section.</span></span>
5. <span data-ttu-id="4991f-120">Velg **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="4991f-120">Choose the **OK** button.</span></span>

<span data-ttu-id="4991f-121">Linjeinformasjonen fra ordren settes inn på bestillingslinjene.</span><span class="sxs-lookup"><span data-stu-id="4991f-121">The line information from the sales order is inserted on the purchase order line(s).</span></span>

<span data-ttu-id="4991f-122">Nå kan du angi at leverandøren skal levere varene til kunden, for eksempel, ved å sende bestillingen på e-post som en PDF-fil.</span><span class="sxs-lookup"><span data-stu-id="4991f-122">You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.</span></span>     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a><span data-ttu-id="4991f-123">Slik viser du den tilknyttede bestillingen fra ordren:</span><span class="sxs-lookup"><span data-stu-id="4991f-123">To view the linked purchase order from the sales order</span></span>
1. <span data-ttu-id="4991f-124">Velg ordrelinjen med direkte levering, velg **Ordre**-handlingen, velg **Direkte levering**-handlingen, og velg deretter **Bestilling**-handlingen.</span><span class="sxs-lookup"><span data-stu-id="4991f-124">Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.</span></span>

<span data-ttu-id="4991f-125">Den tilknyttede bestillingen åpnes.</span><span class="sxs-lookup"><span data-stu-id="4991f-125">The linked purchase order opens.</span></span>

## <a name="to-post-a-drop-shipment"></a><span data-ttu-id="4991f-126">Bokføre en direkte levering</span><span class="sxs-lookup"><span data-stu-id="4991f-126">To post a drop shipment</span></span>
<span data-ttu-id="4991f-127">Når leverandøren har levert varene, kan du bokføre ordren som levert.</span><span class="sxs-lookup"><span data-stu-id="4991f-127">When the vendor has shipped the items, you can post the sales order as shipped.</span></span> <span data-ttu-id="4991f-128">Du kan også bokføre bestillingen, men bare med **Motta**-alternativet til ordren er fakturert.</span><span class="sxs-lookup"><span data-stu-id="4991f-128">You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.</span></span>
1. <span data-ttu-id="4991f-129">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Ordrer** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="4991f-129">In the top right corner, choose the **Search for Page or Report** icon, enter **Sales orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="4991f-130">Åpne ordren som du laget i "Slik oppretter du en ordre med direkte levering".</span><span class="sxs-lookup"><span data-stu-id="4991f-130">Open the sales order that you created in the "To create a sales order for a drop shipment" section.</span></span>
3. <span data-ttu-id="4991f-131">I **Levere (antall)**-feltet angir du hvor mye av ordreantallet som skal leveres, hele eller deler av ordreantallet.</span><span class="sxs-lookup"><span data-stu-id="4991f-131">In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.</span></span>
3. <span data-ttu-id="4991f-132">Velg handlingen **Bokfør** eller **Bokfør og send**.</span><span class="sxs-lookup"><span data-stu-id="4991f-132">Choose the **Post** or **Post and Send** action.</span></span>
4. <span data-ttu-id="4991f-133">Velg **Levere** hvis du vil fakturere senere, eller **Levere og fakturere** hvis du vil fakturere med en gang.</span><span class="sxs-lookup"><span data-stu-id="4991f-133">Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.</span></span>

## <a name="see-also"></a><span data-ttu-id="4991f-134">Se også</span><span class="sxs-lookup"><span data-stu-id="4991f-134">See Also</span></span>
<span data-ttu-id="4991f-135">[Selge produkter](sales-how-sell-products.md)  </span><span class="sxs-lookup"><span data-stu-id="4991f-135">[How to: Sell Products](sales-how-sell-products.md)  </span></span>  
[<span data-ttu-id="4991f-136">Registrere kjøp</span><span class="sxs-lookup"><span data-stu-id="4991f-136">How to: Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="4991f-137">Håndtere salg</span><span class="sxs-lookup"><span data-stu-id="4991f-137">Manage Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="4991f-138">[Håndtere lager](inventory-manage-inventory.md)    </span><span class="sxs-lookup"><span data-stu-id="4991f-138">[Manage Inventory](inventory-manage-inventory.md)    </span></span>  
[<span data-ttu-id="4991f-139">Arbeide med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="4991f-139">Work with Dynamics NAV</span></span>](ui-work-product.md)

