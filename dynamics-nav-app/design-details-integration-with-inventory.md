---
title: Designdetaljer - Integrasjon med lagerbeholdning
description: Modulen Lagerstyring og modulen Lager samhandler med hverandre i vareopptelling og i lagerjustering.
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
ms.openlocfilehash: c6f6c03a1a66f5d4f86c85f43ab7c93a4e003c45
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="design-details-integration-with-inventory"></a><span data-ttu-id="47002-103">Designdetaljer: Integrasjon med lagerbeholdning</span><span class="sxs-lookup"><span data-stu-id="47002-103">Design Details: Integration with Inventory</span></span>
<span data-ttu-id="47002-104">Modulen Lagerstyring og modulen Lager samhandler med hverandre i vareopptelling og i lagerjustering.</span><span class="sxs-lookup"><span data-stu-id="47002-104">The Warehouse Management application area and the Inventory application area interact with one another in physical inventory and in inventory or warehouse adjustment.</span></span>  
  
## <a name="physical-inventory"></a><span data-ttu-id="47002-105">Physical Inventory</span><span class="sxs-lookup"><span data-stu-id="47002-105">Physical Inventory</span></span>  
 <span data-ttu-id="47002-106">Vinduet **Lagervareopptellingskladd** brukes med vinduet **Vareopptellingskladd** for alle avanserte lagerlokasjoner.</span><span class="sxs-lookup"><span data-stu-id="47002-106">The **Whse. Phys. Inventory Journal** window is used with the **Phys. Inventory Journal** window for all advanced warehouse locations.</span></span> <span data-ttu-id="47002-107">Lageret beregnes på hyllenivå, og den lageransatte får en listeutskrift.</span><span class="sxs-lookup"><span data-stu-id="47002-107">The inventory on bin level is calculated, and a printed list is provided for the warehouse employee.</span></span> <span data-ttu-id="47002-108">Listen viser hvilke varer som må telles i hvilke hyller.</span><span class="sxs-lookup"><span data-stu-id="47002-108">The list shows which items in which bins must be counted.</span></span>  
  
 <span data-ttu-id="47002-109">Den lageransatte registrerer det opptalte antallet i vinduet **Lagervareopptellingskladd** og bokfører deretter kladden.</span><span class="sxs-lookup"><span data-stu-id="47002-109">The warehouse employee enters the counted quantity in the **Whse. Phys. Inventory Journal** window and then posts the journal.</span></span>  
  
 <span data-ttu-id="47002-110">Hvis det opptalte antallet er større enn antallet på kladdelinjen, blir det bokført en bevegelse for denne forskjellen fra standard justeringshylle til hyllen som telles.</span><span class="sxs-lookup"><span data-stu-id="47002-110">If the counted quantity is greater than the quantity on the journal line, a movement is posted for this difference from the default adjustment bin to the counted bin.</span></span> <span data-ttu-id="47002-111">Dette øker antallet på den opptalte hyllen og reduserer antallet på standard justeringshylle.</span><span class="sxs-lookup"><span data-stu-id="47002-111">This increases the quantity in the counted bin and decreases the quantity in the default adjustment bin.</span></span>  
  
 <span data-ttu-id="47002-112">Hvis det opptalte antallet er mindre enn antallet på kladdelinjen, blir det bokført en flytting for denne forskjellen fra den talte hyllen til standard justeringshylle.</span><span class="sxs-lookup"><span data-stu-id="47002-112">If the quantity counted is less than the quantity on the journal line, a movement for this difference is posted from the counted bin to the default adjustment bin.</span></span> <span data-ttu-id="47002-113">Dette reduserer antallet på den opptalte hyllen og øker antallet på standard justeringshylle.</span><span class="sxs-lookup"><span data-stu-id="47002-113">This decreases the quantity in the counted bin and increases the quantity in the default adjustment bin.</span></span>  
  
 <span data-ttu-id="47002-114">I avanserte lagerskonfigurasjoner blir verdien i feltet **Antall (beregnet)** hentet fra varepostene, og verdien i feltet **Antall (opptalt)** blir hentet fra lagerposter, unntatt justeringshylleinnholdet.</span><span class="sxs-lookup"><span data-stu-id="47002-114">In advanced warehouse configurations, the value in the **Quantity (Calculated)** field is retrieved from item ledger entries and the value in the **Quantity (Phys. Inventory)** field is retrieved from warehouse entries, excluding the adjustment bin content.</span></span> <span data-ttu-id="47002-115">**Antall**-feltet angir forskjellen mellom de to første feltene, som skal være lik innholdet i justeringshyllen.</span><span class="sxs-lookup"><span data-stu-id="47002-115">The **Quantity** field specifies the difference between the first two fields, which should be equal to the contents of the adjustment bin.</span></span>  
  
 <span data-ttu-id="47002-116">Når du bokfører vareopptellingskladden, oppdateres lageret og standard justeringshylle.</span><span class="sxs-lookup"><span data-stu-id="47002-116">When you post the physical inventory journal, the inventory and the default adjustment bin are updated.</span></span>  
  
### <a name="warehouse-adjustments-to-the-item-ledger"></a><span data-ttu-id="47002-117">Lagerjusteringer i vareposten</span><span class="sxs-lookup"><span data-stu-id="47002-117">Warehouse Adjustments to the Item Ledger</span></span>  
 <span data-ttu-id="47002-118">Du bruker **Varekladd**-vinduet og funksjonen **Beregn lagerjustering** til å justere lagerbeholdningen i vareposten i samsvar med en justering som er gjort i vareantallet i en lagerhylle.</span><span class="sxs-lookup"><span data-stu-id="47002-118">You use the **Item Journal** window and the **Calculate Whse. Adjustment** function to adjust inventory on the item ledger in accordance with an adjustment that has been made to the item quantity in a warehouse bin.</span></span> <span data-ttu-id="47002-119">Hvis du vil opprette en kobling mellom beholdningen og lageret, må du definere en standard justeringshylle per lokasjon.</span><span class="sxs-lookup"><span data-stu-id="47002-119">To create a link between the inventory and the warehouse, you must define a default adjustment bin per location.</span></span>  
  
 <span data-ttu-id="47002-120">Standard justeringshylle registrerer varer på lageret når du bokfører en økning for lageret.</span><span class="sxs-lookup"><span data-stu-id="47002-120">The default adjustment bin registers items in the warehouse when you post an increase for the inventory.</span></span> <span data-ttu-id="47002-121">Hvis du bokfører en reduksjon, blir imidlertid antallet på standardhyllen også redusert.</span><span class="sxs-lookup"><span data-stu-id="47002-121">However, if you post a decrease, the quantity on the default bin is also decreased.</span></span> <span data-ttu-id="47002-122">I begge tilfeller blir det opprettet vareposter og lagerposter.</span><span class="sxs-lookup"><span data-stu-id="47002-122">In both cases, item ledger entries and warehouse entries are created.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="47002-123">Justeringshyllen er ikke inkludert i tilgjengelighetsberegningen.</span><span class="sxs-lookup"><span data-stu-id="47002-123">The adjustment bin is not included in the availability calculation.</span></span>  
  
 <span data-ttu-id="47002-124">Hvis du vil justere hylleinnholdet, kan du bruke lagervarekladden der du kan angi varenummer, sonekode, hyllekode og antall som du vil justere.</span><span class="sxs-lookup"><span data-stu-id="47002-124">If you want to adjust the bin content, you can use the warehouse item journal, from which you can enter the item number, zone code, bin code, and quantity that you want to adjust.</span></span>  
  
 <span data-ttu-id="47002-125">Hvis du angir et positivt antall og bokfører linjen, økes beholdningen som er lagret på hyllen, og antallet i standard justeringshylle reduseres tilsvarende.</span><span class="sxs-lookup"><span data-stu-id="47002-125">If you enter a positive quantity and post the line, then the inventory stored in the bin increases, and the quantity of the default adjustment bin decreases correspondingly.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="47002-126">Se også</span><span class="sxs-lookup"><span data-stu-id="47002-126">See Also</span></span>  
 <span data-ttu-id="47002-127">[Designdetaljer: Lagerstyring](design-details-warehouse-management.md) </span><span class="sxs-lookup"><span data-stu-id="47002-127">[Design Details: Warehouse Management](design-details-warehouse-management.md) </span></span>  
 [<span data-ttu-id="47002-128">Designdetaljer: Tilgjengelighet i lageret</span><span class="sxs-lookup"><span data-stu-id="47002-128">Design Details: Availability in the Warehouse</span></span>](design-details-availability-in-the-warehouse.md)
