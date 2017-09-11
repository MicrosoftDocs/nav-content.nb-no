---
title: "Bokføre salg"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: e87dd5faf7713aecfbe7209d00bb8076fcae9d25
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---

# <a name="posting-sales"></a><span data-ttu-id="75c82-102">Bokføre salg</span><span class="sxs-lookup"><span data-stu-id="75c82-102">Posting Sales</span></span>
<span data-ttu-id="75c82-103">I **Bokføringsgruppe** i et salgsdokument, kan du velge mellom følgende bokføringsfunksjoner:</span><span class="sxs-lookup"><span data-stu-id="75c82-103">In the **Posting group** on a sales document, you can choose between the following posting functions:</span></span>

- <span data-ttu-id="75c82-104">**Bokfør**</span><span class="sxs-lookup"><span data-stu-id="75c82-104">**Post**</span></span>
- <span data-ttu-id="75c82-105">**Kontrollrapport**</span><span class="sxs-lookup"><span data-stu-id="75c82-105">**Test Report**</span></span>
- <span data-ttu-id="75c82-106">**Bokfør og Send**</span><span class="sxs-lookup"><span data-stu-id="75c82-106">**Post and Send**</span></span>
- <span data-ttu-id="75c82-107">**Bokfør og skriv ut**</span><span class="sxs-lookup"><span data-stu-id="75c82-107">**Post and Print**</span></span>
- <span data-ttu-id="75c82-108">**Bokfør og send e-post**</span><span class="sxs-lookup"><span data-stu-id="75c82-108">**Post and Email**</span></span>
- <span data-ttu-id="75c82-109">**Massebokfør**</span><span class="sxs-lookup"><span data-stu-id="75c82-109">**Post Batch**</span></span>
- <span data-ttu-id="75c82-110">**Forhåndsvis bokføring**</span><span class="sxs-lookup"><span data-stu-id="75c82-110">**Preview Posting**</span></span>

<span data-ttu-id="75c82-111">Når du har fylt ut alle linjene og angitt alle opplysningene i ordren, kan du bokføre den.</span><span class="sxs-lookup"><span data-stu-id="75c82-111">When you have completed all the lines and entered all the information on the sales order, you can post it.</span></span> <span data-ttu-id="75c82-112">Dette oppretter en levering og en faktura.</span><span class="sxs-lookup"><span data-stu-id="75c82-112">This creates a shipment and an invoice.</span></span>

<span data-ttu-id="75c82-113">Når en ordre bokføres, oppdateres kundens konto, finans og varepostene.</span><span class="sxs-lookup"><span data-stu-id="75c82-113">When a sales order is posted, the customer's account, the general ledger, and the item ledger entries are updated.</span></span>

<span data-ttu-id="75c82-114">For hver ordre opprettes en salgspost i **Finanspost**-tabellen.</span><span class="sxs-lookup"><span data-stu-id="75c82-114">For each sales order, a sales entry is created in the **G/L Entry** table.</span></span> <span data-ttu-id="75c82-115">Det opprettes også en post på leverandørens konto i **Kundepost**-tabellen, og en finanspost opprettes i den relevante kundekontoen.</span><span class="sxs-lookup"><span data-stu-id="75c82-115">An entry is also created in the customer's account in the **Cust. Ledger Entry** table and a general ledger entry is created in the relevant receivables account.</span></span> <span data-ttu-id="75c82-116">I tillegg kan bokføring av bestillingen resultere i en mva-post og en finanspost for rabattbeløpet.</span><span class="sxs-lookup"><span data-stu-id="75c82-116">In addition, posting the order may result in a VAT entry and a general ledger entry for the discount amount.</span></span> <span data-ttu-id="75c82-117">Om en rabattpost skal bokføres, avhenger av innholdet i feltet **Rabattbokføring** i vinduet **Salgsoppsett**.</span><span class="sxs-lookup"><span data-stu-id="75c82-117">Whether an entry for the discount is posted depends on the contents of the **Discount Posting** field in the **Sales & Receivables Setup** window.</span></span>

<span data-ttu-id="75c82-118">For hver ordrelinje opprettes det en varepost i tabellen **Varepost** (hvis salgslinjen inneholder varenumre), eller det opprettes en finanspost i tabellen **Finanspost** (hvis salgslinjen inneholder en finanskonto).</span><span class="sxs-lookup"><span data-stu-id="75c82-118">For each sales order line, an item ledger entry will be created in the **Item Ledger Entry** table (if the sales lines contain item numbers) or a general ledger entry will be created in the **G/L Entry** table (if the sales lines contain a general ledger account).</span></span> <span data-ttu-id="75c82-119">I tillegg til dette registreres alltid ordrer i tabellene **Følgeseddelhode** og **Salgsfakturahode**.</span><span class="sxs-lookup"><span data-stu-id="75c82-119">In addition to this, sales orders are always recorded in the **Sales Shipment Header** and **Sales Invoice Header** tables.</span></span>

<span data-ttu-id="75c82-120">**Viktig**: Når du bokfører en ordre, kan du opprette både en følgeseddel og en faktura.</span><span class="sxs-lookup"><span data-stu-id="75c82-120">**Important**: When you post an order, you can create both a shipment and an invoice.</span></span> <span data-ttu-id="75c82-121">Dette kan gjøres samtidig eller hver for seg.</span><span class="sxs-lookup"><span data-stu-id="75c82-121">These can be done at the same time or independently.</span></span> <span data-ttu-id="75c82-122">Du kan også opprette en dellevering eller en delfaktura ved å fylle ut feltene **Levere (antall)** og **Fakturer (antall)** på hver enkelt ordrelinje før du bokfører.</span><span class="sxs-lookup"><span data-stu-id="75c82-122">You can also create a partial shipment and a partial invoice by completing the **Qty. to Ship** and **Qty. to Invoice** fields on the individual sales order lines before you post.</span></span> <span data-ttu-id="75c82-123">Merk at du ikke kan opprette en faktura for noe som ikke er levert.</span><span class="sxs-lookup"><span data-stu-id="75c82-123">Note that you cannot create an invoice for something that is not shipped.</span></span> <span data-ttu-id="75c82-124">Det vil si at for å kunne fakturere, er det nødvendig at du på forhånd har registrert en levering, eller at du velger å levere og fakturere samtidig.</span><span class="sxs-lookup"><span data-stu-id="75c82-124">That is, before you can invoice, you must have recorded a shipment, or you must choose to ship and invoice at the same time.</span></span> 

<span data-ttu-id="75c82-125">Når bokføringen er utført, fjernes de bokførte salgslinjene fra bestillingen.</span><span class="sxs-lookup"><span data-stu-id="75c82-125">When the posting is completed, the posted sales lines are removed from the order.</span></span> <span data-ttu-id="75c82-126">En melding viser når bokføringen er gjennomført.</span><span class="sxs-lookup"><span data-stu-id="75c82-126">A message tells you when the posting is completed.</span></span> <span data-ttu-id="75c82-127">Etter dette vil du kunne se de bokførte postene i de forskjellige vinduene som inneholder bokførte poster, for eksempel vinduene **Kundeposter**, **Finansposter**, **Vareposter**, **Bokførte følgesedler** og **Bokført salgsfaktura**.</span><span class="sxs-lookup"><span data-stu-id="75c82-127">After this, you will be able to see the posted entries in the various windows that contain posted entries, such as the **Cust. Ledger Entries**, **G/L Entries**, **Item Ledger Entries**, **Posted Sales Shipments**, and **Posted Sales Invoices** windows.</span></span>

## <a name="see-also"></a><span data-ttu-id="75c82-128">Se også</span><span class="sxs-lookup"><span data-stu-id="75c82-128">See Also</span></span>
[<span data-ttu-id="75c82-129">Sende dokumenter i e-post</span><span class="sxs-lookup"><span data-stu-id="75c82-129">How to: Send Documents by Email</span></span>](ui-how-send-documents-email.md)

