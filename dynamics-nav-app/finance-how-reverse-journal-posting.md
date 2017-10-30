---
title: "Angre en bokføring ved å bokføre en tilbakeføringspost"
description: "Hvis du har foretatt en feilaktig bokføring i finanskladden, kan du bruke funksjonen Tilbakefør transaksjon til å angre bokføringen med et riktig revisjonsspor."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 08/03/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 2970914c36f892a5610509e9dc4015d0fb159642
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-reverse-postings"></a><span data-ttu-id="27dfb-103">Tilbakeføre bokføringer</span><span class="sxs-lookup"><span data-stu-id="27dfb-103">How to: Reverse Postings</span></span>
<span data-ttu-id="27dfb-104">Hvis du vil angre en feilaktig kladdebokføring, velger du posten og oppretter en tilbakeføringspost (poster som er identiske med den opprinnelige posten, men med motsatt fortegn i beløpsfeltet) med samme bilagsnummer og bokføringsdato som den opprinnelige posten.</span><span class="sxs-lookup"><span data-stu-id="27dfb-104">To undo an erroneous journal posting, you select the entry and create a reverse entry (entries identical to the original entry but with opposite sign in the amount field) with the same document number and posting date as the original entry.</span></span> <span data-ttu-id="27dfb-105">Når du har tilbakeført en post, må du lage den riktige posten.</span><span class="sxs-lookup"><span data-stu-id="27dfb-105">After reversing an entry, you must make the correct entry.</span></span>

<span data-ttu-id="27dfb-106">Du kan bare tilbakeføre poster som er bokført fra en finanskladdelinje.</span><span class="sxs-lookup"><span data-stu-id="27dfb-106">You can only reverse entries that are posted from a general journal line.</span></span> <span data-ttu-id="27dfb-107">En post kan bare tilbakeføres én gang.</span><span class="sxs-lookup"><span data-stu-id="27dfb-107">An entry can only be reversed once.</span></span>

<span data-ttu-id="27dfb-108">Hvis du vil ha mer informasjon om bokføring fra en finanskladd, kan du se [Bokføre transaksjoner direkte i Finans](finance-how-post-transactions-directly.md).</span><span class="sxs-lookup"><span data-stu-id="27dfb-108">For more information about posting from a general journal, see [How to: Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md).</span></span>

<span data-ttu-id="27dfb-109">Hvis du har utført en ukorrekt nagativ antallsbokføring, for eksempel en bestilling med galt vareantall, og bokført denne som mottatt (men ikke fakturert), kan du angre bokføringen.</span><span class="sxs-lookup"><span data-stu-id="27dfb-109">If you have made an incorrect negative quantity posting, such as a purchase order with the wrong number of items and posted it as received but not invoiced, then you can undo the posting.</span></span>

<span data-ttu-id="27dfb-110">Hvis du har utført en ukorrekt positiv antallsbokføring, for eksempel en bestillingsretur med galt vareantall, og bokført denne som sendt (men ikke fakturert), kan du angre bokføringen.</span><span class="sxs-lookup"><span data-stu-id="27dfb-110">If you have made an incorrect positive quantity posting, such as a purchase return order with the wrong number of items and posted it as shipped but not invoiced, then you can undo the posting.</span></span>   

## <a name="to-reverse-the-journal-posting-of-a-general-ledger-entry"></a><span data-ttu-id="27dfb-111">Tilbakeføre kladdebokføring av en finanspost</span><span class="sxs-lookup"><span data-stu-id="27dfb-111">To reverse the journal posting of a general ledger entry</span></span>
<span data-ttu-id="27dfb-112">Du kan tilbakeføre poster i alle **Poster**-vinduer.</span><span class="sxs-lookup"><span data-stu-id="27dfb-112">You can reverse entries from all **Ledger Entries** windows.</span></span> <span data-ttu-id="27dfb-113">Fremgangsmåten nedenfor er basert på vinduet **Finansposter**.</span><span class="sxs-lookup"><span data-stu-id="27dfb-113">The following procedure is based on the **General Ledger Entries** window.</span></span>
1. <span data-ttu-id="27dfb-114">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Finansposter**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="27dfb-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Ledger Entries**, and then choose the related link.</span></span>
2. <span data-ttu-id="27dfb-115">Velg posten du vil tilbakeføre, og velg deretter handlingen **Tilbakefør transaksjon**.</span><span class="sxs-lookup"><span data-stu-id="27dfb-115">Select the entry that you want to reverse, and then choose the **Reverse Transaction** action.</span></span> <span data-ttu-id="27dfb-116">Vær oppmerksom på at den må stamme fra en kladdebokføring.</span><span class="sxs-lookup"><span data-stu-id="27dfb-116">Note that is must originate from a journal posting.</span></span>
3. <span data-ttu-id="27dfb-117">I vinduet **Tilbakefør transaksjonsposter** velger du den relevante posten og deretter handlingen **Tilbakefør**.</span><span class="sxs-lookup"><span data-stu-id="27dfb-117">In the **Reverse Transaction Entries** window, select the relevant entry, and then choose the **Reverse** action.</span></span>
4. <span data-ttu-id="27dfb-118">Velg **Ja** i bekreftelsesmeldingen.</span><span class="sxs-lookup"><span data-stu-id="27dfb-118">Choose the **Yes** button on the confirmation message.</span></span>

## <a name="to-undo-a-quantity-posting-on-a-posted-purchase-receipt"></a><span data-ttu-id="27dfb-119">Slik angrer du antallsbokføring på bokførte kjøpsmottak</span><span class="sxs-lookup"><span data-stu-id="27dfb-119">To undo a quantity posting on a posted purchase receipt</span></span>  

1.  <span data-ttu-id="27dfb-120">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bokførte kjøpsmottak**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="27dfb-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Purchase Receipts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="27dfb-121">Åpne det bokførte mottaket som du vil angre.</span><span class="sxs-lookup"><span data-stu-id="27dfb-121">Open the posted receipt that you want to undo.</span></span>  
3.  <span data-ttu-id="27dfb-122">Velg linjen(e) du vil angre.</span><span class="sxs-lookup"><span data-stu-id="27dfb-122">Select the line or lines that you want to undo.</span></span>  
4.  <span data-ttu-id="27dfb-123">Velg **Angre mottak**-handlingen.</span><span class="sxs-lookup"><span data-stu-id="27dfb-123">Choose **Undo Receipt** action.</span></span>

    <span data-ttu-id="27dfb-124">Det settes inn en korreksjonslinje under den valgte mottakslinjen.</span><span class="sxs-lookup"><span data-stu-id="27dfb-124">A corrective line is inserted under the selected receipt line.</span></span>  

    <span data-ttu-id="27dfb-125">Hvis antallet ble mottatt i et lagermottak, settes en korreksjonslinje inn i det bokførte lagermottaket.</span><span class="sxs-lookup"><span data-stu-id="27dfb-125">If the quantity was received in a warehouse receipt, then a corrective line is inserted in the posted warehouse receipt.</span></span>  

    <span data-ttu-id="27dfb-126">Feltene **Mottatt (antall)** og **Mott. antall (ufakt.)** på den tilknyttede bestillingen blir satt til null.</span><span class="sxs-lookup"><span data-stu-id="27dfb-126">The **Quantity Received** and **Qty. Rcd. Not Invoiced** fields on the related purchase order are set to zero.</span></span>

## <a name="to-undo-and-then-redo-a-quantity-posting-on-a-posted-return-shipment"></a><span data-ttu-id="27dfb-127">Slik angrer du og gjør om en antallsbokføring på en bokført returforsendelse</span><span class="sxs-lookup"><span data-stu-id="27dfb-127">To undo and then redo a quantity posting on a posted return shipment</span></span>

1.  <span data-ttu-id="27dfb-128">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bokførte returforsendelser**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="27dfb-128">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Return Shipments**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="27dfb-129">Åpne den bokførte returforsendelsen som du vil angre.</span><span class="sxs-lookup"><span data-stu-id="27dfb-129">Open the posted return shipment that you want to undo.</span></span>
3. <span data-ttu-id="27dfb-130">Velg linjen(e) du vil angre.</span><span class="sxs-lookup"><span data-stu-id="27dfb-130">Select the line or lines you want to undo.</span></span>  

4.  <span data-ttu-id="27dfb-131">Velg handlingen **Angre returforsendelse**.</span><span class="sxs-lookup"><span data-stu-id="27dfb-131">Choose the **Undo Return Shipment** action.</span></span>  

    <span data-ttu-id="27dfb-132">En korreksjonslinje er satt inn i det bokførte dokumentet, og feltene **Returant. levert** og **Returfors., ikke fakt.** på ordrereturen settes til null.</span><span class="sxs-lookup"><span data-stu-id="27dfb-132">A corrective line is inserted in the posted document, and the **Return Qty. Shipped** and **Return Shpd. Not Invd.** fields on the return order are set to zero.</span></span>  

    <span data-ttu-id="27dfb-133">Gå deretter tilbake til bestillingsreturen for å gjøre om bokføringen.</span><span class="sxs-lookup"><span data-stu-id="27dfb-133">Now go back to the purchase return order to redo the posting.</span></span>  

5.  <span data-ttu-id="27dfb-134">Noter nummeret i feltet **Ordrereturnr.** i vinduet **Bokført bestillingsreturseddel**</span><span class="sxs-lookup"><span data-stu-id="27dfb-134">In the **Posted Return Shipment** window, take a note of the number in the **Return Order No.**</span></span> <span data-ttu-id="27dfb-135">.</span><span class="sxs-lookup"><span data-stu-id="27dfb-135">field.</span></span>  
6.  <span data-ttu-id="27dfb-136">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bestillingsreturer**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="27dfb-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Return Orders**, and then choose the related link.</span></span>  
7.  <span data-ttu-id="27dfb-137">Åpne den aktuelle bestillingsreturen, og velg deretter **Åpne på nytt**.</span><span class="sxs-lookup"><span data-stu-id="27dfb-137">Open the return order in question, and then choose the **Reopen** action.</span></span>  
8.  <span data-ttu-id="27dfb-138">Korriger posten i feltet **Antall** og bokfør bestillingsreturen på nytt.</span><span class="sxs-lookup"><span data-stu-id="27dfb-138">Correct the entry in the **Quantity** field and post the purchase return order again.</span></span>  

## <a name="see-also"></a><span data-ttu-id="27dfb-139">Se også</span><span class="sxs-lookup"><span data-stu-id="27dfb-139">See Also</span></span>
[<span data-ttu-id="27dfb-140">Bokføre transaksjoner direkte i Finans</span><span class="sxs-lookup"><span data-stu-id="27dfb-140">How to: Post Transactions Directly to the General Ledger</span></span>](finance-how-post-transactions-directly.md)  
[<span data-ttu-id="27dfb-141">Arbeide med finanskladder</span><span class="sxs-lookup"><span data-stu-id="27dfb-141">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="27dfb-142">Finans</span><span class="sxs-lookup"><span data-stu-id="27dfb-142">Finance</span></span>](finance.md)  
<span data-ttu-id="27dfb-143">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="27dfb-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

