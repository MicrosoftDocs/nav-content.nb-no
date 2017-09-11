---
title: Avslutte perioder
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: ac1ed2d1dcf8bf780bda91fbf0a04e5c5e8d106a
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---
# <a name="close-periods"></a><span data-ttu-id="1c833-102">Avslutte perioder</span><span class="sxs-lookup"><span data-stu-id="1c833-102">Close Periods</span></span>
<span data-ttu-id="1c833-103">Programmet tvinger deg ikke til å avslutte perioder, men det finnes imidlertid mange aktiviteter for periodeslutt (månedsslutt) som kan utføres i programmet hvis du vil.</span><span class="sxs-lookup"><span data-stu-id="1c833-103">The application does not force you to close periods, however, there are many period-end (month-end) activities that can be performed in the application if you want.</span></span> <span data-ttu-id="1c833-104">Dette emnet inneholder en oversikt over disse prosessene og aktivitetene, som er eller ikke er nødvendig for selskapet.</span><span class="sxs-lookup"><span data-stu-id="1c833-104">This topic provides an overview of these processes and activities, which may or may not be necessary for your company.</span></span>

## <a name="general-ledger"></a><span data-ttu-id="1c833-105">Finans</span><span class="sxs-lookup"><span data-stu-id="1c833-105">General Ledger</span></span>
* <span data-ttu-id="1c833-106">Angi systemomfattende og brukerspesifikke bokføringsperioder.</span><span class="sxs-lookup"><span data-stu-id="1c833-106">Specify system-wide and user-specific posting period.</span></span>

    <span data-ttu-id="1c833-107">Dette angir datoene som bokføringer som er tillatt mellom.</span><span class="sxs-lookup"><span data-stu-id="1c833-107">This specifies the dates between which postings are allowed.</span></span> <span data-ttu-id="1c833-108">Avhengig av forretningsbehovene vil du kanskje begrense brukerens bokføringsdatoområder i begynnelsen av prosessen ved periodeslutt eller senere mot slutten av perioden.</span><span class="sxs-lookup"><span data-stu-id="1c833-108">Depending on your business needs, you may want to restrict user posting date ranges at the start of the period-end process or at later time towards the end of the period.</span></span> <span data-ttu-id="1c833-109">Hvis du vil ha mer informasjon, kan du se [Angi bokføringsperioder](finance-setup-how-specify-posting-periods.md).</span><span class="sxs-lookup"><span data-stu-id="1c833-109">For more information, see [How to: Specify Posting Periods](finance-setup-how-specify-posting-periods.md).</span></span>
* <span data-ttu-id="1c833-110">Foreta alle nødvendige finansjusteringer.</span><span class="sxs-lookup"><span data-stu-id="1c833-110">Make all necessary G/L adjustments.</span></span>
* <span data-ttu-id="1c833-111">Oppdater og bokfør gjentakelseskladder.</span><span class="sxs-lookup"><span data-stu-id="1c833-111">Update and post Recurring Journals.</span></span>
<!--* Process Consolidations-->
* <span data-ttu-id="1c833-112">Kjør kontoskjemaer som følger:</span><span class="sxs-lookup"><span data-stu-id="1c833-112">Run account schedules as follows:</span></span>
  1. <span data-ttu-id="1c833-113">Åpne **Kontoskjema**-vinduet, og klikk handlingen **Skriv ut**.</span><span class="sxs-lookup"><span data-stu-id="1c833-113">Open the **Account Schedule** window, and choose the **Print** action.</span></span>
  2. <span data-ttu-id="1c833-114">Fyll ut **Kontoskjema**-forespørselen, og velg handlingen **Skriv ut**.</span><span class="sxs-lookup"><span data-stu-id="1c833-114">Fill the **Account Schedule** request window and choose the **Print** action.</span></span>

## <a name="sales--receivables"></a><span data-ttu-id="1c833-115">Salg</span><span class="sxs-lookup"><span data-stu-id="1c833-115">Sales & Receivables</span></span>
* <span data-ttu-id="1c833-116">Bokfør alle ordrer, fakturaer, kreditnotaer og ordrereturer.</span><span class="sxs-lookup"><span data-stu-id="1c833-116">Post all sales orders, invoices, credit memos, and return orders.</span></span>
* <span data-ttu-id="1c833-117">Bokfør alle innbetalingskladder.</span><span class="sxs-lookup"><span data-stu-id="1c833-117">Post all cash receipt journals.</span></span>
* <span data-ttu-id="1c833-118">Oppdater og bokfør gjentakelseskladder som er relatert til salg.</span><span class="sxs-lookup"><span data-stu-id="1c833-118">Update and post recurring journals that are related to Sales & Receivables.</span></span>
* <span data-ttu-id="1c833-119">Avstem kortsiktige fordringer mot Finans.</span><span class="sxs-lookup"><span data-stu-id="1c833-119">Reconcile accounts receivable to the general ledger.</span></span>
* <span data-ttu-id="1c833-120">Kjør kjørselen **Slett fakturerte ordrer**.</span><span class="sxs-lookup"><span data-stu-id="1c833-120">Run the **Delete Invoiced Sales Orders** batch job.</span></span>

## <a name="purchases--payables"></a><span data-ttu-id="1c833-121">Kjøp</span><span class="sxs-lookup"><span data-stu-id="1c833-121">Purchases & Payables</span></span>
* <span data-ttu-id="1c833-122">Bokfør alle bestillinger, fakturaer, kreditnotaer og ordrereturer.</span><span class="sxs-lookup"><span data-stu-id="1c833-122">Post all purchase orders, invoices, credit memos, and return orders.</span></span>
* <span data-ttu-id="1c833-123">Bokfør alle utbetalingskladder.</span><span class="sxs-lookup"><span data-stu-id="1c833-123">Post all payment journals.</span></span>
* <span data-ttu-id="1c833-124">Oppdater og bokfør gjentakelseskladder som er relatert til kjøp.</span><span class="sxs-lookup"><span data-stu-id="1c833-124">Update and post recurring journals that are related to purchases & payables.</span></span>
* <span data-ttu-id="1c833-125">Kjør rapporten **Aldersfordelt saldoliste - lev.**, og avstem leverandørgjeld mot Finans.</span><span class="sxs-lookup"><span data-stu-id="1c833-125">Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.</span></span>
* <span data-ttu-id="1c833-126">Kjør kjørselen **Slett fakturerte bestillinger**.</span><span class="sxs-lookup"><span data-stu-id="1c833-126">Run the **Delete Invoiced Purchase Orders** batch job.</span></span>

<!-- ### Fixed Assets
* Post all maintenance costs have been posted through the fixed asset journals or invoices.
* Post adjustments.
* Post appreciation.
* Post depreciation.
* Update and post the recurring fixed asset journal.-->

<!--### Intercompany
* Process Intercompany Postings.-->

## <a name="calculate-and-process-sales-tax"></a><span data-ttu-id="1c833-127">Beregn og behandle mva.</span><span class="sxs-lookup"><span data-stu-id="1c833-127">Calculate and Process Sales Tax</span></span>
*  <span data-ttu-id="1c833-128">Fullfør mva-oppgaver.</span><span class="sxs-lookup"><span data-stu-id="1c833-128">Complete Tax Statements.</span></span>

## <a name="see-also"></a><span data-ttu-id="1c833-129">Se også</span><span class="sxs-lookup"><span data-stu-id="1c833-129">See Also</span></span>
[<span data-ttu-id="1c833-130">Avslutt år og perioder</span><span class="sxs-lookup"><span data-stu-id="1c833-130">Closing Years and Periods</span></span>](year-close-years-periods.md)  
[<span data-ttu-id="1c833-131">Lukk bøker</span><span class="sxs-lookup"><span data-stu-id="1c833-131">Close Books</span></span>](year-close-books.md)

