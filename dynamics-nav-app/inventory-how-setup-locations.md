---
title: "Definere et lokasjonskort og definere overføringsruter"
description: "Du oppretter et lokasjonskort for hvert sted der du oppbevarer lagervarer, for eksempel et lager eller distribusjonssenter, og definerer ruter for å overføre varer mellom lokasjoner."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, distribution center
ms.date: 06/02/2017
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 2a0d35e11b6a0ee480cf0034c885157fe1de3916
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-set-up-locations"></a><span data-ttu-id="79b74-103">Definere lokasjoner</span><span class="sxs-lookup"><span data-stu-id="79b74-103">How to: Set Up Locations</span></span>
<span data-ttu-id="79b74-104">Hvis du kjøper, lagrer eller selger varer på flere lokasjoner eller lagre, må du definere hver lokasjon med et lokasjonskort og definere overføringsruter.</span><span class="sxs-lookup"><span data-stu-id="79b74-104">If you buy, store, or sell items at more than one place or warehouse, you must set each location up with a location card and define transfer routes.</span></span>

<span data-ttu-id="79b74-105">Deretter kan du opprette dokumentlinjer for en bestemt lokasjon, vise tilgjengelighet etter lokasjon og overføre beholdning mellom lokasjoner.</span><span class="sxs-lookup"><span data-stu-id="79b74-105">You can then create document lines for a specific location, view availability by location, and transfer inventory between locations.</span></span> <span data-ttu-id="79b74-106">Hvis du vil ha mer informasjon, kan du se [Håndtere lager](inventory-manage-inventory.md).</span><span class="sxs-lookup"><span data-stu-id="79b74-106">For more information, see [Manage Inventory](inventory-manage-inventory.md).</span></span>

## <a name="to-create-a-location-card"></a><span data-ttu-id="79b74-107">Slik oppretter du et lokasjonskort</span><span class="sxs-lookup"><span data-stu-id="79b74-107">To create a location card</span></span>
1. <span data-ttu-id="79b74-108">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Lokasjoner**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="79b74-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span></span>
2. <span data-ttu-id="79b74-109">Velg handlingen **Ny**.</span><span class="sxs-lookup"><span data-stu-id="79b74-109">Choose the **New** action.</span></span>
3. <span data-ttu-id="79b74-110">I vinduet **Lokasjonskort** fyller du ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="79b74-110">In the **Location Card** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="79b74-111">Gjenta trinn 2 og 3 for hver beholdninglokasjon.</span><span class="sxs-lookup"><span data-stu-id="79b74-111">Repeat steps 2 and 3 for every location where you want to keep inventory.</span></span>

> [!NOTE]  
> <span data-ttu-id="79b74-112">Mange felt på lokasjonskortet refererer til håndteringen av varer i inngående og utgående lagerprosesser.</span><span class="sxs-lookup"><span data-stu-id="79b74-112">Many fields on the location card refer to the handling of items in inbound and outbound warehouse processes.</span></span> <span data-ttu-id="79b74-113">Du finner mer informasjon under [Definere lagerstyring](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="79b74-113">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>

## <a name="to-create-a-transfer-route"></a><span data-ttu-id="79b74-114">Slik oppretter du overføringsruter</span><span class="sxs-lookup"><span data-stu-id="79b74-114">To create a transfer route</span></span>
1. <span data-ttu-id="79b74-115">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Overføringsruter**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="79b74-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer Routes**, and then choose the related link.</span></span>
2. <span data-ttu-id="79b74-116">Fra vinduet **Lokasjonskort** kan du også velge handlingen **Overføringsruter**.</span><span class="sxs-lookup"><span data-stu-id="79b74-116">Alternatively, from any **Location Card** window, choose the **Transfer Routes** action.</span></span>
3. <span data-ttu-id="79b74-117">Velg handlingen **Ny**.</span><span class="sxs-lookup"><span data-stu-id="79b74-117">Choose the **New** action.</span></span>
4. <span data-ttu-id="79b74-118">I vinduet **Lokasjonskort** fyller du ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="79b74-118">In the **Location Card** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="79b74-119">Nå kan du overføre lagervarer mellom to lokasjoner.</span><span class="sxs-lookup"><span data-stu-id="79b74-119">You can now transfer inventory items between two locations.</span></span> <span data-ttu-id="79b74-120">Hvis du vil ha mer informasjon, kan du se [Overføre beholdning mellom lokasjoner](inventory-how-transfer-between-locations.md).</span><span class="sxs-lookup"><span data-stu-id="79b74-120">For more information, see [How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md).</span></span>    

## <a name="see-also"></a><span data-ttu-id="79b74-121">Se også</span><span class="sxs-lookup"><span data-stu-id="79b74-121">See Also</span></span>
[<span data-ttu-id="79b74-122">Håndtere lager</span><span class="sxs-lookup"><span data-stu-id="79b74-122">Manage Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="79b74-123">[Overføre beholdning mellom lokasjoner](inventory-how-transfer-between-locations.md)  </span><span class="sxs-lookup"><span data-stu-id="79b74-123">[How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md)  </span></span>  
<span data-ttu-id="79b74-124">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="79b74-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="79b74-125">[Tilpasse [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-customizing-overview.md)</span><span class="sxs-lookup"><span data-stu-id="79b74-125">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-customizing-overview.md)</span></span>  
[<span data-ttu-id="79b74-126">Generelle forretningsfunksjoner</span><span class="sxs-lookup"><span data-stu-id="79b74-126">General Business Functionality</span></span>](ui-across-business-areas.md)

