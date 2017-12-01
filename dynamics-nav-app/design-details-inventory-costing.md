---
title: Designdetaljer - Kostberegning for beholdning
description: Denne dokumentasjonen gir et detaljert teknisk innblikk i begrepene og prinsippene som brukes i funksjonene for kostberegning for beholdning i [!INCLUDE[d365fin](includes/d365fin_md.md)].
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, inventory, costing
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 8403486a897a3031ad0f488b4eb7e415daa1b8a0
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="design-details-inventory-costing"></a><span data-ttu-id="97ab5-103">Designdetaljer: Kostberegning for beholdning</span><span class="sxs-lookup"><span data-stu-id="97ab5-103">Design Details: Inventory Costing</span></span>
<span data-ttu-id="97ab5-104">Denne dokumentasjonen gir et detaljert teknisk innblikk i begrepene og prinsippene som brukes i funksjonene for kostberegning for beholdning i [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="97ab5-104">This documentation provides detailed technical insight to the concepts and principles that are used within the Inventory Costing features in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="97ab5-105">Kostberegning for beholdning, også kalt kostnadsstyring, handler om å registrere og rapportere forretningsdriftskost.</span><span class="sxs-lookup"><span data-stu-id="97ab5-105">Inventory costing, also referred to as cost management, is concerned with recording and reporting business operating costs.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="97ab5-106">I denne delen</span><span class="sxs-lookup"><span data-stu-id="97ab5-106">In This Section</span></span>  
[<span data-ttu-id="97ab5-107">Designdetaljer: Kostmetoder</span><span class="sxs-lookup"><span data-stu-id="97ab5-107">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)  
[<span data-ttu-id="97ab5-108">Designdetaljer: Vareutligning</span><span class="sxs-lookup"><span data-stu-id="97ab5-108">Design Details: Item Application</span></span>](design-details-item-application.md)  
[<span data-ttu-id="97ab5-109">Designdetaljer: Kostjustering</span><span class="sxs-lookup"><span data-stu-id="97ab5-109">Design Details: Cost Adjustment</span></span>](design-details-cost-adjustment.md)  
[<span data-ttu-id="97ab5-110">Designdetaljer: Bokføre forventet kost</span><span class="sxs-lookup"><span data-stu-id="97ab5-110">Design Details: Expected Cost Posting</span></span>](design-details-expected-cost-posting.md)  
[<span data-ttu-id="97ab5-111">Designdetaljer: Gjennomsnittskost</span><span class="sxs-lookup"><span data-stu-id="97ab5-111">Design Details: Average Cost</span></span>](design-details-average-cost.md)  
[<span data-ttu-id="97ab5-112">Designdetaljer: Avvik</span><span class="sxs-lookup"><span data-stu-id="97ab5-112">Design Details: Variance</span></span>](design-details-variance.md)  
[<span data-ttu-id="97ab5-113">Designdetaljer: Avrunding</span><span class="sxs-lookup"><span data-stu-id="97ab5-113">Design Details: Rounding</span></span>](design-details-rounding.md)  
[<span data-ttu-id="97ab5-114">Designdetaljer: Kostkomponenter</span><span class="sxs-lookup"><span data-stu-id="97ab5-114">Design Details: Cost Components</span></span>](design-details-cost-components.md)  
[<span data-ttu-id="97ab5-115">Designdetaljer: Beholdningsperioder</span><span class="sxs-lookup"><span data-stu-id="97ab5-115">Design Details: Inventory Periods</span></span>](design-details-inventory-periods.md)  
[<span data-ttu-id="97ab5-116">Designdetaljer: Lagerbokføring</span><span class="sxs-lookup"><span data-stu-id="97ab5-116">Design Details: Inventory Posting</span></span>](design-details-inventory-posting.md)  
[<span data-ttu-id="97ab5-117">Designdetaljer: Bokføre produksjonsordre</span><span class="sxs-lookup"><span data-stu-id="97ab5-117">Design Details: Production Order Posting</span></span>](design-details-production-order-posting.md)  
[<span data-ttu-id="97ab5-118">Designdetaljer: Bokføre monteringsordre</span><span class="sxs-lookup"><span data-stu-id="97ab5-118">Design Details: Assembly Order Posting</span></span>](design-details-assembly-order-posting.md)  
[<span data-ttu-id="97ab5-119">Designdetaljer: Avstemming med konti i Finans</span><span class="sxs-lookup"><span data-stu-id="97ab5-119">Design Details: Reconciliation with the General Ledger</span></span>](design-details-reconciliation-with-the-general-ledger.md)  
[<span data-ttu-id="97ab5-120">Designdetaljer: Konti i Finans</span><span class="sxs-lookup"><span data-stu-id="97ab5-120">Design Details: Accounts in the General Ledger</span></span>](design-details-accounts-in-the-general-ledger.md)  
[<span data-ttu-id="97ab5-121">Designdetaljer: Revaluering</span><span class="sxs-lookup"><span data-stu-id="97ab5-121">Design Details: Revaluation</span></span>](design-details-revaluation.md)

