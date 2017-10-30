---
title: "Bruke én mva-kode i kladder"
description: "I Norge kan du bruke funksjonen for én mva-kode i en kladd, slik at du kan bokføre mva ved hjelp av ett enkelt felt, **Mva-kode**."
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
ms.openlocfilehash: 46e4b780df7ae8fe795a6732d91879970f356f20
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-use-one-vat-code-in-journals"></a><span data-ttu-id="1ff6c-103">Bruke én mva-kode i kladder</span><span class="sxs-lookup"><span data-stu-id="1ff6c-103">How to: Use One VAT Code in Journals</span></span>
<span data-ttu-id="1ff6c-104">I Norge kan du bruke funksjonen for én mva-kode i en kladd, slik at du kan bokføre mva ved hjelp av ett enkelt felt, **Mva-kode**.</span><span class="sxs-lookup"><span data-stu-id="1ff6c-104">In Norway, you can use the feature one VAT code in a journal, so that you can post VAT by using a single field, **VAT Code**.</span></span> <span data-ttu-id="1ff6c-105">Når én mva-kode er konfigurert, er dette en rask måte å fylle ut mva-felt som brukes ofte.</span><span class="sxs-lookup"><span data-stu-id="1ff6c-105">After it is set up, the one VAT code is a quick way to fill in the commonly used VAT fields.</span></span>  

<span data-ttu-id="1ff6c-106">For å angi mva-koden for bestillinger og ordrer, må de tilsvarende mva-bokføringsgruppene for firma og mva-bokføringsgruppene for varer defineres.</span><span class="sxs-lookup"><span data-stu-id="1ff6c-106">To set up the VAT code for purchase orders and sales orders, the corresponding VAT business posting groups and the VAT product posting groups have to be defined.</span></span>  

<span data-ttu-id="1ff6c-107">Mva-satsen beregnes fra kombinasjonen av mva-firmabokføringsgrupper, kjøperinformasjon og mva-varebokføringsgrupper.</span><span class="sxs-lookup"><span data-stu-id="1ff6c-107">The VAT rate is calculated from the combination of VAT business posting groups, buyer information, and VAT product posting groups.</span></span>  

## <a name="to-create-a-vat-code"></a><span data-ttu-id="1ff6c-108">Slik oppretter du en mva-kode:</span><span class="sxs-lookup"><span data-stu-id="1ff6c-108">To create a VAT code</span></span>  

1.  <span data-ttu-id="1ff6c-109">Velg ikonet ![Søk etter side eller rapport](../../media/ui-search/search_small.png "Søk etter side eller rapport"), angi **VAT-koder**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="1ff6c-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Codes**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="1ff6c-110">Velg handlingen **Ny**.</span><span class="sxs-lookup"><span data-stu-id="1ff6c-110">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="1ff6c-111">Angi opplysninger i feltet **Kode**, **Bokføringstype** og **Beskrivelse** for hver mva-kode.</span><span class="sxs-lookup"><span data-stu-id="1ff6c-111">Enter information in the **Code**, **General Posting Type**, and **Description** fields for each VAT code.</span></span>  
4.  <span data-ttu-id="1ff6c-112">Velg **OK**-knappen for å lukke vinduet **Mva-koder**.</span><span class="sxs-lookup"><span data-stu-id="1ff6c-112">Choose the **OK** button to close the **VAT Codes** window.</span></span>  

 <span data-ttu-id="1ff6c-113">Fremgangsmåten nedenfor beskriver mva-bokføringsoppsettet.</span><span class="sxs-lookup"><span data-stu-id="1ff6c-113">he following procedure explains the VAT posting setup.</span></span>  

## <a name="to-set-up-vat-posting"></a><span data-ttu-id="1ff6c-114">Slik definerer du mva-bokføring:</span><span class="sxs-lookup"><span data-stu-id="1ff6c-114">To set up VAT posting</span></span>  

1.  <span data-ttu-id="1ff6c-115">Velg ikonet ![Søk etter side eller rapport](../../media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Mva-bokføringsoppsett**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="1ff6c-115">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **VAT Posting Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="1ff6c-116">Velg handlingen **Ny**.</span><span class="sxs-lookup"><span data-stu-id="1ff6c-116">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="1ff6c-117">I kortet **Mva-bokføringsoppsett** må du fylle ut følgende felt:</span><span class="sxs-lookup"><span data-stu-id="1ff6c-117">In the **VAT Posting Setup** card, fill in the following fields:</span></span>  

    - <span data-ttu-id="1ff6c-118">**Mva-bokføringsgruppe - firma**</span><span class="sxs-lookup"><span data-stu-id="1ff6c-118">**VAT Business Posting Group**</span></span>  
    - <span data-ttu-id="1ff6c-119">**Mva-bokføringsgruppe - vare**</span><span class="sxs-lookup"><span data-stu-id="1ff6c-119">**VAT Product Posting Group**</span></span>  
    - <span data-ttu-id="1ff6c-120">**Mva-type**</span><span class="sxs-lookup"><span data-stu-id="1ff6c-120">**VAT Identifier**</span></span>  
    - <span data-ttu-id="1ff6c-121">**Mva-prosent**</span><span class="sxs-lookup"><span data-stu-id="1ff6c-121">**VAT Percentage**</span></span>  
    - <span data-ttu-id="1ff6c-122">**Utgående mva-konto**</span><span class="sxs-lookup"><span data-stu-id="1ff6c-122">**Sales VAT Account**</span></span>  
    - <span data-ttu-id="1ff6c-123">**Inngående mva-konto**</span><span class="sxs-lookup"><span data-stu-id="1ff6c-123">**Purchase VAT Account**</span></span>  

4.  <span data-ttu-id="1ff6c-124">I feltet **Mva-kode** velger du en kode fra listen.</span><span class="sxs-lookup"><span data-stu-id="1ff6c-124">In the **VAT Code** field, select a code from the list.</span></span>  

<span data-ttu-id="1ff6c-125">Nå når du bokfører et dokument i finanskladden og lukker det, brukes informasjonen som er angitt i **Mva-bokføringsoppsett**-kortet.</span><span class="sxs-lookup"><span data-stu-id="1ff6c-125">Now, when you post a document in the general journal and close it, the information specified in the **VAT Posting Setup** card is applied.</span></span>  

<span data-ttu-id="1ff6c-126">For eksempel: mva-satsen som er bokført i kladden, defineres av oppsettet du har angitt i **Mva-bokføringsoppsett**-vinduet.</span><span class="sxs-lookup"><span data-stu-id="1ff6c-126">For example, the VAT rate posted in the journal is defined by the setup that you have specified in the **VAT Posting Setup** window.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="1ff6c-127">Feltet **Mva-kode** og **Motkonto-mva. - kode** er lagt til i kladden.</span><span class="sxs-lookup"><span data-stu-id="1ff6c-127">The **VAT Code** and the **Bal. VAT Code**  fields have been added to the journal.</span></span> <span data-ttu-id="1ff6c-128">**Motkonto-mva. - kode** er mva-koden som brukes til å beregne motkontoen.</span><span class="sxs-lookup"><span data-stu-id="1ff6c-128">The **Bal. VAT Code** is the VAT code that is used to calculate the balancing account.</span></span>  
>   
>  <span data-ttu-id="1ff6c-129">Det gjøres ingen endringer i bokføringen.</span><span class="sxs-lookup"><span data-stu-id="1ff6c-129">No changes are made to the posting.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1ff6c-130">Se også</span><span class="sxs-lookup"><span data-stu-id="1ff6c-130">See Also</span></span>  
 [<span data-ttu-id="1ff6c-131">Norske mva-koder</span><span class="sxs-lookup"><span data-stu-id="1ff6c-131">Norwegian VAT Codes</span></span>](norwegian-vat-codes.md)

