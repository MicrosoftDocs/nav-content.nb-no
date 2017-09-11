---
title: "Administrere skyldige beløp"
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
ms.openlocfilehash: 08f72aded5c8090dee9a790487fee1db4393220c
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---

# <a name="manage-payables"></a><span data-ttu-id="51d66-102">Administrere skyldige beløp</span><span class="sxs-lookup"><span data-stu-id="51d66-102">Manage Payables</span></span>
<span data-ttu-id="51d66-103">Det er en sentral aktivitet i håndtering av leverandørgjeld å betale leverandører.</span><span class="sxs-lookup"><span data-stu-id="51d66-103">A central task in managing accounts payable is to pay your vendors.</span></span> <span data-ttu-id="51d66-104">Du kan bruke funksjoner til å automatisk fylle ut vinduet **Betalingskladd** med betalingslinjer for forfalte kjøpsfakturaer.</span><span class="sxs-lookup"><span data-stu-id="51d66-104">You can use functions to automatically fill in the **Payment Journal** window with payments lines for due purchase invoices.</span></span> <span data-ttu-id="51d66-105">Hvis du raskt vil utføre involvert banktransaksjoner, kan du eksportere flere betalingskladdelinjer til en fil, som du deretter laste opp til banken for behandling.</span><span class="sxs-lookup"><span data-stu-id="51d66-105">To quickly perform the involved bank transactions, you can export multiple payment journal lines to a file, which you then upload to your bank for processing.</span></span> <span data-ttu-id="51d66-106">Du kan også betale med sjekk, inkludert å overføre sjekker som elektroniske betalinger.</span><span class="sxs-lookup"><span data-stu-id="51d66-106">You can also make payments by check, including to transmit checks as electronic payments.</span></span>

<span data-ttu-id="51d66-107">En annen vanlig oppgave er å utligne utgående betalinger mot deres relaterte leverandørposter og dermed lukke de beslektede kjøpsfakturaene eller kjøpskreditnotaene som betalt.</span><span class="sxs-lookup"><span data-stu-id="51d66-107">Another typical task is to apply outgoing payments to their related vendor ledger entries and thereby close the related purchase invoices or purchase credit memos as paid.</span></span> <span data-ttu-id="51d66-108">Du kan utføre dette arbeidet i vinduet **Betalingsavstemmingskladd** ved å importere en bankkontoutdragsfil for hurtig å registrere betalinger i Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="51d66-108">You can perform this work in the **Payment Reconciliation Journal** window by importing a bank statement file to quickly register the payments in Dynamics NAV.</span></span> <span data-ttu-id="51d66-109">En funksjon for automatisk utligning utligner betalingene til deres tilknyttede åpne leverandør- eller kundeposter, basert på datasamsvar mellom betalingstekst og postinformasjonen.</span><span class="sxs-lookup"><span data-stu-id="51d66-109">An automatic application function applies the payments to their related open vendor or customer ledger entries based on a data matches between payment text and entry information.</span></span> <span data-ttu-id="51d66-110">Du kan bruke ulike funksjoner til å se gjennom og endre automatiske utligninger før du bokfører kladden.</span><span class="sxs-lookup"><span data-stu-id="51d66-110">You can use various functionality to review and change automatic applications before you post the journal.</span></span> <span data-ttu-id="51d66-111">Du kan velge å lukke alle åpne bankposter relatert til de utlignede postene når du bokfører kladden.</span><span class="sxs-lookup"><span data-stu-id="51d66-111">You can choose to close any open bank account ledger entries related to the applied ledger entries when you post the journal.</span></span> <span data-ttu-id="51d66-112">Dette betyr at bankkontoen avstemmes automatisk når alle betalinger er utlignet.</span><span class="sxs-lookup"><span data-stu-id="51d66-112">This means that the bank account is automatically reconciled when all payments are applied.</span></span>

<span data-ttu-id="51d66-113">Du kan også bruke utgående betalinger manuelt i vinduet **Betalingskladd** eller fra de relaterte leverandørpostene.</span><span class="sxs-lookup"><span data-stu-id="51d66-113">Alternatively, you can apply outgoing payments manually in the **Payment Journal** window or from the related vendor ledger entries.</span></span>

<span data-ttu-id="51d66-114">Tabellen nedenfor beskriver en sekvens av oppgaver i leverandørgjeld, og har koblinger til emnene som beskriver dem.</span><span class="sxs-lookup"><span data-stu-id="51d66-114">The following table describes a sequence of tasks within accounts payable, with links to the topics that describe them.</span></span>

|<span data-ttu-id="51d66-115">Hvis du vil</span><span class="sxs-lookup"><span data-stu-id="51d66-115">To</span></span> |<span data-ttu-id="51d66-116">Se</span><span class="sxs-lookup"><span data-stu-id="51d66-116">See</span></span> |
|---|----|
|<span data-ttu-id="51d66-117">Generere forfalte leverandørbetalinger prioritert i henhold til kontantrabatter og forfalte straffegebyrer.</span><span class="sxs-lookup"><span data-stu-id="51d66-117">Generate due vendor payments prioritized according to payment discounts and overdue penalties.</span></span> <span data-ttu-id="51d66-118">Du kan også eksportere betalingene til en bankfil ved bokføring.</span><span class="sxs-lookup"><span data-stu-id="51d66-118">Optionally, export the payments to a bank file when posting.</span></span>|[<span data-ttu-id="51d66-119">Foreta betalinger</span><span class="sxs-lookup"><span data-stu-id="51d66-119">Make Payments</span></span>](payables-make-payments.md)|
|<span data-ttu-id="51d66-120">Utligne leverandørbetalinger automatisk på ubetalte kjøpsfakturaer ved å importere en bankkontoutdragsfil.</span><span class="sxs-lookup"><span data-stu-id="51d66-120">Apply vendor payments automatically to unpaid purchase invoices by importing a bank statement file.</span></span>|[<span data-ttu-id="51d66-121">Bruke betalinger automatisk og avstemme bankkonti</span><span class="sxs-lookup"><span data-stu-id="51d66-121">Apply Payments Automatically and Reconcile Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md)|
|<span data-ttu-id="51d66-122">Utligne leverandørbetalinger på ubetalte fakturaer manuelt.</span><span class="sxs-lookup"><span data-stu-id="51d66-122">Apply vendor payments to unpaid purchase invoices manually.</span></span>|[<span data-ttu-id="51d66-123">Utligne leverandørbetalinger manuelt</span><span class="sxs-lookup"><span data-stu-id="51d66-123">How to: Apply Vendor Payments Manually</span></span>](payables-how-apply-purchase-transactions-manually.md)|

## <a name="see-also"></a><span data-ttu-id="51d66-124">Se også</span><span class="sxs-lookup"><span data-stu-id="51d66-124">See Also</span></span>
[<span data-ttu-id="51d66-125">Håndtere kjøp</span><span class="sxs-lookup"><span data-stu-id="51d66-125">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="51d66-126">Håndtere fordringer</span><span class="sxs-lookup"><span data-stu-id="51d66-126">Manage Receivables</span></span>](receivables-manage-receivables.md)  
[<span data-ttu-id="51d66-127">Arbeide med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="51d66-127">Work With Dynamics NAV</span></span>](ui-work-product.md)  
[<span data-ttu-id="51d66-128">På tvers av forretningsområder</span><span class="sxs-lookup"><span data-stu-id="51d66-128">Across Business Areas</span></span>](ui-across-business-areas.md)

