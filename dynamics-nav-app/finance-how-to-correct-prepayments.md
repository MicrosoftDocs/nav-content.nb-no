---
title: Korrigere forskudd
description: "Du kan foreta en korrigering i en ordre etter at du har bokført en forskuddsfaktura for ordren. Du kan legge til nye linjer på en ordre etter at du har utstedt et forskudd, og deretter kan du bokføre en ny forskuddsfaktura, men du kan ikke slette en linje fra en ordre etter at et forskudd er fakturert for linjen."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c39223940880514f9a59eae96e88182e19db2b5e
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-correct-prepayments"></a><span data-ttu-id="754f1-104">Korrigere forskudd</span><span class="sxs-lookup"><span data-stu-id="754f1-104">How to: Correct Prepayments</span></span>
<span data-ttu-id="754f1-105">Du kan foreta en korrigering i en ordre etter at du har bokført en forskuddsfaktura for ordren.</span><span class="sxs-lookup"><span data-stu-id="754f1-105">You can make a correction to an order after you have posted a prepayment invoice for the order.</span></span> <span data-ttu-id="754f1-106">Du kan legge til nye linjer på en ordre etter at du har utstedt et forskudd, og deretter kan du bokføre en ny forskuddsfaktura, men du kan ikke slette en linje fra en ordre etter at et forskudd er fakturert for linjen.</span><span class="sxs-lookup"><span data-stu-id="754f1-106">You can add new lines to an order after issuing a prepayment, and then you can post another prepayment invoice, but you cannot delete a line from an order after a prepayment has been invoiced for the line.</span></span>  

## <a name="to-correct-a-prepayment"></a><span data-ttu-id="754f1-107">Slik korrigerer du et forskudd</span><span class="sxs-lookup"><span data-stu-id="754f1-107">To correct a prepayment</span></span>
<span data-ttu-id="754f1-108">Følgende fremgangsmåte viser hvordan du utsteder en forskuddskreditnota som kansellerer alle fakturerte forskudd for en ordre.</span><span class="sxs-lookup"><span data-stu-id="754f1-108">The following procedure shows how to issue a prepayment credit memo to cancel all invoiced prepayments for a sales order.</span></span>  
1. <span data-ttu-id="754f1-109">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Ordrer**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="754f1-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="754f1-110">Åpne den aktuelle ordren.</span><span class="sxs-lookup"><span data-stu-id="754f1-110">Open the relevant sales order.</span></span>
3. <span data-ttu-id="754f1-111">Velg **Forskuddsbetaling**, og velg deretter **Bokfør kreditnota for forskudd** eller **Bokfør og skriv ut forskuddsfaktura**.</span><span class="sxs-lookup"><span data-stu-id="754f1-111">Choose the **Prepayment** action, and then choose the **Post Prepayment Credit Memo** action or the **Post and Print Prepmt. Cr. Memo** action.</span></span>  
4. <span data-ttu-id="754f1-112">I vinduet **Salgskreditnota** fortsette med å korrigere de aktuelle postene, for en salgskreditnota.</span><span class="sxs-lookup"><span data-stu-id="754f1-112">In the **Sales Credit Memo** window, proceed to correct the relevant entries, as for any sales credit memo.</span></span> <span data-ttu-id="754f1-113">Hvis du vil ha mer informasjon, kan du se [Behandle ordrereturer eller annulleringer](sales-how-process-sales-returns-cancellations.md).</span><span class="sxs-lookup"><span data-stu-id="754f1-113">For more information, see [How to: Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).</span></span>     

    > [!NOTE]  
    > <span data-ttu-id="754f1-114">For å redusere beløpet i **Linjebeløp**-feltet må du først øke forskuddsprosenten på linjen slik at verdien i feltet **Linjebeløp for forskudd** ikke blir lavere enn verdien i feltet **Fakturert forskuddsbeløp**.</span><span class="sxs-lookup"><span data-stu-id="754f1-114">To Reduce the amount in the **Line Amount** field, you must first increase the prepayment percentage on the line so that the value in the **Prepmt. Line Amount** field is not decreased below the value in the **Prepmt. Amt. Inv.** field.</span></span>

5. <span data-ttu-id="754f1-115">Når du skal opprette en forskuddsfaktura for nye linjer i en salgskreditnota, velger du **Forskuddsbetaling** og velger deretter **Bokfør forskuddsfaktura** eller **Bokfør og skriv ut forskuddsfaktura**.</span><span class="sxs-lookup"><span data-stu-id="754f1-115">To make a prepayment invoice for any new lines in the sales credit memo, choose the **Prepayment** action, and then choose the **Post Prepayment Invoice** action or the **Post and Print Prepmt. Invoice** action.</span></span>  
6. <span data-ttu-id="754f1-116">Du kan utstede en ny forskuddsfaktura ved å øke forskuddsbeløpet på én eller flere linjer og bokføre forskuddsfakturaen.</span><span class="sxs-lookup"><span data-stu-id="754f1-116">To issue an additional prepayment invoice, increase the prepayment amount on one or more lines and post the prepayment invoice.</span></span> <span data-ttu-id="754f1-117">Det opprettes en ny faktura for differansen mellom forskuddsbeløpene som er fakturert, og de nye forskuddsbeløpene.</span><span class="sxs-lookup"><span data-stu-id="754f1-117">A new invoice will be created for the difference between the prepayment amounts invoiced and the new prepayment amounts.</span></span>  

## <a name="see-also"></a><span data-ttu-id="754f1-118">Se også</span><span class="sxs-lookup"><span data-stu-id="754f1-118">See Also</span></span>  
[<span data-ttu-id="754f1-119">Fakturere forskuddsbetalinger</span><span class="sxs-lookup"><span data-stu-id="754f1-119">Invoicing Prepayments</span></span>](finance-invoice-prepayments.md)  
[<span data-ttu-id="754f1-120">Gjennomgang: konfigurere og fakturere salgsforskudd</span><span class="sxs-lookup"><span data-stu-id="754f1-120">Walkthrough: Setting Up and Invoicing Sales Prepayments</span></span>](walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
[<span data-ttu-id="754f1-121">Finans</span><span class="sxs-lookup"><span data-stu-id="754f1-121">Finance</span></span>](finance.md)  
<span data-ttu-id="754f1-122">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="754f1-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

