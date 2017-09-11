---
title: Bruke ressurser for prosjekter
author: SorenGP
ms.custom: na
ms.date: 12/14/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: cced4bca42b74c2664fd18770f1616c57286e1c3
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-use-resources-for-jobs"></a><span data-ttu-id="973be-102">Bruke ressurser for prosjekter</span><span class="sxs-lookup"><span data-stu-id="973be-102">How to: Use Resources for Jobs</span></span>
<span data-ttu-id="973be-103">Du registrerer ressursforbruket i prosjektkladden for å holde oversikt over kostnader, priser og arbeidstypene som er knyttet til prosjekter.</span><span class="sxs-lookup"><span data-stu-id="973be-103">You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs.</span></span> <span data-ttu-id="973be-104">Hvis du vil ha mer informasjon, kan du se [Registrere forbruk for prosjekter](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="973be-104">For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

<span data-ttu-id="973be-105">Du kan også bokføre ressursforbruket i en ressurskladd.</span><span class="sxs-lookup"><span data-stu-id="973be-105">You can also post the usage of a resource in a resource journal.</span></span> <span data-ttu-id="973be-106">Poster som er bokført i en ressurskladd, har ingen innvirkning på Finans.</span><span class="sxs-lookup"><span data-stu-id="973be-106">Entries posted in a resource journal have no effect on the general ledger.</span></span>

## <a name="to-assign-resources-to-jobs"></a><span data-ttu-id="973be-107">Slik tilordner du ressurser til prosjekter</span><span class="sxs-lookup"><span data-stu-id="973be-107">To assign resources to jobs</span></span>
<span data-ttu-id="973be-108">Du kan tilordne ressurser til prosjekter ved å opprette prosjektplanleggingslinjer for prosjektet.</span><span class="sxs-lookup"><span data-stu-id="973be-108">You assign resources to jobs by creating job planning lines for the job.</span></span> <span data-ttu-id="973be-109">Hvis du vil ha mer informasjon, kan du se [Opprette prosjekter](projects-how-create-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="973be-109">For more information, see [How to: Create Jobs](projects-how-create-jobs.md).</span></span>

## <a name="to-record-resource-usage-for-a-job"></a><span data-ttu-id="973be-110">Slik registrerer du ressursforbruk for et prosjekt</span><span class="sxs-lookup"><span data-stu-id="973be-110">To record resource usage for a job</span></span>

1. <span data-ttu-id="973be-111">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Prosjektkladder** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="973be-111">In the top right corner, choose the **Search for Page or Report** icon, enter **Job Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="973be-112">Åpne en relevant prosjektkladd, og fyll deretter ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="973be-112">Open a relevant job journal batch, and then fill in the fields as necessary.</span></span> <span data-ttu-id="973be-113">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="973be-113">Choose a field to read a short description of the field or link to more information.</span></span>
3. <span data-ttu-id="973be-114">Når kladden er fullført, kan du velge handlingen **Bokfør**.</span><span class="sxs-lookup"><span data-stu-id="973be-114">When the journal is complete, choose the **Post** action.</span></span>

## <a name="to-adjust-resource-prices"></a><span data-ttu-id="973be-115">Slik justerer du ressurspriser</span><span class="sxs-lookup"><span data-stu-id="973be-115">To adjust resource prices</span></span>  
<span data-ttu-id="973be-116">Hvis du vil endre kost- eller salgspriser for en rekke ressurser, kan du bruke en kjørsel.</span><span class="sxs-lookup"><span data-stu-id="973be-116">If you want to change costs or prices for a large number of resources, you can use a batch job.</span></span>  

1. <span data-ttu-id="973be-117">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Juster ressurskost/priser** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="973be-117">In the top right corner, choose the **Search for Page or Report** icon, enter **Adjust Resource Costs/Prices**, and then choose the related link.</span></span>
2. <span data-ttu-id="973be-118">Fyll ut feltene på en linje etter behov, og klikk deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="973be-118">Fill in the fields on a line as necessary, and then choose the **OK** button.</span></span>

<span data-ttu-id="973be-119">**Merk**: Denne kjørselen verken oppretter eller endrer alternative kostnader eller priser for ressurser.</span><span class="sxs-lookup"><span data-stu-id="973be-119">**Note**: This batch job does not create or adjust alternate costs or prices for resources.</span></span> <span data-ttu-id="973be-120">Den endrer bare innholdet i feltet på ressurskortet for **Juster felt**-feltet som du valgte i kjørselen.</span><span class="sxs-lookup"><span data-stu-id="973be-120">It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job.</span></span> <span data-ttu-id="973be-121">Justeringen vil tre i kraft umiddelbart for ressurser, så kontroller justeringsfaktorene før du kjører den satsvise jobben.</span><span class="sxs-lookup"><span data-stu-id="973be-121">The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-existing-alternate-prices"></a><span data-ttu-id="973be-122">Slik får du forslag til ressursprisendringer på bakgrunn av eksisterende alternative priser</span><span class="sxs-lookup"><span data-stu-id="973be-122">To get resource price change suggestions based on existing alternate prices</span></span>  
<span data-ttu-id="973be-123">Hvis du allerede har definert alternative ressurspriser for noen ressurser, kan du bruke en kjørsel til å definere flere alternative ressurspriser.</span><span class="sxs-lookup"><span data-stu-id="973be-123">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="973be-124">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Ressursprisendringer** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="973be-124">In the top right corner, choose the **Search for Page or Report** icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="973be-125">Velg handlingen **Foreslå ress.prisendr. (pris)** og fyll deretter ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="973be-125">Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.</span></span>
3. <span data-ttu-id="973be-126">Velg **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="973be-126">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="973be-127">Når kjørselen er ferdig, viser vinduet **Ressursprisendringer** resultatene av kjørselen.</span><span class="sxs-lookup"><span data-stu-id="973be-127">When the batch job is finished, the **Resource Price Changes** window shows the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-standard-prices"></a><span data-ttu-id="973be-128">Slik får du forslag til ressursprisendringer på bakgrunn av standardpriser</span><span class="sxs-lookup"><span data-stu-id="973be-128">To get resource price change suggestions based on standard prices</span></span>  
<span data-ttu-id="973be-129">Hvis du vil definere flere alternative ressurspriser på bakgrunn av standardprisene på ressurskortene, kan du bruke en kjørsel.</span><span class="sxs-lookup"><span data-stu-id="973be-129">If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.</span></span>  

1. <span data-ttu-id="973be-130">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Ressursprisendringer** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="973be-130">In the top right corner, choose the **Search for Page or Report** icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="973be-131">Velg handlingen **Foreslå ress.prisendr. (ress.)** og fyll deretter ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="973be-131">Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.</span></span>  
3. <span data-ttu-id="973be-132">Velg **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="973be-132">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="973be-133">Når kjørselen er ferdig, åpner du vinduet **Ressursprisendringer** for å se resultatene av kjørselen.</span><span class="sxs-lookup"><span data-stu-id="973be-133">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-alternate-prices"></a><span data-ttu-id="973be-134">Slik får du forslag til ressursprisendringer på bakgrunn av alternative priser</span><span class="sxs-lookup"><span data-stu-id="973be-134">To get resource price change suggestions based on alternate prices</span></span>  
<span data-ttu-id="973be-135">Hvis du allerede har definert alternative ressurspriser for noen ressurser, kan du bruke en kjørsel til å definere flere alternative ressurspriser.</span><span class="sxs-lookup"><span data-stu-id="973be-135">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="973be-136">Skriv inn **Foreslå ress.prisendr. (pris)** i **Søk**-boksen, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="973be-136">In the **Search** box, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.</span></span>  
2. <span data-ttu-id="973be-137">Fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="973be-137">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="973be-138">Velg **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="973be-138">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="973be-139">Når kjørselen er ferdig, åpner du vinduet **Ressursprisendringer** for å se resultatene av kjørselen.</span><span class="sxs-lookup"><span data-stu-id="973be-139">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="973be-140">Se også</span><span class="sxs-lookup"><span data-stu-id="973be-140">See Also</span></span>
[<span data-ttu-id="973be-141">Administrere prosjekter</span><span class="sxs-lookup"><span data-stu-id="973be-141">Manage Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="973be-142">Finans</span><span class="sxs-lookup"><span data-stu-id="973be-142">Finance</span></span>](finance-setup.md)  
<span data-ttu-id="973be-143">[Håndtere kjøp](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="973be-143">[Manage Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="973be-144">[Håndtere salg](sales-manage-sales.md)   </span><span class="sxs-lookup"><span data-stu-id="973be-144">[Manage Sales](sales-manage-sales.md)   </span></span>  
[<span data-ttu-id="973be-145">Arbeide med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="973be-145">Work With Dynamics NAV</span></span>](ui-work-product.md)  

