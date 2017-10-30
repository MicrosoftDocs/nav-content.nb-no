---
title: Gjennomgang - Mottak og plassering i grunnleggende lageroppsett
description: "I [!INCLUDE[d365fin](includes/d365fin_md.md)] kan de inngående prosessene for mottak og plassering utføres på fire måter ved hjelp av forskjellige funksjoner avhengig av kompleksitetsnivået til lageret."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 0a540f5813ed67ee62e43390d6d11b7c3a137f13
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="walkthrough-receiving-and-putting-away-in-basic-warehouse-configurations"></a><span data-ttu-id="06310-103">Gjennomgang: Mottak og plassering i grunnleggende lageroppsett</span><span class="sxs-lookup"><span data-stu-id="06310-103">Walkthrough: Receiving and Putting Away in Basic Warehouse Configurations</span></span>
<span data-ttu-id="06310-104">I [!INCLUDE[d365fin](includes/d365fin_md.md)] kan de inngående prosessene for mottak og plassering utføres på fire måter ved hjelp av forskjellige funksjoner avhengig av kompleksitetsnivået til lageret.</span><span class="sxs-lookup"><span data-stu-id="06310-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the inbound processes for receiving and putting away can be performed in four ways using different functionalities depending on the warehouse complexity level.</span></span>  

|<span data-ttu-id="06310-105">Prinsipp</span><span class="sxs-lookup"><span data-stu-id="06310-105">Method</span></span>|<span data-ttu-id="06310-106">Inngående prosess</span><span class="sxs-lookup"><span data-stu-id="06310-106">Inbound process</span></span>|<span data-ttu-id="06310-107">Hyller</span><span class="sxs-lookup"><span data-stu-id="06310-107">Bins</span></span>|<span data-ttu-id="06310-108">Mottak</span><span class="sxs-lookup"><span data-stu-id="06310-108">Receipts</span></span>|<span data-ttu-id="06310-109">Plassering</span><span class="sxs-lookup"><span data-stu-id="06310-109">Put-aways</span></span>|<span data-ttu-id="06310-110">Kompleksitetsnivå (se [Designdetaljer: Lageroppsett](design-details-warehouse-setup.md))</span><span class="sxs-lookup"><span data-stu-id="06310-110">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span></span>|  
|------------|---------------------|----------|--------------|----------------|--------------------------------------------------------------------------------------------------------------------|  
|<span data-ttu-id="06310-111">A</span><span class="sxs-lookup"><span data-stu-id="06310-111">A</span></span>|<span data-ttu-id="06310-112">Bokføre mottak og plassering fra ordrelinjen</span><span class="sxs-lookup"><span data-stu-id="06310-112">Post receipt and put-away from the order line</span></span>|<span data-ttu-id="06310-113">X</span><span class="sxs-lookup"><span data-stu-id="06310-113">X</span></span>|||<span data-ttu-id="06310-114">2</span><span class="sxs-lookup"><span data-stu-id="06310-114">2</span></span>|  
|<span data-ttu-id="06310-115">B</span><span class="sxs-lookup"><span data-stu-id="06310-115">B</span></span>|<span data-ttu-id="06310-116">Bokføre mottak og plassering fra et lagerplasseringsdokument</span><span class="sxs-lookup"><span data-stu-id="06310-116">Post receipt and put-away from an inventory put-away document</span></span>|||<span data-ttu-id="06310-117">X</span><span class="sxs-lookup"><span data-stu-id="06310-117">X</span></span>|<span data-ttu-id="06310-118">3</span><span class="sxs-lookup"><span data-stu-id="06310-118">3</span></span>|  
|<span data-ttu-id="06310-119">L</span><span class="sxs-lookup"><span data-stu-id="06310-119">C</span></span>|<span data-ttu-id="06310-120">Bokføre mottak og plassering fra et lagermottaksdokument</span><span class="sxs-lookup"><span data-stu-id="06310-120">Post receipt and put-away from a warehouse receipt document</span></span>||<span data-ttu-id="06310-121">X</span><span class="sxs-lookup"><span data-stu-id="06310-121">X</span></span>||<span data-ttu-id="06310-122">4/5/6</span><span class="sxs-lookup"><span data-stu-id="06310-122">4/5/6</span></span>|  
|<span data-ttu-id="06310-123">D</span><span class="sxs-lookup"><span data-stu-id="06310-123">D</span></span>|<span data-ttu-id="06310-124">Bokføre mottak fra et lagermottaksdokument og bokføre plassering fra et lagerplasseringsdokument</span><span class="sxs-lookup"><span data-stu-id="06310-124">Post receipt from a warehouse receipt document and post put-away from a warehouse put-away document</span></span>||<span data-ttu-id="06310-125">X</span><span class="sxs-lookup"><span data-stu-id="06310-125">X</span></span>|<span data-ttu-id="06310-126">X</span><span class="sxs-lookup"><span data-stu-id="06310-126">X</span></span>|<span data-ttu-id="06310-127">4/5/6</span><span class="sxs-lookup"><span data-stu-id="06310-127">4/5/6</span></span>|  

<span data-ttu-id="06310-128">Hvis du vil ha mer informasjon, kan du se [Designdetaljer: Inngående lagerflyt](design-details-inbound-warehouse-flow.md).</span><span class="sxs-lookup"><span data-stu-id="06310-128">For more information, see [Design Details: Inbound Warehouse Flow](design-details-inbound-warehouse-flow.md).</span></span>  

<span data-ttu-id="06310-129">Følgende gjennomgangen demonstrerer metoden B i forrige tabell.</span><span class="sxs-lookup"><span data-stu-id="06310-129">The following walkthrough demonstrates method B in the previous table.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="06310-130">Denne gjennomgangen</span><span class="sxs-lookup"><span data-stu-id="06310-130">About This Walkthrough</span></span>  
<span data-ttu-id="06310-131">I genkle lageroppsett hvor lokasjonen er definert til å kreve plasseringsbehandling, men ikke mottaksbehandling, bruker du vinduet **Lagerplassering** til å registrere og bokføre plasserings- og mottaksopplysninger for de inngående kildedokumentene.</span><span class="sxs-lookup"><span data-stu-id="06310-131">In basic warehouse configurations where your location is set up to require put-away processing but not receive processing, you use the **Inventory Put-away** window to record and post put-away and receipt information for your inbound source documents.</span></span> <span data-ttu-id="06310-132">Det inngående kildedokument kan være en bestilling, en ordreretur, en inngående overføringsordre eller en produksjonsordre med avgang som er klar til plassering.</span><span class="sxs-lookup"><span data-stu-id="06310-132">The inbound source document can be a purchase order, sales return order, inbound transfer order, or production order with output that is ready to be put away.</span></span>

> [!NOTE]
> <span data-ttu-id="06310-133">Selv om innstillingene kalles **Plukk nødv.** og **Plassering nødv.**, kan du bokføre mottak og leveringer direkte fra kildedokumenter for firma på lokasjoner der du velger disse avmerkingsboksene.</span><span class="sxs-lookup"><span data-stu-id="06310-133">Even though the settings are called **Require Pick** and **Require Put-away**, you can still post receipts and shipments directly from the source business documents at locations where you select these check boxes.</span></span>  

<span data-ttu-id="06310-134">Denne gjennomgangen viser følgende oppgaver.</span><span class="sxs-lookup"><span data-stu-id="06310-134">This walkthrough demonstrates the following tasks.</span></span>  

-   <span data-ttu-id="06310-135">Definere SØLV-plassering for lagerplasseringer.</span><span class="sxs-lookup"><span data-stu-id="06310-135">Setting up SILVER location for inventory put aways.</span></span>  
-   <span data-ttu-id="06310-136">Definere SØLV-plassering for hyllehåndtering.</span><span class="sxs-lookup"><span data-stu-id="06310-136">Setting up SILVER location for bin handling.</span></span>  
-   <span data-ttu-id="06310-137">Definere en standardhylle for varen LS-81.</span><span class="sxs-lookup"><span data-stu-id="06310-137">Defining a default bin for item LS-81.</span></span> <span data-ttu-id="06310-138">(LS-75 er allerede er satt opp i CRONUS.)</span><span class="sxs-lookup"><span data-stu-id="06310-138">(LS-75 is already set up in CRONUS.)</span></span>  
-   <span data-ttu-id="06310-139">Opprette en bestilling for leverandør 10000 for 40 høyttalere.</span><span class="sxs-lookup"><span data-stu-id="06310-139">Creating a purchase order for vendor 10000 for 40 loudspeakers.</span></span>  
-   <span data-ttu-id="06310-140">Verifiserer at plasseringshyllene er forhåndsinnstilt i oppsettet.</span><span class="sxs-lookup"><span data-stu-id="06310-140">Verifying that the put-away bins are preset by setup.</span></span>  
-   <span data-ttu-id="06310-141">Frigir bestillingen for lagerhåndtering.</span><span class="sxs-lookup"><span data-stu-id="06310-141">Releasing the purchase order for warehouse handling.</span></span>  
-   <span data-ttu-id="06310-142">Opprette en lagerplassering basert på et frigitt kildedokument.</span><span class="sxs-lookup"><span data-stu-id="06310-142">Creating an inventory put-away based on a released source document.</span></span>  
-   <span data-ttu-id="06310-143">Verifiserer at plasseringshyllene er arvet fra bestillingen.</span><span class="sxs-lookup"><span data-stu-id="06310-143">Verifying that the put-away bins are inherited from the purchase order.</span></span>  
-   <span data-ttu-id="06310-144">Registrerer lagerflyttingen til lageret og bokfører samtidig mottaket for kildebestillingen.</span><span class="sxs-lookup"><span data-stu-id="06310-144">Registering the warehouse movement into the warehouse and at the same time posting the purchase receipt for the source purchase order.</span></span>  

## <a name="roles"></a><span data-ttu-id="06310-145">Roller</span><span class="sxs-lookup"><span data-stu-id="06310-145">Roles</span></span>  
<span data-ttu-id="06310-146">Denne gjennomgangen viser oppgaver som utføres av følgende brukerroller:</span><span class="sxs-lookup"><span data-stu-id="06310-146">This walkthrough demonstrates tasks that are performed by the following user roles:</span></span>  

-   <span data-ttu-id="06310-147">Lagerleder</span><span class="sxs-lookup"><span data-stu-id="06310-147">Warehouse Manager</span></span>  
-   <span data-ttu-id="06310-148">Innkjøper</span><span class="sxs-lookup"><span data-stu-id="06310-148">Purchasing Agent</span></span>  
-   <span data-ttu-id="06310-149">Lagermedarbeider</span><span class="sxs-lookup"><span data-stu-id="06310-149">Warehouse Worker</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="06310-150">Forutsetninger</span><span class="sxs-lookup"><span data-stu-id="06310-150">Prerequisites</span></span>  
<span data-ttu-id="06310-151">For å fullføre denne gjennomgangen må du gjøre følgende:</span><span class="sxs-lookup"><span data-stu-id="06310-151">To complete this walkthrough, you will need:</span></span>  

-   <span data-ttu-id="06310-152">Installere CRONUS Norge AS.</span><span class="sxs-lookup"><span data-stu-id="06310-152">CRONUS International Ltd. installed.</span></span>  
-   <span data-ttu-id="06310-153">Gjør deg til lageransatt på lokasjonen SØLV ved å følge disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="06310-153">To make yourself a warehouse employee at SILVER location by following these steps:</span></span>  

    1.  <span data-ttu-id="06310-154">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Lageransatte**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="06310-154">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Warehouse Employees**, and then choose the related link.</span></span>  
    2.  <span data-ttu-id="06310-155">Velg feltet **Bruker-ID**, og velg din egen brukerkonto i **Brukere**-vinduet.</span><span class="sxs-lookup"><span data-stu-id="06310-155">Choose the **User ID** field, and select your own user account in the **Users** window.</span></span>  
    3.  <span data-ttu-id="06310-156">Skriv inn SØLV i feltet **Lokasjonskode**.</span><span class="sxs-lookup"><span data-stu-id="06310-156">In the **Location Code** field, enter SILVER.</span></span>  
    4.  <span data-ttu-id="06310-157">Velg **Standard**- feltet.</span><span class="sxs-lookup"><span data-stu-id="06310-157">Select the **Default** field.</span></span>  

## <a name="story"></a><span data-ttu-id="06310-158">Hovedscenario</span><span class="sxs-lookup"><span data-stu-id="06310-158">Story</span></span>  
<span data-ttu-id="06310-159">Ellen, lagerlederen hos CRONUS International Ltd., oppretter en bestilling for 10 enheter av varen LS-75 og 30 enheter av varen LS-81 fra leverandør 10000 som skal leveres til SILVER-lageret.</span><span class="sxs-lookup"><span data-stu-id="06310-159">Ellen, the warehouse manager at CRONUS International Ltd., creates a purchase order for 10 units of item LS-75 and 30 units of item LS-81 from vendor 10000 to be delivered to SILVER Warehouse.</span></span> <span data-ttu-id="06310-160">Når leveringen ankommer til lageret, plasserer lagermedarbeideren John varene i standardhyller definert for varene.</span><span class="sxs-lookup"><span data-stu-id="06310-160">When the delivery arrives at the warehouse, John, the warehouse worker, puts the items away in default bins defined for the items.</span></span> <span data-ttu-id="06310-161">Når John bokfører plasseringen, bokføres varene som mottatt på lageret og tilgjengelig for salg eller andre behov.</span><span class="sxs-lookup"><span data-stu-id="06310-161">When John posts the put-away, the items are posted as received into inventory and available for sale or other demand.</span></span>  

## <a name="setting-up-the-location"></a><span data-ttu-id="06310-162">Definere plassering</span><span class="sxs-lookup"><span data-stu-id="06310-162">Setting up the Location</span></span>  
 <span data-ttu-id="06310-163">Oppsettet av vinduet **Lokasjonskort** definerer selskapets lagerflyter.</span><span class="sxs-lookup"><span data-stu-id="06310-163">The setup of the **Location Card** window defines the company’s warehouse flows.</span></span>  

### <a name="to-set-up-the-location"></a><span data-ttu-id="06310-164">Slik definerer du lokasjonen:</span><span class="sxs-lookup"><span data-stu-id="06310-164">To set up the location</span></span>  

1.  <span data-ttu-id="06310-165">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Lokasjoner**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="06310-165">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="06310-166">Åpne lokasjonskortet SØLV.</span><span class="sxs-lookup"><span data-stu-id="06310-166">Open the SILVER location card.</span></span>  
3.  <span data-ttu-id="06310-167">Merk av for **Plassering nødv.**.</span><span class="sxs-lookup"><span data-stu-id="06310-167">Select the **Require Put-away** check box.</span></span>  

    <span data-ttu-id="06310-168">Fortsett med å sette opp en standardhylle for de to varenumrene for å kontrollere hvor de er plassert.</span><span class="sxs-lookup"><span data-stu-id="06310-168">Proceed to set up a default bin for the two item numbers to control where they are put away.</span></span>  

4.  <span data-ttu-id="06310-169">Velg handlingen **Hyller**.</span><span class="sxs-lookup"><span data-stu-id="06310-169">Choose the **Bins** action.</span></span>  
5.  <span data-ttu-id="06310-170">Merk den første raden, hylle S-01-0001, og velg **Innhold**.</span><span class="sxs-lookup"><span data-stu-id="06310-170">Select the first row, for bin S-01-0001, and then choose the **Contents** action.</span></span>  

    <span data-ttu-id="06310-171">Legg merke til at i **Hylleinnhold**-vinduet er varen LS-75 allerede definert som innhold i hyllen S-01-0001.</span><span class="sxs-lookup"><span data-stu-id="06310-171">Notice in the **Bin Content** window that item LS-75 is already set up as content in bin S-01-0001.</span></span>  

6.  <span data-ttu-id="06310-172">Velg handlingen **Ny**.</span><span class="sxs-lookup"><span data-stu-id="06310-172">Choose the **New** action.</span></span>  
7.  <span data-ttu-id="06310-173">Velg feltene **Fast** og **Standard**.</span><span class="sxs-lookup"><span data-stu-id="06310-173">Select the **Fixed** and the **Default** fields.</span></span>  
8.  <span data-ttu-id="06310-174">Angi LS-81 i feltet **Varenr.**.</span><span class="sxs-lookup"><span data-stu-id="06310-174">In the **Item No.** field, enter LS-81.</span></span>  

## <a name="creating-the-purchase-order"></a><span data-ttu-id="06310-175">Opprette bestillingen</span><span class="sxs-lookup"><span data-stu-id="06310-175">Creating the Purchase Order</span></span>  
<span data-ttu-id="06310-176">Bestillinger er den vanligste typen inngående kildedokument.</span><span class="sxs-lookup"><span data-stu-id="06310-176">Purchase orders are the most common type of inbound source document.</span></span>  

### <a name="to-create-the-purchase-order"></a><span data-ttu-id="06310-177">Slik oppretter du bestillingen:</span><span class="sxs-lookup"><span data-stu-id="06310-177">To create the purchase order</span></span>  

1.  <span data-ttu-id="06310-178">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bestillinger**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="06310-178">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="06310-179">Velg handlingen **Ny**.</span><span class="sxs-lookup"><span data-stu-id="06310-179">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="06310-180">Opprett en bestilling for leverandør 10000 på arbeidsdatoen (23. januar) med følgende bestillingslinjer.</span><span class="sxs-lookup"><span data-stu-id="06310-180">Create a purchase order for vendor 10000 on the work date (January 23) with the following purchase order lines.</span></span>  

    |<span data-ttu-id="06310-181">Vare</span><span class="sxs-lookup"><span data-stu-id="06310-181">Item</span></span>|<span data-ttu-id="06310-182">Lokasjonskode</span><span class="sxs-lookup"><span data-stu-id="06310-182">Location code</span></span>|<span data-ttu-id="06310-183">Hyllekode</span><span class="sxs-lookup"><span data-stu-id="06310-183">Bin code</span></span>|<span data-ttu-id="06310-184">Antall</span><span class="sxs-lookup"><span data-stu-id="06310-184">Quantity</span></span>|  
    |----------|-------------------|--------------|--------------|  
    |<span data-ttu-id="06310-185">LS_75</span><span class="sxs-lookup"><span data-stu-id="06310-185">LS_75</span></span>|<span data-ttu-id="06310-186">SØLV</span><span class="sxs-lookup"><span data-stu-id="06310-186">SILVER</span></span>|<span data-ttu-id="06310-187">S-01-0001</span><span class="sxs-lookup"><span data-stu-id="06310-187">S-01-0001</span></span>|<span data-ttu-id="06310-188">10</span><span class="sxs-lookup"><span data-stu-id="06310-188">10</span></span>|  
    |<span data-ttu-id="06310-189">LS-81</span><span class="sxs-lookup"><span data-stu-id="06310-189">LS-81</span></span>|<span data-ttu-id="06310-190">SØLV</span><span class="sxs-lookup"><span data-stu-id="06310-190">SILVER</span></span>|<span data-ttu-id="06310-191">S-01-0001</span><span class="sxs-lookup"><span data-stu-id="06310-191">S-01-0001</span></span>|<span data-ttu-id="06310-192">30</span><span class="sxs-lookup"><span data-stu-id="06310-192">30</span></span>|  

    > [!NOTE]  
    >  <span data-ttu-id="06310-193">Hyllekoden angis automatisk i samsvar med oppsettet du utførte i delen Definere plassering.</span><span class="sxs-lookup"><span data-stu-id="06310-193">The bin code is entered automatically according to the setup that you performed in the “Setting up the Location” section.</span></span>  

    <span data-ttu-id="06310-194">Fortsett med å varsle lageret om at bestillingen er klar for håndtering av lageret når leveringen ankommer.</span><span class="sxs-lookup"><span data-stu-id="06310-194">Proceed to notify the warehouse that the purchase order is ready for warehouse handling when the delivery arrives.</span></span>  

4.  <span data-ttu-id="06310-195">Velg handlingen **Frigi**.</span><span class="sxs-lookup"><span data-stu-id="06310-195">Choose the **Release** action.</span></span>  

    <span data-ttu-id="06310-196">Leveringen av høyttalere fra leverandør 10000 er ankommet på SØLV-lageret, og John fortsetter med å plassere dem.</span><span class="sxs-lookup"><span data-stu-id="06310-196">The delivery of loudspeakers from vendor 10000 has arrived at SILVER warehouse, and John proceeds to put them away.</span></span>  

## <a name="receiving-and-putting-the-items-away"></a><span data-ttu-id="06310-197">Mottak og plassering av varer</span><span class="sxs-lookup"><span data-stu-id="06310-197">Receiving and Putting the Items Away</span></span>  
<span data-ttu-id="06310-198">I vinduet **Lagerplassering** kan du håndtere alle inngående lageraktiviteter for et bestemt kildedokument, for eksempel en bestilling.</span><span class="sxs-lookup"><span data-stu-id="06310-198">In the **Inventory Put-away** window, you can manage all inbound warehouse activities for a specific source document, such as a purchase order.</span></span>  

### <a name="to-receive-and-put-the-items-away"></a><span data-ttu-id="06310-199">Slik mottar og plasserer du varene:</span><span class="sxs-lookup"><span data-stu-id="06310-199">To receive and put the items away</span></span>  

1.  <span data-ttu-id="06310-200">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Lagerplasseringer**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="06310-200">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Inventory Put-aways**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="06310-201">Velg handlingen **Ny**.</span><span class="sxs-lookup"><span data-stu-id="06310-201">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="06310-202">Velg feltet **Kildedokument**, og velg deretter **Bestilling**.</span><span class="sxs-lookup"><span data-stu-id="06310-202">Select the **Source Document** field, and then select **Purchase Order**.</span></span>  
4.  <span data-ttu-id="06310-203">Velg feltet **Kildenr.**, velg linjen for kjøp fra leverandør 10000, og velg deretter **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="06310-203">Select the **Source No.** field, select the line for the purchase from vendor 10000, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="06310-204">På fanebladet **Handlinger** i gruppen **Funksjoner** velger du eventuelt **Hent kildedokument**, og deretter velger du bestillingen.</span><span class="sxs-lookup"><span data-stu-id="06310-204">Alternatively, on the **Actions** tab, in the **Functions** group, choose **Get Source Document**, and then select the purchase order.</span></span>  

5.  <span data-ttu-id="06310-205">Velg handlingen **Autoutfyll ant som skal håndt**.</span><span class="sxs-lookup"><span data-stu-id="06310-205">Choose the **Autofill Qty. to Handle** action.</span></span>  

    <span data-ttu-id="06310-206">Du kan også skrive inn 10 og 30 i de to lagerplasseringslinjene i feltet **Ant. som skal håndt.**.</span><span class="sxs-lookup"><span data-stu-id="06310-206">Alternatively, in the **Qty. to Handle** field, enter 10 and 30 respectively on the two inventory put-away lines.</span></span>  

6.  <span data-ttu-id="06310-207">Velg **Bokfør**-handlingen, velg **Motta og fakturer**, og velg deretter **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="06310-207">Choose the **Post** action, select the **Receive** action, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="06310-208">40 høyttalere er nå registrert som plassert i hyllen S-01-0001, og det opprettes en positiv varepost som gjenspeiler det bokførte kjøpsmottaket.</span><span class="sxs-lookup"><span data-stu-id="06310-208">The 40 loudspeakers are now registered as put away in bin S-01-0001, and a positive item ledger entry is created reflecting the posted purchase receipt.</span></span>  

## <a name="see-also"></a><span data-ttu-id="06310-209">Se også</span><span class="sxs-lookup"><span data-stu-id="06310-209">See Also</span></span>  
 <span data-ttu-id="06310-210">[Plassere varer med lagerplasseringer](warehouse-how-to-put-items-away-with-inventory-put-aways.md) </span><span class="sxs-lookup"><span data-stu-id="06310-210">[How to: Put Items Away with Inventory Put-aways](warehouse-how-to-put-items-away-with-inventory-put-aways.md) </span></span>  
 <span data-ttu-id="06310-211">[Opprette grunnleggende lagre med operasjonsområder](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md) </span><span class="sxs-lookup"><span data-stu-id="06310-211">[How to: Set Up Basic Warehouses with Operations Areas](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md) </span></span>  
 <span data-ttu-id="06310-212">[Flytte komponenter til et operasjonsområde i enkle lageroppsett](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md) </span><span class="sxs-lookup"><span data-stu-id="06310-212">[How to: Move Components to an Operation Area in Basic Warehouse Configurations](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md) </span></span>  
 <span data-ttu-id="06310-213">[Plukke for produksjon eller montering](warehouse-how-to-pick-for-production.md) </span><span class="sxs-lookup"><span data-stu-id="06310-213">[How to: Pick for Production or Assembly](warehouse-how-to-pick-for-production.md) </span></span>  
 <span data-ttu-id="06310-214">[Flytte varer ad hoc i enkle lageroppsett](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md) </span><span class="sxs-lookup"><span data-stu-id="06310-214">[How to: Move Items Ad Hoc in Basic Warehouse Configurations](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md) </span></span>  
 <span data-ttu-id="06310-215">[Designdetaljer: Inngående lagerflyt](design-details-inbound-warehouse-flow.md) </span><span class="sxs-lookup"><span data-stu-id="06310-215">[Design Details: Inbound Warehouse Flow](design-details-inbound-warehouse-flow.md) </span></span>  
 [<span data-ttu-id="06310-216">Gjennomgang av forretningsprosesser</span><span class="sxs-lookup"><span data-stu-id="06310-216">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
 <span data-ttu-id="06310-217">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="06310-217">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

