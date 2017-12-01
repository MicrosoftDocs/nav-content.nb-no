---
title: Dele lageraktivitetslinjer
description: "I plasseringer, flyttinger eller plukkinger og i lagerplasseringer og lagerplukkinger foreslås det hyller for plukking eller plassering av varer. Det kan hende at det faktiske antallet i den foreslåtte hyllen ikke er tilstrekkelig, eller at det ikke er nok plass i den foreslåtte hyllen til å plassere det nødvendige antallet. I slike tilfeller må du dele linjen, slik at varene på en linje blir hentet fra eller plassert i flere enn én hylle."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 8b2ab806f9499f9d54ed3ec79ca2874a71d8c730
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-split-warehouse-activity-lines"></a><span data-ttu-id="07f7c-105">Dele lageraktivitetslinjer</span><span class="sxs-lookup"><span data-stu-id="07f7c-105">How to: Split Warehouse Activity Lines</span></span>
<span data-ttu-id="07f7c-106">I plasseringer, flyttinger eller plukkinger og i lagerplasseringer og lagerplukkinger foreslås det hyller for plukking eller plassering av varer.</span><span class="sxs-lookup"><span data-stu-id="07f7c-106">In warehouse put-aways, movements, or picks, and in inventory put-aways and inventory picks, bins are suggested for the picking or putting away of items.</span></span> <span data-ttu-id="07f7c-107">Det kan hende at det faktiske antallet i den foreslåtte hyllen ikke er tilstrekkelig, eller at det ikke er nok plass i den foreslåtte hyllen til å plassere det nødvendige antallet.</span><span class="sxs-lookup"><span data-stu-id="07f7c-107">The actual quantity in the bin suggested may not be sufficient, or there is not enough room in the suggested bin to put away the required quantity.</span></span> <span data-ttu-id="07f7c-108">I slike tilfeller må du dele linjen, slik at varene på en linje blir hentet fra eller plassert i flere enn én hylle.</span><span class="sxs-lookup"><span data-stu-id="07f7c-108">In these cases, you need to split the line, so that the items for one line are either taken from or placed into more than one bin.</span></span>  

<span data-ttu-id="07f7c-109">Følgende fremgangsmåte gjelder for lagerdokumenter , for eksempel plassering, flytting og plukklinjer, eller lagerplassering, flytting og plukklinjer.</span><span class="sxs-lookup"><span data-stu-id="07f7c-109">The following procedure applies to warehouse documents, such as warehouse put-away, movement, and pick lines, or inventory put-away, movement, and pick lines.</span></span>  

## <a name="to-split-warehouse-activity-lines"></a><span data-ttu-id="07f7c-110">Slik deler du lageraktivitetslinjer:</span><span class="sxs-lookup"><span data-stu-id="07f7c-110">To split warehouse activity lines</span></span>  
1.  <span data-ttu-id="07f7c-111">Åpne en lageraktivitetslinje hvor du prøver å håndtere et utilstrekkelig antall.</span><span class="sxs-lookup"><span data-stu-id="07f7c-111">Open a warehouse activity line where you are trying to handle an insufficient quantity.</span></span>  
2.  <span data-ttu-id="07f7c-112">Angi det reduserte antallet du kan håndtere, i feltet **Ant. som skal håndt.**.</span><span class="sxs-lookup"><span data-stu-id="07f7c-112">In the **Qty. to Handle** field, enter the reduced quantity that you are able to handle.</span></span>  
3.  <span data-ttu-id="07f7c-113">På hurtigfanen **Linjer** velger du handlingen **Handlinger**, **Funksjoner**, og deretter **Del linje**.</span><span class="sxs-lookup"><span data-stu-id="07f7c-113">On the **Lines** FastTab, choose the **Actions** action, choose the **Functions** action, and then choose the **Split Line** action.</span></span> <span data-ttu-id="07f7c-114">Det vises en ny linje som er en kopi av den opprinnelige linjen, bortsett fra at feltet **Ant. som skal håndt.** inneholder antallet du fjernet fra den opprinnelige linjen.</span><span class="sxs-lookup"><span data-stu-id="07f7c-114">A new line appears, which is a copy of the original line, except that the **Qty. to Handle** field contains the quantity that you removed from the original line.</span></span>  
4.  <span data-ttu-id="07f7c-115">Tilordne den aktuelle hyllen og, hvis du bruker lagerstyring, sonen, til den nye linjen, eller del eventuell linjen flere ganger til du finner hyller til alle antallene.</span><span class="sxs-lookup"><span data-stu-id="07f7c-115">Assign an appropriate bin and, if you are using directed put-away and pick, a zone, to this new line, or continue splitting the line as necessary until you find appropriate bins for all of the quantity.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="07f7c-116">Hvis lokasjonen bruker lagerstyring og du deler linjene, må du være kjent med lageret, og du må være i stand til å velge en hylle som samsvarer med lagringskravene for varen, og som oppfyller de generelle kravene i lagerdokumentet.</span><span class="sxs-lookup"><span data-stu-id="07f7c-116">If the location uses directed put-away and pick and you split the lines, you must be familiar with the warehouse and be able to choose a bin that matches the storage requirements of the item and that fulfills the general requirements of the warehouse document.</span></span> <span data-ttu-id="07f7c-117">Du bør for eksempel ikke dele en linje i et plukkdokument og plasser noen varer i masselagringen.</span><span class="sxs-lookup"><span data-stu-id="07f7c-117">For example, you would not split a line on a pick document and place some items in the bulk storage.</span></span>  

## <a name="see-also"></a><span data-ttu-id="07f7c-118">Se også</span><span class="sxs-lookup"><span data-stu-id="07f7c-118">See Also</span></span>  
[<span data-ttu-id="07f7c-119">Lagerstyring</span><span class="sxs-lookup"><span data-stu-id="07f7c-119">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="07f7c-120">Lager</span><span class="sxs-lookup"><span data-stu-id="07f7c-120">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="07f7c-121">[Definere lagerstyring](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="07f7c-121">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="07f7c-122">[Monteringsstyring](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="07f7c-122">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="07f7c-123">Designdetaljer: Lagerstyring</span><span class="sxs-lookup"><span data-stu-id="07f7c-123">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="07f7c-124">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="07f7c-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

