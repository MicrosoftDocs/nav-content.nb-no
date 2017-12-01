---
title: "Definere transportører"
description: "Du kan definere en kode for hver enkelt transportør og angi opplysninger om dem."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 5212c0be8e0efdaa088500edc9ac71c46783eba7
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-set-up-shipping-agents"></a><span data-ttu-id="d47b3-103">Definere transportører</span><span class="sxs-lookup"><span data-stu-id="d47b3-103">How to: Set Up Shipping Agents</span></span>
<span data-ttu-id="d47b3-104">Du kan definere en kode for hver enkelt transportør og angi opplysninger om dem.</span><span class="sxs-lookup"><span data-stu-id="d47b3-104">You can set up a code for each of your shipping agents and enter information about them.</span></span>  

<span data-ttu-id="d47b3-105">Hvis du oppgir en internettadresse til transportøren, og vedkommende tilbyr pakkesporingsservice på Internett, kan du bruke funksjonen for automatisk sporing av pakker.</span><span class="sxs-lookup"><span data-stu-id="d47b3-105">If you enter an Internet address for the shipping agent, and the agent provides package tracking services on the Internet, you can use the automatic package tracking feature.</span></span> <span data-ttu-id="d47b3-106">Hvis du vil ha mer informasjon, kan du se [Spore pakker](sales-how-track-packages.md).</span><span class="sxs-lookup"><span data-stu-id="d47b3-106">For more information, see [How to: Track Packages](sales-how-track-packages.md).</span></span>

<span data-ttu-id="d47b3-107">Når du definerer transportører i ordrene, kan du også angi hvilken service den enkelte transportør tilbyr.</span><span class="sxs-lookup"><span data-stu-id="d47b3-107">When you set up shipping agents on your sales orders, you can also specify the services that each shipping agent offers.</span></span>  
<span data-ttu-id="d47b3-108">Du kan definere et ubegrenset serviceantall for hver transportør, og angi en leveringstid for den enkelte service som utføres.</span><span class="sxs-lookup"><span data-stu-id="d47b3-108">For each shipping agent, you can set up an unlimited number of services, and you can specify a shipping time for each service.</span></span>  

<span data-ttu-id="d47b3-109">Når du har tilordnet en transportørservice til en ordrelinje, tas leveringstiden for servicen med i beregningen av ordrebekreftelsen for denne linjen.</span><span class="sxs-lookup"><span data-stu-id="d47b3-109">When you have assigned a shipping agent service to a sales order line, the shipping time of the service will be included in the order promising calculation, for that line.</span></span> <span data-ttu-id="d47b3-110">Hvis du vil ha mer informasjon, kan du se [Beregne ordrebekreftelsesdatoer](sales-how-to-calculate-order-promising-dates.md).</span><span class="sxs-lookup"><span data-stu-id="d47b3-110">For more information, see [How to: Calculate Order Promising Dates](sales-how-to-calculate-order-promising-dates.md).</span></span>

## <a name="to-set-up-a-shipping-agent"></a><span data-ttu-id="d47b3-111">Slik definerer du transportører</span><span class="sxs-lookup"><span data-stu-id="d47b3-111">To set up a shipping agent</span></span>  
1.  <span data-ttu-id="d47b3-112">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport")-ikonet, angi **Transportører**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="d47b3-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Shipping Agents**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="d47b3-113">Fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="d47b3-113">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]<span data-ttu-id="d47b3-114">.</span><span class="sxs-lookup"><span data-stu-id="d47b3-114">.</span></span>  
3.  <span data-ttu-id="d47b3-115">Velg handlingen **Transportørservice**.</span><span class="sxs-lookup"><span data-stu-id="d47b3-115">Choose the **Shipping Agent Services** action.</span></span>
4. <span data-ttu-id="d47b3-116">I vinduet **Transportørservice** fyller du ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="d47b3-116">In the **Shipping Agent Services**, fill in the fields as necessary.</span></span>

> [!NOTE]  
>  <span data-ttu-id="d47b3-117">Hvis du sletter transportøren på ordrelinjen, slettes også transportørservicekoden.</span><span class="sxs-lookup"><span data-stu-id="d47b3-117">If you delete the shipping agent on the order line, the shipping agent service code is also deleted.</span></span> <span data-ttu-id="d47b3-118">Innholdet i feltene som var delvis basert på transportørservice, beregnes på nytt.</span><span class="sxs-lookup"><span data-stu-id="d47b3-118">The contents of fields that were based in part on the shipping agent service are recalculated.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d47b3-119">Se også</span><span class="sxs-lookup"><span data-stu-id="d47b3-119">See Also</span></span>
<span data-ttu-id="d47b3-120">[Spore pakker](sales-how-track-packages.md)  </span><span class="sxs-lookup"><span data-stu-id="d47b3-120">[How to: Track Packages](sales-how-track-packages.md)  </span></span>  
[<span data-ttu-id="d47b3-121">Lagerstyring</span><span class="sxs-lookup"><span data-stu-id="d47b3-121">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="d47b3-122">Lager</span><span class="sxs-lookup"><span data-stu-id="d47b3-122">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="d47b3-123">[Definere lagerstyring](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="d47b3-123">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="d47b3-124">[Monteringsstyring](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="d47b3-124">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="d47b3-125">Designdetaljer: Lagerstyring</span><span class="sxs-lookup"><span data-stu-id="d47b3-125">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="d47b3-126">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d47b3-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

