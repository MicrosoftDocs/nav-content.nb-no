---
title: Arbeide med sjekker
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 421516a7580a90d6eabc8ecfcc841215839994c9
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-checks"></a><span data-ttu-id="803d6-102">Arbeide med sjekker</span><span class="sxs-lookup"><span data-stu-id="803d6-102">How to: Work With Checks</span></span>
<span data-ttu-id="803d6-103">Dynamics NAV støtter elektronisk og manuell utstedelse av sjekker.</span><span class="sxs-lookup"><span data-stu-id="803d6-103">Dynamics NAV supports electronic and manual check issuance.</span></span> <span data-ttu-id="803d6-104">Begge metodene bruker utbetalingskladden til å utstede sjekker til leverandører.</span><span class="sxs-lookup"><span data-stu-id="803d6-104">Both methods use the payment journal to issue checks to vendors.</span></span> <span data-ttu-id="803d6-105">Du kan også kansellere sjekker og vise sjekkposter.</span><span class="sxs-lookup"><span data-stu-id="803d6-105">You can also void checks and view check ledger entries.</span></span>

<span data-ttu-id="803d6-106">Prosessen med å utstede sjekker foreslår utbetalinger, oppretter poster og skriver ut de maskinelle sjekkene.</span><span class="sxs-lookup"><span data-stu-id="803d6-106">The process of issuing checks suggests payments, creates ledger entries, and prints the computer checks.</span></span>

<span data-ttu-id="803d6-107">Skriveren må være riktig konfigurert for sjekkskjemaene, og du må definere hvilke sjekkoppsett som skal brukes.</span><span class="sxs-lookup"><span data-stu-id="803d6-107">Your printer must be correctly set up with the check forms, and you must define which check layout to use.</span></span> <span data-ttu-id="803d6-108">Hvis du vil ha mer informasjon, kan du se [Definere sjekkoppsett](finance-setup-how-define-check-layouts.md)</span><span class="sxs-lookup"><span data-stu-id="803d6-108">For more information, see [How to: Define Check Layouts](finance-setup-how-define-check-layouts.md)</span></span>

## <a name="to-issue-checks"></a><span data-ttu-id="803d6-109">Utstede sjekker</span><span class="sxs-lookup"><span data-stu-id="803d6-109">To issue checks</span></span>
1. <span data-ttu-id="803d6-110">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Betalingskladder** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="803d6-110">In the top right corner, choose the **Search for Page or Report** icon, enter **Payment Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="803d6-111">Fyll ut kladden med relevante betalinger, for eksempel ved hjelp av funksjonen Betalingsforslag - leverandør.</span><span class="sxs-lookup"><span data-stu-id="803d6-111">Fill in the journal with relevant payments, for example by using the Suggest Vendor Payments function.</span></span> <span data-ttu-id="803d6-112">Hvis du vil ha mer informasjon, kan du se [Betalingsforslag - leverandør](payables-how-suggest-vendor-payments.md).</span><span class="sxs-lookup"><span data-stu-id="803d6-112">For more information, see [How to: Suggest Vendor Payments](payables-how-suggest-vendor-payments.md).</span></span>
3. <span data-ttu-id="803d6-113">I **Bankbetalingstype**-feltet på kladdelinjer for betaling som du vil gjøre med sjekker, velger du ett av følgende alternativer:</span><span class="sxs-lookup"><span data-stu-id="803d6-113">In the **Bank Payment Type** field on journal lines for payment that you want to make with checks, select one of the following options:</span></span>

 - <span data-ttu-id="803d6-114">**Maskinell sjekk**: Velg dette alternativet hvis du vil at programmet skal opprette og senere skrive ut en sjekk på beløpet på betalingskladdelinjen.</span><span class="sxs-lookup"><span data-stu-id="803d6-114">**Computer Check**: Select this option if you want to print a check for the amount on the payment journal line.</span></span> <span data-ttu-id="803d6-115">Du må skrive ut sjekkene før du kan bokføre kladdelinjene.</span><span class="sxs-lookup"><span data-stu-id="803d6-115">You must print the checks before you can post the journal lines.</span></span> <span data-ttu-id="803d6-116">Du kan bare velge **Maskinell sjekk** hvis **Motkontotype** eller **Kontotype** er **Bankkonto**.</span><span class="sxs-lookup"><span data-stu-id="803d6-116">You can only select **Computer Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span></span>

 - <span data-ttu-id="803d6-117">**Manuell sjekk**: Velg dette alternativet hvis du manuelt har skrevet en sjekk og vil at programmet skal opprette en tilhørende sjekkpost på dette beløpet.</span><span class="sxs-lookup"><span data-stu-id="803d6-117">**Manual Check**: Select this option if you have created a check manually and want to create a corresponding check ledger entry for this amount.</span></span> <span data-ttu-id="803d6-118">Når du bruker dette alternativet, kan du ikke skrive ut sjekker fra Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="803d6-118">By using this option, you cannot print checks from Dynamics NAV.</span></span> <span data-ttu-id="803d6-119">Du kan bare velge **Manuell sjekk** hvis **Motkontotype** eller **Kontotype** er **Bankkonto**.</span><span class="sxs-lookup"><span data-stu-id="803d6-119">You can only select **Manual Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span></span>

    <span data-ttu-id="803d6-120">**Merk**: Du må skrive ut maskinelle sjekkene før du kan bokføre de relaterte kladdelinjene.</span><span class="sxs-lookup"><span data-stu-id="803d6-120">**Note**: You must print computer checks before you post the related journal lines.</span></span>
4. <span data-ttu-id="803d6-121">Velg **Skriv ut sjekk** for maskinelle sjekker.</span><span class="sxs-lookup"><span data-stu-id="803d6-121">In case of computer checks, choose **Print Check**.</span></span>
5. <span data-ttu-id="803d6-122">Fyll ut feltene etter behov i vinduet **Sjekk**.</span><span class="sxs-lookup"><span data-stu-id="803d6-122">In the **Check** window, fill in the fields as necessary.</span></span> <span data-ttu-id="803d6-123">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="803d6-123">Choose a field to read a short description of the field or link to more information.</span></span>
6. <span data-ttu-id="803d6-124">Velg **Skriv ut**.</span><span class="sxs-lookup"><span data-stu-id="803d6-124">Choose the **Print** button.</span></span>

<span data-ttu-id="803d6-125">**Merk**: Hvis du vil skrive ut sjekker i flere valutaer fra forskjellige bankkonti, må du utføre kjørselen **Skriv ut sjekk** separat for hver enkelt valuta og angi riktig bankkonto.</span><span class="sxs-lookup"><span data-stu-id="803d6-125">**Note**: If you want to print checks in more than one currency from different bank accounts, you must run the **Print Check** batch job separately for each currency and specify the appropriate bank account.</span></span>

## <a name="to-cancel-printed-checks-that-are-not-posted"></a><span data-ttu-id="803d6-126">Kansellere utskrevne sjekker som ikke er bokført</span><span class="sxs-lookup"><span data-stu-id="803d6-126">To cancel printed checks that are not posted</span></span>
<span data-ttu-id="803d6-127">Du kan kansellere ikke-bokførte sjekker etter at de er skrevet ut, ved hjelp av handlingen **Kanseller sjekk** i vinduet **Betalingskladd**.</span><span class="sxs-lookup"><span data-stu-id="803d6-127">You can cancel non-posted checks after they have been printed by using the **Void Check** action in the **Payment Journal** window.</span></span>
1. <span data-ttu-id="803d6-128">I vinduet **Betalingskladd** velger du **Kanseller sjekk**, og deretter velger du hvilke sjekker som skal kanselleres.</span><span class="sxs-lookup"><span data-stu-id="803d6-128">In the **Payment Journal** window, choose the **Void Check**, and then choose which checks to cancel.</span></span>

## <a name="to-void-checks"></a><span data-ttu-id="803d6-129">Kansellere sjekker</span><span class="sxs-lookup"><span data-stu-id="803d6-129">To void checks</span></span>
<span data-ttu-id="803d6-130">Når sjekkbetaliner er bokført, kan du bare kansellere (void) sjekker fra de resulterende bankpostene.</span><span class="sxs-lookup"><span data-stu-id="803d6-130">When check payment have been posted, you can only cancel (void) checks from the resulting bank ledger entries.</span></span>

1. <span data-ttu-id="803d6-131">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Bankkonti** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="803d6-131">In the top right corner, choose the **Search for Page or Report** icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="803d6-132">Velg relevant bankkonto, velg handlingene **Rediger** og **Sjekkposter**.</span><span class="sxs-lookup"><span data-stu-id="803d6-132">Select the relevant bank account, choose the **Edit** action, and then choose the **Check Ledger Entries** action.</span></span>
3. <span data-ttu-id="803d6-133">I vinduet **Sjekkposter** velger du handlingen **Kanseller sjekk**.</span><span class="sxs-lookup"><span data-stu-id="803d6-133">In the **Check Ledger Entries** window, choose the **Void Check** action.</span></span>
4. <span data-ttu-id="803d6-134">Merk av for **Kanseller sjekk**.</span><span class="sxs-lookup"><span data-stu-id="803d6-134">Select the **Void Check Only** check box.</span></span>
5. <span data-ttu-id="803d6-135">Velg **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="803d6-135">Choose the **OK**button.</span></span>

## <a name="see-also"></a><span data-ttu-id="803d6-136">Se også</span><span class="sxs-lookup"><span data-stu-id="803d6-136">See Also</span></span>
[<span data-ttu-id="803d6-137">Administrere skyldige beløp</span><span class="sxs-lookup"><span data-stu-id="803d6-137">Manage Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="803d6-138">Definere bankvesen</span><span class="sxs-lookup"><span data-stu-id="803d6-138">Set Up Banking</span></span>](bank-setup-banking.md)  

