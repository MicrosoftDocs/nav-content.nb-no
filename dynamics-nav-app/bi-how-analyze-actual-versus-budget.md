---
title: "Analysere faktiske i forhold til budsjetterte beløp"
description: "Beskriver hvordan du analyserer faktiske beløp i forhold til budsjetterte beløp."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 06/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: da2cdce3ada29fff98ceb875414f750a8af51855
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-analyze-actual-amounts-versus-budgeted-amounts"></a><span data-ttu-id="950d2-103">Analysere faktiske beløp i forhold til budsjetterte beløp</span><span class="sxs-lookup"><span data-stu-id="950d2-103">How to: Analyze Actual Amounts Versus Budgeted Amounts</span></span>
<span data-ttu-id="950d2-104">Som en del av innsamling, analyse og deling av selskapsdataene viser du faktiske beløp sammenlignet med budsjetterte beløp for alle konti og for flere perioder.</span><span class="sxs-lookup"><span data-stu-id="950d2-104">As a part of gathering, analyzing, and sharing your company data, you view actual amounts compared to budgeted amounts for all accounts and for several periods.</span></span>

<span data-ttu-id="950d2-105">Hvis du vil analysere budsjetterte beløp, må du først opprette budsjetter.</span><span class="sxs-lookup"><span data-stu-id="950d2-105">To analyze budgeted amounts, you must first create budgets.</span></span> <span data-ttu-id="950d2-106">Hvis du vil ha mer informasjon, kan du se [Opprette budsjetter](finance-how-create-budgets.md).</span><span class="sxs-lookup"><span data-stu-id="950d2-106">For more information, see [How to: Create Budgets](finance-how-create-budgets.md).</span></span>

## <a name="to-view-a-budget"></a><span data-ttu-id="950d2-107">Slik viser du et budsjett</span><span class="sxs-lookup"><span data-stu-id="950d2-107">To view a budget</span></span>
<span data-ttu-id="950d2-108">I et budsjett med dimensjoner kan du filtrere postene og se de bestemte budsjettene.</span><span class="sxs-lookup"><span data-stu-id="950d2-108">In a budget with dimensions, you can filter the entries and see specific budgets.</span></span>

1. <span data-ttu-id="950d2-109">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Finansbudsjetter**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="950d2-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Budgets**, and then choose the related link.</span></span>
2. <span data-ttu-id="950d2-110">Åpne budsjettet du vil vise, i vinduet **Finansbudsjetter**.</span><span class="sxs-lookup"><span data-stu-id="950d2-110">In the **G/L Budgets** window, open the budget that you want to view.</span></span>  
3. <span data-ttu-id="950d2-111">Øverst i vinduet fyller du ut feltene etter behov for å definere det som skal vises.</span><span class="sxs-lookup"><span data-stu-id="950d2-111">At the top of the window, fill in the fields as necessary to define what is shown.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   <span data-ttu-id="950d2-112">Hvis du har valgt **Periode** i feltet **Vis som linjer** eller feltet **Vis som kolonner**, må du fylle ut **Vis etter**-feltet.</span><span class="sxs-lookup"><span data-stu-id="950d2-112">If you have selected **Period** in either the **Show as Lines** or the **Show as Columns** field, then you must fill in the **View by** field.</span></span> <span data-ttu-id="950d2-113">Hvis du ikke har valgt **Periode** i feltet **Vis som linjer** eller feltet **Vis som kolonner**, angir du riktig periode i **Datofilter**-feltet.</span><span class="sxs-lookup"><span data-stu-id="950d2-113">If you have not selected **Period** in either the **Show as Lines** or **Show as Columns** field, then enter the appropriate period in **Date Filter** field.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="950d2-114">Beregningen tar bare med poster fra finansbudsjettet som har filterkodene du angir på hurtigfanen **Filtre**.</span><span class="sxs-lookup"><span data-stu-id="950d2-114">Only entries from the general ledger budget with the filter codes that you enter on the **Filters** FastTab are included in the calculation.</span></span> <span data-ttu-id="950d2-115">Budsjettposter med andre filterkoder, eller uten filterkoder, tas ikke med.</span><span class="sxs-lookup"><span data-stu-id="950d2-115">Budget entries with other filter codes or without any filter codes are not included.</span></span> <span data-ttu-id="950d2-116">Så lenge filteret beholdes i vinduet, viser budsjettet bare budsjettpostene med disse filterkodene.</span><span class="sxs-lookup"><span data-stu-id="950d2-116">As long as the filter remains on the window, the budget only displays the budget entries with these filter codes.</span></span>  

> [!TIP]  
>   <span data-ttu-id="950d2-117">Hvis du vil endre budsjettet, kan du endre budsjettpostene.</span><span class="sxs-lookup"><span data-stu-id="950d2-117">If you want to modify the budget, you can modify the budget entries.</span></span> <span data-ttu-id="950d2-118">Velg et beløp for å vise de underliggende finansbudsjettpostene.</span><span class="sxs-lookup"><span data-stu-id="950d2-118">Choose an amount to view the underlying general ledger budget entries.</span></span>

## <a name="to-view-actual-and-budgeted-amounts-for-all-accounts"></a><span data-ttu-id="950d2-119">Slik viser du faktiske og budsjetterte beløp for alle konti</span><span class="sxs-lookup"><span data-stu-id="950d2-119">To view actual and budgeted amounts for all accounts</span></span>  
<span data-ttu-id="950d2-120">Du kan vise finansbudsjetter og sammenligne dem med reelle tall, i flere moduler i [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="950d2-120">You can view general ledger budgets and compare them with actual figures in several areas of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

1. <span data-ttu-id="950d2-121">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Kontoplan**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="950d2-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="950d2-122">I vinduet **Kontoplan** velger du handlingen **Finanssaldo/Budsjett**.</span><span class="sxs-lookup"><span data-stu-id="950d2-122">In the **Chart of Accounts** window, choose the **G/L Balance/Budget** action.</span></span>
3. <span data-ttu-id="950d2-123">Øverst i vinduet fyller du ut feltene etter behov for å definere det som skal vises.</span><span class="sxs-lookup"><span data-stu-id="950d2-123">At the top of the window, fill in the fields as necessary to define what is shown.</span></span>  
4. <span data-ttu-id="950d2-124">Hvis du vil vise en spesifisering som utgjør beløpet som vises, velger du feltet.</span><span class="sxs-lookup"><span data-stu-id="950d2-124">To see a specification that makes up the amount shown, choose the field.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="950d2-125">Filtrene du angir i hodet, brukes på finansposter og også på budsjettposter.</span><span class="sxs-lookup"><span data-stu-id="950d2-125">The filters you set in the window header will be applied to general ledger entries and also budget entries.</span></span>

<span data-ttu-id="950d2-126">Kolonnene ytterst til venstre inneholder kontoplanen.</span><span class="sxs-lookup"><span data-stu-id="950d2-126">The leftmost columns contain the chart of accounts.</span></span> <span data-ttu-id="950d2-127">Av de fem kolonnene lengst til høyr, viser de fire første de faktiske og budsjetterte debet- og kreditbeløpene for hver konto.</span><span class="sxs-lookup"><span data-stu-id="950d2-127">Of the five columns on the rightmost side, the first four columns show actual and budgeted debit and credit amounts for each account.</span></span> <span data-ttu-id="950d2-128">Den femte kolonnen viser det proporsjonale forholdet mellom de faktiske og de budsjetterte beløpene på finanskontoen.</span><span class="sxs-lookup"><span data-stu-id="950d2-128">The fifth column shows the proportional relationship between the actual and the budgeted amounts on the general ledger account.</span></span>  

> [!TIP]  
>   <span data-ttu-id="950d2-129">Bruk **Vis etter**-feltet i vinduet **Finanssaldo/budsjett** til å velge periodelengden.</span><span class="sxs-lookup"><span data-stu-id="950d2-129">Use the **View by** field in the **G/L Balance/Budget** window to select the period length.</span></span> <span data-ttu-id="950d2-130">Bruk **Vis som**-feltet til å velge hvordan beløpene skal beregnes, **Bevegelse** eller **Saldo per dato**.</span><span class="sxs-lookup"><span data-stu-id="950d2-130">Use the **View as** field to select the way the amounts will be calculated, **Net Change** or **Balance at Date**.</span></span> <span data-ttu-id="950d2-131">Velg handlingen **Forrige periode** eller **Neste periode** for å endre perioden.</span><span class="sxs-lookup"><span data-stu-id="950d2-131">Choose the **Previous Period** or **Next Period** action to change the period.</span></span>  

## <a name="to-view-actual-and-budgeted-amounts-for-several-periods"></a><span data-ttu-id="950d2-132">Slik viser du faktiske og budsjetterte beløp for flere perioder</span><span class="sxs-lookup"><span data-stu-id="950d2-132">To view actual and budgeted amounts for several periods</span></span>  
<span data-ttu-id="950d2-133">I stedet for å vise de faktiske og budsjetterte beløpene for alle konti i én enkelt periode, kan du vise et antall perioder for én enkelt konto.</span><span class="sxs-lookup"><span data-stu-id="950d2-133">Instead of viewing the actual and budgeted amounts for all accounts within a single period, you can view a number of periods for a single account.</span></span>  

1. <span data-ttu-id="950d2-134">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Kontoplan**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="950d2-134">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="950d2-135">I vinduet **Kontoplan** velger du den aktuelle finanskontoen, og deretter velger du handlingen **Finanskontosaldo/Budsjett**.</span><span class="sxs-lookup"><span data-stu-id="950d2-135">In the **Chart of Accounts** window, select the relevant general ledger account, and then choose the **G/L Account Balance/Budget** action.</span></span>  
3. <span data-ttu-id="950d2-136">Øverst i vinduet fyller du ut feltene etter behov for å definere det som skal vises.</span><span class="sxs-lookup"><span data-stu-id="950d2-136">At the top of the window, fill in the fields as necessary to define what is shown.</span></span>   
4. <span data-ttu-id="950d2-137">Hvis du vil vise en spesifisering av et beløp som vises, velger du feltet.</span><span class="sxs-lookup"><span data-stu-id="950d2-137">To see a specification of an amount shown, choose the field.</span></span>  

## <a name="see-also"></a><span data-ttu-id="950d2-138">Se også</span><span class="sxs-lookup"><span data-stu-id="950d2-138">See Also</span></span>
<span data-ttu-id="950d2-139">[Forretningsintelligens](bi.md)
[Arbeide med kontoskjemaer](bi-how-work-account-schedule.md)</span><span class="sxs-lookup"><span data-stu-id="950d2-139">[Business Intelligence](bi.md)
[How to: Work with Account Schedules](bi-how-work-account-schedule.md)</span></span>  
[<span data-ttu-id="950d2-140">Finans</span><span class="sxs-lookup"><span data-stu-id="950d2-140">Finance</span></span>](finance.md)  
[<span data-ttu-id="950d2-141">Konfigurere finans</span><span class="sxs-lookup"><span data-stu-id="950d2-141">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="950d2-142">Finans og kontoplanen</span><span class="sxs-lookup"><span data-stu-id="950d2-142">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="950d2-143">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="950d2-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

