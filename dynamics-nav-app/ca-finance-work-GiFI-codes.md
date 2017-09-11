---
title: Arbeide med GIFI-koder i Canada
author: SorenGP
ms.custom: na
ms.date: 09/21/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 695bca0a6836c47610210b759ae48af27484761f
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

#<a name="how-to-work-with-gifi-codes-in-canada"></a><span data-ttu-id="748e8-102">Arbeide med GIFI-koder i Canada</span><span class="sxs-lookup"><span data-stu-id="748e8-102">How to: Work With GIFI Codes in Canada</span></span>
<span data-ttu-id="748e8-103">Økonomiske informasjonen kan inkludere finanskontoer, rapporter, resultatregnskap, balanse og kontoutdrag for fri egenkapital.</span><span class="sxs-lookup"><span data-stu-id="748e8-103">Fiscal information can include general ledger accounts, reports, income statements, balance sheets, and statements of retained earnings.</span></span> <span data-ttu-id="748e8-104">Økonomisk informasjon klassifiseres ved hjelp av koder.</span><span class="sxs-lookup"><span data-stu-id="748e8-104">Fiscal information is classified using codes.</span></span> <span data-ttu-id="748e8-105">Bruken av koder lar myndighetene behandle informasjon, klargjøre for elektronisk lagring og validere mva-informasjon elektronisk.</span><span class="sxs-lookup"><span data-stu-id="748e8-105">The use of codes helps the government to process information, prepare for electronic filing, and validate tax information electronically.</span></span> <span data-ttu-id="748e8-106">Bruken av koder bidrar også til at statistiske organisasjoner kan arbeide mer effektivt. Økonomiske opplysninger er for eksempel lettere tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="748e8-106">The use of codes also helps statistical organizations to work more efficiently, as financial information is more readily available.</span></span> <span data-ttu-id="748e8-107">Hvis du vil ha mer informasjon, kan du se [nettstedet for CRA](http://www.cra-arc.gc.ca/).</span><span class="sxs-lookup"><span data-stu-id="748e8-107">For more information, see the [Canada Revenue Agency website](http://www.cra-arc.gc.ca/).</span></span>

<span data-ttu-id="748e8-108">CRA bruker GIFI-koder (General Index of Financial Information) til å innhente, validere og behandle elektronisk økonomiske opplysninger og mva-informasjon.</span><span class="sxs-lookup"><span data-stu-id="748e8-108">The Canada Revenue Agency uses General Index of Financial Information (GIFI) codes to collect, validate, and process financial and tax information electronically.</span></span> <span data-ttu-id="748e8-109">Anbefalt fremgangsmåte er å tilordne GIFI-koder bare til bokføringskonti, slik at alle summeringer gjøres av din programvare for mva-klargjøring.</span><span class="sxs-lookup"><span data-stu-id="748e8-109">It is a best practice to assign GIFI codes only to posting accounts, so that all totaling is done by your tax preparation software.</span></span>

<span data-ttu-id="748e8-110">Når en konto tilknyttes en GIFI-kode, rapporteres den til skattemyndighetene under denne koden.</span><span class="sxs-lookup"><span data-stu-id="748e8-110">When an account is associated with a GIFI code, it is reported to the revenue agency under that code.</span></span> <span data-ttu-id="748e8-111">Flere konti kan alle ha samme GIFI-kode, men hver konto kan ha bare én GIFI-kode.</span><span class="sxs-lookup"><span data-stu-id="748e8-111">Multiple accounts can all have the same GIFI code, but each account can have only one GIFI code.</span></span>

<span data-ttu-id="748e8-112">Du kan eksportere saldoinformasjon etter GIFI-kode og lagre den eksporterte filen i Excel, noe som er nyttig for overføring av informasjon til din programvare for mva-klargjøring.</span><span class="sxs-lookup"><span data-stu-id="748e8-112">You can export balance information by GIFI code and save the exported file in Excel, which is useful for transferring information to your tax preparation software.</span></span>

## <a name="to-set-up-gifi-codes"></a><span data-ttu-id="748e8-113">Definere GIFI-koder</span><span class="sxs-lookup"><span data-stu-id="748e8-113">To set up GIFI codes</span></span>
<span data-ttu-id="748e8-114">I Dynamics NAV må du definere GIFI-koder for finanskontoer, rapporter, balanse, resultatregnskap og utdrag for fri egenkapital.</span><span class="sxs-lookup"><span data-stu-id="748e8-114">In Dynamics NAV, you must set up GIFI codes for general ledger accounts, reports, balance sheets, income sheets, and statements of retained earnings.</span></span>

1. <span data-ttu-id="748e8-115">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **GIFI-koder** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="748e8-115">In the top right corner, choose the **Search for Page or Report** icon, enter **GIFI Codes**, and then choose the related link.</span></span>
2. <span data-ttu-id="748e8-116">I vinduet **GIFI-koder** velger du handlingen **Ny**.</span><span class="sxs-lookup"><span data-stu-id="748e8-116">In the **GIFI Codes** window, choose the **New** action.</span></span>
3. <span data-ttu-id="748e8-117">Definer GIFI-koder ved å fylle ut feltene.</span><span class="sxs-lookup"><span data-stu-id="748e8-117">Set up GIFI codes by filling the fields.</span></span> <span data-ttu-id="748e8-118">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="748e8-118">Choose a field to read a short description of the field or link to more information.</span></span>

## <a name="to-associate-gifi-codes-with-gl-accounts"></a><span data-ttu-id="748e8-119">Knytte GIFI-koder til finanskonti</span><span class="sxs-lookup"><span data-stu-id="748e8-119">To associate GIFI codes with G/L accounts</span></span>
<span data-ttu-id="748e8-120">Hvis du vil rapportere økonomiske opplysninger, må hver GIFI-kode være tilknyttet de aktuelle kontoene i kontoplanen.</span><span class="sxs-lookup"><span data-stu-id="748e8-120">To report financial information by GIFI code, each GIFI code must be associated with the appropriate accounts in the chart of accounts.</span></span>

1. <span data-ttu-id="748e8-121">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kontoplan** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="748e8-121">In the top right corner, choose the **Search for Page or Report** icon, enter **Chart of Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="748e8-122">Velg en relevant finanskonto, og velg deretter handlingen **Rediger**.</span><span class="sxs-lookup"><span data-stu-id="748e8-122">Select a relevant general ledger account, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="748e8-123">I hurtigfanen **Kostregnskap**, i **GIFI-kode**-feltet , velger du en passende GIFI-kode.</span><span class="sxs-lookup"><span data-stu-id="748e8-123">On the **Cost Accounting** FastTab, in the **GIFI Code** field, select an appropriate GIFI code.</span></span>

## <a name="to-view-account-balances-using-the-gifi-code-report"></a><span data-ttu-id="748e8-124">Vise kontosaldoer ved hjelp av GIFI-koderapporten</span><span class="sxs-lookup"><span data-stu-id="748e8-124">To view account balances using the GIFI code report</span></span>
<span data-ttu-id="748e8-125">Du kan se gjennom kontosaldoene etter GIFI-kode ved hjelp av rapporten **Kontosaldoer etter GIFI-koder**.</span><span class="sxs-lookup"><span data-stu-id="748e8-125">You can review your account balances by GIFI code by using the **Account Balances by GIFI Code** report.</span></span>

1. <span data-ttu-id="748e8-126">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kontosaldoer etter GIFI-kode** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="748e8-126">In the top right corner, choose the **Search for Page or Report** icon, enter **Account Balances by GIFI Code**, and then choose the related link.</span></span>
2. <span data-ttu-id="748e8-127">Angi hva du vil inkludere i rapporten ved å fylle ut feltene.</span><span class="sxs-lookup"><span data-stu-id="748e8-127">Specify what to include in the report by filling the fields.</span></span> <span data-ttu-id="748e8-128">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="748e8-128">Choose a field to read a short description of the field or link to more information.</span></span>
3. <span data-ttu-id="748e8-129">Velg knappen **Skriv ut** eller **Forhåndsvisning**.</span><span class="sxs-lookup"><span data-stu-id="748e8-129">Choose the **Print** or the **Preview** button.</span></span>

## <a name="to-export-balance-information-using-gifi-codes"></a><span data-ttu-id="748e8-130">Eksportere saldoinformasjon ved hjelp av GIFI-koder</span><span class="sxs-lookup"><span data-stu-id="748e8-130">To export balance information using GIFI codes</span></span>
<span data-ttu-id="748e8-131">Du kan eksportere saldoinformasjon ved hjelp av GIFI-koder, og lagre den eksporterte filen i Excel.</span><span class="sxs-lookup"><span data-stu-id="748e8-131">You can export balance information using GIFI codes and save the exported file in Excel.</span></span> <span data-ttu-id="748e8-132">Du kan endre, lagre eller slette filen.</span><span class="sxs-lookup"><span data-stu-id="748e8-132">You can modify, save, or delete the file.</span></span> <span data-ttu-id="748e8-133">Du kan bruke filen til å overføre informasjon til din programvare for mva-klargjøring.</span><span class="sxs-lookup"><span data-stu-id="748e8-133">You can use the file to transfer information to your tax preparation software.</span></span>

1. <span data-ttu-id="748e8-134">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Eksporter GIFI-informasjon til Excel** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="748e8-134">In the top right corner, choose the **Search for Page or Report** icon, enter **Export GIFI Info. to Excel**, and then choose the related link.</span></span>
2. <span data-ttu-id="748e8-135">Angi hva du vil eksportere til Excel ved å fylle ut feltene.</span><span class="sxs-lookup"><span data-stu-id="748e8-135">Specify what to export to Excel by filling the fields.</span></span> <span data-ttu-id="748e8-136">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="748e8-136">Choose a field to read a short description of the field or link to more information.</span></span>
3. <span data-ttu-id="748e8-137">Velg **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="748e8-137">Choose the **OK** button.</span></span>

<span data-ttu-id="748e8-138">**Merk:** Excel-filen har følgende egenskaper:</span><span class="sxs-lookup"><span data-stu-id="748e8-138">**Note:** The Excel file has the following characteristics:</span></span>

* <span data-ttu-id="748e8-139">Saldoen er avrundet til nærmeste prosent, men celleverdien beholder den samme prosenten som den gjør i Finans.</span><span class="sxs-lookup"><span data-stu-id="748e8-139">The balance is rounded to the nearest percentage, but the cell value maintains the same percentage as it does in the general ledger.</span></span>

* <span data-ttu-id="748e8-140">Negative tall representeres som positive tall i hakeparenteser.</span><span class="sxs-lookup"><span data-stu-id="748e8-140">Negative numbers are represented as positive number in brackets.</span></span> <span data-ttu-id="748e8-141">-123 er derfor representert som (123).</span><span class="sxs-lookup"><span data-stu-id="748e8-141">Accordingly, -123 is represented as (123).</span></span>

## <a name="see-also"></a><span data-ttu-id="748e8-142">Se også</span><span class="sxs-lookup"><span data-stu-id="748e8-142">See Also</span></span>
<span data-ttu-id="748e8-143">[Finans](finance-setup.md) </span><span class="sxs-lookup"><span data-stu-id="748e8-143">[Finance](finance-setup.md) </span></span>  
[<span data-ttu-id="748e8-144">Definere kjerneprosesser for økonomi</span><span class="sxs-lookup"><span data-stu-id="748e8-144">Set Up Core Financial Processes</span></span>](finance-setup-setup-finance-setup.md)

