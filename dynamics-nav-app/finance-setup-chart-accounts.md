---
title: Definere eller endre kontoplanen
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 2a2f1f2ec3ac5bdd935ec19c11d74e16bdee7686
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---

# <a name="set-up-or-change-the-chart-of-accounts"></a><span data-ttu-id="135ad-102">Definere eller endre kontoplanen</span><span class="sxs-lookup"><span data-stu-id="135ad-102">Set Up or Change the Chart of Accounts</span></span>
<span data-ttu-id="135ad-103">Kontoplanen viser finanskontoene som lagrer dine økonomiske data.</span><span class="sxs-lookup"><span data-stu-id="135ad-103">The chart of accounts shows the ledger accounts that store your financial data.</span></span> <span data-ttu-id="135ad-104">Dynamics NAV inneholder en standard kontoplan som er klar til å støtte forretningsvirksomheten din.</span><span class="sxs-lookup"><span data-stu-id="135ad-104">Dynamics NAV includes a standard chart of accounts that is ready to support your business.</span></span>
<span data-ttu-id="135ad-105">Du kan imidlertid endre standardkontoene, og du kan legge til nye kontoer.</span><span class="sxs-lookup"><span data-stu-id="135ad-105">However, you can change the default accounts, and you can add new accounts.</span></span>  

## <a name="adding-or-changing-accounts"></a><span data-ttu-id="135ad-106">Legge til eller endre kontoer</span><span class="sxs-lookup"><span data-stu-id="135ad-106">Adding or Changing Accounts</span></span>
<span data-ttu-id="135ad-107">For hver kontoplan kan du åpne finanskontoen og legge til eller endre innstillinger.</span><span class="sxs-lookup"><span data-stu-id="135ad-107">From the chart of accounts, you can open each G/L account and add or change settings.</span></span>

<span data-ttu-id="135ad-108">**Merk**: Du kan slette en finanskonto.</span><span class="sxs-lookup"><span data-stu-id="135ad-108">**Note**: You can delete a general ledger account.</span></span> <span data-ttu-id="135ad-109">Før du sletter den, må imidlertid følgende være oppfylt:</span><span class="sxs-lookup"><span data-stu-id="135ad-109">However, before you delete it, the following must be true:</span></span>  
- <span data-ttu-id="135ad-110">Saldo på kontoen må være null.</span><span class="sxs-lookup"><span data-stu-id="135ad-110">The balance on the account must be zero.</span></span>  
- <span data-ttu-id="135ad-111">Feltet **Tillat sletting av finanskto. før** må være satt i vinduet **Finansoppsett**, og kontoen kan ikke ha finansposter på eller etter denne datoen.</span><span class="sxs-lookup"><span data-stu-id="135ad-111">The **Allow G/L Acc. Deletion Before** field must be set in the **General Ledger Setup** window, and the account must not have ledger entries on or after that date.</span></span>  
- <span data-ttu-id="135ad-112">Hvis feltet **Kontroller finanskontobruk** er valgt i vinduet **Finansoppsett**, må ikke kontoen brukes i bokføringsgrupper eller bokføringsoppsett.</span><span class="sxs-lookup"><span data-stu-id="135ad-112">If the **Check G/L Account Usage** field in the **General Ledger Setup** window is selected, then the account must not be used in any posting groups or posting setup.</span></span>  

<span data-ttu-id="135ad-113">Dynamics NAV hindrer deg i å slette en finanskonto som lagrer data som er nødvendige i kontoplanen.</span><span class="sxs-lookup"><span data-stu-id="135ad-113">Dynamics NAV will prevent you from deleting a general ledger account that stores data that is needed in the chart of accounts.</span></span>  

##<a name="see-also"></a><span data-ttu-id="135ad-114">Se også</span><span class="sxs-lookup"><span data-stu-id="135ad-114">See Also</span></span>  
[<span data-ttu-id="135ad-115">Økonomimodulen og kontoplanen</span><span class="sxs-lookup"><span data-stu-id="135ad-115">The General Ledger and the Chart of Accounts</span></span>](finance-setup-general-ledger.md)  
[<span data-ttu-id="135ad-116">Håndtere bankkonti</span><span class="sxs-lookup"><span data-stu-id="135ad-116">Manage Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="135ad-117">Dimensjoner</span><span class="sxs-lookup"><span data-stu-id="135ad-117">Dimensions</span></span>](finance-setup-dimensions.md)  
[<span data-ttu-id="135ad-118">Arbeide med GIFI-koder i Canada</span><span class="sxs-lookup"><span data-stu-id="135ad-118">How to: Work With GIFI Codes in Canada</span></span>](ca-finance-setup-work-GiFI-codes.md)

