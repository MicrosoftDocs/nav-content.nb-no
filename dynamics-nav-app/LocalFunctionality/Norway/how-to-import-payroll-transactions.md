---
title: "Lese inn lønnstransaksjoner"
description: "Du kan importere lønnstransaksjoner til en finanskladd fra to eksterne lønnslisteløsninger."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 02a1b9f99e5d282740fc4ff2e1db0c91a098fd51
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-import-payroll-transactions"></a><span data-ttu-id="a8621-103">Lese inn lønnstransaksjoner</span><span class="sxs-lookup"><span data-stu-id="a8621-103">How to: Import Payroll Transactions</span></span>
<span data-ttu-id="a8621-104">Du kan importere lønnstransaksjoner til en finanskladd fra to eksterne lønnslisteløsninger: Huldt & Lillevik og Hogia.</span><span class="sxs-lookup"><span data-stu-id="a8621-104">You can import payroll transactions into a general journal from two external payroll solutions: Huldt & Lillevik and Hogia.</span></span> <span data-ttu-id="a8621-105">Deretter kan du bruke finanskladden til å bokføre de importerte lønnstransaksjonene i finanskladdekontoer eller bankkontoer.</span><span class="sxs-lookup"><span data-stu-id="a8621-105">You can then use the general journal to post the imported payroll transactions to general ledger accounts or bank accounts.</span></span> <span data-ttu-id="a8621-106">Du må opprette lønnsintegrasjon før du kan importere lønnstransaksjoner.</span><span class="sxs-lookup"><span data-stu-id="a8621-106">To import payroll transactions, you must first set up payroll integration.</span></span>  

## <a name="to-set-up-payroll-integration"></a><span data-ttu-id="a8621-107">Slik oppretter du lønnsintegrasjon</span><span class="sxs-lookup"><span data-stu-id="a8621-107">To set up payroll integration</span></span>  

1.  <span data-ttu-id="a8621-108">Velg ikonet ![Søk etter side eller rapport](../../media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Oppsett lønnsintegrasjon**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="a8621-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payroll Integration Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="a8621-109">I hurtigfanen **Generelt** fyller du ut feltene som beskrevet i tabellen nedenfor.</span><span class="sxs-lookup"><span data-stu-id="a8621-109">On the **General** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="a8621-110">Felt</span><span class="sxs-lookup"><span data-stu-id="a8621-110">Field</span></span>|<span data-ttu-id="a8621-111">Description</span><span class="sxs-lookup"><span data-stu-id="a8621-111">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="a8621-112">**Lønnssystem**</span><span class="sxs-lookup"><span data-stu-id="a8621-112">**Payroll System**</span></span>|<span data-ttu-id="a8621-113">Velg et lønnssystem.</span><span class="sxs-lookup"><span data-stu-id="a8621-113">Select a payroll system.</span></span>|  
    |<span data-ttu-id="a8621-114">**Filnavn**</span><span class="sxs-lookup"><span data-stu-id="a8621-114">**File Name**</span></span>|<span data-ttu-id="a8621-115">Skriv inn hele banen til filen.</span><span class="sxs-lookup"><span data-stu-id="a8621-115">Enter the full path of the file.</span></span>|  
    |<span data-ttu-id="a8621-116">**Lagre lønnsfil**</span><span class="sxs-lookup"><span data-stu-id="a8621-116">**Save Payroll File**</span></span>|<span data-ttu-id="a8621-117">Velg dette alternativet for å lagre lønnsfila.</span><span class="sxs-lookup"><span data-stu-id="a8621-117">Select to save the payroll file.</span></span>|  
    |<span data-ttu-id="a8621-118">**Importer avdeling og prosjekt**</span><span class="sxs-lookup"><span data-stu-id="a8621-118">**Import Department and Project**</span></span>|<span data-ttu-id="a8621-119">Velg dette alternativet for å importere informasjon om avdeling og prosjekt.</span><span class="sxs-lookup"><span data-stu-id="a8621-119">Select to import department and project information.</span></span>|  
    |<span data-ttu-id="a8621-120">**Kladdemalnavn**</span><span class="sxs-lookup"><span data-stu-id="a8621-120">**Journal Template Name**</span></span>|<span data-ttu-id="a8621-121">Angi navnet på kladdemalen.</span><span class="sxs-lookup"><span data-stu-id="a8621-121">Select the name of the journal template.</span></span>|  
    |<span data-ttu-id="a8621-122">**Kladdenavn**</span><span class="sxs-lookup"><span data-stu-id="a8621-122">**Journal Name**</span></span>|<span data-ttu-id="a8621-123">Velg kladden som lønnstransaksjonene skal importeres til:</span><span class="sxs-lookup"><span data-stu-id="a8621-123">Select a journal to receive the imported payroll transactions.</span></span>|  
    |<span data-ttu-id="a8621-124">**Bokfør i**</span><span class="sxs-lookup"><span data-stu-id="a8621-124">**Post to**</span></span>|<span data-ttu-id="a8621-125">Velg kontotypen som lønnstransaksjonene skal bokføres i.</span><span class="sxs-lookup"><span data-stu-id="a8621-125">Select the account type to post the payroll transactions to.</span></span> <span data-ttu-id="a8621-126">Kontotyper inkluderer **Finanskonto** og **Bankkonto**.</span><span class="sxs-lookup"><span data-stu-id="a8621-126">Account types include **G/L Account** and **Bank Account**.</span></span>|  

3.  <span data-ttu-id="a8621-127">Velg **OK**.</span><span class="sxs-lookup"><span data-stu-id="a8621-127">Choose the **OK** button.</span></span>  

## <a name="to-import-payroll-transactions"></a><span data-ttu-id="a8621-128">Slik importerer du lønnstransaksjoner</span><span class="sxs-lookup"><span data-stu-id="a8621-128">To import payroll transactions</span></span>  

1.  <span data-ttu-id="a8621-129">Velg ikonet ![Søk etter side eller rapport](../../media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Finanskladder**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="a8621-129">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journals**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="a8621-130">Velg handlingen **Importer lønnskostnad**.</span><span class="sxs-lookup"><span data-stu-id="a8621-130">Choose the **Import Payroll** action.</span></span>  
3.  <span data-ttu-id="a8621-131">I hurtigfanen **Alternativer** fyller du ut feltene som beskrevet i tabellen nedenfor.</span><span class="sxs-lookup"><span data-stu-id="a8621-131">On the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="a8621-132">Felt</span><span class="sxs-lookup"><span data-stu-id="a8621-132">Field</span></span>|<span data-ttu-id="a8621-133">Description</span><span class="sxs-lookup"><span data-stu-id="a8621-133">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="a8621-134">**Bokføringsdato**</span><span class="sxs-lookup"><span data-stu-id="a8621-134">**Posting Date**</span></span>|<span data-ttu-id="a8621-135">Velg et lønnssystem.</span><span class="sxs-lookup"><span data-stu-id="a8621-135">Select a payroll system.</span></span>|  
    |<span data-ttu-id="a8621-136">**Bilagstekst**</span><span class="sxs-lookup"><span data-stu-id="a8621-136">**Document text**</span></span>|<span data-ttu-id="a8621-137">Skriv inn hele banen til filen.</span><span class="sxs-lookup"><span data-stu-id="a8621-137">Enter the full path of the file.</span></span>|  
    |<span data-ttu-id="a8621-138">**Filnavn**</span><span class="sxs-lookup"><span data-stu-id="a8621-138">**File Name**</span></span>|<span data-ttu-id="a8621-139">Angi filnavnet til lønnsfilen.</span><span class="sxs-lookup"><span data-stu-id="a8621-139">Specify the file name for the payroll file.</span></span>|  

4.  <span data-ttu-id="a8621-140">Velg **OK**.</span><span class="sxs-lookup"><span data-stu-id="a8621-140">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a8621-141">Se også</span><span class="sxs-lookup"><span data-stu-id="a8621-141">See Also</span></span>  
 [<span data-ttu-id="a8621-142">Funksjonalitet som er spesifikk for norske brukere</span><span class="sxs-lookup"><span data-stu-id="a8621-142">Norway Local Functionality</span></span>](norway-local-functionality.md)

