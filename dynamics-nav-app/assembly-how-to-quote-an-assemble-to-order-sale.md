---
title: "Gi tilbud på et montere-til-ordre-salg"
description: "Du kan bruke monteringsstyring for å tilpasse en monteringsvare i henhold til en kundeforespørsel under salgsprosessen."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 0835be9e00b7958bfc0506cf99a856905e057d4b
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-quote-an-assemble-to-order-sale"></a><span data-ttu-id="5b80d-103">Gi tilbud på et montere-til-ordre-salg</span><span class="sxs-lookup"><span data-stu-id="5b80d-103">How to: Quote an Assemble-to-Order Sale</span></span>
<span data-ttu-id="5b80d-104">Du kan bruke monteringsstyring for å tilpasse en monteringsvare i henhold til en kundeforespørsel under salgsprosessen.</span><span class="sxs-lookup"><span data-stu-id="5b80d-104">You can use assembly management to customize an assembly item to a customer’s request during the sales process.</span></span> <span data-ttu-id="5b80d-105">Hvis du vil ha mer informasjon, kan du se [Selge varer som er montert til ordre](assembly-how-to-sell-items-assembled-to-order.md).</span><span class="sxs-lookup"><span data-stu-id="5b80d-105">For more information, see [How to: Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span></span>  

<span data-ttu-id="5b80d-106">Etter hvert som du selger en hvilken som helst annen type vare, kan du også opprette et tilbud for en tilpasset monteringsvare før du konverterer det til en ordre.</span><span class="sxs-lookup"><span data-stu-id="5b80d-106">As when you sell any other type of item, you can also create a sales quote for a customized assembly item before converting it to a sales order.</span></span> <span data-ttu-id="5b80d-107">Denne prosessen omfatter flere ekstra trinn når du sammenligner den med å opprette et vanlig tilbud, og den bruker en variant av en koblet monteringsordre, som er et monteringstilbud.</span><span class="sxs-lookup"><span data-stu-id="5b80d-107">This process involves several extra steps when you compare it to creating a regular sales quote, and it uses a variation of a linked assembly order, which is an assembly quote.</span></span>

> [!NOTE]  
>  <span data-ttu-id="5b80d-108">I likhet med alle typer tilbud brukes ikke antallene på monteringstilbud i tilgjengelighet, planlegging eller reservasjoner.</span><span class="sxs-lookup"><span data-stu-id="5b80d-108">Like all types of quotes, the quantities on assembly quotes are not used in availability, planning, or reservations.</span></span>  

## <a name="to-create-a-sales-quote-for-an-assemble-to-order-item"></a><span data-ttu-id="5b80d-109">Slik oppretter du et tilbud for en montere-til-ordre-vare:</span><span class="sxs-lookup"><span data-stu-id="5b80d-109">To create a sales quote for an assemble-to-order item</span></span>  
1.  <span data-ttu-id="5b80d-110">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Tilbud**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="5b80d-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Quote**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="5b80d-111">Opprette en ny tilbudslinje med én linje for en monteringsvare.</span><span class="sxs-lookup"><span data-stu-id="5b80d-111">Create a sales quote line with one line for an assembly item.</span></span> <span data-ttu-id="5b80d-112">Hvis du vil ha mer informasjon, kan du se [Gi tilbud](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="5b80d-112">For more information, see [How to: Make Offers](sales-how-make-offers.md).</span></span>  
3.  <span data-ttu-id="5b80d-113">Angi hele antallet i feltet **Ant. som skal monteres til ordre**.</span><span class="sxs-lookup"><span data-stu-id="5b80d-113">In the **Qty. to Assemble to Order** field, enter the full quantity.</span></span>

    > [!NOTE]  
    >  <span data-ttu-id="5b80d-114">Du bør ikke gi tilbud på et delvist antall.</span><span class="sxs-lookup"><span data-stu-id="5b80d-114">You should not quote a partial quantity.</span></span> <span data-ttu-id="5b80d-115">Du må derfor angi samme antall som du skrev inn i feltet **Antall** på tilbudslinjen.</span><span class="sxs-lookup"><span data-stu-id="5b80d-115">Therefore, you must enter the same quantity that you entered in the **Quantity** field on the sales quote line.</span></span>  

4.  <span data-ttu-id="5b80d-116">På hurtigfanen **Linjer**, velg **Linje**, **Monter til ordre**, og deretter **Montere til ordre – linjer**.</span><span class="sxs-lookup"><span data-stu-id="5b80d-116">On the **Lines** FastTab, choose **Line**, choose **Assemble to Order**, and then choose **Assemble-to-Order Lines**.</span></span> <span data-ttu-id="5b80d-117">Du kan også merke feltet **Ant. som skal monteres til ordre** på linjen.</span><span class="sxs-lookup"><span data-stu-id="5b80d-117">Alternatively, choose the **Qty. to Assemble to Order** field on the line.</span></span>  
5.  <span data-ttu-id="5b80d-118">Gå gjennom eller endre monteringsordrelinjene i henhold til tilbudet kunden ber om, i vinduet **Montere til ordre – linjer**.</span><span class="sxs-lookup"><span data-stu-id="5b80d-118">In the **Assemble-to-Order Lines** window, review or modify the assembly order lines according to the quote that the customer is requesting.</span></span> <span data-ttu-id="5b80d-119">Hvis du vil vise mer informasjon, velger du **Vis dokument** for å åpne hele rammetilbudsordren.</span><span class="sxs-lookup"><span data-stu-id="5b80d-119">If you want to view more information, choose the **Show Document** action to open the complete blanket quote order.</span></span> <span data-ttu-id="5b80d-120">Du kan ikke endre innholdet i de fleste av feltene, og du kan ikke bokføre.</span><span class="sxs-lookup"><span data-stu-id="5b80d-120">You cannot change the contents of most fields, and you cannot post.</span></span>  
6.  <span data-ttu-id="5b80d-121">Når du har justert monteringsordrelinjene i henhold til tilbudet, lukker du vinduet **Montere til ordre – linjer** for å gå tilbake til vinduet **Tilbud**.</span><span class="sxs-lookup"><span data-stu-id="5b80d-121">When you have adjusted the assembly order lines according to the quote, close the **Assemble-to-Order Lines** window to return to the **Sales Quote** window.</span></span>  
7.  <span data-ttu-id="5b80d-122">Hvis kunden godtar tilbudet, oppretter du en ordre for den aktuelle monteringsvaren.</span><span class="sxs-lookup"><span data-stu-id="5b80d-122">If the customer accepts the quote, then create a sales order for the quoted assembly item.</span></span> <span data-ttu-id="5b80d-123">Hvis du vil ha mer informasjon, kan du se [Gi tilbud](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="5b80d-123">For more information, see [How to: Make Offers](sales-how-make-offers.md).</span></span> <span data-ttu-id="5b80d-124">Det koblede monteringstilbudet og eventuelle tilpasninger knyttes til denne nye salgsordren for å klargjøre for montering av varen(e) som skal selges.</span><span class="sxs-lookup"><span data-stu-id="5b80d-124">The linked assembly quote and any customizations are linked to that new sales order to prepare for assembly of the item or items to be sold.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5b80d-125">Se også</span><span class="sxs-lookup"><span data-stu-id="5b80d-125">See Also</span></span>  
[<span data-ttu-id="5b80d-126">Monteringsstyring</span><span class="sxs-lookup"><span data-stu-id="5b80d-126">Assembly Management</span></span>](assembly-assemble-items.md)  
[<span data-ttu-id="5b80d-127">Arbeide med stykklister</span><span class="sxs-lookup"><span data-stu-id="5b80d-127">How to: Work with Bills of Material</span></span>](inventory-how-work-BOMs.md)  
[<span data-ttu-id="5b80d-128">Lager</span><span class="sxs-lookup"><span data-stu-id="5b80d-128">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="5b80d-129">Designdetaljer: Lagerstyring</span><span class="sxs-lookup"><span data-stu-id="5b80d-129">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="5b80d-130">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5b80d-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

