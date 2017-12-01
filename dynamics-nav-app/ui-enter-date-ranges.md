---
title: Angi datointervaller i Dynamics NAV
description: "Finn ut hvordan du får en rapport til å vise data fra bestemte tidsperioder ved å bruke datointervaller i Dynamics NAV."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: dates, reporting, filter
ms.date: 05/29/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 2773a1ce91ecd8e1216ffd9fdd5c3ceeb490e9e3
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="entering-date-ranges-in-dynamics-nav"></a><span data-ttu-id="64dc4-103">Sette inn datointervaller i Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="64dc4-103">Entering Date Ranges in Dynamics NAV</span></span>
<span data-ttu-id="64dc4-104">Du kan angi filtre som inneholder en startdato og en sluttdato, for å vise bare dataene innenfor dette datointervallet eller tidsintervallet.</span><span class="sxs-lookup"><span data-stu-id="64dc4-104">You can set filters containing a start date and an end date to display only the data contained in that date range or time interval.</span></span> <span data-ttu-id="64dc4-105">Særlige regler gjelder for angivelse av datointervaller.</span><span class="sxs-lookup"><span data-stu-id="64dc4-105">Special rules apply to the way you set date ranges.</span></span> <span data-ttu-id="64dc4-106">La oss ta **Kunde - ti på topp** som eksempel:</span><span class="sxs-lookup"><span data-stu-id="64dc4-106">Let's take the **Customer Top 10** as an example:</span></span>

![Angi et datointervall på forespørselssiden for Kunde - ti på topp-listen](./media/ui-enter-date-ranges/customer-top10-list.png)

<span data-ttu-id="64dc4-108">Her kan du begrense rapporten til et datointervall, for eksempel de to siste ukene eller totalt seks uker, eller et hvilket som helst intervall du vil bruke.</span><span class="sxs-lookup"><span data-stu-id="64dc4-108">Here you can limit the report to a date range such as the past 2 weeks, or a total of 6 weeks, or whatever range you want.</span></span> <span data-ttu-id="64dc4-109">Du angir datointervaller ved å angi datoene og deretter bruke **..**</span><span class="sxs-lookup"><span data-stu-id="64dc4-109">To set date ranges, you enter dates and then use either **..**</span></span> <span data-ttu-id="64dc4-110">eller **|** til å angi intervallet.</span><span class="sxs-lookup"><span data-stu-id="64dc4-110">or **|** to set the range.</span></span> <span data-ttu-id="64dc4-111">Hvis du vil vise de ti beste kundene for de to første ukene i mai i eksemplet vårt, setter du datofilteret til *05 01 17..05 14 17*.</span><span class="sxs-lookup"><span data-stu-id="64dc4-111">In our example, to show the top 10 customers for the first two weeks of May, you would set the date filter to *05 01 17..05 14 17*.</span></span>
<span data-ttu-id="64dc4-112">Her er noen andre eksempler:</span><span class="sxs-lookup"><span data-stu-id="64dc4-112">Here are a couple of other examples:</span></span>

| <span data-ttu-id="64dc4-113">Betyr</span><span class="sxs-lookup"><span data-stu-id="64dc4-113">Meaning</span></span> | <span data-ttu-id="64dc4-114">Eksempel</span><span class="sxs-lookup"><span data-stu-id="64dc4-114">Example</span></span> | <span data-ttu-id="64dc4-115">Tar med poster</span><span class="sxs-lookup"><span data-stu-id="64dc4-115">Entries included</span></span> |
|---|---|---|
|<span data-ttu-id="64dc4-116">Lik</span><span class="sxs-lookup"><span data-stu-id="64dc4-116">Equal to</span></span>| <span data-ttu-id="64dc4-117">12 15 16</span><span class="sxs-lookup"><span data-stu-id="64dc4-117">12 15 16</span></span> |<span data-ttu-id="64dc4-118">Bare de som er bokført 15. desember 2016.</span><span class="sxs-lookup"><span data-stu-id="64dc4-118">Only those posted on December 15 2016.</span></span>|
|<span data-ttu-id="64dc4-119">Intervall</span><span class="sxs-lookup"><span data-stu-id="64dc4-119">Interval</span></span>| <span data-ttu-id="64dc4-120">12 15 16..01 15 17</span><span class="sxs-lookup"><span data-stu-id="64dc4-120">12 15 16..01 15 17</span></span><br /><br /><span data-ttu-id="64dc4-121">..12 15 16</span><span class="sxs-lookup"><span data-stu-id="64dc4-121">..12 15 16</span></span>|<span data-ttu-id="64dc4-122">De som er bokført på datoer mellom og inkludert 15. desember 2016 og 15. januar 2017.</span><span class="sxs-lookup"><span data-stu-id="64dc4-122">Those posted on dates between and including December 15 2016 and January 15 2017.</span></span><br /><br /><span data-ttu-id="64dc4-123">De som er bokført 15. desember 2016 eller tidligere.</span><span class="sxs-lookup"><span data-stu-id="64dc4-123">Those posted on December 15 2016 or earlier.</span></span>|
|<span data-ttu-id="64dc4-124">Enten/eller</span><span class="sxs-lookup"><span data-stu-id="64dc4-124">Either/or</span></span>|<span data-ttu-id="64dc4-125">12 15 16&#124;12 16 16</span><span class="sxs-lookup"><span data-stu-id="64dc4-125">12 15 16&#124;12 16 16</span></span>|<span data-ttu-id="64dc4-126">De som er bokført 15. eller 16. desember 2016.</span><span class="sxs-lookup"><span data-stu-id="64dc4-126">Those posted on either December 15 or December 16 2016.</span></span> <span data-ttu-id="64dc4-127">Hvis det er bokført poster begge dagene, vises alle postene.</span><span class="sxs-lookup"><span data-stu-id="64dc4-127">If there are entries posted on both days, they will all be displayed.</span></span>|

<span data-ttu-id="64dc4-128">Grunnformene kan også kombineres innbyrdes.</span><span class="sxs-lookup"><span data-stu-id="64dc4-128">You can also combine the various format types.</span></span>

| <span data-ttu-id="64dc4-129">Eksempel</span><span class="sxs-lookup"><span data-stu-id="64dc4-129">Example</span></span> | <span data-ttu-id="64dc4-130">Tar med poster</span><span class="sxs-lookup"><span data-stu-id="64dc4-130">Entries included</span></span> |
|---|---|
|<span data-ttu-id="64dc4-131">12 15 16&#124;12 01 16..05 31 17</span><span class="sxs-lookup"><span data-stu-id="64dc4-131">12 15 16&#124;12 01 16..05 31 17</span></span> | <span data-ttu-id="64dc4-132">Poster som enten er bokført 15. desember 2016 eller på datoer mellom og inkludert 1. desember 2016 og 31. mai 2017.</span><span class="sxs-lookup"><span data-stu-id="64dc4-132">Entries posted either on December 15 2016 or on dates between and including December 01 2016 and May 31 2017.</span></span> |
|<span data-ttu-id="64dc4-133">..12 14 16&#124;12 30 16..</span><span class="sxs-lookup"><span data-stu-id="64dc4-133">..12 14 16&#124;12 30 16..</span></span> | <span data-ttu-id="64dc4-134">Poster som er bokført 14. desember eller tidligere, eller poster som er bokført 30. desember eller senere, det vil si alle poster unntatt de som er bokført på datoer mellom og inkludert 15. og 29. desember.</span><span class="sxs-lookup"><span data-stu-id="64dc4-134">Entries posted on December 14 or earlier, or entries posted on December 30 or later - that is, all entries except those posted on dates between and including December 15 and 29.</span></span> |

<span data-ttu-id="64dc4-135">Vær oppmerksom på at vi har brukt det amerikanske datoformatet MMDDÅÅ her.</span><span class="sxs-lookup"><span data-stu-id="64dc4-135">Note that we have used the US date format MMDDYY here.</span></span> <span data-ttu-id="64dc4-136">Etter hvert som [!INCLUDE[d365fin](includes/d365fin_md.md)] blir tilgjengelig på andre markeder, kan du bruke formatene du er vant med.</span><span class="sxs-lookup"><span data-stu-id="64dc4-136">As [!INCLUDE[d365fin](includes/d365fin_md.md)] becomes available in other markets, you'll be able to use the formats that you are used to.</span></span>

## <a name="see-also"></a><span data-ttu-id="64dc4-137">Se også</span><span class="sxs-lookup"><span data-stu-id="64dc4-137">See Also</span></span>
<span data-ttu-id="64dc4-138">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="64dc4-138">[Working with [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="64dc4-139">Angi vilkår i filtre</span><span class="sxs-lookup"><span data-stu-id="64dc4-139">Entering Criteria in Filters </span></span>](ui-enter-criteria-filters.md)  
[<span data-ttu-id="64dc4-140">Generelle forretningsfunksjoner</span><span class="sxs-lookup"><span data-stu-id="64dc4-140">General Business Functionality</span></span>](ui-across-business-areas.md)

