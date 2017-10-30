---
title: Definere ressurstildeling
description: "Finn ut hvordan systemet kan sørge for at du tilordner en person som ikke har de nødvendige kompetansen til å yte service."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: resource, skill, service, zones
ms.date: 08/22/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 9ca6bb733eb0f7cf090551da7a6d5c7b5cd3216b
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-set-up-resource-allocation"></a><span data-ttu-id="919bc-103">Definere ressurstildeling</span><span class="sxs-lookup"><span data-stu-id="919bc-103">How to: Set Up Resource Allocation</span></span>
<span data-ttu-id="919bc-104">For å sikre at en serviceoppgave utføres tilfredsstillende, er det viktig å finne en ressurs som er kvalifisert for å gjøre arbeidet.</span><span class="sxs-lookup"><span data-stu-id="919bc-104">To ensure that a service task is performed well, it's important to find a resource who is qualified to do the work.</span></span> <span data-ttu-id="919bc-105">Du kan definere [!INCLUDE[d365fin](includes/d365fin_md.md)], slik at det er enkelt å tildele en person som har riktig kompetansen for prosjektet.</span><span class="sxs-lookup"><span data-stu-id="919bc-105">You can set up [!INCLUDE[d365fin](includes/d365fin_md.md)] so that it's easy to allocate someone who has the right skills for the job.</span></span> <span data-ttu-id="919bc-106">I [!INCLUDE[d365fin](includes/d365fin_md.md)] kaller vi dette _ressurstildeling_.</span><span class="sxs-lookup"><span data-stu-id="919bc-106">In [!INCLUDE[d365fin](includes/d365fin_md.md)], we call this _resource allocation_.</span></span> <span data-ttu-id="919bc-107">Du kan tildele ressurser basert på kompetanse, tilgjengelighet eller om de er i samme servicesone som kunden.</span><span class="sxs-lookup"><span data-stu-id="919bc-107">You can allocate resources based on their skill, availability, or whether they are in the same service zone as the customer.</span></span> 

<span data-ttu-id="919bc-108">Hvis du vil bruke ressurstildeling, må du definere:</span><span class="sxs-lookup"><span data-stu-id="919bc-108">To use resource allocation, you must set up:</span></span>  
  
* <span data-ttu-id="919bc-109">Kompetansene som kreves for å reparere og vedlikeholde servicevarer.</span><span class="sxs-lookup"><span data-stu-id="919bc-109">The skills required to repair and maintain service items.</span></span> <span data-ttu-id="919bc-110">Du tilordner disse til servicevarer og ressurser.</span><span class="sxs-lookup"><span data-stu-id="919bc-110">You assign these to service items and resources.</span></span>  
* <span data-ttu-id="919bc-111">Geografiske områder, som kalles soner, som du definerer for markedet.</span><span class="sxs-lookup"><span data-stu-id="919bc-111">Geographic regions, called zones, that you define for your market.</span></span> <span data-ttu-id="919bc-112">Det kan for eksempel være øst, vest, midten og så videre.</span><span class="sxs-lookup"><span data-stu-id="919bc-112">For example, East, West, Central, and so on.</span></span> <span data-ttu-id="919bc-113">Du tilordner disse til kunder og ressurser.</span><span class="sxs-lookup"><span data-stu-id="919bc-113">You assign these to customers and resources.</span></span>  
* <span data-ttu-id="919bc-114">Om du vil vise ressurskompetanse og soner, og om det skal vises en advarsel hvis noen velger en ukvalifisert ressurs eller en ressurs som ikke er i kundesonen.</span><span class="sxs-lookup"><span data-stu-id="919bc-114">Whether to display resource skills and zones, and whether to display a warning if someone chooses unqualified resource, or a resource that is not in the customer zone.</span></span>  

## <a name="to-set-up-skills"></a><span data-ttu-id="919bc-115">Definere kompetanser</span><span class="sxs-lookup"><span data-stu-id="919bc-115">To set up skills</span></span>
1. <span data-ttu-id="919bc-116">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Kompetanse**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="919bc-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Skills**, and then choose the related link.</span></span>  
2. <span data-ttu-id="919bc-117">Fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="919bc-117">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-assign-skills-to-service-items-and-resources"></a><span data-ttu-id="919bc-118">Du tilordner disse til servicevarer og ressurser.</span><span class="sxs-lookup"><span data-stu-id="919bc-118">To assign skills to service items and resources</span></span>
1. <span data-ttu-id="919bc-119">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Servicevarer** eller **Ressurser**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="919bc-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Items** or **Resources**, and then choose the related link.</span></span>  
2. <span data-ttu-id="919bc-120">Åpne kortet for servicevaren eller ressursen, og velg deretter ett av følgende:</span><span class="sxs-lookup"><span data-stu-id="919bc-120">Open the card for the service item or resource, and then choose one of the following:</span></span>  
  
    * <span data-ttu-id="919bc-121">For servicevarer velger du **Ressurskompetanse**.</span><span class="sxs-lookup"><span data-stu-id="919bc-121">For service items, choose **Resource Skills**.</span></span>  
    * <span data-ttu-id="919bc-122">For ressurser velger du **Kompetanse**.</span><span class="sxs-lookup"><span data-stu-id="919bc-122">For resources, choose **Skills**.</span></span>  

## <a name="to-set-up-zones"></a><span data-ttu-id="919bc-123">Definere soner</span><span class="sxs-lookup"><span data-stu-id="919bc-123">To set up zones</span></span>
1. <span data-ttu-id="919bc-124">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Kompetanse**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="919bc-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Zones**, and then choose the related link.</span></span>  
2. <span data-ttu-id="919bc-125">Fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="919bc-125">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-assign-zones-to-customers-and-resources"></a><span data-ttu-id="919bc-126">Tilordne soner til kunder og ressurser</span><span class="sxs-lookup"><span data-stu-id="919bc-126">To assign zones to customers and resources</span></span> 
1. <span data-ttu-id="919bc-127">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Kunder** eller **Ressurser**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="919bc-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers** or **Resources**, and then choose the related link.</span></span>  
2. <span data-ttu-id="919bc-128">Åpne kortet for servicevaren eller ressursen, og velg deretter ett av følgende:</span><span class="sxs-lookup"><span data-stu-id="919bc-128">Open the card for the service item or resource, and then choose one of the following:</span></span>  
  
    * <span data-ttu-id="919bc-129">For kunder velger du en sone i feltet **Servicesonekode**.</span><span class="sxs-lookup"><span data-stu-id="919bc-129">For customers, choose a zone in the **Service Zone Code** field.</span></span>  
    * <span data-ttu-id="919bc-130">For ressurser velger du handlingen **Servicesoner**.</span><span class="sxs-lookup"><span data-stu-id="919bc-130">For resources, choose the **Service Zones** action.</span></span>  

## <a name="to-specify-what-to-show-when-a-resource-is-chosen"></a><span data-ttu-id="919bc-131">Angi hva som skal vises når en ressurs er valgt</span><span class="sxs-lookup"><span data-stu-id="919bc-131">To specify what to show when a resource is chosen</span></span>
1. <span data-ttu-id="919bc-132">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Serviceoppsett**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="919bc-132">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Setup**, and then choose the related link.</span></span> 
2. <span data-ttu-id="919bc-133">I feltet **Alt. for ressurskompetanse** velger du ett av alternativene som er beskrevet i tabellen nedenfor.</span><span class="sxs-lookup"><span data-stu-id="919bc-133">In the **Resource Skills Option** field, choose one of the options described in the following table.</span></span>  
  
    |<span data-ttu-id="919bc-134">**Alternativ**</span><span class="sxs-lookup"><span data-stu-id="919bc-134">**Option**</span></span>|<span data-ttu-id="919bc-135">**Beskrivelse**</span><span class="sxs-lookup"><span data-stu-id="919bc-135">**Description**</span></span>|  
    |------------|-------------|  
    |<span data-ttu-id="919bc-136">Vis kode</span><span class="sxs-lookup"><span data-stu-id="919bc-136">Code Shown</span></span> | <span data-ttu-id="919bc-137">Viser bare koden.</span><span class="sxs-lookup"><span data-stu-id="919bc-137">Displays the code only.</span></span>|  
    |<span data-ttu-id="919bc-138">Vis advarsel</span><span class="sxs-lookup"><span data-stu-id="919bc-138">Warning Displayed</span></span> | <span data-ttu-id="919bc-139">Viser informasjonen og en advarsel hvis du velger en ressurs som ikke er kvalifisert.</span><span class="sxs-lookup"><span data-stu-id="919bc-139">Shows the information and displays a warning if you choose a resource that is not qualified.</span></span>|  
    |<span data-ttu-id="919bc-140">Ikke i bruk</span><span class="sxs-lookup"><span data-stu-id="919bc-140">Not Used</span></span> | <span data-ttu-id="919bc-141">Viser ikke denne informasjonen.</span><span class="sxs-lookup"><span data-stu-id="919bc-141">Does not show this information.</span></span>|  

## <a name="to-update-resource-capacity"></a><span data-ttu-id="919bc-142">Oppdatere ressurskapasitet</span><span class="sxs-lookup"><span data-stu-id="919bc-142">To update resource capacity</span></span>  
<span data-ttu-id="919bc-143">Du må kanskje endre kapasiteten for ressurser.</span><span class="sxs-lookup"><span data-stu-id="919bc-143">You may need to change the capacity of resources.</span></span>  
  
1. <span data-ttu-id="919bc-144">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Ressurskapasitet**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="919bc-144">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resource Capacity**, and then choose the related link.</span></span>  
2. <span data-ttu-id="919bc-145">Velg ressursen, og velg deretter handlingen **Angi kapasitet**.</span><span class="sxs-lookup"><span data-stu-id="919bc-145">Choose the resource, and then choose the **Set Capacity** action.</span></span>  
3. <span data-ttu-id="919bc-146">Utfør endringen, og velge deretter **Oppdater kapasitet**.</span><span class="sxs-lookup"><span data-stu-id="919bc-146">Make the changes, and then choose **Update Capacity**.</span></span>  

## <a name="to-update-skills-for-items-service-items-or-service-item-groups"></a><span data-ttu-id="919bc-147">Oppdatere kompetanse for varer, servicevarer eller servicevaregrupper</span><span class="sxs-lookup"><span data-stu-id="919bc-147">To update skills for items, service items, or service item groups</span></span>
<span data-ttu-id="919bc-148">Hvis du vil endre kompetansekodene som er tilordnet til varer, for eksempel fra **PC** til **PCS**, kan du gjøre dette for en vare, servicevare eller for alle varer i en servicevaregruppe.</span><span class="sxs-lookup"><span data-stu-id="919bc-148">If you want to change the skill codes assigned to items, for example from **PC** to **PCS**, you can do so either for an item, service item, or for all items in a service item group.</span></span>  
  
1. <span data-ttu-id="919bc-149">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Varer**, **Servicevare** eller **Servicevaregruppe**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="919bc-149">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items** or **Service Item**, or **Service Item Group**, and then choose the related link.</span></span>  
2. <span data-ttu-id="919bc-150">Velg enheten som skal oppdateres, og velg deretter handlingen **Ressurskompetanse**.</span><span class="sxs-lookup"><span data-stu-id="919bc-150">Choose the entity to update, and then choose the **Resource Skills** action.</span></span>  
3. <span data-ttu-id="919bc-151">På linjen med koden som skal endres, velger du den relevante kompetansekoden i **Kompetansekode**-feltet.</span><span class="sxs-lookup"><span data-stu-id="919bc-151">On the line with the code to be changed, in the **Skill Code** field, choose the relevant skill code.</span></span>  
4.  <span data-ttu-id="919bc-152">Hvis varen har tilordnede servicevarer, åpnes det en dialogboks med følgende to alternativer:</span><span class="sxs-lookup"><span data-stu-id="919bc-152">If the item has associated service items, a dialog box opens with the following two options:</span></span>  
  
    * <span data-ttu-id="919bc-153">Endre kompetansekodene til den valgte verdien: Velg dette alternativet hvis du vil erstatte den gamle kompetansekoden med den nye for alle relaterte servicevarer.</span><span class="sxs-lookup"><span data-stu-id="919bc-153">Change the skill codes to the selected value: Select this option if you want to replace the old skill code with the new one on all the related service items.</span></span>  
    * <span data-ttu-id="919bc-154">Slett kompetansekodene eller oppdater relasjonen: Velg dette alternativet hvis du vil endre kompetansekoden bare for denne varen.</span><span class="sxs-lookup"><span data-stu-id="919bc-154">Delete the skill codes or update their relation: Select this option if you want to change the skill code on this item only.</span></span> <span data-ttu-id="919bc-155">Kompetansekoden for relaterte servicevarer tilordnes på nytt, dvs. at **Tilordnet fra**-feltet blir oppdatert.</span><span class="sxs-lookup"><span data-stu-id="919bc-155">The skill code on the related service items will be reassigned, that is, the **Assigned From** field will be updated.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="919bc-156">Se også</span><span class="sxs-lookup"><span data-stu-id="919bc-156">See Also</span></span>
[<span data-ttu-id="919bc-157">Tildele ressurser</span><span class="sxs-lookup"><span data-stu-id="919bc-157">How to: Allocate Resources</span></span>](service-how-to-allocate-resources.md)  
[<span data-ttu-id="919bc-158">Konfigurere arbeidstimer og servicetimer</span><span class="sxs-lookup"><span data-stu-id="919bc-158">How to: Set Up Work Hours and Service Hours</span></span>](service-how-setup-work-service-hours.md)  
[<span data-ttu-id="919bc-159">Definere feilrapportering</span><span class="sxs-lookup"><span data-stu-id="919bc-159">How to: Set Up Fault Reporting</span></span>](service-how-setup-fault-reporting.md)  
[<span data-ttu-id="919bc-160">Definere koder for standardservicer</span><span class="sxs-lookup"><span data-stu-id="919bc-160">How to: Set Up Codes for Standard Services</span></span>](service-how-setup-service-coding.md)  
 


