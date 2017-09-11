---
title: "Foreslå leverandørbetalinger"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 3ede5942798e34fd0e4b3ab8cc48ca94eed3d1a4
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-suggest-vendor-payments"></a><span data-ttu-id="7784f-102">Foreslå leverandørbetalinger</span><span class="sxs-lookup"><span data-stu-id="7784f-102">How to: Suggest Vendor Payments</span></span>
<span data-ttu-id="7784f-103">I vinduet **Betalingskladd** kan du bruke en funksjon til å foreslå betalingslinjer i henhold til dine innstillinger, for eksempel betalinger som forfaller snart eller betalinger der kontantrabatt er tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="7784f-103">In the **Payment Journal** window, you can use a function to suggest payment lines according to your settings, such as payments that are due soon or payments where a payment discount is available.</span></span>

<span data-ttu-id="7784f-104">Hvis du vil dra full nytte funksjonen Betalingsforslag - leverandør, må du først prioritere leverandørene.</span><span class="sxs-lookup"><span data-stu-id="7784f-104">To benefit fully from the Suggest Vendor Payments function, you must first prioritize your vendors.</span></span> <span data-ttu-id="7784f-105">Hvis du vil ha mer informasjon, kan du se [Prioritere leverandører](purchasing-how-prioritize-vendors.md).</span><span class="sxs-lookup"><span data-stu-id="7784f-105">For more information, see [How to: Prioritize Vendors](purchasing-how-prioritize-vendors.md).</span></span>

<span data-ttu-id="7784f-106">Leverandørposter som er merket med **Avvent** tas ikke med i kjørselen.</span><span class="sxs-lookup"><span data-stu-id="7784f-106">Vendor entries that are not marked **On Hold** are not included in the batch job.</span></span>  

<span data-ttu-id="7784f-107">**Viktig**: Hvis du vil dra nytte av kontantrabatter og få angitt et disponibelt beløp, brukes beløpet først til prioriterte forfalte leverandørposter i prioritetsrekkefølge, deretter til forfalte leverandørposter som ikke er prioritert, og til slutt til åpne leverandørposter med rett til kontantrabatter, sortert etter leverandørnummer.</span><span class="sxs-lookup"><span data-stu-id="7784f-107">**Important**: If you want to take advantage of payment discounts and have entered an available amount, the amount will be used for prioritized overdue vendor entries first in order of priority, and then for overdue vendor entries that are not prioritized, and finally for open vendor entries that qualify for payment discounts in order of vendor number.</span></span>

## <a name="to-use-the-suggest-vendor-payments-function"></a><span data-ttu-id="7784f-108">Bruke funksjonen Betalingsforslag - leverandør</span><span class="sxs-lookup"><span data-stu-id="7784f-108">To use the Suggest Vendor Payments function</span></span>
1. <span data-ttu-id="7784f-109">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Betalingskladder** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="7784f-109">In the top right corner, choose the **Search for Page or Report** icon, enter **Payment Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="7784f-110">Åpne den aktuelle kladden, og velg deretter handlingen **Betalingsforslag - leverandør**.</span><span class="sxs-lookup"><span data-stu-id="7784f-110">Open the relevant journal, and then choose the **Suggest Vendor Payments** action.</span></span>
3. <span data-ttu-id="7784f-111">Fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="7784f-111">Fill in the fields as necessary.</span></span> <span data-ttu-id="7784f-112">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="7784f-112">Choose a field to read a short description of the field or link to more information.</span></span>
4. <span data-ttu-id="7784f-113">Velg **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="7784f-113">Choose the **OK** button.</span></span>

## <a name="to-insert-the-due-date-as-posting-date-on-payment-journal-lines"></a><span data-ttu-id="7784f-114">Sette inn forfallsdato som bokføringsdato på betalingskladdelinjer</span><span class="sxs-lookup"><span data-stu-id="7784f-114">To insert the due date as posting date on payment journal lines</span></span>
<span data-ttu-id="7784f-115">Når du bruker kjørselen **Betalingsforslag - leverandør** til å opprette betalingslinjer for leverandørene, kan du fylle ut to spesialfelt for å sikre at de genererte linjene bruker forfallsdatoen til å beregne bokføringsdatoen.</span><span class="sxs-lookup"><span data-stu-id="7784f-115">When you use the **Suggest Vendor Payments** batch job to create payment lines for your vendors, you can fill two special fields to make sure that the generated lines use the due date to calculate the posting date.</span></span> <span data-ttu-id="7784f-116">Disse feltene er **Beregn bokføringsdato fra forfallsdato for utligningsbilag** og **Forskyvning av forfallsdato for utligningsbilag**.</span><span class="sxs-lookup"><span data-stu-id="7784f-116">These fields are **Calculate Posting Date from Applies-to-Doc Due Date** and **Applies-to-Doc Due Date Offset**.</span></span>

<span data-ttu-id="7784f-117">**Viktig**: Du kan ikke bruke feltet **Beregn bokføringsdato fra forfallsdato for utligningsbilag** sammen med feltet **Søk etter kontantrabatter** eller feltet **Summer per leverandør**.</span><span class="sxs-lookup"><span data-stu-id="7784f-117">**Important**: You cannot use the **Calculate Posting Date from Applies-to-Doc Due Date** field together with the **Find Payment Discounts** field or the **Summarize per Vendor** field.</span></span> <span data-ttu-id="7784f-118">Årsaken er at hvis bokføringsdatoen er basert på forfallsdatoen, kan det hende at en del kontantrabatt ikke beregnes på riktig måte, fordi bokføringsdatoen kan komme etter kontantrabattdatoen.</span><span class="sxs-lookup"><span data-stu-id="7784f-118">The reason is that if the posting date is based on the due date, then some payment discount may not be calculated correctly, because the posting date could occur after the payment discount date.</span></span>
<span data-ttu-id="7784f-119">Hvis den beregnede bokføringsdatoen er passert, vil bokføringsdatoen også bli flyttet til arbeidsdatoen og det vil vises en advarsel.</span><span class="sxs-lookup"><span data-stu-id="7784f-119">Also, if the calculated posting date occurs in the past, then the posting date will be moved up to the work date, and a warning is displayed.</span></span>

<span data-ttu-id="7784f-120">Du kan også opprette betalingslinjer manuelt ved å bruke forfallsdatoen til å beregne bokføringsdatoen.</span><span class="sxs-lookup"><span data-stu-id="7784f-120">Alternatively, you can also manually create payment lines using the due date to calculate the posting date.</span></span> <span data-ttu-id="7784f-121">Når du har utlignet leverandørposter, kan du bruke handlingen **Beregn bokføringsdato**.</span><span class="sxs-lookup"><span data-stu-id="7784f-121">After you have applied vendor ledger entries, you can use the **Calculate Posting Date** action.</span></span> <span data-ttu-id="7784f-122">Dett vil oppdatere bokføringsdatoen på kladdelinjen med forfallsdatoen for den tilknyttede kjøpsfakturaen.</span><span class="sxs-lookup"><span data-stu-id="7784f-122">This will update the posting date on the journal line with the due date of the related purchase invoice.</span></span> <span data-ttu-id="7784f-123">Hvis du vil ha mer informasjon, kan du se [Utligne kjøpstransaksjoner manuelt](payables-how-apply-purchase-transactions-manually.md).</span><span class="sxs-lookup"><span data-stu-id="7784f-123">For more information, see [How to: Apply Purchase Transactions Manually](payables-how-apply-purchase-transactions-manually.md).</span></span>  

<span data-ttu-id="7784f-124">**Merk**: Hvis kjøpsfakturaen er forfalt, vil bokføringsdatoen bli satt til arbeidsdatoen, og skriftfargen på linjen endres til rød.</span><span class="sxs-lookup"><span data-stu-id="7784f-124">**Note**: If the purchase invoice is overdue, then the posting date will be set to the work date, and the font on the line will change to red color.</span></span>

## <a name="see-also"></a><span data-ttu-id="7784f-125">Se også</span><span class="sxs-lookup"><span data-stu-id="7784f-125">See Also</span></span>
[<span data-ttu-id="7784f-126">Administrere skyldige beløp</span><span class="sxs-lookup"><span data-stu-id="7784f-126">Manage Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="7784f-127">Foreta betalinger</span><span class="sxs-lookup"><span data-stu-id="7784f-127">Make Payments</span></span>](payables-make-payments.md)  
[<span data-ttu-id="7784f-128">Arbeide med finanskladder</span><span class="sxs-lookup"><span data-stu-id="7784f-128">Work with General Journals</span></span>](ui-work-general-journals.md)

