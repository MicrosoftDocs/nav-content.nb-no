---
title: Opprette KID-numre for salgsdokumenter
description: "Kunde-ID (KID) er et kundeidentifikasjonsnummer som inneholder en betalingsreferanse til leverandøren, og sikrer at betalingen bokføres riktig hos leverandøren."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: a1fb7e77f56aa8731efa3e138fda53feb0490802
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-kid-numbers-on-sales-documents"></a><span data-ttu-id="fa2db-103">Opprette KID-numre for salgsdokumenter</span><span class="sxs-lookup"><span data-stu-id="fa2db-103">How to: Set Up KID Numbers on Sales Documents</span></span>
<span data-ttu-id="fa2db-104">Kunde-ID (KID) er et kundeidentifikasjonsnummer som inneholder en betalingsreferanse til leverandøren, og sikrer at betalingen bokføres riktig hos leverandøren.</span><span class="sxs-lookup"><span data-stu-id="fa2db-104">Kunde ID (KID) is a customer identification number that provides a payment reference to the vendor and ensures that the vendor is posting the payment correctly.</span></span> <span data-ttu-id="fa2db-105">Du kan opprette KID-numre på salgsdokumenter for å identifisere bilags- og kundeinformasjon ved elektroniske banktransaksjoner.</span><span class="sxs-lookup"><span data-stu-id="fa2db-105">You can set up KID numbers on sales documents to identify document and customer information on electronic banking transactions.</span></span>  

## <a name="to-set-up-kid-numbers-on-sales-documents"></a><span data-ttu-id="fa2db-106">Slik oppretter du KID-numre på salgsdokumenter</span><span class="sxs-lookup"><span data-stu-id="fa2db-106">To set up KID numbers on sales documents</span></span>  

1.  <span data-ttu-id="fa2db-107">Velg ikonet ![Søk etter side eller rapport](../../media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Salgsoppsett**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="fa2db-107">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="fa2db-108">I hurtigfanen **Dokumenter** fyller du ut feltene som beskrevet i tabellen nedenfor.</span><span class="sxs-lookup"><span data-stu-id="fa2db-108">On the **Documents** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="fa2db-109">Felt</span><span class="sxs-lookup"><span data-stu-id="fa2db-109">Field</span></span>|<span data-ttu-id="fa2db-110">Description</span><span class="sxs-lookup"><span data-stu-id="fa2db-110">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="fa2db-111">**KID-oppsett**</span><span class="sxs-lookup"><span data-stu-id="fa2db-111">**KID Setup**</span></span>|<span data-ttu-id="fa2db-112">Angir et KID-nummerformat.</span><span class="sxs-lookup"><span data-stu-id="fa2db-112">Specifies a KID number format.</span></span>|  
    |<span data-ttu-id="fa2db-113">**Bilagsnr.lengde**</span><span class="sxs-lookup"><span data-stu-id="fa2db-113">**Document No. length**</span></span>|<span data-ttu-id="fa2db-114">Angi hvor mange sifre som skal brukes i bilagsnummeret.</span><span class="sxs-lookup"><span data-stu-id="fa2db-114">Enter the number of digits used for the document number.</span></span>|  
    |<span data-ttu-id="fa2db-115">**Kundenr.lengde**</span><span class="sxs-lookup"><span data-stu-id="fa2db-115">**Customer No. length**</span></span>|<span data-ttu-id="fa2db-116">Angi hvor mange sifre som skal brukes i kundenummeret.</span><span class="sxs-lookup"><span data-stu-id="fa2db-116">Enter the number of digits used for the customer number.</span></span>|  
    |<span data-ttu-id="fa2db-117">**Bruk KID på rentenota**</span><span class="sxs-lookup"><span data-stu-id="fa2db-117">**Use KID on Fin. Charge Memo**</span></span>|<span data-ttu-id="fa2db-118">Velg å skrive ut KID-numre på rentenotaer.</span><span class="sxs-lookup"><span data-stu-id="fa2db-118">Select to print KID numbers on finance charge memos.</span></span> <span data-ttu-id="fa2db-119">**Obs!**  Hvis dette alternativet er valgt, må du også velge formatet **Bilagstype + bilagsnr.** i feltet **KID-oppsett**.</span><span class="sxs-lookup"><span data-stu-id="fa2db-119">**Note:**  If selected, then you must also select the **Document Type + Document No.** format in the **KID Setup** field.</span></span>|  
    |<span data-ttu-id="fa2db-120">**Bruk KID på purring**</span><span class="sxs-lookup"><span data-stu-id="fa2db-120">**Use KID on Reminder**</span></span>|<span data-ttu-id="fa2db-121">Velg å skrive ut KID-numre på purringer.</span><span class="sxs-lookup"><span data-stu-id="fa2db-121">Select to print KID numbers on reminders.</span></span> <span data-ttu-id="fa2db-122">**Obs!**  Hvis dette alternativet er valgt, må du også velge formatet **Bilagstype + bilagsnr.** i feltet **KID-oppsett**.</span><span class="sxs-lookup"><span data-stu-id="fa2db-122">**Note:**  If selected, then you must also select the **Document Type + Document No.** format in the **KID Setup** field.</span></span>|  
    |<span data-ttu-id="fa2db-123">**Skriv ut kvittering på giro**</span><span class="sxs-lookup"><span data-stu-id="fa2db-123">**Print Receipt on Giro**</span></span>|<span data-ttu-id="fa2db-124">Velg å skrive ut kvitteringsdelen på salgsfakturaer, kreditnotaer, purringer eller rentenotaer. Du kan velge mellom flere ulike oppsettalternativer når du skal skrive ut kvitteringsdelen på salgsdokumenter som inneholder en giro.</span><span class="sxs-lookup"><span data-stu-id="fa2db-124">Select to print the receipt section on sales invoices, credit memos, reminders, or finance charge memos.There are several layout options available when printing the receipt section on sales documents that contain a Giro.</span></span> <span data-ttu-id="fa2db-125">Se [Norske salgsdokumenter](norwegian-sales-documents.md) for mer informasjon</span><span class="sxs-lookup"><span data-stu-id="fa2db-125">For more information, see [Norwegian Sales Documents](norwegian-sales-documents.md)</span></span>|  

3.  <span data-ttu-id="fa2db-126">Velg **OK**.</span><span class="sxs-lookup"><span data-stu-id="fa2db-126">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fa2db-127">Se også</span><span class="sxs-lookup"><span data-stu-id="fa2db-127">See Also</span></span>  
 <span data-ttu-id="fa2db-128">[Elektroniske banktjenester i Norge](electronic-banking-in-norway.md) </span><span class="sxs-lookup"><span data-stu-id="fa2db-128">[Electronic Banking in Norway](electronic-banking-in-norway.md) </span></span>  
 [<span data-ttu-id="fa2db-129">Norske salgsdokumenter</span><span class="sxs-lookup"><span data-stu-id="fa2db-129">Norwegian Sales Documents</span></span>](norwegian-sales-documents.md)

