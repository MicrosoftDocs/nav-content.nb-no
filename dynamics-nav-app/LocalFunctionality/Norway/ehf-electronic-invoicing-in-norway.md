---
title: "EHF – Elektronisk fakturering i Norge"
description: "Selskaper som må sende salgsfakturaer og kreditnotaer elektronisk til norsk offentlig sektor i Elektronisk Handelsformat (EHF) basert på UBL (Universal Business Language)."
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
ms.openlocfilehash: c014c393b43608fdaf2ce5ec2e9c1b7e7f0d8ed9
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="ehf-electronic-invoicing-in-norway"></a><span data-ttu-id="1c11f-103">EHF – Elektronisk fakturering i Norge</span><span class="sxs-lookup"><span data-stu-id="1c11f-103">EHF Electronic Invoicing in Norway</span></span>
<span data-ttu-id="1c11f-104">Selskaper som må sende salgsfakturaer og kreditnotaer elektronisk til norsk offentlig sektor i Elektronisk Handelsformat (EHF) basert på UBL (Universal Business Language).</span><span class="sxs-lookup"><span data-stu-id="1c11f-104">Companies must send sales invoices and credit memos to the Norwegian public sector electronically in the Elektronisk Handelsformat (EHF) based on Universal Business Language (UBL).</span></span> <span data-ttu-id="1c11f-105">Hvis et selskap ikke sender dokumentene elektronisk, kan myndighetene nekte betaling.</span><span class="sxs-lookup"><span data-stu-id="1c11f-105">If a company does not send these documents electronically, the authorities can deny payment.</span></span> <span data-ttu-id="1c11f-106">Standardformatet som støttes for elektronisk utveksling mellom parter, er formatet Ehandel.no.</span><span class="sxs-lookup"><span data-stu-id="1c11f-106">The standard supported format for electronic exchange between parties is the Ehandel.no format.</span></span>  

<span data-ttu-id="1c11f-107">Hvis du vil ha mer informasjon om elektronisk fakturering i EHF, kan du se [Implementeringsveiledning for EHF: Faktura og kreditnota](http://www.nets.eu/no-nb/support/Test%20og%20Implementering/eFaktura%20B2B%20Utsteder/Documents/Imp%20guide%20eng.pdf) og [EHF-faktura](http://www.anskaffelser.no/ehf-formater-innhold/pages-english/ehf-invoice).</span><span class="sxs-lookup"><span data-stu-id="1c11f-107">For more information on EHF electronic invoicing, see [EHF Implementation Guide: Invoice and Credit Note](http://www.nets.eu/no-nb/support/Test%20og%20Implementering/eFaktura%20B2B%20Utsteder/Documents/Imp%20guide%20eng.pdf) and [EHF Invoice](http://www.anskaffelser.no/ehf-formater-innhold/pages-english/ehf-invoice).</span></span>  

## <a name="implementation-in-includenavnowincludesnavnowmdmd"></a><span data-ttu-id="1c11f-108">Implementering i [!INCLUDE[navnow](../../includes/navnow_md.md)]</span><span class="sxs-lookup"><span data-stu-id="1c11f-108">Implementation in [!INCLUDE[navnow](../../includes/navnow_md.md)]</span></span>  
 <span data-ttu-id="1c11f-109">Gjeldende krav for å sende elektroniske fakturaer er basert på standarden Universal Business Language (UBL) versjon 2.1.</span><span class="sxs-lookup"><span data-stu-id="1c11f-109">The current requirements for sending electronic invoices are based on the Universal Business Language (UBL) version 2.1 standard.</span></span> <span data-ttu-id="1c11f-110">Hvis du vil ha mer informasjon, kan du se nettstedet til [OASIS UBL](http://go.microsoft.com/fwlink/?LinkId=212593).</span><span class="sxs-lookup"><span data-stu-id="1c11f-110">For more information, see the [OASIS UBL](http://go.microsoft.com/fwlink/?LinkId=212593) website.</span></span> <span data-ttu-id="1c11f-111">De genererte XML-dokumentene kan deretter sendes til kunden.</span><span class="sxs-lookup"><span data-stu-id="1c11f-111">The generated XML documents can then be sent to the customer.</span></span>  

 <span data-ttu-id="1c11f-112">Hvis du vil sende dokumenter elektronisk, må du tilordne EAN-lokasjonsnumre (European Article Numbering) og kontokoder til de aktuelle kundene i **Kundekort**-vinduet.</span><span class="sxs-lookup"><span data-stu-id="1c11f-112">To send documents electronically, you must assign European Article Numbering (EAN) location numbers and account codes to the relevant customers in the **Customer Card** window.</span></span> <span data-ttu-id="1c11f-113">Se [Sette opp kunder for EHF](how-to-set-up-customers-for-ehf.md) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="1c11f-113">For more information, see [How to: Set Up Customers for EHF](how-to-set-up-customers-for-ehf.md).</span></span> <span data-ttu-id="1c11f-114">Disse numrene inkluderes når du oppretter dokumenter, og bokfører eller utsteder dem.</span><span class="sxs-lookup"><span data-stu-id="1c11f-114">These numbers are included when you create documents, and post or issue them.</span></span> <span data-ttu-id="1c11f-115">Nå dokumentene er bokført eller utstedt, kan du opprette elektroniske versjoner som skal sendes til kunden.</span><span class="sxs-lookup"><span data-stu-id="1c11f-115">After the documents have been posted or issued, you can create electronic versions to be sent to the customer.</span></span>  

 [!INCLUDE[navnow](../../includes/navnow_md.md)]<span data-ttu-id="1c11f-116"> eksporterer enkelte elektroniske dokumenter i versjon 2.0, som bruker UBL versjon 2.1.</span><span class="sxs-lookup"><span data-stu-id="1c11f-116"> exports certain electronic documents in version 2.0, which uses UBL version 2.1.</span></span> <span data-ttu-id="1c11f-117">Du kan sende følgende typer dokumenter:</span><span class="sxs-lookup"><span data-stu-id="1c11f-117">You can submit the following types of documents:</span></span>  

- <span data-ttu-id="1c11f-118">Salgsfaktura</span><span class="sxs-lookup"><span data-stu-id="1c11f-118">Sales invoice</span></span>  
- <span data-ttu-id="1c11f-119">Servicefaktura</span><span class="sxs-lookup"><span data-stu-id="1c11f-119">Service invoice</span></span>  
- <span data-ttu-id="1c11f-120">Salgskreditnota</span><span class="sxs-lookup"><span data-stu-id="1c11f-120">Sales credit memo</span></span>  
- <span data-ttu-id="1c11f-121">Salgskreditnota (service)</span><span class="sxs-lookup"><span data-stu-id="1c11f-121">Service credit memo</span></span>  

 [!INCLUDE[navnow](../../includes/navnow_md.md)]<span data-ttu-id="1c11f-122"> eksporterer andre elektroniske dokumenter i versjon 1.6, som bruker UBL versjon 2.0.</span><span class="sxs-lookup"><span data-stu-id="1c11f-122"> exports other electronic documents in version 1.6, which uses UBL version 2.0.</span></span> <span data-ttu-id="1c11f-123">Du kan sende følgende typer dokumenter:</span><span class="sxs-lookup"><span data-stu-id="1c11f-123">You can submit the following types of documents:</span></span>  

- <span data-ttu-id="1c11f-124">Rentenota</span><span class="sxs-lookup"><span data-stu-id="1c11f-124">Finance charge memo</span></span>  
- <span data-ttu-id="1c11f-125">Purring</span><span class="sxs-lookup"><span data-stu-id="1c11f-125">Reminder</span></span>  

<span data-ttu-id="1c11f-126">De elektroniske dokumentene lagres i lokasjonene som defineres i vinduet Salgsoppsett.</span><span class="sxs-lookup"><span data-stu-id="1c11f-126">The electronic documents are stored in the locations that are defined in the Sales & Receivables Setup.</span></span>  

## <a name="vat-treatment"></a><span data-ttu-id="1c11f-127">Mva-justering</span><span class="sxs-lookup"><span data-stu-id="1c11f-127">VAT Treatment</span></span>  
 <span data-ttu-id="1c11f-128">Mva-prosenter og transaksjonstypen bestemmer mva-typen som eksporteres i det elektroniske dokumentet.</span><span class="sxs-lookup"><span data-stu-id="1c11f-128">VAT percentages and the type of transaction determine the VAT Type that is exported in the electronic document.</span></span>  

|<span data-ttu-id="1c11f-129">XML</span><span class="sxs-lookup"><span data-stu-id="1c11f-129">XML</span></span>|<span data-ttu-id="1c11f-130">Type</span><span class="sxs-lookup"><span data-stu-id="1c11f-130">Type</span></span>|<span data-ttu-id="1c11f-131">Prosentsats</span><span class="sxs-lookup"><span data-stu-id="1c11f-131">Percentage Rate</span></span>|  
|---------|----------|---------------------|  
|<span data-ttu-id="1c11f-132">S</span><span class="sxs-lookup"><span data-stu-id="1c11f-132">S</span></span>|<span data-ttu-id="1c11f-133">Utgående mva, vanlige sats</span><span class="sxs-lookup"><span data-stu-id="1c11f-133">Outgoing VAT, ordinary rate</span></span>|<span data-ttu-id="1c11f-134">25</span><span class="sxs-lookup"><span data-stu-id="1c11f-134">25</span></span>|  
|<span data-ttu-id="1c11f-135">H</span><span class="sxs-lookup"><span data-stu-id="1c11f-135">H</span></span>|<span data-ttu-id="1c11f-136">Utgående mva, redusert sats – matvarer og drikkevarer</span><span class="sxs-lookup"><span data-stu-id="1c11f-136">Outgoing VAT, reduced rate – food and beverage</span></span>|<span data-ttu-id="1c11f-137">15</span><span class="sxs-lookup"><span data-stu-id="1c11f-137">15</span></span>|  
|<span data-ttu-id="1c11f-138">R</span><span class="sxs-lookup"><span data-stu-id="1c11f-138">R</span></span>|<span data-ttu-id="1c11f-139">Utgående mva, redusert sats – rå fisk</span><span class="sxs-lookup"><span data-stu-id="1c11f-139">Outgoing VAT, reduced rate – raw fish</span></span>|<span data-ttu-id="1c11f-140">11.11</span><span class="sxs-lookup"><span data-stu-id="1c11f-140">11.11</span></span>|  
|<span data-ttu-id="1c11f-141">AA</span><span class="sxs-lookup"><span data-stu-id="1c11f-141">AA</span></span>|<span data-ttu-id="1c11f-142">Utgående mva, lav sats</span><span class="sxs-lookup"><span data-stu-id="1c11f-142">Outgoing VAT, low rate</span></span>|<span data-ttu-id="1c11f-143">8</span><span class="sxs-lookup"><span data-stu-id="1c11f-143">8</span></span>|  
|<span data-ttu-id="1c11f-144">Ø</span><span class="sxs-lookup"><span data-stu-id="1c11f-144">E</span></span>|<span data-ttu-id="1c11f-145">Mva-fritak</span><span class="sxs-lookup"><span data-stu-id="1c11f-145">VAT Exempt</span></span>|<span data-ttu-id="1c11f-146">0</span><span class="sxs-lookup"><span data-stu-id="1c11f-146">0</span></span>|  
|<span data-ttu-id="1c11f-147">Z</span><span class="sxs-lookup"><span data-stu-id="1c11f-147">Z</span></span>|<span data-ttu-id="1c11f-148">Mva-fritak (varer og tjenester som ikke omfattes av mva-bestemmelsene)</span><span class="sxs-lookup"><span data-stu-id="1c11f-148">VAT Exempt (goods and services not included in the VAT regulations)</span></span>|<span data-ttu-id="1c11f-149">Ingen, rapporteres som 0</span><span class="sxs-lookup"><span data-stu-id="1c11f-149">None, reported as 0</span></span>|  
|<span data-ttu-id="1c11f-150">K</span><span class="sxs-lookup"><span data-stu-id="1c11f-150">K</span></span>|<span data-ttu-id="1c11f-151">Utslippstillatelser for private og offentlige bedrifter – kjøperen beregner mva</span><span class="sxs-lookup"><span data-stu-id="1c11f-151">Emission allowances for private or public businesses – buyer calculates VAT</span></span>|<span data-ttu-id="1c11f-152">Ingen, rapporteres som 0</span><span class="sxs-lookup"><span data-stu-id="1c11f-152">None, reported as 0</span></span>|  

## <a name="see-also"></a><span data-ttu-id="1c11f-153">Se også</span><span class="sxs-lookup"><span data-stu-id="1c11f-153">See Also</span></span>  
 [<span data-ttu-id="1c11f-154">Sette opp kunder for EHF</span><span class="sxs-lookup"><span data-stu-id="1c11f-154">How to: Set Up Customers for EHF</span></span>](how-to-set-up-customers-for-ehf.md)

