---
title: "Håndtere bankkonti"
description: "Du må regelmessig avstemme bankposter i Dynamics NAV med de relaterte banktransaksjonene i bankkontiene."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reconcile
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: cd33af7062b5a8e75937f8750e09414f734d8c04
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="managing-bank-accounts"></a><span data-ttu-id="17d44-103">Håndtere bankkonti</span><span class="sxs-lookup"><span data-stu-id="17d44-103">Managing Bank Accounts</span></span>
<span data-ttu-id="17d44-104">Med jevne mellomrom må du avstemme bankposter i [!INCLUDE[d365fin](includes/d365fin_md.md)] med tilknyttede banktransaksjoner i bankkontoer i banken din, og deretter bokføre saldoen på bankkontoen din.</span><span class="sxs-lookup"><span data-stu-id="17d44-104">At regular intervals, you must reconcile your bank ledger entries in [!INCLUDE[d365fin](includes/d365fin_md.md)] with the related bank transactions in bank accounts at your bank, and then post the balance to your bank account.</span></span> <span data-ttu-id="17d44-105">Du kan utføre denne oppgaven som en del av behandling av betalinger, som er representert i et bankkontoutdrag i **Betalingsavstemmingskladd**.</span><span class="sxs-lookup"><span data-stu-id="17d44-105">You can perform this task either as part of processing the payments represented on a bank statement in the **Payment Reconciliation Journal**.</span></span> <span data-ttu-id="17d44-106">Du kan også utføre oppgaven separat fra betalingsbehandlingen, i vinduet **Bankkontoavstemming**, som støtter sjekkposter.</span><span class="sxs-lookup"><span data-stu-id="17d44-106">Alternatively, you can perform the task separately from payment processing, in the **Bank Acc. Reconciliation** window, which supports check ledger entries.</span></span> <span data-ttu-id="17d44-107">I begge tilfellene fyller du ut vinduene ved å importere bankkontoutdraget til [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="17d44-107">In both cases, you fill in the windows by importing the bank statement into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

<span data-ttu-id="17d44-108">Noen ganger må du overføre beløp mellom bankkonti i [!INCLUDE[d365fin](includes/d365fin_md.md)] for å gjenspeile overføringer i banken.</span><span class="sxs-lookup"><span data-stu-id="17d44-108">Sometimes, you need to transfer amounts between bank account in [!INCLUDE[d365fin](includes/d365fin_md.md)] to reflect transfers at your bank.</span></span> <span data-ttu-id="17d44-109">Du utfører denne oppgaven på ulike måter i vinduet **Finanskladd**, avhengig av valutaen for midlene.</span><span class="sxs-lookup"><span data-stu-id="17d44-109">You perform this task in the **General Journal** window, in different ways depending on the currency of the funds.</span></span>

<span data-ttu-id="17d44-110">Før du kan administrere bankkonti, må du definere hver bankkonto som et bankkort.</span><span class="sxs-lookup"><span data-stu-id="17d44-110">Before you can manage bank accounts, you must set each bank account up as a bank account card.</span></span> <span data-ttu-id="17d44-111">I tillegg må du definere elektroniske tjenester som du kan bruke for import av bankutdrag og eksport av betalingsfil.</span><span class="sxs-lookup"><span data-stu-id="17d44-111">In addition, you must set up electronic services that you may use for bank statement import and payment file export.</span></span> <span data-ttu-id="17d44-112">Hvis du vil ha mer informasjon, kan du se [Opprette bankkonti](bank-setup-banking.md).</span><span class="sxs-lookup"><span data-stu-id="17d44-112">For more information, see [Set Up Bank Accounts](bank-setup-banking.md).</span></span>

<span data-ttu-id="17d44-113">Tabellen nedenfor beskriver en sekvens av oppgaver, og har koblinger til emnene som beskriver dem.</span><span class="sxs-lookup"><span data-stu-id="17d44-113">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

| <span data-ttu-id="17d44-114">Hvis du vil</span><span class="sxs-lookup"><span data-stu-id="17d44-114">To</span></span> | <span data-ttu-id="17d44-115">Se</span><span class="sxs-lookup"><span data-stu-id="17d44-115">See</span></span> |
| --- | --- |
| <span data-ttu-id="17d44-116">Avstemme bankkonti i forbindelse med betalingsbehandling i vinduet **Betalingsavstemmingskladd**.</span><span class="sxs-lookup"><span data-stu-id="17d44-116">Reconcile bank accounts in connection with payment processing in the **Payment Reconciliation Journal** window.</span></span> |[<span data-ttu-id="17d44-117">Utligne betalinger automatisk og avstemme bankkonti</span><span class="sxs-lookup"><span data-stu-id="17d44-117">Applying Payments Automatically and Reconciling Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md) |
| <span data-ttu-id="17d44-118">Avstemme bankkonti, inkludert sjekkposter, som en separat oppgave i vinduet **Bankkontoavstemming**.</span><span class="sxs-lookup"><span data-stu-id="17d44-118">Reconcile bank accounts, including check ledger entries, as a separate task in the **Bank Acc. Reconciliation** window.</span></span> |[<span data-ttu-id="17d44-119">Avstemme bankkonti separat</span><span class="sxs-lookup"><span data-stu-id="17d44-119">How to: Reconcile Bank Accounts Separately</span></span>](bank-how-reconcile-bank-accounts-separately.md) |
| <span data-ttu-id="17d44-120">Bokføre overføringer mellom bankkonti i samme eller ulike valutaer.</span><span class="sxs-lookup"><span data-stu-id="17d44-120">Post transfers between bank accounts in the same currency or in different currencies.</span></span> |[<span data-ttu-id="17d44-121">Overføre bankkapital</span><span class="sxs-lookup"><span data-stu-id="17d44-121">How to: Transfer Bank Funds</span></span>](bank-how-transfer-bank-funds.md) |

## <a name="see-also"></a><span data-ttu-id="17d44-122">Se også</span><span class="sxs-lookup"><span data-stu-id="17d44-122">See Also</span></span>
[<span data-ttu-id="17d44-123">Konfigurere banktjenester</span><span class="sxs-lookup"><span data-stu-id="17d44-123">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="17d44-124">Håndtere fordringer</span><span class="sxs-lookup"><span data-stu-id="17d44-124">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="17d44-125">[Administrere skyldige beløp](payables-manage-payables.md)  </span><span class="sxs-lookup"><span data-stu-id="17d44-125">[Managing Payables](payables-manage-payables.md)  </span></span>  
<span data-ttu-id="17d44-126">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="17d44-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="17d44-127">Generelle forretningsfunksjoner</span><span class="sxs-lookup"><span data-stu-id="17d44-127">General Business Functionality</span></span>](ui-across-business-areas.md)  

