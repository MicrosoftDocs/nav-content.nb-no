---
title: "Bruke fordelingsnøkler i finanskladder"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: ca21d9d129dbc98d75371d1b2b7a0ffad4aa2848
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---

#  <a name="how-to-use-allocation-keys-in-general-journals"></a><span data-ttu-id="6add3-102">Bruke fordelingsnøkler i finanskladder</span><span class="sxs-lookup"><span data-stu-id="6add3-102">How to: Use Allocation Keys in General Journals</span></span>
<span data-ttu-id="6add3-103">Du kan fordele en post i en finanskladd på flere forskjellige konti når du bokfører kladden.</span><span class="sxs-lookup"><span data-stu-id="6add3-103">You can allocate an entry in a general journal to several different accounts when you post the journal.</span></span> <span data-ttu-id="6add3-104">Fordelingen kan gjøres etter antall, prosent eller beløp.</span><span class="sxs-lookup"><span data-stu-id="6add3-104">The allocation can be made by quantity, percentage, or amount.</span></span>

## <a name="to-set-up-allocation-keys"></a><span data-ttu-id="6add3-105">Definere fordelingsnøkler</span><span class="sxs-lookup"><span data-stu-id="6add3-105">To set up allocation keys</span></span> 
1. <span data-ttu-id="6add3-106">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Gjentakende finanskladd** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="6add3-106">In the top right corner, choose the **Search for Page or Report** icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="6add3-107">Velg feltet **Bunkenavn** for å åpne vinduet **Finanskladder**.</span><span class="sxs-lookup"><span data-stu-id="6add3-107">Choose the **Batch Name** field to open the **General Journal Batches** window.</span></span>
3. <span data-ttu-id="6add3-108">Du kan endre fordelinger på en eksisterende bunke i listen, eller du kan opprette en ny bunke med tildelinger.</span><span class="sxs-lookup"><span data-stu-id="6add3-108">You can either modify allocations on an existing batch in the list or create a new batch with allocations.</span></span>
  * <span data-ttu-id="6add3-109">Hvis du vil opprette en ny bunke, velger du handlingen **Ny** og går til neste trinn.</span><span class="sxs-lookup"><span data-stu-id="6add3-109">To create a new batch, choose the **New** action, and go to the next step.</span></span>
  * <span data-ttu-id="6add3-110">Hvis du vil endre fordelinger for en eksisterende kladd, velger du kladden og går til trinn 7.</span><span class="sxs-lookup"><span data-stu-id="6add3-110">To change the allocations of an existing journal, select the journal and go to step 7.</span></span>    
4. <span data-ttu-id="6add3-111">I feltet **Navn** skriver du inn et navn på kladden, for eksempel RENGJØRING.</span><span class="sxs-lookup"><span data-stu-id="6add3-111">In the **Name** field, enter a name for the batch, such as CLEANING.</span></span> <span data-ttu-id="6add3-112">I feltet **Beskrivelse** angir du en beskrivelse som for eksempel Kladd for rengjøringsutgifter.</span><span class="sxs-lookup"><span data-stu-id="6add3-112">In the **Description** field, enter a description, such as Cleaning Expenses Journal.</span></span>
5. <span data-ttu-id="6add3-113">Når du er ferdig, lukker du vinduet.</span><span class="sxs-lookup"><span data-stu-id="6add3-113">When you are done, close the window.</span></span> <span data-ttu-id="6add3-114">En ny, tom gjentakende kladd åpnes.</span><span class="sxs-lookup"><span data-stu-id="6add3-114">A new, empty recurring journal opens.</span></span> 
6. <span data-ttu-id="6add3-115">Fyll ut feltene på linjen.</span><span class="sxs-lookup"><span data-stu-id="6add3-115">Fill in the fields in the line.</span></span>
7. <span data-ttu-id="6add3-116">Velg handlingen **Fordelinger**.</span><span class="sxs-lookup"><span data-stu-id="6add3-116">Choose the **Allocations** action.</span></span> 
8. <span data-ttu-id="6add3-117">Legg til en linje for hver fordeling.</span><span class="sxs-lookup"><span data-stu-id="6add3-117">Add a line for each allocation.</span></span> <span data-ttu-id="6add3-118">Du må fylle ut enten feltet **Andel i pst.**, **Andel i antall** eller **Beløp**.</span><span class="sxs-lookup"><span data-stu-id="6add3-118">You must fill in either the **Allocation %**, **Allocation Quantity**, or **Amount** field.</span></span> <span data-ttu-id="6add3-119">Du må også fylle ut **Kontonummer**</span><span class="sxs-lookup"><span data-stu-id="6add3-119">You must also fill in the **Account No.**</span></span> <span data-ttu-id="6add3-120">-feltet, og hvis du fordeler transaksjonen på globale dimensjoner, må du også fylle ut feltene for globale dimensjoner.</span><span class="sxs-lookup"><span data-stu-id="6add3-120">field and, if you are allocating the transaction among global dimensions, the global dimension fields.</span></span>
9. <span data-ttu-id="6add3-121">Hvis du angir en prosentsats på en linje, beregnes beløpet i feltet **Beløp** automatisk.</span><span class="sxs-lookup"><span data-stu-id="6add3-121">If you enter a percentage on a line, the amount in the **Amount** field is calculated automatically.</span></span> <span data-ttu-id="6add3-122">Disse beløpene har motsatt fortegn av det totale beløpet i feltet **Beløp** i den gjentakende kladden.</span><span class="sxs-lookup"><span data-stu-id="6add3-122">These amounts have the opposite sign from the total amount in the **Amount** field in the recurring journal.</span></span>
10. <span data-ttu-id="6add3-123">Når du har angitt fordelingslinjene, velger du **OK** for å gå tilbake til vinduet **Gjentakende finanskladd**.</span><span class="sxs-lookup"><span data-stu-id="6add3-123">After entering the allocations lines, choose **OK** to return to the **Recurring General Journal** window.</span></span> <span data-ttu-id="6add3-124">Feltet **Fordelt beløp (USD)** fylles ut og samsvarer med **Beløp**-feltet.</span><span class="sxs-lookup"><span data-stu-id="6add3-124">The **Allocated Amt. (USD)** field is filled in and matches the **Amount** field.</span></span>
11. <span data-ttu-id="6add3-125">Bokfør kladden.</span><span class="sxs-lookup"><span data-stu-id="6add3-125">Post the journal.</span></span>

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a><span data-ttu-id="6add3-126">Endre en fordelingsnøkkel som allerede er definert</span><span class="sxs-lookup"><span data-stu-id="6add3-126">To change an allocation key that has already been set up</span></span>
1. <span data-ttu-id="6add3-127">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Gjentakende finanskladd** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="6add3-127">In the top right corner, choose the **Search for Page or Report** icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="6add3-128">Velg kladden med fordelingen, i vinduet **Finansgjentak.kladd**.</span><span class="sxs-lookup"><span data-stu-id="6add3-128">In the **Recurring General Journal** window, select the journal with the allocation.</span></span>
3. <span data-ttu-id="6add3-129">Velg linjen med fordelingen, og velg deretter handlingen **Fordelinger**.</span><span class="sxs-lookup"><span data-stu-id="6add3-129">Choose the line with the allocation, and then choose **Allocations** action.</span></span>
4. <span data-ttu-id="6add3-130">Endre de relevante feltene, og lukk vinduet.</span><span class="sxs-lookup"><span data-stu-id="6add3-130">Change the relevant fields, and close the window.</span></span>

## <a name="see-also"></a><span data-ttu-id="6add3-131">Se også</span><span class="sxs-lookup"><span data-stu-id="6add3-131">See Also</span></span>
[<span data-ttu-id="6add3-132">Arbeide med finanskladder</span><span class="sxs-lookup"><span data-stu-id="6add3-132">Work With General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="6add3-133">Bokføre dokumenter og kladder</span><span class="sxs-lookup"><span data-stu-id="6add3-133">Post Documents and Journals</span></span>](ui-post-documents-journals.md)




