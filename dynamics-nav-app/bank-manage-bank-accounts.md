---
title: "Håndtere bankkonti"
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
ms.openlocfilehash: d97c3afba0e899768bda1b637c4f288db210d38c
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---

# <a name="manage-bank-accounts"></a><span data-ttu-id="99326-102">Håndtere bankkonti</span><span class="sxs-lookup"><span data-stu-id="99326-102">Manage Bank Accounts</span></span>
<span data-ttu-id="99326-103">Med jevne mellomrom må du avstemme bankposter i Dynamics NAV med tilknyttede banktransaksjoner i bankkontoer i banken din, og deretter bokføre saldoen på bankkontoen din.</span><span class="sxs-lookup"><span data-stu-id="99326-103">At regular intervals, you must reconcile your bank ledger entries in Dynamics NAV with the related bank transactions in bank accounts at your bank, and then post the balance to your bank account.</span></span> <span data-ttu-id="99326-104">Du kan utføre denne oppgaven som en del av behandling av betalinger, som er representert i et bankkontoutdrag i **Betalingsavstemmingskladd**.</span><span class="sxs-lookup"><span data-stu-id="99326-104">You can perform this task either as part of processing the payments represented on a bank statement in the **Payment Reconciliation Journal**.</span></span> <span data-ttu-id="99326-105">Du kan også utføre oppgaven separat fra betalingsbehandlingen, i vinduet **Bankkontoavstemming**, som støtter sjekkposter.</span><span class="sxs-lookup"><span data-stu-id="99326-105">Alternatively, you can perform the task separately from payment processing, in the **Bank Acc. Reconciliation** window, which supports check ledger entries.</span></span> <span data-ttu-id="99326-106">I begge tilfellene fyller du ut vinduene ved å importere bankkontoutdraget til Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="99326-106">In both cases, you fill the windows by importing the bank statement into Dynamics NAV.</span></span>

<span data-ttu-id="99326-107">Noen ganger må du overføre beløp mellom bankkonti i Dynamics NAV for å gjenspeile overføringer i banken.</span><span class="sxs-lookup"><span data-stu-id="99326-107">Sometimes, you need to transfer amounts between bank account in Dynamics NAV to reflect transfers at your bank.</span></span> <span data-ttu-id="99326-108">Du utfører denne oppgaven på ulike måter i vinduet **Finanskladd**, avhengig av valutaen for midlene.</span><span class="sxs-lookup"><span data-stu-id="99326-108">You perform this task in the **General Journal** window, in different ways depending on the currency of the funds.</span></span>

<span data-ttu-id="99326-109">Før du kan administrere bankkonti, må du definere hver bankkonto som et bankkort.</span><span class="sxs-lookup"><span data-stu-id="99326-109">Before you can manage bank accounts, you must set each bank account up as a bank account card.</span></span> <span data-ttu-id="99326-110">I tillegg må du definere elektroniske tjenester som du kan bruke for import av bankutdrag og eksport av betalingsfil.</span><span class="sxs-lookup"><span data-stu-id="99326-110">In addition, you must set up electronic services that you may use for bank statement import and payment file export.</span></span> <span data-ttu-id="99326-111">Hvis du vil ha mer informasjon, kan du se [Opprette bankkonti](bank-setup-banking.md).</span><span class="sxs-lookup"><span data-stu-id="99326-111">For more information, see [Set Up Bank Accounts](bank-setup-banking.md).</span></span>

<span data-ttu-id="99326-112">Tabellen nedenfor beskriver en sekvens av oppgaver, og har koblinger til emnene som beskriver dem.</span><span class="sxs-lookup"><span data-stu-id="99326-112">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="99326-113">Hvis du vil</span><span class="sxs-lookup"><span data-stu-id="99326-113">To</span></span> |<span data-ttu-id="99326-114">Se</span><span class="sxs-lookup"><span data-stu-id="99326-114">See</span></span> |
|---|----|
|<span data-ttu-id="99326-115">Avstemme bankkonti i forbindelse med betalingsbehandling i vinduet **Betalingsavstemmingskladd**.</span><span class="sxs-lookup"><span data-stu-id="99326-115">Reconcile bank accounts in connection with payment processing in the **Payment Reconciliation Journal** window.</span></span>|[<span data-ttu-id="99326-116">Bruke betalinger automatisk og avstemme bankkonti</span><span class="sxs-lookup"><span data-stu-id="99326-116">Apply Payments Automatically and Reconcile Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md)|
|<span data-ttu-id="99326-117">Avstemme bankkonti, inkludert sjekkposter, som en separat oppgave i vinduet **Bankkontoavstemming**.</span><span class="sxs-lookup"><span data-stu-id="99326-117">Reconcile bank accounts, including check ledger entries, as a separate task in the **Bank Acc. Reconciliation** window.</span></span>|[<span data-ttu-id="99326-118">Avstemme bankkonti separat</span><span class="sxs-lookup"><span data-stu-id="99326-118">How to: Reconcile Bank Accounts Separately</span></span>](bank-how-reconcile-bank-accounts-separately.md)|
|<span data-ttu-id="99326-119">Bokføre overføringer mellom bankkonti i samme eller ulike valutaer.</span><span class="sxs-lookup"><span data-stu-id="99326-119">Post transfers between bank accounts in the same currency or in different currencies.</span></span>|[<span data-ttu-id="99326-120">Overføre bankkapital</span><span class="sxs-lookup"><span data-stu-id="99326-120">How to: Transfer Bank Funds</span></span>](bank-how-transfer-bank-funds.md)
## <a name="see-also"></a><span data-ttu-id="99326-121">Se også</span><span class="sxs-lookup"><span data-stu-id="99326-121">See Also</span></span>  
[<span data-ttu-id="99326-122">Definere bankvesen</span><span class="sxs-lookup"><span data-stu-id="99326-122">Set Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="99326-123">Håndtere fordringer</span><span class="sxs-lookup"><span data-stu-id="99326-123">Manage Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="99326-124">[Administrere skyldige beløp](payables-manage-payables.md)  </span><span class="sxs-lookup"><span data-stu-id="99326-124">[Manage Payables](payables-manage-payables.md)  </span></span>  
[<span data-ttu-id="99326-125">Arbeide med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="99326-125">Work With Dynamics NAV</span></span>](ui-work-product.md)  
[<span data-ttu-id="99326-126">På tvers av forretningsområder</span><span class="sxs-lookup"><span data-stu-id="99326-126">Across Business Areas</span></span>](ui-across-business-areas.md)

