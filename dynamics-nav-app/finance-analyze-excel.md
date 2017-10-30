---
title: "Arbeide med økonomiske oversikter i Excel"
description: "Lær om hvordan du åpner regnskapene i Microsoft Excel fra Dynamics NAV for bedre analyser."
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, financial report
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 6d246ca7e02c8bd081636abc6aca871993b3fbbf
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="analyzing-financial-statements-in-microsoft-excel"></a><span data-ttu-id="31860-103">Analysere årsregnskap i Microsoft Excel</span><span class="sxs-lookup"><span data-stu-id="31860-103">Analyzing Financial Statements in Microsoft Excel</span></span>
<span data-ttu-id="31860-104">I [!INCLUDE[d365fin](includes/d365fin_md.md)] kan du se ytelsesindikatorer og få en oversikt over selskapets økonomiske tilstand.</span><span class="sxs-lookup"><span data-stu-id="31860-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], you can see KPIs and get overviews of the company's financial state.</span></span> <span data-ttu-id="31860-105">Du kan også åpne lister i Excel og analysere dataene der.</span><span class="sxs-lookup"><span data-stu-id="31860-105">You can also open lists in Excel and analyze the data there.</span></span> <span data-ttu-id="31860-106">Men du kan også eksportere tunge årsregnskap, for eksempel balansen eller resultatregnskapet til Excel, analysere data og skrive ut rapportene.</span><span class="sxs-lookup"><span data-stu-id="31860-106">But you can also export heavy financial statements such as the balance sheet or the income statement to Excel, analyze the data, and print the reports.</span></span>  

<span data-ttu-id="31860-107">I rollesentrene for forretningsleder og regnskapsfører kan du velge hvilke årsregnskap som skal vises i Excel, fra en rullegardinmeny i Rapporter-delen på båndet.</span><span class="sxs-lookup"><span data-stu-id="31860-107">In the Business Manager and Accountant Role Centers, you can choose which financial statements to view in Excel from a drop-down menu in the Reports section of the ribbon.</span></span> <span data-ttu-id="31860-108">Når du velger et regnskap, åpnes det i Excel eller Excel Online.</span><span class="sxs-lookup"><span data-stu-id="31860-108">When you choose a statement, it will be opened in Excel or Excel Online.</span></span> <span data-ttu-id="31860-109">Et tillegg kobler dataene til [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="31860-109">An add-in connects the data to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="31860-110">Du må imidlertid logge på med den samme kontoen som du bruker med [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="31860-110">However, you have to sign in with the same account that you use with [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="getting-the-overview-and-the-details-in-excel"></a><span data-ttu-id="31860-111">Få oversikten og detaljene i Excel</span><span class="sxs-lookup"><span data-stu-id="31860-111">Getting the Overview and the Details in Excel</span></span>
<span data-ttu-id="31860-112">Velg den aktuelle Excel-rapporten på båndet, og la den åpne slik at du får oversikten du søker etter.</span><span class="sxs-lookup"><span data-stu-id="31860-112">In the ribbon, choose the relevant Excel report, and let it open so you can get the overview that you were looking for.</span></span> <span data-ttu-id="31860-113">I denne versjonen av [!INCLUDE[d365fin](includes/d365fin_md.md)] tilbyr vi følgende Excel-rapporter:</span><span class="sxs-lookup"><span data-stu-id="31860-113">In this version of [!INCLUDE[d365fin](includes/d365fin_md.md)], we offer the following Excel reports:</span></span>

- <span data-ttu-id="31860-114">Balanse</span><span class="sxs-lookup"><span data-stu-id="31860-114">Balance Sheet</span></span>  
- <span data-ttu-id="31860-115">Resultatregnskap</span><span class="sxs-lookup"><span data-stu-id="31860-115">Income Statement</span></span>  
- <span data-ttu-id="31860-116">Kontantstrømutdrag</span><span class="sxs-lookup"><span data-stu-id="31860-116">Cash Flow Statement</span></span>  
- <span data-ttu-id="31860-117">Kontoutdrag for fri egenkapital</span><span class="sxs-lookup"><span data-stu-id="31860-117">Retained Earnings Statement</span></span>  
- <span data-ttu-id="31860-118">Aldersfordelt saldoliste - leverandør</span><span class="sxs-lookup"><span data-stu-id="31860-118">Aged Accounts Payable</span></span>  
- <span data-ttu-id="31860-119">Aldersford. saldoliste - kunde</span><span class="sxs-lookup"><span data-stu-id="31860-119">Aged Accounts Receivable</span></span>  

<span data-ttu-id="31860-120">La oss si at du vil se nærmere på kontantstrømmen din.</span><span class="sxs-lookup"><span data-stu-id="31860-120">Let's say you want to dig deeper into your cash flow.</span></span> <span data-ttu-id="31860-121">Du kan åpne ut kontoutdrag-rapporten i Excel fra firma lederen eller regnskapsføreren rollesenter, men hva som skjer faktisk er vi eksportere dataene relevante for deg, og oppretter en Excel-arbeidsbok basert på en forhåndsdefinert mal.</span><span class="sxs-lookup"><span data-stu-id="31860-121">From the Business Manager or Accountant Role Center, you can open the Cash Flow Statement report in Excel, but what actually happens is that we export the relevant data for you and create an Excel workbook based on a predefined template.</span></span> <span data-ttu-id="31860-122">Avhengig av webleseren må du kanskje skal åpnes eller lagres arbeidsboken.</span><span class="sxs-lookup"><span data-stu-id="31860-122">Depending on your browser, you might be prompted to open or save the workbook.</span></span>  

<span data-ttu-id="31860-123">I Excel ser du en fane der dataene er ordnet du første forslaget.</span><span class="sxs-lookup"><span data-stu-id="31860-123">In Excel, you see a tab where the data is laid out for you on the first worksheet.</span></span> <span data-ttu-id="31860-124">Data som ble eksportert finnes også i andre forslagene, i tilfelle du trenger den.</span><span class="sxs-lookup"><span data-stu-id="31860-124">All the data that was exported is also present in other worksheets in case you need it.</span></span> <span data-ttu-id="31860-125">Du kan skrive ut rapporten én gang, eller du kan endre den til du har oversikten, og du vil ha detaljer.</span><span class="sxs-lookup"><span data-stu-id="31860-125">You can print the report right away, or you can modify it until you have the overview and the details that you want.</span></span> <span data-ttu-id="31860-126">Bruk [!INCLUDE[d365fin](includes/d365fin_md.md)] Excel-tillegget til å filtrere og analysere dataene.</span><span class="sxs-lookup"><span data-stu-id="31860-126">Use the [!INCLUDE[d365fin](includes/d365fin_md.md)] Excel Add-in to further filter and analyze data.</span></span>  

## <a name="the-included365finincludesd365finmdmd-excel-add-in"></a><span data-ttu-id="31860-127">[!INCLUDE[d365fin](includes/d365fin_md.md)] Excel-tillegget</span><span class="sxs-lookup"><span data-stu-id="31860-127">The [!INCLUDE[d365fin](includes/d365fin_md.md)] Excel Add-in</span></span>
<span data-ttu-id="31860-128">Din [!INCLUDE[d365fin](includes/d365fin_md.md)]-opplevelse inneholder et tillegg til Excel.</span><span class="sxs-lookup"><span data-stu-id="31860-128">Your [!INCLUDE[d365fin](includes/d365fin_md.md)] experience includes an add-in for Excel.</span></span> <span data-ttu-id="31860-129">Avhengig av abonnementet er du logget på automatisk, eller du må angi samme pålogging som du bruker for [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="31860-129">Depending on your subscription, you are logged in automatically, or you must specify the same login details that you use for [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="31860-130">Med tillegget kan du få ferske data fra [!INCLUDE[d365fin](includes/d365fin_md.md)], og du kan overføre endringer i [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="31860-130">With the add-in, you can get fresh data from [!INCLUDE[d365fin](includes/d365fin_md.md)], and you can push changes back into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="31860-131">Muligheten til å legge inn data tilbake til databasen deaktiveres imidlertid for Excel-årsregnskap i listen ovenfor.</span><span class="sxs-lookup"><span data-stu-id="31860-131">However, the ability to push data back to the database is disabled for the financial Excel reports in the list above.</span></span>  

## <a name="see-also"></a><span data-ttu-id="31860-132">Se også</span><span class="sxs-lookup"><span data-stu-id="31860-132">See Also</span></span>
[<span data-ttu-id="31860-133">Finans</span><span class="sxs-lookup"><span data-stu-id="31860-133">Finance</span></span>](finance.md)  
[<span data-ttu-id="31860-134">Konfigurere finans</span><span class="sxs-lookup"><span data-stu-id="31860-134">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="31860-135">Finans og kontoplanen</span><span class="sxs-lookup"><span data-stu-id="31860-135">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
[<span data-ttu-id="31860-136">Arbeide med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="31860-136">Working with Dynamics NAV</span></span>](ui-work-product.md)  

