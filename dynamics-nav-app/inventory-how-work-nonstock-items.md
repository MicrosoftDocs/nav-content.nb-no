---
title: Opprette og administrere katalogvarer
description: "Beskriver hvordan du handler med indirekte varer eller varer som ikke oppbevares på lager."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: non-inventoriable
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: dee8b9ec3b47760f0ececc0a13f68c0039ad4c1a
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-work-with-nonstock-items"></a><span data-ttu-id="93e3a-103">Arbeide med katalogvarer</span><span class="sxs-lookup"><span data-stu-id="93e3a-103">How to: Work with Nonstock Items</span></span>
<span data-ttu-id="93e3a-104">Du kan tilby bestemte varer til kundene for å gjøre det mer bekvemmelig for dem, som du ikke vil ha på lager før du begynner å selge dem.</span><span class="sxs-lookup"><span data-stu-id="93e3a-104">You can offer certain items to your customers for their convenience, which you do not want to maintain in inventory until you start selling them.</span></span> <span data-ttu-id="93e3a-105">Når du vil begynne å ha slike varer på lager, kan du konvertere dem til vanlige varekort på to måter.</span><span class="sxs-lookup"><span data-stu-id="93e3a-105">When you want to start maintaining such items in inventory, you can convert them to normal item cards in two ways.</span></span>

* <span data-ttu-id="93e3a-106">Fra et katalogvarekort kan du opprette et nytt varekort basert på en mal.</span><span class="sxs-lookup"><span data-stu-id="93e3a-106">From a nonstock item card, create a new item card based on a template.</span></span>
* <span data-ttu-id="93e3a-107">Fra en salgsordrelinje av typen **Vare** med et tomt **Nei*-felt velger du en katalogvare.</span><span class="sxs-lookup"><span data-stu-id="93e3a-107">From a sales order line of type **Item** with an empty **No* field, select a nonstock item.</span></span> <span data-ttu-id="93e3a-108">Et varekort opprettes automatisk for katalogvaren.</span><span class="sxs-lookup"><span data-stu-id="93e3a-108">An item card is automatically created for the nonstock item.</span></span>

> [!NOTE]  
>   <span data-ttu-id="93e3a-109">Du kan ikke velge en katalogvare fra **Salgsfaktura**-vinduet.</span><span class="sxs-lookup"><span data-stu-id="93e3a-109">You cannot select a nonstock item from the **Sales Invoice** window.</span></span> <span data-ttu-id="93e3a-110">Du kan velge en katalogvare fra **Tilbud**-vinduet, men katalogvaren vil ikke bli konvertert til en vanlig vare når du bruker **Lag ordre**-funksjonen.</span><span class="sxs-lookup"><span data-stu-id="93e3a-110">You can select a nonstock item from the **Sales Quote** window, but the nonstock item will not be converted to a normal item when you use the **Make Order** function.</span></span>

<span data-ttu-id="93e3a-111">En katalogvare har vanligvis varenummeret til leverandøren som leverer den.</span><span class="sxs-lookup"><span data-stu-id="93e3a-111">A nonstock item typically has the item number of the vendor who supplies it.</span></span> <span data-ttu-id="93e3a-112">For å gjøre det mulig å konvertere et katalogvarekort til et vanlig varekort, må du først definere hvordan varenummerering for leverandør skal konverteres til din egen varenummerering.</span><span class="sxs-lookup"><span data-stu-id="93e3a-112">To enable conversion of a nonstock item card to a normal item card, you must first set up how vendor item numbering is converted to your own item numbering.</span></span>   

## <a name="to-create-a-nonstock-item"></a><span data-ttu-id="93e3a-113">Slik oppretter du en katalogvare:</span><span class="sxs-lookup"><span data-stu-id="93e3a-113">To create a nonstock item</span></span>
<span data-ttu-id="93e3a-114">Katalogvarekort har mye mindre informasjon enn vanlige varekort fordi du bare bruker dem til tilbud i salgstilbud og på andre måter.</span><span class="sxs-lookup"><span data-stu-id="93e3a-114">Nonstock item cards have much less information than normal item cards because you only use them to offer on quotes and in other ways.</span></span> <span data-ttu-id="93e3a-115">Derfor må de konverteres til vanlige varekort før du kan bokføre salgstransaksjoner for dem.</span><span class="sxs-lookup"><span data-stu-id="93e3a-115">For that reason, they must be converted to normal item cards before you can post sales transactions for them.</span></span>

1. <span data-ttu-id="93e3a-116">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Katalogvarer**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="93e3a-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Nonstock Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="93e3a-117">Velg handlingen **Ny**.</span><span class="sxs-lookup"><span data-stu-id="93e3a-117">Choose the **New** action.</span></span>
3. <span data-ttu-id="93e3a-118">Fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="93e3a-118">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-how-nonstock-item-numbers-are-converted-to-your-own-numbering"></a><span data-ttu-id="93e3a-119">Slik definerer du hvordan katalogvarenumre konverteres til din egen nummerering:</span><span class="sxs-lookup"><span data-stu-id="93e3a-119">To set up how nonstock item numbers are converted to your own numbering</span></span>
<span data-ttu-id="93e3a-120">For å gjøre det mulig å konvertere et katalogvarekort til et vanlig varekort, må du først definere hvordan varenummereringen for leverandøren skal konverteres til ditt eget varenummereringsformat.</span><span class="sxs-lookup"><span data-stu-id="93e3a-120">To enable conversion of a nonstock item card to a normal item card, you must first set up how the vendor's item numbering is converted to your own item number format.</span></span>

1. <span data-ttu-id="93e3a-121">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Katalogvare - oppsett**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="93e3a-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Nonstock Item Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="93e3a-122">Fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="93e3a-122">Fill in the fields as necessary.</span></span>

## <a name="to-convert-a-nonstock-item-to-a-normal-item"></a><span data-ttu-id="93e3a-123">Slik konverterer du en katalogvare til en vanlig vare:</span><span class="sxs-lookup"><span data-stu-id="93e3a-123">To convert a nonstock item to a normal item</span></span>
1. <span data-ttu-id="93e3a-124">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Katalogvarer**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="93e3a-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Nonstock Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="93e3a-125">Åpne kortet for katalogvaren som du vil konvertere til en vanlig vare.</span><span class="sxs-lookup"><span data-stu-id="93e3a-125">Open the card for a nonstock item that you want to convert to a normal item.</span></span>
3. <span data-ttu-id="93e3a-126">I vinduet **Kort for katalogvare** velger du handlingen **Opprett vare**.</span><span class="sxs-lookup"><span data-stu-id="93e3a-126">In the **Nonstock Item Card** window, choose the **Create Item** action.</span></span>

<span data-ttu-id="93e3a-127">Et nytt varekort forhåndsutfylt med informasjon fra katalogvaren og en relevant varemal opprettes.</span><span class="sxs-lookup"><span data-stu-id="93e3a-127">A new item card prefilled with information from the nonstock item and a relevant item template is created.</span></span> <span data-ttu-id="93e3a-128">Du kan deretter fylle ut eller redigere felt på det nye varekortet etter behov.</span><span class="sxs-lookup"><span data-stu-id="93e3a-128">You can then fill or edit fields on the new item card as necessary.</span></span> <span data-ttu-id="93e3a-129">Hvis du vil ha mer informasjon, kan du se [Registrere nye varer](inventory-how-register-new-items.md).</span><span class="sxs-lookup"><span data-stu-id="93e3a-129">For more information, see [How to: Register New Items](inventory-how-register-new-items.md).</span></span>

## <a name="to-sell-a-nonstock-item-and-convert-it-to-a-normal-item"></a><span data-ttu-id="93e3a-130">Slik selger du en katalogvare og konverterer den til en vanlig vare:</span><span class="sxs-lookup"><span data-stu-id="93e3a-130">To sell a nonstock item, and convert it to a normal item</span></span>
1. <span data-ttu-id="93e3a-131">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Ordrer**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="93e3a-131">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="93e3a-132">Velg handlingen **Ny**.</span><span class="sxs-lookup"><span data-stu-id="93e3a-132">Choose the **New** action.</span></span> <span data-ttu-id="93e3a-133">Fyll ut feltene på hurtigfanen **Generelt** som for ordrer.</span><span class="sxs-lookup"><span data-stu-id="93e3a-133">Fill in the fields on the **General** FastTab as for any sales order.</span></span> <span data-ttu-id="93e3a-134">Hvis du vil ha mer informasjon, kan du se [Selge produkter](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="93e3a-134">For more information, see [How to: Sell Products](sales-how-sell-products.md).</span></span>
3. <span data-ttu-id="93e3a-135">På en ny salgslinje, i **Type**-feltet velger du **Vare**, men lar feltet **Nr.**</span><span class="sxs-lookup"><span data-stu-id="93e3a-135">On a new sales line, in the **Type** field, select **Item**, but leave the **No.**</span></span> <span data-ttu-id="93e3a-136">stå tomt.</span><span class="sxs-lookup"><span data-stu-id="93e3a-136">field empty.</span></span>
4. <span data-ttu-id="93e3a-137">Velg handlingen **Linje** og velg deretter handlingen **Velg katalogvarer**.</span><span class="sxs-lookup"><span data-stu-id="93e3a-137">Choose the **Line** action, and then choose the **Select Nonstock Items** action.</span></span>

    <span data-ttu-id="93e3a-138">Katalogvaren konverteres til en vanlig vare.</span><span class="sxs-lookup"><span data-stu-id="93e3a-138">The nonstock item is converted to a normal item.</span></span> <span data-ttu-id="93e3a-139">Et nytt varekort forhåndsutfylt med informasjon fra katalogvaren og en relevant varemal opprettes.</span><span class="sxs-lookup"><span data-stu-id="93e3a-139">A new item card prefilled with information from the nonstock item and a relevant item template is created.</span></span>
5. <span data-ttu-id="93e3a-140">I **Katalogvarer**-vinduet velger du katalogvaren du vil selge, og velger deretter **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="93e3a-140">In the **Nonstock Items** window, select the nonstock item that you want to sell, and then choose the **OK** button.</span></span>
6. <span data-ttu-id="93e3a-141">Når ordren er fullført, kan du velge handlingen **Bokfør**.</span><span class="sxs-lookup"><span data-stu-id="93e3a-141">When the sales order is complete, choose the **Post** action.</span></span>

<span data-ttu-id="93e3a-142">Du kan deretter fylle ut eller redigere felt på det nye varekortet etter behov.</span><span class="sxs-lookup"><span data-stu-id="93e3a-142">You can then fill or edit fields on the new item card as necessary.</span></span> <span data-ttu-id="93e3a-143">Hvis du vil ha mer informasjon, kan du se [Registrere nye varer](inventory-how-register-new-items.md).</span><span class="sxs-lookup"><span data-stu-id="93e3a-143">For more information, see [How to: Register New Items](inventory-how-register-new-items.md).</span></span>

> [!NOTE]  
>   <span data-ttu-id="93e3a-144">En varekryssreferansepost opprettes automatisk for leverandøren av varen mellom leverandørens varenummer og det nye varenummeret ditt.</span><span class="sxs-lookup"><span data-stu-id="93e3a-144">An Item cross reference record is automatically created for the vendor of the item between the vendor's item number and your new item number.</span></span>

## <a name="see-also"></a><span data-ttu-id="93e3a-145">Se også</span><span class="sxs-lookup"><span data-stu-id="93e3a-145">See Also</span></span>
[<span data-ttu-id="93e3a-146">Registrere nye varer</span><span class="sxs-lookup"><span data-stu-id="93e3a-146">How to: Register New Items</span></span>](inventory-how-register-new-items.md)  
<span data-ttu-id="93e3a-147">[Opprette spesialbestillinger](sales-how-to-create-special-orders.md)|</span><span class="sxs-lookup"><span data-stu-id="93e3a-147">[How to: Create Special Orders](sales-how-to-create-special-orders.md)|</span></span>  
[<span data-ttu-id="93e3a-148">Lager</span><span class="sxs-lookup"><span data-stu-id="93e3a-148">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="93e3a-149">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="93e3a-149">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

