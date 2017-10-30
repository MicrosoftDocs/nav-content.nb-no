---
title: Definere koder for standardservicer
description: "Finn ut hvordan du kan definere koder for serviceaktiviteter som utføres ofte."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: service, service item, service order, repairs, maintenance
ms.date: 08/22/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 109e71ab1b06ccbe0a931a998ae0681713eff9da
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-set-up-standard-service-codes"></a><span data-ttu-id="75d43-103">Definere standard servicekoder</span><span class="sxs-lookup"><span data-stu-id="75d43-103">How to: Set Up Standard Service Codes</span></span>
<span data-ttu-id="75d43-104">Når du utfører typisk service, må du ofte opprette servicedokumenter som bruker servicelinjer som inneholder omtrent samme opplysninger.</span><span class="sxs-lookup"><span data-stu-id="75d43-104">When you perform typical service, you often have to create service documents that use service lines that contain similar information.</span></span> <span data-ttu-id="75d43-105">Hvis du vil gjøre det enkelt å opprette disse linjene, kan du definere standard servicekoder som er et forhåndsdefinert sett med servicelinjer.</span><span class="sxs-lookup"><span data-stu-id="75d43-105">To make it easy to create these lines, you can set up standard service codes that have a predefined set of service lines.</span></span> <span data-ttu-id="75d43-106">Når du velger koden i et servicedokument, angis linjene automatisk.</span><span class="sxs-lookup"><span data-stu-id="75d43-106">When you choose the code on a service document, the lines are entered automatically.</span></span> <span data-ttu-id="75d43-107">Du kan angi så mange standard servicekoder du vil, og hver kode kan ha et ubegrenset antall servicelinjer av ulike typer, inkludert vare, ressurs, kostnad eller standardtekst, knyttet til seg.</span><span class="sxs-lookup"><span data-stu-id="75d43-107">You can set up any number of standard service codes, and each code can have an unlimited number of service lines of different types, including item, resource, cost, or standrd text linked to it.</span></span> <span data-ttu-id="75d43-108">Det kan opprettes servicelinjer for hver standard servicekode i korter **Standard servicekode**.</span><span class="sxs-lookup"><span data-stu-id="75d43-108">You create service lines of each standard serice code on the **Standard Service Code** card.</span></span> <span data-ttu-id="75d43-109">Du tilordner deretter standard servicekoder til servicevaregrupper på siden **Standard servicevaregruppekoder**.</span><span class="sxs-lookup"><span data-stu-id="75d43-109">You then assign standard service codes to service item groups on the **Standard Serv. Item Gr. Codes** page.</span></span> <span data-ttu-id="75d43-110">Senere, når du oppretter et servicedokument, kan du bruke handlingen **Hent standard servicekoder** for å legge til servicelinjer.</span><span class="sxs-lookup"><span data-stu-id="75d43-110">Later, when you create a service document, you can use the **Get Standard Service Codes** action to add service lines.</span></span>  
  
> [!Tip]
>  <span data-ttu-id="75d43-111">Du kan bruke samme metode for å opprette linjer i salgs- og kjøpsdokumenter.</span><span class="sxs-lookup"><span data-stu-id="75d43-111">You can use the same concept to create lines on sales and purchase documents.</span></span> <span data-ttu-id="75d43-112">Hvis du vil ha mer informasjon, se [Opprette gjentakende salgs- og kjøpslinjer](sales-how-work-standard-lines.md).</span><span class="sxs-lookup"><span data-stu-id="75d43-112">For more information, see [How to: Create Recurring Sales and Purchase Lines](sales-how-work-standard-lines.md).</span></span>    
  
## <a name="to-set-up-a-standard-service-code"></a><span data-ttu-id="75d43-113">Slik definerer du standard servicekoder</span><span class="sxs-lookup"><span data-stu-id="75d43-113">To set up a standard service code</span></span>    
1. <span data-ttu-id="75d43-114">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Standard servicekoder**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="75d43-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Standard Service Codes**, and then choose the related link.</span></span>  
2. <span data-ttu-id="75d43-115">Fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="75d43-115">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. <span data-ttu-id="75d43-116">Fyll ut servicelinjene som er koblet til denne servicekoden.</span><span class="sxs-lookup"><span data-stu-id="75d43-116">Fill in the service lines linked to this service code.</span></span>  

## <a name="to-assign-a-standard-service-code-to-a-service-item-group"></a><span data-ttu-id="75d43-117">Slik knytter du en standard servicekode til en servicevaregruppe</span><span class="sxs-lookup"><span data-stu-id="75d43-117">To assign a standard service code to a service item group</span></span>
1. <span data-ttu-id="75d43-118">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Servicevaregrupper**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="75d43-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service item Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="75d43-119">Fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="75d43-119">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="75d43-120">Fyll ut servicelinjene som er koblet til denne servicekoden.</span><span class="sxs-lookup"><span data-stu-id="75d43-120">Fill in the service lines linked to this service code.</span></span>  

## <a name="see-also"></a><span data-ttu-id="75d43-121">Se også</span><span class="sxs-lookup"><span data-stu-id="75d43-121">See Also</span></span>
[<span data-ttu-id="75d43-122">Servicehåndtering</span><span class="sxs-lookup"><span data-stu-id="75d43-122">Service Management</span></span>](service-service.md)
