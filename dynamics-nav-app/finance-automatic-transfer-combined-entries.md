---
title: "Automatisk overføring og sammensatte poster"
description: "I kostnadsregnskap kan du overføre finansposter til en kosttype ved å bruke en kombinert bokføring. Du kan angi om en kosttype mottar kombinerte poster i feltet **Kombiner poster** i kosttypedefinisjonen. Tabellen nedenfor beskriver de ulike alternativene."
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
ms.openlocfilehash: ad5b24acd2b73b716bc02435906d9a1f47242e6a
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="automatic-transfer-and-combined-entries"></a><span data-ttu-id="b45a0-105">Automatisk overføring og sammensatte poster</span><span class="sxs-lookup"><span data-stu-id="b45a0-105">Automatic Transfer and Combined Entries</span></span>
<span data-ttu-id="b45a0-106">I kostnadsregnskap kan du overføre finansposter til en kosttype ved å bruke en kombinert bokføring.</span><span class="sxs-lookup"><span data-stu-id="b45a0-106">In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting.</span></span> <span data-ttu-id="b45a0-107">Du kan angi om en kosttype mottar kombinerte poster i feltet **Kombiner poster** i kosttypedefinisjonen.</span><span class="sxs-lookup"><span data-stu-id="b45a0-107">You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition.</span></span> <span data-ttu-id="b45a0-108">Tabellen nedenfor beskriver de ulike alternativene.</span><span class="sxs-lookup"><span data-stu-id="b45a0-108">The following table describes the different options.</span></span>  

|<span data-ttu-id="b45a0-109">Kombiner poster</span><span class="sxs-lookup"><span data-stu-id="b45a0-109">Combine entries</span></span>|<span data-ttu-id="b45a0-110">Beskrivelse</span><span class="sxs-lookup"><span data-stu-id="b45a0-110">Description</span></span>|  
|---------------------|-----------------|  
|<span data-ttu-id="b45a0-111">Ingen</span><span class="sxs-lookup"><span data-stu-id="b45a0-111">None</span></span>|<span data-ttu-id="b45a0-112">Hver finanspost overføres individuelt til tilsvarende kosttype.</span><span class="sxs-lookup"><span data-stu-id="b45a0-112">Each general ledger entry is transferred individually to the corresponding cost type.</span></span>|  
|<span data-ttu-id="b45a0-113">Dag</span><span class="sxs-lookup"><span data-stu-id="b45a0-113">Day</span></span>|<span data-ttu-id="b45a0-114">Finansposter med samme bokføringsdato overføres som én post til tilsvarende kosttype.</span><span class="sxs-lookup"><span data-stu-id="b45a0-114">General ledger entries with the same posting date are transferred as one entry to the corresponding cost type.</span></span>|  
|<span data-ttu-id="b45a0-115">Måned</span><span class="sxs-lookup"><span data-stu-id="b45a0-115">Month</span></span>|<span data-ttu-id="b45a0-116">Alle finansposter som har samme kalendermåned, overføres som én post til den tilsvarende kosttypen.</span><span class="sxs-lookup"><span data-stu-id="b45a0-116">All general ledger entries in the same calendar month are transferred as one entry to the corresponding cost type.</span></span>|  

> [!IMPORTANT]  
>  <span data-ttu-id="b45a0-117">Hvis du har merket av for **Overfør automatisk fra Finans** i vinduet **Kostregnskapsoppsett**, oppdaterer [!INCLUDE[d365fin](includes/d365fin_md.md)] kostregnskapet etter hver bokføring i finans.</span><span class="sxs-lookup"><span data-stu-id="b45a0-117">If you have selected the **Auto Transfer from G/L** check box in the **Cost Accounting Setup** window, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the cost accounting after every posting in the general ledger.</span></span> <span data-ttu-id="b45a0-118">Kombinerte poster er ikke mulig.</span><span class="sxs-lookup"><span data-stu-id="b45a0-118">Combined entries are not possible.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b45a0-119">Se også</span><span class="sxs-lookup"><span data-stu-id="b45a0-119">See Also</span></span>  
 <span data-ttu-id="b45a0-120">[Overføre finansposter til kostposter](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="b45a0-120">[How to: Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="b45a0-121">[Kriterier for overføring av finansposter til kostposter](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="b45a0-121">[Criteria for Transferring General Ledger Entries to Cost Entries](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="b45a0-122">[Resultater av overføringen](finance-results-of-the-transfer.md) </span><span class="sxs-lookup"><span data-stu-id="b45a0-122">[Results of the Transfer](finance-results-of-the-transfer.md) </span></span>  
 [<span data-ttu-id="b45a0-123">Overføre og bokføre kostposter</span><span class="sxs-lookup"><span data-stu-id="b45a0-123">Transferring and Posting Cost Entries</span></span>](finance-transfer-and-post-cost-entries.md)  
 <span data-ttu-id="b45a0-124">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b45a0-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

