---
title: Administrere lagerkostnader
description: "Kostnadsstyring, også kalt \"kostredegjøring\", handler om å registrere og rapportere kostnader ved forretningsdrift. Det inkluderer rapportering av produksjonskost og lagerkost, det vil si verdien av varene."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 5fc94b0e695f65f19f9d4c5a35814c410aacbd2a
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="managing-inventory-costs"></a><span data-ttu-id="1e4d5-104">Administrere lagerkostnader</span><span class="sxs-lookup"><span data-stu-id="1e4d5-104">Managing Inventory Costs</span></span>
<span data-ttu-id="1e4d5-105">Kostnadsstyring, også kalt "kostredegjøring", handler om å registrere og rapportere kostnader ved forretningsdrift.</span><span class="sxs-lookup"><span data-stu-id="1e4d5-105">Cost management, also referred to as “costing”, is concerned with recording and reporting business operating costs.</span></span> <span data-ttu-id="1e4d5-106">Det inkluderer rapportering av produksjonskost og lagerkost, det vil si verdien av varene.</span><span class="sxs-lookup"><span data-stu-id="1e4d5-106">It includes the reporting of manufacturing costs and inventory costs, that is, the value of items.</span></span>   

<span data-ttu-id="1e4d5-107">Sentrale prinsipper å forstå er at lagermetoder definerer hvordan varer verdsettes når de forlater lageret, at kostjustering oppdaterer solgte varers kost med relatert kjøpskost bokført etter salget, og at lagerverdier må bokføres til dedikerte finanskonti ved regelmessige intervaller.</span><span class="sxs-lookup"><span data-stu-id="1e4d5-107">Central principles to understand are that costing methods define how items are valued when they leave inventory, that cost adjustment updates the cost of goods sold with related purchase costs posted after the sale, and that inventory values must be posted to dedicated G/L accounts at regular intervals.</span></span>

<span data-ttu-id="1e4d5-108">Tabellen nedenfor beskriver en sekvens av oppgaver, og har koblinger til emnene som beskriver dem.</span><span class="sxs-lookup"><span data-stu-id="1e4d5-108">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="1e4d5-109">**Hvis du vil**</span><span class="sxs-lookup"><span data-stu-id="1e4d5-109">**To**</span></span>|<span data-ttu-id="1e4d5-110">**Se**</span><span class="sxs-lookup"><span data-stu-id="1e4d5-110">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="1e4d5-111">Lese diverse begrepsmessig informasjon for å forstå prinsippene og definisjonene som styrer funksjonene for lagerkostregnskap i [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="1e4d5-111">Read various conceptual information to understand the principles and definitions that govern the inventory costing accounting functionality in [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)].</span></span>|[<span data-ttu-id="1e4d5-112">Om lagerkost</span><span class="sxs-lookup"><span data-stu-id="1e4d5-112">About Inventory Costing</span></span>](finance-learn-about-costing.md)|  
|<span data-ttu-id="1e4d5-113">Definer lagerperioder, lagermetoder og avrundingsmetoder.</span><span class="sxs-lookup"><span data-stu-id="1e4d5-113">Set up inventory periods, costing methods, and rounding methods.</span></span>|[<span data-ttu-id="1e4d5-114">Definere lagerverdisetting og kostberegning</span><span class="sxs-lookup"><span data-stu-id="1e4d5-114">Setting Up Inventory Valuation and Costing</span></span>](finance-set-up-inventory-valuation-and-costing.md)|
|<span data-ttu-id="1e4d5-115">Skriv opp eller skriv ned verdien av én eller flere varer på lager ved postering av den gjeldende, beregnede verdien.</span><span class="sxs-lookup"><span data-stu-id="1e4d5-115">Appreciate or depreciate the value of one or more items in inventory by posting their current, calculated value.</span></span>|[<span data-ttu-id="1e4d5-116">Revaluere beholdning</span><span class="sxs-lookup"><span data-stu-id="1e4d5-116">How to: Revalue Inventory</span></span>](inventory-how-revalue-inventory.md)|
|<span data-ttu-id="1e4d5-117">Juster varekost, enten automatisk eller manuelt, for å til videreføre kostnadsendringer fra inngående poster til relaterte utgående poster.</span><span class="sxs-lookup"><span data-stu-id="1e4d5-117">Adjust item costs, either automatically or manually, to forward cost changes from inbound entries to their related outbound entries.</span></span>|[<span data-ttu-id="1e4d5-118">Justere varekost</span><span class="sxs-lookup"><span data-stu-id="1e4d5-118">How to: Adjust Item Costs</span></span>](inventory-how-adjust-item-costs.md)|
|<span data-ttu-id="1e4d5-119">Bruk spesielle kostberegningsfunksjoner for daglige varetransaksjoner i vareoperasjonene.</span><span class="sxs-lookup"><span data-stu-id="1e4d5-119">Use special costing functions for every-day item transactions in the item operations.</span></span>|[<span data-ttu-id="1e4d5-120">Håndtere lager- og produksjonskost</span><span class="sxs-lookup"><span data-stu-id="1e4d5-120">Handling Inventory and Manufacturing Costs</span></span>](finance-handle-inventory-and-manufacturing-costs.md)|  
|<span data-ttu-id="1e4d5-121">Oppdater regelmessig standardkostnadene for komponenter, i monterings- eller produksjonsstykklister, og oppruller de nye kostnadene til den overordnede varen.</span><span class="sxs-lookup"><span data-stu-id="1e4d5-121">Periodically update the standard costs of components, in assembly or production BOMs, and roll the new costs up to the parent item.</span></span>|[<span data-ttu-id="1e4d5-122">Oppdatere standardkost</span><span class="sxs-lookup"><span data-stu-id="1e4d5-122">How to: Update Standard Costs</span></span>](finance-how-to-update-standard-costs.md)|
|<span data-ttu-id="1e4d5-123">Utføre kontroll- og rapporteringsoppgaver ved periodeslutt, for eksempel beregne lagerverdien og bokføre kost til Finans.</span><span class="sxs-lookup"><span data-stu-id="1e4d5-123">Perform period-end control and reporting tasks, such calculate the value of inventory and post costs to the general ledger.</span></span>|[<span data-ttu-id="1e4d5-124">Rapportere kostnader og avstemme med Finans</span><span class="sxs-lookup"><span data-stu-id="1e4d5-124">Reporting Costs and Reconciling with the General Ledger</span></span>](finance-report-costs-and-reconcile-with-the-general-ledger.md)|  
|<span data-ttu-id="1e4d5-125">Lær om alle mekanismene i kostsystemet.</span><span class="sxs-lookup"><span data-stu-id="1e4d5-125">Learn about all mechanisms in the costing system.</span></span>|[<span data-ttu-id="1e4d5-126">Designdetaljer: Kostberegning for beholdning</span><span class="sxs-lookup"><span data-stu-id="1e4d5-126">Design Details: Inventory Costing</span></span>](design-details-inventory-costing.md)|  

## <a name="see-also"></a><span data-ttu-id="1e4d5-127">Se også</span><span class="sxs-lookup"><span data-stu-id="1e4d5-127">See Also</span></span>  
 [<span data-ttu-id="1e4d5-128">Finans</span><span class="sxs-lookup"><span data-stu-id="1e4d5-128">Finance</span></span>](finance.md)  
 <span data-ttu-id="1e4d5-129">[Lager](inventory-manage-inventory.md) </span><span class="sxs-lookup"><span data-stu-id="1e4d5-129">[Inventory](inventory-manage-inventory.md) </span></span>  
 <span data-ttu-id="1e4d5-130">[Salg](sales-manage-sales.md) </span><span class="sxs-lookup"><span data-stu-id="1e4d5-130">[Sales](sales-manage-sales.md) </span></span>  
 [<span data-ttu-id="1e4d5-131">Innkjøp</span><span class="sxs-lookup"><span data-stu-id="1e4d5-131">Purchasing</span></span>](purchasing-manage-purchasing.md)  
 <span data-ttu-id="1e4d5-132">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1e4d5-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

