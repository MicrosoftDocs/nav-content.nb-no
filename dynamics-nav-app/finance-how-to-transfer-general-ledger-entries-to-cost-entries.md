---
title: "Overføre finansposter til kostposter"
description: "Du kan overføre finansposter til kostposter."
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
ms.openlocfilehash: f03cd367d01e9978f3a42191dc2653742877d7f4
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-transfer-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="56183-103">Overføre finansposter til kostposter</span><span class="sxs-lookup"><span data-stu-id="56183-103">How to: Transfer General Ledger Entries to Cost Entries</span></span>
<span data-ttu-id="56183-104">Du kan overføre finansposter til kostposter.</span><span class="sxs-lookup"><span data-stu-id="56183-104">You can transfer general ledger entries to cost entries.</span></span>  

<span data-ttu-id="56183-105">Før du kjører prosessen for overføring av finansposter til kostposter, må du klargjøre overføringen for å unngå manuell korrigeringsbokføring.</span><span class="sxs-lookup"><span data-stu-id="56183-105">Before you run the process for transferring general ledger entries to cost entries, you must prepare the transfer to avoid manual correction posting.</span></span>  

## <a name="to-prepare-the-transfer"></a><span data-ttu-id="56183-106">Klargjøre overføringen</span><span class="sxs-lookup"><span data-stu-id="56183-106">To prepare the transfer</span></span>  

1.  <span data-ttu-id="56183-107">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Kostregnskapsoppsett**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="56183-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Cost Accounting Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="56183-108">I vinduet **Kostregnskapsoppsett** kontrollerer du at feltet **Startdato for finansoverføring** er satt til den riktige verdien.</span><span class="sxs-lookup"><span data-stu-id="56183-108">In the **Cost Accounting Setup** window, verify that the **Starting Date for G/L Transfer** field is set to the correct value.</span></span>  
3.  <span data-ttu-id="56183-109">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Diagram med kosttyper**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="56183-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Cost Types**, and then choose the related link.</span></span>  
4.  <span data-ttu-id="56183-110">Kontroller at feltet **Finanskto. fra/til** i vinduet **Kosttypekort** er riktig koblet for hver kosttype, slik at poster hentes fra finans.</span><span class="sxs-lookup"><span data-stu-id="56183-110">In the **Cost Type Card** window, verify that the **G/L Account Range** field is linked correctly for each cost type to take entries from the general ledger.</span></span>  
5.  <span data-ttu-id="56183-111">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Kontoplan**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="56183-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
6.  <span data-ttu-id="56183-112">For hver relevant finanskonto i **Finanskort-vinduet** kontrollerer du at **Kosttypenr.**</span><span class="sxs-lookup"><span data-stu-id="56183-112">For each relevant general ledger account, in the **G/L Account Card** window, verify that the **Cost Type No.**</span></span> <span data-ttu-id="56183-113">-feltet er riktig tilknyttet en kostnadstype.</span><span class="sxs-lookup"><span data-stu-id="56183-113">field is linked correctly to a cost type.</span></span> <span data-ttu-id="56183-114">Hvis du vil ha mer informasjon, kan du se [Definere forholdet mellom kostnadstyper og finanskontoer](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md)</span><span class="sxs-lookup"><span data-stu-id="56183-114">For more information, see [Defining the Relationship Between Cost Types and General Ledger Accounts](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md).</span></span>  
7.  <span data-ttu-id="56183-115">Kontroller at alle relevante finansposter har dimensjonsverdier som svarer til et kostsenter og et kostobjekt.</span><span class="sxs-lookup"><span data-stu-id="56183-115">Verify that all relevant general ledger entries have dimension values that correspond to a cost center and a cost object.</span></span>  

## <a name="to-transfer-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="56183-116">Slik overfører du finansposter til kostposter:</span><span class="sxs-lookup"><span data-stu-id="56183-116">To transfer general ledger entries to cost entries</span></span>  
1.  <span data-ttu-id="56183-117">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Overfør finansposter til KR**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="56183-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer GL Entries to CA**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="56183-118">Velg **Ja**-knappen for å starte overføringen.</span><span class="sxs-lookup"><span data-stu-id="56183-118">Choose the **Yes** button to start the transfer.</span></span> <span data-ttu-id="56183-119">Prosessen overfører alle finansposter som ikke allerede er overført.</span><span class="sxs-lookup"><span data-stu-id="56183-119">The process transfers all general ledger entries that have not already been transferred.</span></span>  

    <span data-ttu-id="56183-120">Under overføringen oppretter prosessen forbindelser i postene i tabellen **Kostpost** og i tabellen **Kostjournal**.</span><span class="sxs-lookup"><span data-stu-id="56183-120">During the transfer, the process creates connections in the entries in the **Cost Entry** table and the **Cost Register** table.</span></span> <span data-ttu-id="56183-121">Dette gjør det mulig å spore kilden til kostposter.</span><span class="sxs-lookup"><span data-stu-id="56183-121">This makes it possible to trace the source of cost entries.</span></span>  

## <a name="see-also"></a><span data-ttu-id="56183-122">Se også</span><span class="sxs-lookup"><span data-stu-id="56183-122">See Also</span></span>  
 <span data-ttu-id="56183-123">[Kriterier for overføring av finansposter til kostposter](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="56183-123">[Criteria for Transferring General Ledger Entries to Cost Entries](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="56183-124">[Automatisk overføring og sammensatte poster](finance-automatic-transfer-combined-entries.md) </span><span class="sxs-lookup"><span data-stu-id="56183-124">[Automatic Transfer and Combined Entries](finance-automatic-transfer-combined-entries.md) </span></span>  
 <span data-ttu-id="56183-125">[Resultater av overføringen](finance-results-of-the-transfer.md) </span><span class="sxs-lookup"><span data-stu-id="56183-125">[Results of the Transfer](finance-results-of-the-transfer.md) </span></span>  
 <span data-ttu-id="56183-126">[Overføre og bokføre kostposter](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="56183-126">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
 [<span data-ttu-id="56183-127">Definere forholdet mellom kostnadstyper og finanskontoer</span><span class="sxs-lookup"><span data-stu-id="56183-127">Defining the Relationship Between Cost Types and General Ledger Accounts</span></span>](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md)   

