---
title: Bruke utvidelsen QuickBooks Datamigrering
description: "Beskriver hvordan du bruker utvidelsen til å overføre kunder, leverandører, varer og konti fra QuickBooks Online til Dynamics NAV."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, QuickBooks, import
ms.date: 05/24/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: e4854a5695f050c710440c5652d70ae7c4bc02bd
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---

# <a name="the-quickbooks-online-data-migration-extension-for-dynamics-nav"></a><span data-ttu-id="0f8ba-103">Utvidelsen QuickBooks Online Datamigrering for Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="0f8ba-103">The QuickBooks Online Data Migration Extension for Dynamics NAV</span></span>
<span data-ttu-id="0f8ba-104">Utvidelsen er inkludert i den assisterte oppsettsveiledningen **Datamigrering** for å hjelpe deg å overføre viktige forretningsdata fra QuickBooks Online til [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="0f8ba-104">This extension is included in the **Data Migration** assisted setup guide to help you migrate important business data from QuickBooks Online to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="0f8ba-105">Dette er for eksempel praktisk når virksomheten er i vekst og du har besluttet å oppgradere appen for forretningsdrift ved å begynne å bruke [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="0f8ba-105">For example, this is useful when your business is growing, and you've decided to upgrade your business management app by starting to use [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="what-data-can-i-import-from-quickbooks-online"></a><span data-ttu-id="0f8ba-106">Hvilke data kan jeg importere fra QuickBooks Online?</span><span class="sxs-lookup"><span data-stu-id="0f8ba-106">What data can I import from QuickBooks Online?</span></span>
<span data-ttu-id="0f8ba-107">Du kan importere følgende data fra QuickBooks Online til [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span><span class="sxs-lookup"><span data-stu-id="0f8ba-107">You can import the following data from QuickBooks Online to [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span></span>  

* <span data-ttu-id="0f8ba-108">Kunder</span><span class="sxs-lookup"><span data-stu-id="0f8ba-108">Customers</span></span>
* <span data-ttu-id="0f8ba-109">Leverandører</span><span class="sxs-lookup"><span data-stu-id="0f8ba-109">Vendors</span></span>
* <span data-ttu-id="0f8ba-110">Varer</span><span class="sxs-lookup"><span data-stu-id="0f8ba-110">Items</span></span>
* <span data-ttu-id="0f8ba-111">Kontoplan</span><span class="sxs-lookup"><span data-stu-id="0f8ba-111">Chart of accounts</span></span> 
* <span data-ttu-id="0f8ba-112">Startsaldotransaksjon i Finans</span><span class="sxs-lookup"><span data-stu-id="0f8ba-112">Beginning balance transaction in the general ledger</span></span>
* <span data-ttu-id="0f8ba-113">Beholdningsantall for lagervarer</span><span class="sxs-lookup"><span data-stu-id="0f8ba-113">On-hand quantities for inventory items</span></span>
* <span data-ttu-id="0f8ba-114">Åpne dokumenter for kunder og leverandører, for eksempel fakturaer, kreditnotaer og betalinger</span><span class="sxs-lookup"><span data-stu-id="0f8ba-114">Open documents for customers and vendors, such as invoices, credit memos, and payments</span></span>

<span data-ttu-id="0f8ba-115">Vi overfører bare hele beløp på salgs- og kjøpsdokumenter.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-115">We migrate only full amounts on sales and purchase documents.</span></span> <span data-ttu-id="0f8ba-116">Vi oppdaterer ikke delvis betalte beløp.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-116">We do not update partially paid amounts.</span></span> <span data-ttu-id="0f8ba-117">Hvis en kunde for eksempel har betalt 300 av totalt 500 kroner på en salgsfaktura, overfører vi hele beløpet på 500.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-117">For example, if a customer has paid 300 of a total of 500 dollars on a sales invoice, we migrate the full 500.</span></span> <span data-ttu-id="0f8ba-118">Hvis du har mottatt delbetalinger, må du oppdatere disse manuelt før eller etter at du har overført data.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-118">If you have received partial payments, you must update these manually, either before or after you migrate data.</span></span> <span data-ttu-id="0f8ba-119">Vi anbefaler at du utligner utestående transaksjoner før du overfører, bare for å gjøre ting enklere senere.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-119">We recommend that you apply outstanding transactions before you migrate, just to make things easier afterward.</span></span>

> [!NOTE]  
>   <span data-ttu-id="0f8ba-120">Vi overfører ikke bestillinger eller ordrer.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-120">We do not migrate purchase orders or sales orders.</span></span>

## <a name="before-you-start"></a><span data-ttu-id="0f8ba-121">Før du begynner</span><span class="sxs-lookup"><span data-stu-id="0f8ba-121">Before you start</span></span>
<span data-ttu-id="0f8ba-122">En viktig del av overføringen er å angi kontiene som transaksjonene skal overføres til.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-122">An important part of the migration process is to specify the accounts to migrate transactions to.</span></span> <span data-ttu-id="0f8ba-123">Det er lurt å planlegge denne tilordningen før du overfører data.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-123">It's a good idea to plan this mapping before you migrate data.</span></span> <span data-ttu-id="0f8ba-124">Kontiene der du for eksempel bokfører transaksjoner for følgende:</span><span class="sxs-lookup"><span data-stu-id="0f8ba-124">For example, the accounts where you post transactions for:</span></span>  
  
* <span data-ttu-id="0f8ba-125">Salg av varer eller tjenestene til kunder.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-125">The sale of items or services to customers.</span></span>
* <span data-ttu-id="0f8ba-126">Kjøp av varer eller tjenester fra leverandører.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-126">The purchase of items or services from vendors.</span></span>  
* <span data-ttu-id="0f8ba-127">Justeringer i Finans.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-127">Adjustments in the general ledger.</span></span>  

[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="0f8ba-128"> krever at det er tilordnet kontonumre til finanskonti.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-128"> requires that general ledger accounts have account numbers assigned to them.</span></span> <span data-ttu-id="0f8ba-129">Kontroller at kontonumre er tilordnet til kontiene i QuickBooks Online.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-129">Make sure that account numbers are assigned to your accounts in QuickBooks Online.</span></span>

<span data-ttu-id="0f8ba-130">Hvis transaksjoner i QuickBooks Online har mva-beløp, må du definere en mva-konto for mva-jurisdiksjonene i [!INCLUDE[d365fin](includes/d365fin_md.md)] før du kan bokføre transaksjoner.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-130">If transactions in QuickBooks Online have tax amounts, you must set up a tax account for your tax jurisdictions in [!INCLUDE[d365fin](includes/d365fin_md.md)] before you can post transactions.</span></span>

## <a name="how-do-i-start-using-the-extension"></a><span data-ttu-id="0f8ba-131">Hvordan begynner jeg å bruke utvidelsen?</span><span class="sxs-lookup"><span data-stu-id="0f8ba-131">How do I start using the extension?</span></span>
<span data-ttu-id="0f8ba-132">Det er enkelt å komme i gang.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-132">Getting started is easy.</span></span> <span data-ttu-id="0f8ba-133">Alt du trenger å gjøre, er å kjøre den assisterte oppsettsveiledningen **Datamigrering**.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-133">All you need to do is run the **Data Migration** assisted setup guide.</span></span> <span data-ttu-id="0f8ba-134">Slik gjør du det:</span><span class="sxs-lookup"><span data-stu-id="0f8ba-134">Here's how:</span></span>

1. <span data-ttu-id="0f8ba-135">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Assistert oppsett**, og velg deretter **Overfør forretningsdata**.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Assisted Setup**, and then choose **Migrate business data**.</span></span>
2. <span data-ttu-id="0f8ba-136">Følg instruksjonene for hvert trinn i den assisterte oppsettsveiledningen.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-136">Follow the instructions on each step in the assisted setup guide.</span></span>

## <a name="what-do-i-do-after-i-migrate-data"></a><span data-ttu-id="0f8ba-137">Hva gjør jeg etter at jeg har overført dataene?</span><span class="sxs-lookup"><span data-stu-id="0f8ba-137">What do I do after I migrate data?</span></span>
<span data-ttu-id="0f8ba-138">Etter at du har overført dataene, har transaksjoner statusen **Ikke bokført**, slik at du kan se gjennom dem og foreta justeringer.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-138">After you migrate data, transactions have the status **Unposted**, so you can review them and make adjustments.</span></span> <span data-ttu-id="0f8ba-139">Hvis du vil se gjennom transaksjonene, går du til siden der de vanligvis er.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-139">To review the transactions, go to the page where you would normally find them.</span></span> <span data-ttu-id="0f8ba-140">Hvis du for eksempel vil se gjennom ikke-bokførte salgsfakturaer, går du til siden **Salgsfakturaer**.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-140">For example, to review unposted sales invoices, go to the **Sales Invoices** page.</span></span> <span data-ttu-id="0f8ba-141">Hvis du vil se gjennom utbetalingskladder, går du til siden **Utbetalingskladder**.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-141">To review payment journals, go to the **Payment Journals** page.</span></span>   

<span data-ttu-id="0f8ba-142">Det er enkelte bestemte ting du bør gjøre:</span><span class="sxs-lookup"><span data-stu-id="0f8ba-142">There are a few things in particular that you should do:</span></span>

* <span data-ttu-id="0f8ba-143">Hvis transaksjonene i QuickBooks Online hadde påslags- eller rabattbeløp, må du legge til beløpene manuelt i de relaterte transaksjonene i [!INCLUDE[d365fin](includes/d365fin_md.md)] før du bokfører dem.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-143">If the transactions in QuickBooks Online had markup or discount amounts, you must manually add the amounts to the related transactions in [!INCLUDE[d365fin](includes/d365fin_md.md)] before you post them.</span></span>
* <span data-ttu-id="0f8ba-144">Hvis du bruker merverdiavgift (mva), må du kanskje legge til en bokføringsgruppe for firma og en varebokføringsgruppe i bokføringsoppsettet, slik at du kan bokføre mva-beløp.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-144">If you are using value added tax (VAT), you may need to add a business posting group and a product posting group to the posting setup so that you can post VAT amounts.</span></span>
* <span data-ttu-id="0f8ba-145">Kontroller startsaldoene for konti i Finans.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-145">Verify the beginning balances for accounts in the general ledger.</span></span> <span data-ttu-id="0f8ba-146">QuickBooks Online lagrer ikke gjeldende saldo for alle konti, så du må kanskje rette startsaldoer.</span><span class="sxs-lookup"><span data-stu-id="0f8ba-146">QuickBooks Online does not store the current balance for all accounts, so you might need to correct beginning balances.</span></span>

## <a name="see-also"></a><span data-ttu-id="0f8ba-147">Se også</span><span class="sxs-lookup"><span data-stu-id="0f8ba-147">See Also</span></span>
[<span data-ttu-id="0f8ba-148">Importere forretningsdata fra andre økonomisystemer</span><span class="sxs-lookup"><span data-stu-id="0f8ba-148">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="0f8ba-149">[Tilpasse [!INCLUDE[d365fin](includes/d365fin_md.md)] ved hjelp av utvidelser](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="0f8ba-149">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  

