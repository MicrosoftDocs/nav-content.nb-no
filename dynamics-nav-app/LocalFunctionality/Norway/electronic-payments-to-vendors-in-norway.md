---
title: "Elektroniske betalinger til leverandører i Norge"
description: "Forbedringer i den norske versjonen inkluderer automatisk betaling til leverandører."
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
ms.openlocfilehash: 470514afa654a382e5d7ae883f8414616a2f7537
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="electronic-payments-to-vendors-in-norway"></a><span data-ttu-id="3f4ce-103">Elektroniske betalinger til leverandører i Norge</span><span class="sxs-lookup"><span data-stu-id="3f4ce-103">Electronic Payments to Vendors in Norway</span></span>
[!INCLUDE[navnow](../../includes/navnow_md.md)]<span data-ttu-id="3f4ce-104">inkluderer forbedringer i den norske versjonen for automatisk betaling til leverandører.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-104"> includes Norwegian enhancements for automatically making payments to vendors.</span></span> <span data-ttu-id="3f4ce-105">Dette reduserer sjansen for at feil skal oppstå på grunn av manuell registrering av data.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-105">This reduces errors that occur from manual data entry.</span></span> <span data-ttu-id="3f4ce-106">Denne funksjonaliteten kan brukes til å utføre følgende operasjoner:</span><span class="sxs-lookup"><span data-stu-id="3f4ce-106">You can use this functionality to perform the following operations:</span></span>  

- <span data-ttu-id="3f4ce-107">Søke etter fakturaer som er forfalt, basert på ulike kriterier.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-107">Search invoices that are due based on different conditions.</span></span>  
- <span data-ttu-id="3f4ce-108">Sende betalinger til banken.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-108">Send payments to the bank.</span></span>  
- <span data-ttu-id="3f4ce-109">Motta meldinger fra banken om status for betalinger.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-109">Receive messages from the bank on the status of payments.</span></span>  
- <span data-ttu-id="3f4ce-110">Motta informasjon om betalte transaksjoner som skal bokføres.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-110">Receive paid transaction information to be posted.</span></span>  

<span data-ttu-id="3f4ce-111">Du kan utføre elektroniske betalinger i følgende formater:</span><span class="sxs-lookup"><span data-stu-id="3f4ce-111">You can make electronic payments using the following formats:</span></span>  

- <span data-ttu-id="3f4ce-112">TelePay</span><span class="sxs-lookup"><span data-stu-id="3f4ce-112">TelePay</span></span>  
- <span data-ttu-id="3f4ce-113">Remitteringsoppdrag</span><span class="sxs-lookup"><span data-stu-id="3f4ce-113">Remittance payment</span></span>  

## <a name="electronic-payment-process"></a><span data-ttu-id="3f4ce-114">Elektronisk betalingsprosess</span><span class="sxs-lookup"><span data-stu-id="3f4ce-114">Electronic Payment Process</span></span>  
<span data-ttu-id="3f4ce-115">Elektroniske betalinger behandles på følgende måte:</span><span class="sxs-lookup"><span data-stu-id="3f4ce-115">The following steps show how electronic payments are processed:</span></span>  

1.  <span data-ttu-id="3f4ce-116">Betalingsforslaget kjøres i den elektroniske betalingsfunksjonen og overføres til banken ved hjelp av bankens programvare.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-116">The payment proposal is run in the electronic payments feature and transferred to the bank by using the bank’s software.</span></span>  
2.  <span data-ttu-id="3f4ce-117">Bankens programvare mottar betalingene og overfører dem til banken.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-117">The bank's software receives the payments and transfers payments to the bank.</span></span>  
3.  <span data-ttu-id="3f4ce-118">Banken mottar betalingene og sender den første mottaksreturen til [!INCLUDE[navnow](../../includes/navnow_md.md)] via bankens programvare.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-118">The bank receives the payments and sends the first-time return receipt to [!INCLUDE[navnow](../../includes/navnow_md.md)] using the bank's software.</span></span>  
4.  <span data-ttu-id="3f4ce-119">Banken utfører betalingene og sender avregningsreturen (andre mottaksretur) til [!INCLUDE[navnow](../../includes/navnow_md.md)] via bankens programvare, hvor betalingene bokføres.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-119">The bank executes the payments and sends the settlement return (second-time return receipt) to [!INCLUDE[navnow](../../includes/navnow_md.md)] using the bank's software where the payments are posted.</span></span>  

## <a name="vendor-payment-requirements"></a><span data-ttu-id="3f4ce-120">Krav til leverandørbetalinger</span><span class="sxs-lookup"><span data-stu-id="3f4ce-120">Vendor Payment Requirements</span></span>  
<span data-ttu-id="3f4ce-121">Hvis betalingstransaksjonene ikke oppfyller kravene, vises en feilmelding, og du kan ikke opprette en betalingsfil for overføringer til banken.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-121">If the payment transactions do not fulfill the requirements, an error message appears and you cannot create a payment file for transfers to the bank.</span></span> <span data-ttu-id="3f4ce-122">Følgende kriterier må oppfylles ved når du behandler betalinger til leverandører:</span><span class="sxs-lookup"><span data-stu-id="3f4ce-122">The following criteria must be met when you process payments to vendors:</span></span>  

- <span data-ttu-id="3f4ce-123">Betalingstransaksjonen må være positiv eller null.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-123">The payment transaction must be positive or zero.</span></span> <span data-ttu-id="3f4ce-124">En betalingstransaksjon må overføre et positivt beløp (eller null) til betalingsmottakeren.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-124">A payment transaction must transfer a positive amount (or zero) to the payment receiver.</span></span> <span data-ttu-id="3f4ce-125">Dette betyr at når en kreditnota skal trekkes fra, må fakturaen i samme betalingstransaksjon lyde på det samme eller et høyere beløp.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-125">This means that deducting a credit memo requires an invoice with the same or higher amount in the same payment transaction.</span></span> <span data-ttu-id="3f4ce-126">Det er ikke mulig å trekke fra penger på leverandørens konto.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-126">Money cannot be deducted from the vendor's account.</span></span>  

- <span data-ttu-id="3f4ce-127">Det må anvendes en kreditnota sammen med fakturaen.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-127">A credit memo must be applied with the invoice.</span></span> <span data-ttu-id="3f4ce-128">En kreditnota inneholder vanligvis ikke en Kunde-ID (KID).</span><span class="sxs-lookup"><span data-stu-id="3f4ce-128">Generally a credit memo does not contain a Kunde ID (KID).</span></span> <span data-ttu-id="3f4ce-129">Du kan ikke betale en kreditnota i en betalingstransaksjon med fakturaer som inneholder et KID-nummer.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-129">You cannot pay a credit memo in a payment transaction with invoices that contain a KID.</span></span> <span data-ttu-id="3f4ce-130">Årsaken er at betalinger vanligvis deles opp i transaksjoner med eller uten KID-nummer.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-130">This is because payments are usually split into transactions with or without a KID.</span></span> <span data-ttu-id="3f4ce-131">Det betyr at hvis en kreditnota uten KID-nummer betales sammen med en faktura i samme betalingstransaksjon, må fakturaen betales uten KID-nummer, og mottakerreferansenummeret må brukes i stedet.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-131">This means that if a credit memo without a KID is paid with an invoice in the same payment transaction, the invoice must be paid without a KID, and the recipient reference number must be used instead.</span></span>  

- <span data-ttu-id="3f4ce-132">Hvis fakturaen og kreditnotaen betales i samme betalingstransaksjon, må betalingen finne sted på samme dato, i samme valuta og med samme valutakurs.</span><span class="sxs-lookup"><span data-stu-id="3f4ce-132">If the invoice and credit memo are paid in the same payment transaction, the payment must occur on the same date using the same currency and exchange rate.</span></span>  

## <a name="see-also"></a><span data-ttu-id="3f4ce-133">Se også</span><span class="sxs-lookup"><span data-stu-id="3f4ce-133">See Also</span></span>  
 <span data-ttu-id="3f4ce-134">[Funksjonalitet som er spesifikk for norske brukere](norway-local-functionality.md) </span><span class="sxs-lookup"><span data-stu-id="3f4ce-134">[Norway Local Functionality](norway-local-functionality.md) </span></span>  
 <span data-ttu-id="3f4ce-135">[Sette opp remitteringsavtaler](how-to-set-up-remittance-agreements.md) </span><span class="sxs-lookup"><span data-stu-id="3f4ce-135">[How to: Set Up Remittance Agreements](how-to-set-up-remittance-agreements.md) </span></span>  
 <span data-ttu-id="3f4ce-136">[Opprette remitteringskontoer](how-to-create-remittance-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="3f4ce-136">[How to: Create Remittance Accounts](how-to-create-remittance-accounts.md) </span></span>  
 <span data-ttu-id="3f4ce-137">[Angi leverandører for remittering](how-to-set-up-vendors-for-remittance.md) </span><span class="sxs-lookup"><span data-stu-id="3f4ce-137">[How to: Set Up Vendors for Remittance](how-to-set-up-vendors-for-remittance.md) </span></span>  
 <span data-ttu-id="3f4ce-138">[Mottakerreferansekoder](recipient-reference-codes.md) </span><span class="sxs-lookup"><span data-stu-id="3f4ce-138">[Recipient Reference Codes](recipient-reference-codes.md) </span></span>  
 <span data-ttu-id="3f4ce-139">[Opprette remitteringsforslag](how-to-create-remittance-suggestions.md) </span><span class="sxs-lookup"><span data-stu-id="3f4ce-139">[How to: Create Remittance Suggestions](how-to-create-remittance-suggestions.md) </span></span>  
 <span data-ttu-id="3f4ce-140">[Opprette manuelle remitteringsoppdrag](how-to-create-manual-remittance-payments.md) </span><span class="sxs-lookup"><span data-stu-id="3f4ce-140">[How to: Create Manual Remittance Payments](how-to-create-manual-remittance-payments.md) </span></span>  
 <span data-ttu-id="3f4ce-141">[Definere betalingslinjeinformasjon](how-to-set-up-payment-line-information.md) </span><span class="sxs-lookup"><span data-stu-id="3f4ce-141">[How to: Set Up Payment Line Information](how-to-set-up-payment-line-information.md) </span></span>  
 <span data-ttu-id="3f4ce-142">[Kontrollere remitteringsoppdrag](how-to-test-remittance-payments.md) </span><span class="sxs-lookup"><span data-stu-id="3f4ce-142">[How to: Test Remittance Payments](how-to-test-remittance-payments.md) </span></span>  
 <span data-ttu-id="3f4ce-143">[Eksportere remitteringsoppdrag](how-to-export-remittance-payments.md) </span><span class="sxs-lookup"><span data-stu-id="3f4ce-143">[How to: Export Remittance Payments](how-to-export-remittance-payments.md) </span></span>  
 <span data-ttu-id="3f4ce-144">[Typer betalingsreturfiler](types-of-payment-returns-files.md) </span><span class="sxs-lookup"><span data-stu-id="3f4ce-144">[Types of Payment Returns Files](types-of-payment-returns-files.md) </span></span>  
 <span data-ttu-id="3f4ce-145">[Importere betalingsreturdata](how-to-import-payment-return-data.md) </span><span class="sxs-lookup"><span data-stu-id="3f4ce-145">[How to: Import Payment Return Data](how-to-import-payment-return-data.md) </span></span>  
 <span data-ttu-id="3f4ce-146">[Slette remitteringsoppdrag](how-to-delete-remittance-payment-orders.md) </span><span class="sxs-lookup"><span data-stu-id="3f4ce-146">[How to: Delete Remittance Payment Orders](how-to-delete-remittance-payment-orders.md) </span></span>  
 <span data-ttu-id="3f4ce-147">[Remitteringsfeil](remittance-errors.md) </span><span class="sxs-lookup"><span data-stu-id="3f4ce-147">[Remittance Errors](remittance-errors.md) </span></span>  
 <span data-ttu-id="3f4ce-148">[Vise remitteringsfeilkoder](how-to-view-remittance-error-codes.md) </span><span class="sxs-lookup"><span data-stu-id="3f4ce-148">[How to: View Remittance Error Codes](how-to-view-remittance-error-codes.md) </span></span>  
 [<span data-ttu-id="3f4ce-149">Annullere betalinger</span><span class="sxs-lookup"><span data-stu-id="3f4ce-149">How to: Cancel Payments</span></span>](how-to-cancel-payments.md)

