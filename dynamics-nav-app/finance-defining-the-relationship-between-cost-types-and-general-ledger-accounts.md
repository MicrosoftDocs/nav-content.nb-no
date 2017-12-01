---
title: Definere forholdet mellom kostnadstyper og finanskontoer
description: Finn ut hvordan du definerer relasjonen mellom kosttypen og finanskontoen.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost types, general ledger
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: fcaeab6a164abf20011beec35ec004057098b360
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="defining-the-relationship-between-cost-types-and-general-ledger-accounts"></a><span data-ttu-id="02b94-103">Definere forholdet mellom kostnadstyper og finanskontoer</span><span class="sxs-lookup"><span data-stu-id="02b94-103">Defining the Relationship Between Cost Types and General Ledger Accounts</span></span>
<span data-ttu-id="02b94-104">Forholdet mellom kosttypen og finanskontoen opprettes i kosttypen og finanskontoen.</span><span class="sxs-lookup"><span data-stu-id="02b94-104">The relationship between the cost type and the general ledger account is created in the cost type and in the general ledger account.</span></span>  

* <span data-ttu-id="02b94-105">Feltet **Finanskto. fra/til** i **Kosttype**-tabellen angir hvilke finanskontoer som tilhører en kostnadstype.</span><span class="sxs-lookup"><span data-stu-id="02b94-105">The **G/L Account Range** field in the **Cost Type** table establishes which general ledger accounts belong to a cost type.</span></span>  
* <span data-ttu-id="02b94-106">Feltet **Kosttypenr.**</span><span class="sxs-lookup"><span data-stu-id="02b94-106">The **Cost Type No.**</span></span> <span data-ttu-id="02b94-107">i kontoplanen angir hvilken kostnadstype en finanskontoer tilhører.</span><span class="sxs-lookup"><span data-stu-id="02b94-107">field in the chart of accounts establishes which cost type a general ledger account belongs to.</span></span>  

<span data-ttu-id="02b94-108">Disse to feltene er automatisk utfylt når du bruker funksjonen **Hent kosttyper fra kontoplan**.</span><span class="sxs-lookup"><span data-stu-id="02b94-108">These two fields are filled automatically when you use the **Get Cost Types from Chart of Accounts** function.</span></span>  

## <a name="relationship-between-general-ledger-accounts-and-cost-types"></a><span data-ttu-id="02b94-109">Forhold mellom finanskontoer og kostnadstyper</span><span class="sxs-lookup"><span data-stu-id="02b94-109">Relationship Between General Ledger Accounts and Cost Types</span></span>  
<span data-ttu-id="02b94-110">Det er et n:1-forhold mellom finanskonti og kosttyper.</span><span class="sxs-lookup"><span data-stu-id="02b94-110">There is an n:1 relationship between general ledger accounts and cost types.</span></span> <span data-ttu-id="02b94-111">Flere finanskontoer kan tilhøre én kosttype, men hver finanskonto tilhører bare én kosttype.</span><span class="sxs-lookup"><span data-stu-id="02b94-111">Several general ledger accounts can belong to one cost type, but each general ledger account belongs to only one cost type.</span></span> <span data-ttu-id="02b94-112">Tabellen nedenfor beskriver detaljene om forholdet.</span><span class="sxs-lookup"><span data-stu-id="02b94-112">The following table describes the details in the relationship.</span></span>  

|<span data-ttu-id="02b94-113">Forbindelser</span><span class="sxs-lookup"><span data-stu-id="02b94-113">Relationship</span></span>|<span data-ttu-id="02b94-114">**Finanskto. fra/til**</span><span class="sxs-lookup"><span data-stu-id="02b94-114">**G/L Account Range**</span></span>|<span data-ttu-id="02b94-115">**Kosttypenr.**</span><span class="sxs-lookup"><span data-stu-id="02b94-115">**Cost Type No.**</span></span>|  
|------------------|------------------------------------------------|-------------------------------------------|  
|<span data-ttu-id="02b94-116">Én finanskonto for hver kosttype</span><span class="sxs-lookup"><span data-stu-id="02b94-116">One general ledger account for each cost type</span></span>|<span data-ttu-id="02b94-117">Én finanskonto</span><span class="sxs-lookup"><span data-stu-id="02b94-117">One general ledger account</span></span>|<span data-ttu-id="02b94-118">En kosttype</span><span class="sxs-lookup"><span data-stu-id="02b94-118">One cost type</span></span>|  
|<span data-ttu-id="02b94-119">Flere finanskontoer for én kosttype.</span><span class="sxs-lookup"><span data-stu-id="02b94-119">Several general ledger accounts for one cost type</span></span>|<span data-ttu-id="02b94-120">Finanskontoområdet, for eksempel 7110–7193 for hver finanskonto</span><span class="sxs-lookup"><span data-stu-id="02b94-120">General ledger account range, for example, 7110..7193 for each general ledger account</span></span>|<span data-ttu-id="02b94-121">For hver finanskonto i området er det bare én kosttype</span><span class="sxs-lookup"><span data-stu-id="02b94-121">For each general ledger account in the range, there is only one cost type</span></span>|  
|<span data-ttu-id="02b94-122">Kosttyper uten tilsvarende finanskontoer</span><span class="sxs-lookup"><span data-stu-id="02b94-122">Cost types without corresponding general ledger accounts</span></span>|<Empty>||  
|<span data-ttu-id="02b94-123">Finanskonti der poster ikke overføres</span><span class="sxs-lookup"><span data-stu-id="02b94-123">General ledger accounts whose entries will not be transferred</span></span>||<Empty>|  

## <a name="cost-types-without-a-relationship-to-the-general-ledger"></a><span data-ttu-id="02b94-124">Kosttyper uten en relasjon til finans</span><span class="sxs-lookup"><span data-stu-id="02b94-124">Cost Types Without a Relationship to the General Ledger</span></span>  
<span data-ttu-id="02b94-125">En kostnadstype kan ikke ha en relasjon til finanskontoer hvis én av følgende betingelser er oppfylt:</span><span class="sxs-lookup"><span data-stu-id="02b94-125">A cost type may not have a relationship to general ledger accounts if one of the following conditions is true:</span></span>  

* <span data-ttu-id="02b94-126">Kontoer for driftsregnskap, for eksempel beregnede renter og avskrivning, tar bare kostnader fra driftsregnskapet.</span><span class="sxs-lookup"><span data-stu-id="02b94-126">Accounts for operational accounting, such as Calc. Interest and Depreciation, only take costs from the operational accounting.</span></span>  
* <span data-ttu-id="02b94-127">Hjelpekosttyper, for eksempel kosttypene 9901, 9902 og 9903 i [!INCLUDE[d365fin](includes/d365fin_md.md)]-databasen, brukes som kredit- og debetkontoer for fordelinger.</span><span class="sxs-lookup"><span data-stu-id="02b94-127">Helping cost types, such as cost types 9901, 9902, and 9903 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, are used as credit and debit accounts for allocations.</span></span>  
* <span data-ttu-id="02b94-128">Hjelpekontoen, 9920 i [!INCLUDE[d365fin](includes/d365fin_md.md)]-databasen, inneholder faktiske avsetninger som viser differansen mellom kost og utgiftene fra Finans.</span><span class="sxs-lookup"><span data-stu-id="02b94-128">The helping account, 9920 in the [!INCLUDE[d365fin](includes/d365fin_md.md)] database, contains actual accruals that show the difference between costs and the expense from the general ledger.</span></span>  

## <a name="see-also"></a><span data-ttu-id="02b94-129">Se også</span><span class="sxs-lookup"><span data-stu-id="02b94-129">See Also</span></span>  
[<span data-ttu-id="02b94-130">Gjøre rede for kostnader</span><span class="sxs-lookup"><span data-stu-id="02b94-130">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="02b94-131">[Definere kost.regnskap](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="02b94-131">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
[<span data-ttu-id="02b94-132">Om kostregnskap</span><span class="sxs-lookup"><span data-stu-id="02b94-132">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
<span data-ttu-id="02b94-133">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="02b94-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

