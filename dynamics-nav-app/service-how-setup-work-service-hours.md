---
title: Konfigurere arbeidstimer og servicetimer
description: "Du kan angi de vanlige servicearbeidstimene i selskapet. Disse servicetimene brukes til å beregne responsdatoen og -klokkeslettet for serviceordrer og -tilbud, og til å sende advarsler om responstid."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 9c325af29d5ffd0f0e52b65318d88c48cdba80d4
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-set-up-work-hours-and-service-hours"></a><span data-ttu-id="cb1ae-104">Konfigurere arbeidstimer og servicetimer</span><span class="sxs-lookup"><span data-stu-id="cb1ae-104">How to: Set Up Work Hours and Service Hours</span></span>
<span data-ttu-id="cb1ae-105">Med et servicesystem kan du vanligvis spore ressurstimer og serviceordrestatus for å prognostisere arbeidsmengder og servicebehov.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-105">Typically, a service management system tracks resource hours and service order status in order to forecast workloads and service needs.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="cb1ae-106"> har innebygde verktøy du kan tilpasse for å registrere denne typen informasjon.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-106"> has built-in tools that you can customize to record this kind of information.</span></span>  
  
<span data-ttu-id="cb1ae-107">Etter at du har angitt selskapets standard servicetimer, kan du beregne responstiden for serviceordrer eller sende advarsler eller varsler når det kommer serviceanrop.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-107">After you set the default service hours of your company, you can calculate response times for service orders or send warnings or alerts when service calls come in.</span></span> <span data-ttu-id="cb1ae-108">Varslingsfunksjonen implementeres sammen med jobbskjemaet.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-108">The alert feature is implemented together with the job scheduler.</span></span>   
  
<span data-ttu-id="cb1ae-109">Når du arbeider med en serviceordre, vil du oppdaterer statusen slik at du kan overvåke fremdriften.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-109">As you work on a service order, you will want to update it's status so that you can monitor progress.</span></span> <span data-ttu-id="cb1ae-110">Serviceordrestatusen gjenspeiler reparasjonsstatusen til alle servicevarene i serviceordren.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-110">The service order status reflects the repair status of all the service items in the service order.</span></span> <span data-ttu-id="cb1ae-111">Hvis du vil ha mer informasjon, kan du se [Forstå serviceordre- og reparasjonsstatus](service-order-repair-status.md).</span><span class="sxs-lookup"><span data-stu-id="cb1ae-111">For more information, see [Understanding Service Order and Repair Status](service-order-repair-status.md).</span></span> 

## <a name="to-set-up-default-service-hours"></a><span data-ttu-id="cb1ae-112">Slik definerer du Standard servicetimer</span><span class="sxs-lookup"><span data-stu-id="cb1ae-112">To set up default service hours</span></span>  
<span data-ttu-id="cb1ae-113">Du bruker vinduet **Standard servicetimer** til å definere selskapets normale antall servicearbeidstimer.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-113">You use the **Default Service Hours** window to set up the usual service working hours in your company.</span></span> <span data-ttu-id="cb1ae-114">Disse servicetimene brukes til å beregne responsdatoen og -klokkeslettet for serviceordrer og -tilbud, og til å sende advarsler om responstid.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-114">These service hours are used to calculate the response date and time for service orders and quotes and to send response time warnings.</span></span> <span data-ttu-id="cb1ae-115">Standard servicetimer brukes for servicekontrakter hvis du ikke angir spesifikke servicetimer for en kontrakt.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-115">The default service hours are used for service contracts unless you specify special service hours for a contract.</span></span>  
  
1. <span data-ttu-id="cb1ae-116">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Standard servicetimer**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Default Service Hours**, and then choose the related link.</span></span>  
2. <span data-ttu-id="cb1ae-117">Fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-117">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
  
> [!IMPORTANT]  
>  <span data-ttu-id="cb1ae-118">Hvis du lar linjene i vinduet **Standard servicetimer** stå tomme, bruker programmet 24 timer som standardverdi, som bare er gjelder for arbeidsdager fra kalenderen.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-118">If you leave the lines in the **Default Service Hours** window empty, the default value is 24 hours, valid only for calendar working days.</span></span>  
  
## <a name="to-set-up-work-hour-templates"></a><span data-ttu-id="cb1ae-119">Definere arbeidstidsmaler</span><span class="sxs-lookup"><span data-stu-id="cb1ae-119">To set up work-hour templates</span></span>
<span data-ttu-id="cb1ae-120">Du kan bruke vinduet **Arbeidstidsmal** til å definere maler som inneholder vanlige arbeidstider i selskapet.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-120">You can use the **Work-Hour Template** window to set up templates that contain the typical working hours in your company.</span></span> <span data-ttu-id="cb1ae-121">Du kan for eksempel opprette maler for heltidsteknikere og deltidsteknikere.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-121">For example, you can create templates for full time technicians and part time technicians.</span></span> <span data-ttu-id="cb1ae-122">Du kan bruke arbeidstidsmaler når du legger til kapasitet i ressurser.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-122">You can use work-hour templates when you add capacity to resources.</span></span>  
  
1. <span data-ttu-id="cb1ae-123">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Arbeidstidsmaler**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Work Hour Templates**, and then choose the related link.</span></span>  
2. <span data-ttu-id="cb1ae-124">Fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-124">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
  
> [!Note]
> <span data-ttu-id="cb1ae-125">Når du har angitt arbeidstimer for hver dag, beregnes verdien i feltet **Sum per uke** automatisk.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-125">After you enter work hours for each day, the value in the **Total per Week** field is calculated automatically.</span></span>  

## <a name="to-set-up-contract-specific-service-hours"></a><span data-ttu-id="cb1ae-126">Slik definerer du kontraktsspesifikke servicetimer</span><span class="sxs-lookup"><span data-stu-id="cb1ae-126">To set up contract specific service hours</span></span>  
<span data-ttu-id="cb1ae-127">Du kan bruke vinduet **Servicetimer** til å definere spesifikke servicetimer timer for kunden som eier servicekontrakten.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-127">You can use the **Service Hours** window to set up specific service hours for the customer that owns the service contract.</span></span> <span data-ttu-id="cb1ae-128">Servicetimer brukes til å beregne responsdatoen og -tiden for serviceordrer og -tilbud som hører til servicekontrakten.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-128">Service hours are used to calculate the response date and time for service orders and quotes that belong to the service contract.</span></span>  
  
<span data-ttu-id="cb1ae-129">Hvis du ikke definerer spesifikke servicetimer for servicekontrakten, brukes standard servicetimer for servicekontraktene.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-129">If you do not set up specific service hours for the service contract, the default service hours for service contracts are used.</span></span>  
  
1. <span data-ttu-id="cb1ae-130">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Servicekontrakter**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-130">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Contracts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="cb1ae-131">Åpne servicekontrakten du vil definere spesifikke servicetimer for, og velg **Servicetimer**.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-131">Open the service contract you want to set up specific service hours for, and choose **Service Hours**.</span></span>  
4. <span data-ttu-id="cb1ae-132">Hvis du vil definere servicetimer basert på standard servicetimer, velger du handlingen **Kopier std. servicetimer**.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-132">To set up service hours based on default service hours, choose the **Copy Default Service Hours** action.</span></span>  
5. <span data-ttu-id="cb1ae-133">Rediger feltene i servicetimepostene.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-133">Edit the fields in the service hours entries.</span></span> <span data-ttu-id="cb1ae-134">Sett inn eller slett poster for å definere servicetimer for kontrakten.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-134">Insert or delete entries to set up the service hours for the contract.</span></span> <span data-ttu-id="cb1ae-135">Merk at feltene **Dag**, **Starttidspunkt** og **Sluttidspunkt** kreves for hver linje.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-135">Note that the fields **Day**, **Starting Time** and **Ending Time** are required for each line.</span></span>  
6. <span data-ttu-id="cb1ae-136">Hvis du vil at servicetimene skal gjelde fra en bestemt dato, fyller du ut feltet **Startdato**.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-136">If you want the service hours to be valid from a specific date, fill in the **Starting Date** field.</span></span>  
7. <span data-ttu-id="cb1ae-137">Hvis du vil at servicetimene skal gjelde i ferier, setter du en hake i avmerkingsboksen i feltet **Gyldig i ferier**.</span><span class="sxs-lookup"><span data-stu-id="cb1ae-137">If you want the service hours to be valid on holidays, select the check box in the **Valid on Holidays** field.</span></span>  

## <a name="see-also"></a><span data-ttu-id="cb1ae-138">Se også</span><span class="sxs-lookup"><span data-stu-id="cb1ae-138">See Also</span></span>  
[<span data-ttu-id="cb1ae-139">Forstå tildelingsstatus og reparasjonsstatus</span><span class="sxs-lookup"><span data-stu-id="cb1ae-139">Understanding Allocation Status and Repair Status</span></span>](service-allocation-status-and-repair-status.md)  
[<span data-ttu-id="cb1ae-140">Konfigurere servicehåndtering</span><span class="sxs-lookup"><span data-stu-id="cb1ae-140">Setting Up Service Management</span></span>](service-setup-service.md)  
[<span data-ttu-id="cb1ae-141">Forstå serviceordre- og reparasjonsstatus</span><span class="sxs-lookup"><span data-stu-id="cb1ae-141">Understanding Service Order and Repair Status</span></span>](service-order-repair-status.md)  

