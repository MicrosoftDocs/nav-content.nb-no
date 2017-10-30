---
title: "Designdetaljer - Strukturen til bokføringsgrensesnittet"
description: "Dette emnet gir en oversikt over de globale fremgangsmåtene i strukturen til bokføringsgrensesnittet."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: posting, interface, design
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: cc5efca8087bc24ab988ae592a9ba60e4caf46bb
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-posting-interface-structure"></a><span data-ttu-id="5aafa-103">Designdetaljer: Strukturen til bokføringsgrensesnittet</span><span class="sxs-lookup"><span data-stu-id="5aafa-103">Design Details: Posting Interface Structure</span></span>
<span data-ttu-id="5aafa-104">I strukturen til bokføringsgrensesnittet i [!INCLUDE[d365fin](includes/d365fin_md.md)] er det flere globale prosedyrer der samme struktur brukes:</span><span class="sxs-lookup"><span data-stu-id="5aafa-104">In the [!INCLUDE[d365fin](includes/d365fin_md.md)] posting interface structure, there are several global procedures that use the same structure:</span></span>  
  
* <span data-ttu-id="5aafa-105">RunWithCheck og RunWithoutCheck kaller prosedyrekode – generisk bokføringsgrensesnitt for finanskladdelinje.</span><span class="sxs-lookup"><span data-stu-id="5aafa-105">RunWithCheck and RunWithoutCheck call procedure Code – generic posting interface for Gen. Jnl Line.</span></span>  
* <span data-ttu-id="5aafa-106">CustPostApplyCustLedgEntry – bokfør kundeutligning, kalles fra kodeenhet 226 Kundepost – utlign bokførte poster.</span><span class="sxs-lookup"><span data-stu-id="5aafa-106">CustPostApplyCustLedgEntry – post customer application, called from codeunit 226 CustEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="5aafa-107">VendPostApplyVendLedgEntry – bokfør leverandørutligning, kalles fra kodeenhet 227 Leverandørpost – utlign bokførte poster.</span><span class="sxs-lookup"><span data-stu-id="5aafa-107">VendPostApplyVendLedgEntry – post vendor application, called from codeunit 227 VendEntry-Apply Posted Entries.</span></span>  
* <span data-ttu-id="5aafa-108">UnapplyCustLedgEntry – bokfør oppheving av kundeutligning, kalles fra kodeenhet 226 Kundepost – utlign bokførte poster</span><span class="sxs-lookup"><span data-stu-id="5aafa-108">UnapplyCustLedgEntry – post unapply of customer application, called from codeunit 226 CustEntry-Apply Posted Entries</span></span>  
* <span data-ttu-id="5aafa-109">UnapplyVendLedgEntry – bokfør oppheving av leverandørutligning, kalles fra kodeenhet 227 Leverandørpost – utlign bokførte poster</span><span class="sxs-lookup"><span data-stu-id="5aafa-109">UnapplyVendLedgEntry – post unapply of vendor application, called from codeunit 227 VendEntry-Apply Posted Entries</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="5aafa-110">Se også</span><span class="sxs-lookup"><span data-stu-id="5aafa-110">See Also</span></span>  
[<span data-ttu-id="5aafa-111">Designdetaljer: Strukturen til bokføringsmotoren</span><span class="sxs-lookup"><span data-stu-id="5aafa-111">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)
