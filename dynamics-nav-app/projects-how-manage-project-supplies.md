---
title: Administrere prosjektforsyninger
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 00b9ed8480f6b5ab9265beb0fe2dc0060b1c3192
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-manage-job-supplies"></a><span data-ttu-id="bc2ad-102">Administrere prosjektforsyninger</span><span class="sxs-lookup"><span data-stu-id="bc2ad-102">How to: Manage Job Supplies</span></span>
<span data-ttu-id="bc2ad-103">Behandling av prosjektforsyninger som varer, tjenester og utgifter inngår i og er en viktig del av alle prosjektutførelser.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-103">Managing project supplies of items, services, and expenses is an integral and critical aspect of the execution of all jobs.</span></span> <span data-ttu-id="bc2ad-104">Du kan bruke lagerantallene eller foreta prosjektspesifikke kjøp ved hjelp av bestillinger eller kjøpsfakturaer.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-104">You can use inventory quantities or make job-specific purchases using purchase orders or purchase invoices.</span></span> <span data-ttu-id="bc2ad-105">En servicejobb på en datamaskin krever for eksempel en ny disk.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-105">For example, a service job on a computer requires a new disk.</span></span> <span data-ttu-id="bc2ad-106">Du oppretter en kjøpsfaktura for å kjøpe en ny disk, og registrerer prosjektet den skal brukes på.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-106">You create a purchase invoice to buy a new disk and record the job that it will be used on.</span></span>

<span data-ttu-id="bc2ad-107">Hvis kjøpsprosessen ikke krever at den fysiske transaksjonen registreres separat, kan et kjøp behandles i vinduet **Finanskladd for prosjekt**.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-107">If the purchase process does not require that the physical transaction be recorded separately, then a purchase may be processed in the **Job G/L Journal** window.</span></span> <span data-ttu-id="bc2ad-108">Hvis du vil ha mer informasjon, kan du se [Registrere forbruk for prosjekter](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="bc2ad-108">For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

## <a name="to-purchase-items-or-services-for-a-job"></a><span data-ttu-id="bc2ad-109">Slik kjøper du varer eller tjenester for et prosjekt</span><span class="sxs-lookup"><span data-stu-id="bc2ad-109">To purchase items or services for a job</span></span>
<span data-ttu-id="bc2ad-110">Følgende fremgangsmåte viser hvordan du bruker en kjøpsfaktura til å kjøpe produkter for et prosjekt.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-110">The following procedure shows how to use a purchase invoice to purchase products for a job.</span></span> <span data-ttu-id="bc2ad-111">Bruk samme fremgangsmåte når du bruker en bestilling.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-111">The same steps apply when using a purchase order.</span></span>  

1. <span data-ttu-id="bc2ad-112">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kjøpsfakturaer** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-112">In the top right corner, choose the **Search for Page or Report** icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="bc2ad-113">Velg handlingen **Nytt** og fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-113">Choose the **New** action and fill in the fields as necessary.</span></span> <span data-ttu-id="bc2ad-114">Hvis du vil ha mer informasjon, kan du se [Registrere kjøp](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="bc2ad-114">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
3. <span data-ttu-id="bc2ad-115">I feltene **Prosjektnr.**</span><span class="sxs-lookup"><span data-stu-id="bc2ad-115">In the **Job No.**</span></span> <span data-ttu-id="bc2ad-116">og **Prosjektoppgavenr.**</span><span class="sxs-lookup"><span data-stu-id="bc2ad-116">and **Job Task No.**</span></span> <span data-ttu-id="bc2ad-117">velger du informasjonen på prosjektet som du vil kjøpe varer eller tjenester for.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-117">fields, select the information of the job that you want to purchase items or services for.</span></span>  

    <span data-ttu-id="bc2ad-118">Verdien du velger i feltet **Prosjektlinjetype**, definerer om en planleggingslinje blir opprettet når du bokfører forbruket for varen.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-118">The value that you select in the **Job Line Type** field defines whether a planning line is created when you post the usage of the item.</span></span> <span data-ttu-id="bc2ad-119">Hvis feltet inneholder **Fakturerbar**, opprettes det prosjektplanleggingslinjer som er klare for å faktureres kunden.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-119">If the field contains **Billable**, then job planning lines that are ready to be invoiced to the customer are created.</span></span> <span data-ttu-id="bc2ad-120">Hvis du vil ha mer informasjon, kan du se [Fakturere prosjekter](projects-how-invoice-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="bc2ad-120">For more information, see [How to: Invoice Jobs](projects-how-invoice-jobs.md).</span></span>

4. <span data-ttu-id="bc2ad-121">Velg handlingen **Bokfør**.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-121">Choose the **Post** action.</span></span>

## <a name="to-view-the-value-of-purchases-for-a-job"></a><span data-ttu-id="bc2ad-122">Slik viser du verdien av kjøp for et prosjekt</span><span class="sxs-lookup"><span data-stu-id="bc2ad-122">To view the value of purchases for a job</span></span>  

1. <span data-ttu-id="bc2ad-123">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Prosjekter** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-123">In the top right corner, choose the **Search for Page or Report** icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="bc2ad-124">Åpne et aktuelt prosjektkort.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-124">Open a relevant job card.</span></span>

    <span data-ttu-id="bc2ad-125">På hurtigfanen **Oppgaver** viser feltet **Utestående bestillinger** det totale utestående beløpet, i lokal valuta, for lagervarer og tjenester i kjøpsdokumenter for prosjektoppgavelinjen.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-125">On the **Tasks** FastTab, the **Outstanding Orders** field shows the total outstanding amount, in local currency, of inventory items and services on purchase documents for the job task line.</span></span>  

    <span data-ttu-id="bc2ad-126">Feltet **Mottatt, ikke fakturert (beløp)** viser verdien for varer som er levert i kjøpsdokumenter, men som ennå ikke er fakturert.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-126">The **Amt. Rec. Not Invoiced** field shows the value of items delivered on purchase documents, but not yet invoiced.</span></span>  

3. <span data-ttu-id="bc2ad-127">Velg enten feltene for å åpne vinduet **Bestillingslinjer**, der du kan gå gjennom informasjon om de relaterte kjøpsdokumentlinjene, inkludert hvilke varer eller tjenester som er mottatt.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-127">Choose either of the fields to open the **Purchase Lines** window where you can review information about the related purchase document lines, including which items or services have been received.</span></span>

## <a name="to-post-a-job-related-expense"></a><span data-ttu-id="bc2ad-128">Slik bokfører du en prosjektrelatert utgift</span><span class="sxs-lookup"><span data-stu-id="bc2ad-128">To post a job-related expense</span></span>  
<span data-ttu-id="bc2ad-129">Hvis du pådrar deg ekstraordinære eller enkeltstående prosjektutgifter, kan du bruke vinduet **Finanskladd for prosjekt** til å bokføre dem direkte til den aktuelle prosjektkontoen.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-129">If you incur extraordinary or one-time job expenses, you can use the **Job G/L Journal** window to post them directly to the relevant job account.</span></span>

1. <span data-ttu-id="bc2ad-130">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Finanskladder for prosjekt** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-130">In the top right corner, choose the **Search for Page or Report** icon, enter **Job G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="bc2ad-131">Opprett en ny linje, og skriv inn informasjon om utgiften, inkludert informasjon i feltene **Prosjektnr.**</span><span class="sxs-lookup"><span data-stu-id="bc2ad-131">Create a new line and enter information about the expense, including information in the **Job No.**</span></span> <span data-ttu-id="bc2ad-132">og **Prosjektoppgavenr.**</span><span class="sxs-lookup"><span data-stu-id="bc2ad-132">and **Job Task No** fields.</span></span>  
3. <span data-ttu-id="bc2ad-133">Når kladden er fullført, kan du velge handlingen **Bokfør**.</span><span class="sxs-lookup"><span data-stu-id="bc2ad-133">When the journal is complete, choose the **Post** action.</span></span>


## <a name="see-also"></a><span data-ttu-id="bc2ad-134">Se også</span><span class="sxs-lookup"><span data-stu-id="bc2ad-134">See Also</span></span>
[<span data-ttu-id="bc2ad-135">Administrere prosjekter</span><span class="sxs-lookup"><span data-stu-id="bc2ad-135">Manage Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="bc2ad-136">Finans</span><span class="sxs-lookup"><span data-stu-id="bc2ad-136">Finance</span></span>](finance-setup.md)  
<span data-ttu-id="bc2ad-137">[Håndtere kjøp](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="bc2ad-137">[Manage Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="bc2ad-138">[Håndtere salg](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="bc2ad-138">[Manage Sales](sales-manage-sales.md)    </span></span>  
[<span data-ttu-id="bc2ad-139">Arbeide med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="bc2ad-139">Work With Dynamics NAV</span></span>](ui-work-product.md)  

