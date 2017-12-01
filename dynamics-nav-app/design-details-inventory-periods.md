---
title: Designdetaljer - Beholdningsperioder
description: "Tilbakedaterte transaksjoner eller kostnadsjusteringer påvirker ofte saldoer og lagerverdier for regnskapsperioder som kan anses som avsluttet. Dette kan ha en negativ virkning på nøyaktig rapportering, særlig i globale selskaper. Du kan bruke Lagerperioder-funksjonen til å unngå slike problemer, ved å åpne eller lukke lagerperioder for å begrense bokføring i en angitt tidsperiode."
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
ms.openlocfilehash: b318595552cd48bc5b3590a6ff7858412631ba71
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="design-details-inventory-periods"></a><span data-ttu-id="4c3f6-105">Designdetaljer: Beholdningsperioder</span><span class="sxs-lookup"><span data-stu-id="4c3f6-105">Design Details: Inventory Periods</span></span>
<span data-ttu-id="4c3f6-106">Tilbakedaterte transaksjoner eller kostnadsjusteringer påvirker ofte saldoer og lagerverdier for regnskapsperioder som kan anses som avsluttet.</span><span class="sxs-lookup"><span data-stu-id="4c3f6-106">Backdated transactions or cost adjustments often affect balances and stock valuations for accounting periods that may be considered closed.</span></span> <span data-ttu-id="4c3f6-107">Dette kan ha en negativ virkning på nøyaktig rapportering, særlig i globale selskaper.</span><span class="sxs-lookup"><span data-stu-id="4c3f6-107">This can have adverse effects on accurate reporting, especially within global corporations.</span></span> <span data-ttu-id="4c3f6-108">Du kan bruke Lagerperioder-funksjonen til å unngå slike problemer, ved å åpne eller lukke lagerperioder for å begrense bokføring i en angitt tidsperiode.</span><span class="sxs-lookup"><span data-stu-id="4c3f6-108">The Inventory Periods feature can be used to avoid such problems by opening or closing inventory periods to limit posting in a set period of time.</span></span>  

 <span data-ttu-id="4c3f6-109">En lagerperiode er en bestemt periode, angitt av en sluttdato, der du bokfører lagertransaksjoner.</span><span class="sxs-lookup"><span data-stu-id="4c3f6-109">An inventory period is a period of time, defined by an ending date, in which you post inventory transactions.</span></span> <span data-ttu-id="4c3f6-110">Når du lukker en lagerperiode, kan ingen verdiendringer bokføres i den lukkede periode.</span><span class="sxs-lookup"><span data-stu-id="4c3f6-110">When you close an inventory period, no value changes can be posted in the closed period.</span></span> <span data-ttu-id="4c3f6-111">Dette omfatter nye verdibokføringer, forventede eller fakturerte bokføringer, endring av eksisterende verdier og kostjusteringer.</span><span class="sxs-lookup"><span data-stu-id="4c3f6-111">This includes new value postings, expected or invoiced postings, changes to existing values, and cost adjustments.</span></span> <span data-ttu-id="4c3f6-112">Du kan imidlertid framdels bruke på en åpen varepost som er i en lukket periode.</span><span class="sxs-lookup"><span data-stu-id="4c3f6-112">However, you can still apply to an open item ledger entry that falls in the closed period.</span></span> <span data-ttu-id="4c3f6-113">Hvis du vil ha mer informasjon, kan du se [Designdetaljer: Vareutligning](design-details-item-application.md).</span><span class="sxs-lookup"><span data-stu-id="4c3f6-113">For more information, see [Design Details: Item Application](design-details-item-application.md).</span></span>  

 <span data-ttu-id="4c3f6-114">For å sikre at alle transaksjonsposter i en lukket periode er endelige, må følgende betingelser oppfylles før en lagerperiode kan lukkes:</span><span class="sxs-lookup"><span data-stu-id="4c3f6-114">To make sure that all transaction entries in a closed period are final, the following conditions must be met before an inventory period can close:</span></span>  

-   <span data-ttu-id="4c3f6-115">Alle utgående vareposter i perioden må avsluttes (ingen negativ beholdning).</span><span class="sxs-lookup"><span data-stu-id="4c3f6-115">All outbound item ledger entries in the period must be closed (no negative inventory).</span></span>  
-   <span data-ttu-id="4c3f6-116">Alle varekostnader i perioden må justeres.</span><span class="sxs-lookup"><span data-stu-id="4c3f6-116">All item costs in the period must be adjusted.</span></span>  
-   <span data-ttu-id="4c3f6-117">Alle frigitte og ferdige produksjonsordrer i perioden må kostnadsjusteres.</span><span class="sxs-lookup"><span data-stu-id="4c3f6-117">All released and finished production orders in the period must be cost adjusted.</span></span>  

 <span data-ttu-id="4c3f6-118">Når du lukker en lagerperiode, opprettes en lagerperiode ved hjelp av nummeret på den siste varejournalen i lagerperioden.</span><span class="sxs-lookup"><span data-stu-id="4c3f6-118">When you close an inventory period, an inventory period entry is created by using the number of the last item register that falls in the inventory period.</span></span> <span data-ttu-id="4c3f6-119">I tillegg registreres klokkeslett, dato og brukerkode i lagerperiodeposten for brukeren som lukker perioden.</span><span class="sxs-lookup"><span data-stu-id="4c3f6-119">In addition, the time, date, and user code of the user closing the period are recorded in the inventory period entry.</span></span> <span data-ttu-id="4c3f6-120">Ved hjelp av denne informasjonen med siste varejournalen for forrige periode, kan du se hvilke lagertransaksjonene som bokført i lagerperioden.</span><span class="sxs-lookup"><span data-stu-id="4c3f6-120">By using this information with the last item register for the previous period, you can see which inventory transactions were posted in the inventory period.</span></span> <span data-ttu-id="4c3f6-121">Det er også mulig å åpne lagerperioder på nytt hvis du må bokføre i en lukket periode.</span><span class="sxs-lookup"><span data-stu-id="4c3f6-121">It is also possible to reopen inventory periods if you need to post in a closed period.</span></span> <span data-ttu-id="4c3f6-122">Når du åpner en lagerperiode på nytt, blir det opprettet en lagerperiodepost.</span><span class="sxs-lookup"><span data-stu-id="4c3f6-122">When you reopen an inventory period, an inventory period entry is created.</span></span>  

## <a name="see-also"></a><span data-ttu-id="4c3f6-123">Se også</span><span class="sxs-lookup"><span data-stu-id="4c3f6-123">See Also</span></span>  
 <span data-ttu-id="4c3f6-124">[Designdetaljer: Kostberegning for beholdning](design-details-inventory-costing.md) [Administrere lagerkostnader](finance-manage-inventory-costs.md) [Finans](finance.md)</span><span class="sxs-lookup"><span data-stu-id="4c3f6-124">[Design Details: Inventory Costing](design-details-inventory-costing.md) [Managing Inventory Costs](finance-manage-inventory-costs.md) [Finance](finance.md)</span></span>  
 [<span data-ttu-id="4c3f6-125">Arbeide med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="4c3f6-125">Working with Dynamics NAV</span></span>](ui-work-product.md)

