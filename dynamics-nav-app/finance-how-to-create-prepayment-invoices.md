---
title: Opprette forskuddsfakturaer
description: "Lær hvordan du vil håndtere situasjoner der du eller leverandøren krever forskuddsbetaling."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: a5480e9a4ad332a5faf668cc53ea7a750cfa0e17
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-prepayment-invoices"></a><span data-ttu-id="43159-103">Opprette forskuddsfakturaer</span><span class="sxs-lookup"><span data-stu-id="43159-103">How to: Create Prepayment Invoices</span></span>
<span data-ttu-id="43159-104">Hvis du krever at kundene skal betale før du leverer en ordre til dem, eller hvis leverandøren krever at du betaler før de leverer en ordre til deg, kan du bruke funksjonaliteten for forskudd.</span><span class="sxs-lookup"><span data-stu-id="43159-104">If you require your customers to submit payment before you ship an order to them, or if your vendor requires you to submit payment before they ship an order to you, you can use the prepayment functionality.</span></span>  

<span data-ttu-id="43159-105">Når du har opprettet en ordre eller bestilling, kan du opprette en forskuddsfaktura.</span><span class="sxs-lookup"><span data-stu-id="43159-105">After you create a sales or purchase order, you can create a prepayment invoice.</span></span> <span data-ttu-id="43159-106">Du kan bruke standardprosentene for hver salgslinje eller bestillingslinje, eller du kan justere beløpet etter behov.</span><span class="sxs-lookup"><span data-stu-id="43159-106">You can use the default percentages for each sales or purchase line, or you can adjust the amount as necessary.</span></span> <span data-ttu-id="43159-107">Du kan for eksempel angi et totalbeløp for hele ordren.</span><span class="sxs-lookup"><span data-stu-id="43159-107">For example, you can specify a total amount for the entire order.</span></span>  

<span data-ttu-id="43159-108">Fremgangsmåten nedenfor beskriver hvordan du fakturerer et forskudd for en ordre.</span><span class="sxs-lookup"><span data-stu-id="43159-108">The following procedure describes how to invoice a prepayment for a sales orders.</span></span> <span data-ttu-id="43159-109">Trinnene er de samme for bestillinger.</span><span class="sxs-lookup"><span data-stu-id="43159-109">The steps are similar for purchase orders.</span></span>  

## <a name="to-create-a-prepayment-invoice"></a><span data-ttu-id="43159-110">Slik oppretter du en forskuddsfaktura:</span><span class="sxs-lookup"><span data-stu-id="43159-110">To create a prepayment invoice</span></span>  
1. <span data-ttu-id="43159-111">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Ordrer**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="43159-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="43159-112">Opprett en ny ordre.</span><span class="sxs-lookup"><span data-stu-id="43159-112">Create a new sales order.</span></span> <span data-ttu-id="43159-113">Hvis du vil ha mer informasjon, kan du se [Selge produkter](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="43159-113">For more information, see [How to: sell Products](sales-how-sell-products.md).</span></span>  

    <span data-ttu-id="43159-114">På hurtigfanen **Forskudd** fylles **Forskuddsprosent**-feltet ut automatisk hvis det er angitt en standard forskuddsprosent på kundekortet.</span><span class="sxs-lookup"><span data-stu-id="43159-114">On the **Prepayment** FastTab, the **Prepayment %** field will be filled in automatically if there is a default prepayment percentage on the customer card.</span></span> <span data-ttu-id="43159-115">Du kan endre innholdet i feltet.</span><span class="sxs-lookup"><span data-stu-id="43159-115">You can change the contents of the field.</span></span> <span data-ttu-id="43159-116">Forskuddsprosenten kopieres bare fra hodet til linjer som ikke kopierer standard forskuddsprosent fra varen.</span><span class="sxs-lookup"><span data-stu-id="43159-116">The prepayment percentage is only copied from the header to lines that do not copy the default prepayment percentage from the item.</span></span>  

    <span data-ttu-id="43159-117">Hvis feltet **Komprimer forskudd** er valgt, kombineres linjene på fakturaen hvis følgende er tilfelle:</span><span class="sxs-lookup"><span data-stu-id="43159-117">If the **Compress Prepayment** field is selected, lines will be combined on the invoice if:</span></span>  
    - <span data-ttu-id="43159-118">De har samme finanskonto for forskudd, som definert i det generelle bokføringsoppsettet.</span><span class="sxs-lookup"><span data-stu-id="43159-118">They have the same general ledger account for prepayments as determined by the general posting setup.</span></span>  
    - <span data-ttu-id="43159-119">De har samme dimensjoner.</span><span class="sxs-lookup"><span data-stu-id="43159-119">They have the same dimensions.</span></span>  

    <span data-ttu-id="43159-120">La feltet stå tomt hvis du vil definere en forskuddsfaktura med én linje for hver ordrelinje som har en forskuddsprosent.</span><span class="sxs-lookup"><span data-stu-id="43159-120">Leave the field blank if you want to specify a prepayment invoice with one line for each sales order line that has a prepayment percentage.</span></span>  

3. <span data-ttu-id="43159-121">Fyll ut salgslinjene.</span><span class="sxs-lookup"><span data-stu-id="43159-121">Fill in the sales lines.</span></span>  

    <span data-ttu-id="43159-122">Hvis det er definert standard forskuddsprosenter for varene, kopieres de automatisk til **Forskuddsprosent**-feltet på linjen.</span><span class="sxs-lookup"><span data-stu-id="43159-122">If default prepayment percentages have been set up for your items, they are automatically copied to the **Prepayment %** field on the line.</span></span> <span data-ttu-id="43159-123">Ellers kopieres forskuddsprosenten fra hodet.</span><span class="sxs-lookup"><span data-stu-id="43159-123">Otherwise, the prepayment percentage is copied from the header.</span></span> <span data-ttu-id="43159-124">Du kan endre verdien i **Forskuddsprosent**-feltet på linjen.</span><span class="sxs-lookup"><span data-stu-id="43159-124">You can change the contents of the **Prepayment %** field on the line.</span></span>  
4. <span data-ttu-id="43159-125">Hvis du vil bruke én forskuddsprosent på hele ordren, endrer du **Forskuddsprosent**-feltet på hodet etter at du har fylt ut linjene.</span><span class="sxs-lookup"><span data-stu-id="43159-125">If you want to apply one prepayment percentage to the entire order, change the **Prepayment %** field on the header after filling in the lines.</span></span>  
5. <span data-ttu-id="43159-126">Du kan vise det totale forskuddsbeløpet ved å velge **Statistikk**-handlingen.</span><span class="sxs-lookup"><span data-stu-id="43159-126">To view the total prepayment amount, choose the **Statistics** action.</span></span>

    <span data-ttu-id="43159-127">Hvis du vil justere det totale forskuddsbeløpet for ordren, kan du endre verdien i **Forskuddsbeløp**-feltet i **Ordrestatistikk**-vinduet.</span><span class="sxs-lookup"><span data-stu-id="43159-127">If you want to adjust the total prepayment amount for the order, you can change the contents of the **Prepayment Amount** field in the **Sales Order Statistics** window.</span></span>  

    <span data-ttu-id="43159-128">Hvis feltet **Priser inkl. mva.** er valgt, kan du redigere feltet **Forskuddsbeløp inkl. mva**.</span><span class="sxs-lookup"><span data-stu-id="43159-128">If the **Prices Including VAT** field is selected, the **Prepayment Amount Incl. VAT** field is editable.</span></span>  

    <span data-ttu-id="43159-129">Hvis du endrer verdien i **Forskuddsbeløp**-feltet, blir beløpet fordelt proporsjonalt mellom alle linjene, unntatt de som har **0** i **Forskuddsprosent**-feltet.</span><span class="sxs-lookup"><span data-stu-id="43159-129">If you change the contents of the **Prepayment Amount** field, the amount will be distributed proportionately between all lines, except those that have **0** in the **Prepayment %** field.</span></span>  
6. <span data-ttu-id="43159-130">Hvis du vil skrive ut en testrapport før du bokfører forskuddsfakturaen, velger du **Forskuddsbetaling** og velger deretter **Testrapport for forskudd**.</span><span class="sxs-lookup"><span data-stu-id="43159-130">To print a test report before posting the prepayment invoice, choose the **Prepayment** action, and then choose the **Prepayment Test Report** action.</span></span>  
7. <span data-ttu-id="43159-131">Hvis du vil bokføre forskuddsfakturaen, velger du **Forskuddsbetaling** og velger deretter **Bokfør forskuddsfaktura**.</span><span class="sxs-lookup"><span data-stu-id="43159-131">To post the prepayment invoice, choose the **Prepayment** action, and then choose the **Post Prepayment Invoice** action.</span></span>  

    <span data-ttu-id="43159-132">Hvis du vil bokføre og skrive ut forskuddsfakturaen, velger du handlingen **Bokfør og skriv ut forskuddsfaktura**.</span><span class="sxs-lookup"><span data-stu-id="43159-132">To post and print the prepayment invoice, choose the **Post and Print Prepmt. Invoice** action.</span></span>  

<span data-ttu-id="43159-133">Du kan utstede flere forskuddsfakturaer for ordren.</span><span class="sxs-lookup"><span data-stu-id="43159-133">You can issue additional prepayment invoices for the order.</span></span> <span data-ttu-id="43159-134">Dette gjør du ved å øke forskuddsbeløpet på én eller flere linjer, justere dokumentdatoen om nødvendig, og bokføre forskuddsfakturaen.</span><span class="sxs-lookup"><span data-stu-id="43159-134">To do this, increase the prepayment amount on one or more lines, adjust the document date if necessary, and post the prepayment invoice.</span></span> <span data-ttu-id="43159-135">Det opprettes en ny faktura for differansen mellom forskuddsbeløpene som er fakturert hittil, og det nye forskuddsbeløpet.</span><span class="sxs-lookup"><span data-stu-id="43159-135">A new invoice will be created for the difference between the prepayment amounts invoiced so far and the new prepayment amount.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="43159-136">Hvis du befinner deg i Nord-Amerika, kan du ikke endre forskuddsprosenten når den forskuddsbetalte fakturaen er bokført.</span><span class="sxs-lookup"><span data-stu-id="43159-136">If you are located in North America, you cannot change the prepayment percentage after the prepayment invoice has been posted.</span></span> <span data-ttu-id="43159-137">Dette er ikke tillatt i Nord-Amerika-versjonen av [!INCLUDE[d365fin](includes/d365fin_md.md)] fordi beregningen av merverdiavgift ellers blir feil.</span><span class="sxs-lookup"><span data-stu-id="43159-137">This is prevented in the North American version of [!INCLUDE[d365fin](includes/d365fin_md.md)] because the calculation of sales tax will otherwise be incorrect.</span></span>  

 <span data-ttu-id="43159-138">Når du er klar til å bokføre resten av fakturaen, bokfører du den som en hvilken som helst annen faktura, og forskuddsbeløpet blir automatisk trukket fra forfallsbeløpet.</span><span class="sxs-lookup"><span data-stu-id="43159-138">When you are ready to post the rest of the invoice, post it as you would post any invoice, and the prepayment amount will automatically be deducted from the amount due.</span></span>  

## <a name="see-also"></a><span data-ttu-id="43159-139">Se også</span><span class="sxs-lookup"><span data-stu-id="43159-139">See Also</span></span>  
[<span data-ttu-id="43159-140">Fakturere forskuddsbetalinger</span><span class="sxs-lookup"><span data-stu-id="43159-140">Invoicing Prepayments</span></span>](finance-invoice-prepayments.md)  
[<span data-ttu-id="43159-141">Gjennomgang: konfigurere og fakturere salgsforskudd</span><span class="sxs-lookup"><span data-stu-id="43159-141">Walkthrough: Setting Up and Invoicing Sales Prepayments</span></span>](walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
[<span data-ttu-id="43159-142">Finans</span><span class="sxs-lookup"><span data-stu-id="43159-142">Finance</span></span>](finance.md)  
<span data-ttu-id="43159-143">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="43159-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

