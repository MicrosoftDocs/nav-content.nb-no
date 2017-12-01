---
title: Bruke utvidelsen Quickbooks Payroll-filimport
description: "Beskriver hvordan du bruker utvidelsen til å importere lønn og lønnstransaksjoner fra Quickbooks Payroll-tjenesten."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, salary, wage
ms.date: 03/29/2017
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 6399a444e6459e31bb697890d72b74d0c44bf82e
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="the-quickbooks-payroll-file-import-extension-to-dynamics-nav"></a><span data-ttu-id="95325-103">Utvidelsen Quickbooks Payroll-filimport for Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="95325-103">The Quickbooks Payroll File Import Extension to Dynamics NAV</span></span>
<span data-ttu-id="95325-104">For å ta høyde for lønnsutbetalinger og relaterte transaksjoner, må du importere og bokføre finansielle transaksjoner som er utført av lønnssystemet til Finans.</span><span class="sxs-lookup"><span data-stu-id="95325-104">To account for salary payments and related transactions, you must import and post financial transactions made by your payroll provider to the general ledger.</span></span>

<span data-ttu-id="95325-105">Hvis du vil gjøre dette, importerer du først filen som du mottar fra lønnssystemet til vinduet **Finanskladd**.</span><span class="sxs-lookup"><span data-stu-id="95325-105">To do this, you first import a file that you receive from the payroll provider into the **General Journal** window.</span></span> <span data-ttu-id="95325-106">Deretter tilordner du eksterne kontoer i lønnsfilen til de relevante finanskontiene.</span><span class="sxs-lookup"><span data-stu-id="95325-106">Then you map the external accounts in the payroll file to the relevant G/L accounts.</span></span> <span data-ttu-id="95325-107">Til slutt kan du bokføre lønnstransaksjoner etter kontotilordningen.</span><span class="sxs-lookup"><span data-stu-id="95325-107">Lastly, you post the payroll transactions according to the account mapping.</span></span> <span data-ttu-id="95325-108">Hvis du vil ha mer informasjon, kan du se [Importere lønnstransaksjoner](finance-how-import-payroll-transactions.md).</span><span class="sxs-lookup"><span data-stu-id="95325-108">For more information, see [How to: Import Payroll Transactions](finance-how-import-payroll-transactions.md).</span></span>

<span data-ttu-id="95325-109">Utvidelsen for Quickbooks Payroll-filimport lar deg importere lønnstransaksjon fra Quickbooks Payroll-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="95325-109">The Quickbooks Payroll File Import extension allows you to import payroll transaction from the Quickbooks Payroll service.</span></span>

## <a name="see-also"></a><span data-ttu-id="95325-110">Se også</span><span class="sxs-lookup"><span data-stu-id="95325-110">See Also</span></span>
<span data-ttu-id="95325-111">[Tilpasse [!INCLUDE[d365fin](includes/d365fin_md.md)] ved hjelp av utvidelser](ui-extensions.md)  </span><span class="sxs-lookup"><span data-stu-id="95325-111">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)  </span></span>  
<span data-ttu-id="95325-112">[Finans](finance.md)  </span><span class="sxs-lookup"><span data-stu-id="95325-112">[Finance](finance.md)  </span></span>  
<span data-ttu-id="95325-113">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="95325-113">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

