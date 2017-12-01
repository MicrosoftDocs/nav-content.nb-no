---
title: Eksportere remitteringsoppdrag
description: "Du kan bruke funksjonen for eksport av remitteringsoppdrag til å eksportere betalingsfilen til datamaskinen din."
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
ms.openlocfilehash: e5898959c71984b1436309fa4bd5959fa03c6246
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-export-remittance-payments"></a><span data-ttu-id="2ef7a-103">Eksportere remitteringsoppdrag</span><span class="sxs-lookup"><span data-stu-id="2ef7a-103">How to: Export Remittance Payments</span></span>
<span data-ttu-id="2ef7a-104">Du kan bruke funksjonen for eksport av remitteringsoppdrag til å eksportere betalingsfilen til datamaskinen din.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-104">You can use the export remittance payments process to export the payments file to your computer.</span></span> <span data-ttu-id="2ef7a-105">Deretter kan du overføre remitteringsoppdragene til banken.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-105">You can then transfer the remittance payments to the bank.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="2ef7a-106">Før du kan eksportere et remitteringsoppdrag, må du velge et betalingsformat i feltet **Betalingseksportformat** i **Bankkort**-vinduet.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-106">Before you can export a remittance payment, you must select a payment format in the **Payment Export Format** field in the **Bank Account Card** window.</span></span>  

<span data-ttu-id="2ef7a-107">Du eksporterer betalinger til en bankfil ved å velge **Eksporter betalinger**-knappen i **Utbetalingskladd**-vinduet.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-107">You export payments to a bank file by choosing the **Export Payments** button in the **Payment Journal** window.</span></span> <span data-ttu-id="2ef7a-108">Prosessen kan være forskjellig avhengig av eksportformatet du velger:</span><span class="sxs-lookup"><span data-stu-id="2ef7a-108">The process may be different, depending on the export format that you select:</span></span>  

- <span data-ttu-id="2ef7a-109">Betalinger ved hjelp av SEPA-betalingsstandarden eksporteres direkte til en fil når du velger **Eksporter betalinger**-knappen.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-109">Payments using the SEPA payment standard are directly exported to a file when you choose the **Export Payments** button.</span></span> <span data-ttu-id="2ef7a-110">Hvis du vil ha mer informasjon, kan du se [Utføre betalinger](../../payables-make-payments.md).</span><span class="sxs-lookup"><span data-stu-id="2ef7a-110">For more information, see [Making Payments](../../payables-make-payments.md).</span></span>  

- <span data-ttu-id="2ef7a-111">Betalinger ved hjelp av lokale betalingsstandarder som **Telepay**, eksporteres med enten **Remittering - les ut (bank)**- eller **Remittering - les ut (BBS)**-rapporten som åpnes automatisk når du velger **Eksporter betalinger**-knappen.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-111">Payments using local payment standards, such as **Telepay**, are exported with either the **Remittance - export (bank)** or the **Remittance - export (BBS)** report, which automatically opens when you choose the **Export Payments** button.</span></span>  

<span data-ttu-id="2ef7a-112">Fremgangsmåten for å eksportere betalinger ved hjelp av **Eksporter remittering**-kjørselen beskrives i dette emnet.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-112">The procedure for exporting payments using the **Remittance – Export** batch job is described in this topic.</span></span>  

## <a name="to-export-remittance-payments-using-the-remittance---export-batch-jobs"></a><span data-ttu-id="2ef7a-113">Slik eksporterer du remitteringsoppdrag ved hjelp av Eksporter remittering-kjørsler:</span><span class="sxs-lookup"><span data-stu-id="2ef7a-113">To export remittance payments using the Remittance - Export batch jobs</span></span>  

1.  <span data-ttu-id="2ef7a-114">Velg ikonet ![Søk etter side eller rapport](../../media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Betalingskladder**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-114">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="2ef7a-115">Klargjør for å eksportere betalingene fra kladden.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-115">Prepare to export the payments from the journal.</span></span> <span data-ttu-id="2ef7a-116">Hvis du vil ha mer informasjon, kan du se [Eksportere betalinger til en bankfil](../../payables-how-export-payments-bank-file.md).</span><span class="sxs-lookup"><span data-stu-id="2ef7a-116">For more information, see [How to: Export Payments to a Bank File](../../payables-how-export-payments-bank-file.md).</span></span>  
3.  <span data-ttu-id="2ef7a-117">Velg handlingen **Eksporter betalinger**.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-117">Choose the **Export Payments** action.</span></span>  
4.  <span data-ttu-id="2ef7a-118">Fyll ut feltene som beskrevet i tabellen nedenfor, ved å velge hurtigfanen **Alternativer** i rapportvinduet som åpnes.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-118">In the report window that opens, choose the **Options** FastTab, and fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="2ef7a-119">Felt</span><span class="sxs-lookup"><span data-stu-id="2ef7a-119">Field</span></span>|<span data-ttu-id="2ef7a-120">Description</span><span class="sxs-lookup"><span data-stu-id="2ef7a-120">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="2ef7a-121">**Remitteringsavtalekode**</span><span class="sxs-lookup"><span data-stu-id="2ef7a-121">**Remittance agreement code**</span></span>|<span data-ttu-id="2ef7a-122">Angi koden for avtalen.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-122">Specify the code for the agreement.</span></span>|  
    |<span data-ttu-id="2ef7a-123">**Operator**</span><span class="sxs-lookup"><span data-stu-id="2ef7a-123">**Operator**</span></span>|<span data-ttu-id="2ef7a-124">Angi operatornummer.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-124">Specify the operator number.</span></span>|  
    |<span data-ttu-id="2ef7a-125">**Passord**</span><span class="sxs-lookup"><span data-stu-id="2ef7a-125">**Password**</span></span>|<span data-ttu-id="2ef7a-126">Angi passordet for betalingene.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-126">Specify the password for the payments.</span></span>|  
    |<span data-ttu-id="2ef7a-127">**Divisjon**</span><span class="sxs-lookup"><span data-stu-id="2ef7a-127">**Division**</span></span>|<span data-ttu-id="2ef7a-128">Angi divisjonen som betaler remittering.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-128">Specify the division that is paying remittance.</span></span>|  
    |<span data-ttu-id="2ef7a-129">**Oppdragsbemerkning**</span><span class="sxs-lookup"><span data-stu-id="2ef7a-129">**Current note**</span></span>|<span data-ttu-id="2ef7a-130">Angi en bemerkning for betalingen.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-130">Specify a note for the payment.</span></span>|  
    |<span data-ttu-id="2ef7a-131">**Filnavn**</span><span class="sxs-lookup"><span data-stu-id="2ef7a-131">**Filename**</span></span>|<span data-ttu-id="2ef7a-132">Angi navnet og mappen for betalingsfilen.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-132">Specify the name and directory of the payment file.</span></span>|  

5.  <span data-ttu-id="2ef7a-133">Velg **OK**.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-133">Choose the **OK** button.</span></span>  

<span data-ttu-id="2ef7a-134">Betalingsinformasjonen eksporteres til filen som er angitt i remitteringsavtalen.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-134">The payment information is exported to the file that is set up in the remittance agreement.</span></span>  

<span data-ttu-id="2ef7a-135">Utbetalingskladden slettes og transaksjonene overføres til ventekladden.</span><span class="sxs-lookup"><span data-stu-id="2ef7a-135">The payment journal is deleted and the transactions are transferred to the waiting journal.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2ef7a-136">Se også</span><span class="sxs-lookup"><span data-stu-id="2ef7a-136">See Also</span></span>  
 <span data-ttu-id="2ef7a-137">[Elektroniske betalinger til leverandører i Norge](electronic-payments-to-vendors-in-norway.md) </span><span class="sxs-lookup"><span data-stu-id="2ef7a-137">[Electronic Payments to Vendors in Norway](electronic-payments-to-vendors-in-norway.md) </span></span>  
 <span data-ttu-id="2ef7a-138">[Sette opp remitteringsavtaler](how-to-set-up-remittance-agreements.md) </span><span class="sxs-lookup"><span data-stu-id="2ef7a-138">[How to: Set Up Remittance Agreements](how-to-set-up-remittance-agreements.md) </span></span>  
 <span data-ttu-id="2ef7a-139">[Opprette remitteringskontoer](how-to-create-remittance-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="2ef7a-139">[How to: Create Remittance Accounts](how-to-create-remittance-accounts.md) </span></span>  
 <span data-ttu-id="2ef7a-140">[Angi leverandører for remittering](how-to-set-up-vendors-for-remittance.md) </span><span class="sxs-lookup"><span data-stu-id="2ef7a-140">[How to: Set Up Vendors for Remittance](how-to-set-up-vendors-for-remittance.md) </span></span>  
 <span data-ttu-id="2ef7a-141">[Mottakerreferansekoder](recipient-reference-codes.md) </span><span class="sxs-lookup"><span data-stu-id="2ef7a-141">[Recipient Reference Codes](recipient-reference-codes.md) </span></span>  
 <span data-ttu-id="2ef7a-142">[Opprette remitteringsforslag](how-to-create-remittance-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="2ef7a-142">[How to: Create Remittance Suggestions](how-to-create-remittance-suggestions.md) </span></span>  
 <span data-ttu-id="2ef7a-143">[Opprette manuelle remitteringsoppdrag](how-to-create-manual-remittance-payments.md) </span><span class="sxs-lookup"><span data-stu-id="2ef7a-143">[How to: Create Manual Remittance Payments](how-to-create-manual-remittance-payments.md) </span></span>  
 <span data-ttu-id="2ef7a-144">[Definere betalingslinjeinformasjon](how-to-set-up-payment-line-information.md) </span><span class="sxs-lookup"><span data-stu-id="2ef7a-144">[How to: Set Up Payment Line Information](how-to-set-up-payment-line-information.md) </span></span>  
 <span data-ttu-id="2ef7a-145">[Kontrollere remitteringsoppdrag](how-to-test-remittance-payments.md) </span><span class="sxs-lookup"><span data-stu-id="2ef7a-145">[How to: Test Remittance Payments](how-to-test-remittance-payments.md) </span></span>  
 <span data-ttu-id="2ef7a-146">[Typer betalingsreturfiler](types-of-payment-returns-files.md) </span><span class="sxs-lookup"><span data-stu-id="2ef7a-146">[Types of Payment Returns Files](types-of-payment-returns-files.md) </span></span>  
 <span data-ttu-id="2ef7a-147">[Importere betalingsreturdata](how-to-import-payment-return-data.md) </span><span class="sxs-lookup"><span data-stu-id="2ef7a-147">[How to: Import Payment Return Data](how-to-import-payment-return-data.md) </span></span>  
 <span data-ttu-id="2ef7a-148">[Slette remitteringsoppdrag](how-to-delete-remittance-payment-orders.md) </span><span class="sxs-lookup"><span data-stu-id="2ef7a-148">[How to: Delete Remittance Payment Orders](how-to-delete-remittance-payment-orders.md) </span></span>  
 <span data-ttu-id="2ef7a-149">[Remitteringsfeil](remittance-errors.md) </span><span class="sxs-lookup"><span data-stu-id="2ef7a-149">[Remittance Errors](remittance-errors.md) </span></span>  
 <span data-ttu-id="2ef7a-150">[Vise remitteringsfeilkoder](how-to-view-remittance-error-codes.md) </span><span class="sxs-lookup"><span data-stu-id="2ef7a-150">[How to: View Remittance Error Codes](how-to-view-remittance-error-codes.md) </span></span>  
 [<span data-ttu-id="2ef7a-151">Annullere betalinger</span><span class="sxs-lookup"><span data-stu-id="2ef7a-151">How to: Cancel Payments</span></span>](how-to-cancel-payments.md)

