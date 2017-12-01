---
title: "Skrive ut remitteringsønske"
description: "Du kan hjelpe leverandørene med å utføre avstemminger ved å skrive ut remitteringsønsker før du bokfører en utbetalingskladd, og etter at du har bokført en betaling."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/26/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 7c7004ac5ded9436861bf5034f59a9c2bcd99dd0
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---

#<a name="how-to-print-remittance-advice"></a><span data-ttu-id="516e7-103">Skrive ut remitteringsønske</span><span class="sxs-lookup"><span data-stu-id="516e7-103">How to: Print Remittance Advice</span></span>
<span data-ttu-id="516e7-104">Du kan skrive ut et remitteringsønske før du bokfører en utbetalingskladd, og etter at du har bokført en betaling.</span><span class="sxs-lookup"><span data-stu-id="516e7-104">You can print remittance advice before posting a payment journal and after posting a payment.</span></span> <span data-ttu-id="516e7-105">Remitteringsønsket viser leverandørfakturanumrene, noe som hjelper leverandører å utføre avstemminger.</span><span class="sxs-lookup"><span data-stu-id="516e7-105">This advice displays vendor invoice numbers, which helps vendors to perform reconciliations.</span></span>

##<a name="to-print-remittance-advice"></a><span data-ttu-id="516e7-106">Skrive ut remitteringsønske</span><span class="sxs-lookup"><span data-stu-id="516e7-106">To print remittance advice</span></span>
1. <span data-ttu-id="516e7-107">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Betalingskladder**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="516e7-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="516e7-108">I **Betalingskladd**-vinduet velger du betalingen som remitteringsønsket skal skrives ut for.</span><span class="sxs-lookup"><span data-stu-id="516e7-108">In the **Payment Journal** window, select the payment for which remittance advice must be printed.</span></span>  
3. <span data-ttu-id="516e7-109">Velg handlingen **Skrive ut remitteringsønske**.</span><span class="sxs-lookup"><span data-stu-id="516e7-109">Choose the **Print Remittance Advice** action.</span></span>  
4. <span data-ttu-id="516e7-110">Velg aktuelle filtre i kjørselen **Remitteringsønske – Kladd**, på hurtigfanen **Finanskladdelinje**.</span><span class="sxs-lookup"><span data-stu-id="516e7-110">In the **Remittance Advice - Journal** batch job, on the **Fen. Journal Line** FastTab, choose the appropriate filters.</span></span>  
  
    >[!Note]
    > <span data-ttu-id="516e7-111">Du kan filtrere ved hjelp av leverandørens eksterne dokumentnummer for å samsvare betalinger med fakturaer.</span><span class="sxs-lookup"><span data-stu-id="516e7-111">You can filter using the vendor's external document number to match payments with invoices.</span></span>

5. <span data-ttu-id="516e7-112">Velg aktuelle filtre i hurtigfanen **Leverandør**.</span><span class="sxs-lookup"><span data-stu-id="516e7-112">On the **Vendor** FastTab, choose the appropriate filters.</span></span>  
6. <span data-ttu-id="516e7-113">Velg **Skriv ut** hvis du vil skrive ut rapporten, eller **Forhåndsvisning** hvis du vil se rapporten nå.</span><span class="sxs-lookup"><span data-stu-id="516e7-113">Choose **Print** to print the report, or choose **Preview** to view it now.</span></span>  

## <a name="using-remittance-advice-reports"></a><span data-ttu-id="516e7-114">Bruke remitteringsønskerapporter</span><span class="sxs-lookup"><span data-stu-id="516e7-114">Using Remittance Advice Reports</span></span>
<span data-ttu-id="516e7-115">Tabellen nedenfor beskriver rapportene som kan brukes ved remitteringsønsker:</span><span class="sxs-lookup"><span data-stu-id="516e7-115">The following table describes the reports that you can use with remittance advice:</span></span>

|<span data-ttu-id="516e7-116">Rapport</span><span class="sxs-lookup"><span data-stu-id="516e7-116">Report</span></span>|<span data-ttu-id="516e7-117">Description</span><span class="sxs-lookup"><span data-stu-id="516e7-117">Description</span></span>|
|----|----|
|<span data-ttu-id="516e7-118">Remitteringsønske – Kladderapport</span><span class="sxs-lookup"><span data-stu-id="516e7-118">Remittance Advice - Journal Report</span></span>|<span data-ttu-id="516e7-119">Denne rapporten viser hvilke dokumenter som er inkludert i betalingen.</span><span class="sxs-lookup"><span data-stu-id="516e7-119">This report indicates which documents are included in the payment.</span></span> <span data-ttu-id="516e7-120">For finanskladdelinjer kan du angi hvilken kladdemal og kladd remitteringsønsket vil bli skrevet ut fra, datoen for første aktiviteten som skal skrives ut, og du kan filtrere etter et bilagsnummer.</span><span class="sxs-lookup"><span data-stu-id="516e7-120">For general journal lines, you can specify the journal template and journal batch from which the remittance advices will be printed, the date of the first activity to print, and filter on a document number.</span></span> <span data-ttu-id="516e7-121">Ved leverandører kan du bestemme leverandørnumrene som skal inngå i rapporten.</span><span class="sxs-lookup"><span data-stu-id="516e7-121">For vendors, you can enter the vendor numbers to include in the report.</span></span> |
|<span data-ttu-id="516e7-122">Remitteringsønske – Postrapport</span><span class="sxs-lookup"><span data-stu-id="516e7-122">Remittance Advice - Entries Report</span></span>| <span data-ttu-id="516e7-123">Denne rapporten viser hvilke dokumenter som er inkludert i betalingen.</span><span class="sxs-lookup"><span data-stu-id="516e7-123">This report indicates which documents are included in the payment.</span></span> <span data-ttu-id="516e7-124">Du kan definere innhold i rapporten ved å definere filtre.</span><span class="sxs-lookup"><span data-stu-id="516e7-124">You define the report contents by setting filters.</span></span> <span data-ttu-id="516e7-125">Du kan angi flere felt på fanebladet ved å velge **Felt**-feltet.</span><span class="sxs-lookup"><span data-stu-id="516e7-125">You can set additional fields on the tab by choosing the **Field** field.</span></span> <span data-ttu-id="516e7-126">For leverandørposter kan du angi hvilke leverandører som skal tas med i rapporten, datoen for første aktiviteten som skal skrives ut, valuta, og løpenummeret som skal tas med.</span><span class="sxs-lookup"><span data-stu-id="516e7-126">For vendor ledger entries, you can specify the vendors to include in the report, the date of the first activity to print, the currency, and the entry number to include.</span></span> |

> [!Note]
> <span data-ttu-id="516e7-127">Remitteringsønske - Kladderapport støtter ikke scenarier med valutautligning eller betalingstoleranser.</span><span class="sxs-lookup"><span data-stu-id="516e7-127">The Remittance Advice - Journal Report does not support cross currency application scenarios or payment tolerances.</span></span> <span data-ttu-id="516e7-128">Hvis du vil ha mer informasjon, kan du se [Aktivere utligning av kundeposter i forskjellige valutaer](finance-how-enable-application-ledger-entries-different-currencies.md).</span><span class="sxs-lookup"><span data-stu-id="516e7-128">For more information, see [How to: Enable Application of Ledger Entries in Different Currencies](finance-how-enable-application-ledger-entries-different-currencies.md).</span></span>

> [!Tip]
> <span data-ttu-id="516e7-129">Hvis du vil ha mer informasjon om hvordan du arbeider med rapporter, kan du se [Vise testrapporter før bokføring](ui-how-view-test-reports-posting.md), [Arbeide med rapporter](ui-work-report.md), og [Søke etter, filtrere og sortere data](ui-enter-criteria-filters.md).</span><span class="sxs-lookup"><span data-stu-id="516e7-129">For more information about how to work with reports, see [Viewing Test Reports before Posting](ui-how-view-test-reports-posting.md), [Work with Reports](ui-work-report.md), and [Searching, Filtering, and Sorting Data](ui-enter-criteria-filters.md).</span></span>

##<a name="see-also"></a><span data-ttu-id="516e7-130">Se også</span><span class="sxs-lookup"><span data-stu-id="516e7-130">See Also</span></span>  
[<span data-ttu-id="516e7-131">Velkommen til Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="516e7-131">Welcome to Dynamics NAV</span></span>](across-get-started.md)
