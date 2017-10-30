---
title: Sette opp kunder for EHF
description: "Hvis du vil opprette dokumenter i Elektronisk Handelsformat (EHF) for kunder i offentlig sektor, må du legge til EHF-informasjon for de aktuelle kundene."
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
ms.openlocfilehash: 889cf2defc40a21a0db258c857f676396676a319
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-customers-for-ehf"></a><span data-ttu-id="886ae-103">Sette opp kunder for EHF</span><span class="sxs-lookup"><span data-stu-id="886ae-103">How to: Set Up Customers for EHF</span></span>
<span data-ttu-id="886ae-104">Hvis du vil opprette dokumenter i Elektronisk Handelsformat (EHF) for kunder i offentlig sektor, må du legge til EHF-informasjon for de aktuelle kundene.</span><span class="sxs-lookup"><span data-stu-id="886ae-104">To create Elektronisk Handelsformat (EHF) documents for customers in the public sector, you must add EHF information to the relevant customers.</span></span>  

<span data-ttu-id="886ae-105">Dette emnet beskriver bare felt som gjelder EHF.</span><span class="sxs-lookup"><span data-stu-id="886ae-105">This topic only describes fields that apply to EHF.</span></span> <span data-ttu-id="886ae-106">Hvis du vil ha mer informasjon om hvordan du konfigurerer kunder generelt, se [Registrere nye kunder](how-to-register-new-customers.md).</span><span class="sxs-lookup"><span data-stu-id="886ae-106">For more information on setting up customers, in general, see [How to: Register New Customers](how-to-register-new-customers.md).</span></span>  

## <a name="to-set-up-a-customer-that-uses-elektronisk-handelsformat"></a><span data-ttu-id="886ae-107">Slik definerer du en kunde som bruker Elektronisk Handelsformat:</span><span class="sxs-lookup"><span data-stu-id="886ae-107">To set up a customer that uses Elektronisk Handelsformat</span></span>  

1.  <span data-ttu-id="886ae-108">Velg ikonet ![Søk etter side eller rapport](../../media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Kunder**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="886ae-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="886ae-109">Åpne kunden du vil aktivere for EHF.</span><span class="sxs-lookup"><span data-stu-id="886ae-109">Open the customer that you want to enable for EHF.</span></span>  
3.  <span data-ttu-id="886ae-110">I hurtigfanen **Fakturering** fyller du ut feltene som beskrevet i tabellen nedenfor.</span><span class="sxs-lookup"><span data-stu-id="886ae-110">On the **Invoicing** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="886ae-111">Felt</span><span class="sxs-lookup"><span data-stu-id="886ae-111">Field</span></span>|<span data-ttu-id="886ae-112">Description</span><span class="sxs-lookup"><span data-stu-id="886ae-112">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="886ae-113">**GLN**</span><span class="sxs-lookup"><span data-stu-id="886ae-113">**GLN**</span></span>|<span data-ttu-id="886ae-114">Påkrevd.</span><span class="sxs-lookup"><span data-stu-id="886ae-114">Required.</span></span> <span data-ttu-id="886ae-115">Angi det globale lokasjonsnummeret (GLN) for kunden.</span><span class="sxs-lookup"><span data-stu-id="886ae-115">Enter the Global Location Number (GLN) for the customer.</span></span>|  
    |<span data-ttu-id="886ae-116">**Kontokode**</span><span class="sxs-lookup"><span data-stu-id="886ae-116">**Account Code**</span></span>|<span data-ttu-id="886ae-117">Angi kontokoden for kunden.</span><span class="sxs-lookup"><span data-stu-id="886ae-117">Enter the account code for the customer.</span></span><br /><br /> <span data-ttu-id="886ae-118">Kunder i offentlig sektor gir en kontokode når de plasserer en ordre eller rekvisisjon.</span><span class="sxs-lookup"><span data-stu-id="886ae-118">Customers in the public sector provide an account code when they place an order or requisition.</span></span> <span data-ttu-id="886ae-119">Basert på verdien i dette feltet, inkluderes kontokoden i EHF-dokumentene du oppretter i [!INCLUDE[navnow](../../includes/navnow_md.md)].</span><span class="sxs-lookup"><span data-stu-id="886ae-119">Based on the value of this field, the account code is included in the EHF documents that you create in [!INCLUDE[navnow](../../includes/navnow_md.md)].</span></span> <span data-ttu-id="886ae-120">Se Kontokode for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="886ae-120">For more information, see Account Code.</span></span>|  
    |<span data-ttu-id="886ae-121">**E-faktura**</span><span class="sxs-lookup"><span data-stu-id="886ae-121">**E-Invoice**</span></span>|<span data-ttu-id="886ae-122">Merk av for å bruke elektronisk fakturering med kunden.</span><span class="sxs-lookup"><span data-stu-id="886ae-122">Select the check box to use electronic invoicing with this customer.</span></span>|  
    |<span data-ttu-id="886ae-123">**Ansvarssenter**</span><span class="sxs-lookup"><span data-stu-id="886ae-123">**Responsibility Center**</span></span>|<span data-ttu-id="886ae-124">Kontroller at ansvarssenteret du har valgt, har angitt en lands-/regionkode.</span><span class="sxs-lookup"><span data-stu-id="886ae-124">Make sure that the Responsibility Center that you have selected has a Country/Region Code specified.</span></span>|  

<span data-ttu-id="886ae-125">Disse feltene er spesifikke for EHF.</span><span class="sxs-lookup"><span data-stu-id="886ae-125">These fields are specific to EHF.</span></span> <span data-ttu-id="886ae-126">Verdiene brukes i alle EHF-dokumenter du oppretter for denne kunden.</span><span class="sxs-lookup"><span data-stu-id="886ae-126">The values are used in all EHF documents that you create for this customer.</span></span> <span data-ttu-id="886ae-127">Hvis du vil ha mer informasjon, se [EHF – Elektronisk fakturering i Norge](ehf-electronic-invoicing-in-norway.md).</span><span class="sxs-lookup"><span data-stu-id="886ae-127">For more information, see [EHF Electronic Invoicing in Norway](ehf-electronic-invoicing-in-norway.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="886ae-128">Se også</span><span class="sxs-lookup"><span data-stu-id="886ae-128">See Also</span></span>  
 <span data-ttu-id="886ae-129">[Opprette elektroniske dokumenter for EHF](how-to-create-electronic-documents-for-ehf.md) </span><span class="sxs-lookup"><span data-stu-id="886ae-129">[How to: Create Electronic Documents for EHF](how-to-create-electronic-documents-for-ehf.md) </span></span>  
 [<span data-ttu-id="886ae-130">Sette opp EHF</span><span class="sxs-lookup"><span data-stu-id="886ae-130">How to: Set Up EHF</span></span>](how-to-set-up-ehf.md)

