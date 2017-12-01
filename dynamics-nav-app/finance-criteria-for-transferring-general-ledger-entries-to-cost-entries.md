---
title: "Kriterier for overføring av finansposter til kostposter"
description: "Det er viktig å forstå kriteriene for overføring av finansposter til kostposter. Under overføringen bruker kjørselen **Overfør finansposter til KR** følgende kriterier for å avgjøre om og hvordan finanspostene er overført."
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
ms.openlocfilehash: b4262f340801801f70bc890f529e329ce07dc830
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="criteria-for-transferring-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="aa8d5-104">Kriterier for overføring av finansposter til kostposter</span><span class="sxs-lookup"><span data-stu-id="aa8d5-104">Criteria for Transferring General Ledger Entries to Cost Entries</span></span>
<span data-ttu-id="aa8d5-105">Det er viktig å forstå kriteriene for overføring av finansposter til kostposter.</span><span class="sxs-lookup"><span data-stu-id="aa8d5-105">It is important to understand the criteria for transferring general ledger entries to cost entries.</span></span> <span data-ttu-id="aa8d5-106">Under overføringen bruker kjørselen **Overfør finansposter til KR** følgende kriterier for å avgjøre om og hvordan finanspostene er overført.</span><span class="sxs-lookup"><span data-stu-id="aa8d5-106">During the transfer, the **Transfer GL Entries to CA** batch job uses the following criteria to determine if and how the general ledger entries are transferred.</span></span>  

<span data-ttu-id="aa8d5-107">Finansposter overføres hvis følgende er tilfelle:</span><span class="sxs-lookup"><span data-stu-id="aa8d5-107">General ledger entries are transferred if:</span></span>  

-   <span data-ttu-id="aa8d5-108">Postene har dimensjonsverdier som tilsvarer enten et kostsenter eller et kostobjekt.</span><span class="sxs-lookup"><span data-stu-id="aa8d5-108">The entries have dimension values corresponding to either a cost center or a cost object.</span></span>  
-   <span data-ttu-id="aa8d5-109">Postene har dimensjonsverdier som tilsvarer et kostsenter og et kostobjekt.</span><span class="sxs-lookup"><span data-stu-id="aa8d5-109">The entries have dimension values that correspond to a cost center and a cost object.</span></span> <span data-ttu-id="aa8d5-110">For disse postene har kostsenteret forrang.</span><span class="sxs-lookup"><span data-stu-id="aa8d5-110">For these entries, the cost center takes precedence.</span></span> <span data-ttu-id="aa8d5-111">Dette bidrar til å unngå en situasjon der en kosttype vises i både et kostobjekt og et kostsenter og telles derfor to ganger i statistikken.</span><span class="sxs-lookup"><span data-stu-id="aa8d5-111">This helps avoid a situation where a cost type appears in both a cost object and a cost center and is therefore counted twice in the statistics.</span></span>  
-   <span data-ttu-id="aa8d5-112">Bilagsnummeret i postene er tomt, slik at det vises med bilagsnummeret 0000 i kostpostene.</span><span class="sxs-lookup"><span data-stu-id="aa8d5-112">The document number in the entries is empty, so it will appear with a document number of 0000 in the cost entries.</span></span>  
-   <span data-ttu-id="aa8d5-113">Postene overføres til en kosttype som tillater kombinerte poster, og disse postene overføres som en kombinert post enten månedlig eller daglig.</span><span class="sxs-lookup"><span data-stu-id="aa8d5-113">The entries are transferred to a cost type that allows for combined entries and these entries are transferred as a combined entry either monthly or daily.</span></span>  

<span data-ttu-id="aa8d5-114">Finansposter overføres ikke hvis følgende er tilfelle:</span><span class="sxs-lookup"><span data-stu-id="aa8d5-114">General ledger entries are not transferred if:</span></span>  

-   <span data-ttu-id="aa8d5-115">Postene har dimensjonsverdier som ikke tilsvarer et kostsenter eller et kostobjekt.</span><span class="sxs-lookup"><span data-stu-id="aa8d5-115">The entries have dimension values that do not correspond to a cost center or a cost object.</span></span>  
-   <span data-ttu-id="aa8d5-116">Postene har et beløp på null.</span><span class="sxs-lookup"><span data-stu-id="aa8d5-116">The entries have an amount of zero.</span></span>  
-   <span data-ttu-id="aa8d5-117">Postene har en finanskonto som er slettet.</span><span class="sxs-lookup"><span data-stu-id="aa8d5-117">The entries have a general ledger account that has been deleted.</span></span>  
-   <span data-ttu-id="aa8d5-118">Postene har en finanskonto som ikke er av typen **Resultatregnskap**.</span><span class="sxs-lookup"><span data-stu-id="aa8d5-118">The entries have a general ledger account that is not of the type **Income Statement**.</span></span>  
-   <span data-ttu-id="aa8d5-119">Postene har en finanskonto som det ikke er tilordnet en kosttype for.</span><span class="sxs-lookup"><span data-stu-id="aa8d5-119">The entries have a general ledger account that is not assigned a cost type.</span></span>  
-   <span data-ttu-id="aa8d5-120">Postene har en bokføringsdato som er tidligere enn **Startdato for finansoverføring**.</span><span class="sxs-lookup"><span data-stu-id="aa8d5-120">The entries have a posting date before the **Starting Date for G/L Transfer**.</span></span>  
-   <span data-ttu-id="aa8d5-121">Postene er bokført med en avslutningsdato.</span><span class="sxs-lookup"><span data-stu-id="aa8d5-121">The entries have been posted with a closing date.</span></span> <span data-ttu-id="aa8d5-122">Dette er vanligvis poster som tilbakestiller saldoen i resultatregnskapet på slutten av året.</span><span class="sxs-lookup"><span data-stu-id="aa8d5-122">These are typically entries that set back the balance of the income statement at the end of the year.</span></span>  

## <a name="see-also"></a><span data-ttu-id="aa8d5-123">Se også</span><span class="sxs-lookup"><span data-stu-id="aa8d5-123">See Also</span></span>  
[<span data-ttu-id="aa8d5-124">Gjøre rede for kostnader</span><span class="sxs-lookup"><span data-stu-id="aa8d5-124">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
 <span data-ttu-id="aa8d5-125">[Overføre finansposter til kostposter](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="aa8d5-125">[How to: Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="aa8d5-126">[Overføre og bokføre kostposter](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="aa8d5-126">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
 [<span data-ttu-id="aa8d5-127">Om kostregnskap</span><span class="sxs-lookup"><span data-stu-id="aa8d5-127">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
 <span data-ttu-id="aa8d5-128">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d5-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

