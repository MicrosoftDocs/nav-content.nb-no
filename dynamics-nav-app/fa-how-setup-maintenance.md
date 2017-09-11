---
title: Definere vedlikehold av aktiva
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: ace0fb13d2be71c7204f16f34f6b65b54ff98230
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-fixed-asset-maintenance"></a><span data-ttu-id="069c0-102">Definere vedlikehold av aktiva</span><span class="sxs-lookup"><span data-stu-id="069c0-102">How to: Set Up Fixed Asset Maintenance</span></span>
<span data-ttu-id="069c0-103">For å styre vedlikehold av aktiva, må du først definere noen generelle vedlikeholdsopplysninger, en bokføringskonto for vedlikeholdskostnader og vedlikeholdskoder for typer arbeid, for eksempel rutineservice eller reparasjon.</span><span class="sxs-lookup"><span data-stu-id="069c0-103">To manage fixed asset maintenance, you must first set up some general maintenance information, a posting account for maintenance costs, and maintenance codes for types of work, such as Routine Service or Repair.</span></span>

## <a name="to-set-up-general-maintenance-information"></a><span data-ttu-id="069c0-104">Slik definerer du generelle vedlikeholdsopplysninger:</span><span class="sxs-lookup"><span data-stu-id="069c0-104">To set up general maintenance information</span></span>
<span data-ttu-id="069c0-105">Hvis du definerer vedlikeholdsfeltene, kan du bokføre vedlikeholdsutgifter fra aktivakladden.</span><span class="sxs-lookup"><span data-stu-id="069c0-105">If you set up the fields for maintenance, you can post maintenance expenses from the fixed asset journal.</span></span>
1. <span data-ttu-id="069c0-106">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktiva** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="069c0-106">In the top right corner, choose the **Search for Page or Report** icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="069c0-107">Velg aktivaet du vil definere forsikringsdekning for, og velg deretter handlingen **Rediger**.</span><span class="sxs-lookup"><span data-stu-id="069c0-107">Select the fixed asset that you to define insurance coverage for, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="069c0-108">Fyll ut feltene på hurtigfanen **Vedlikehold** etter behov.</span><span class="sxs-lookup"><span data-stu-id="069c0-108">On the **Maintenance** FastTab, fill in the fields as necessary.</span></span> <span data-ttu-id="069c0-109">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="069c0-109">Choose a field to read a short description of the field or link to more information.</span></span>

## <a name="to-set-up-maintenance-codes"></a><span data-ttu-id="069c0-110">Slik definerer du vedlikeholdskoder</span><span class="sxs-lookup"><span data-stu-id="069c0-110">To set up maintenance codes</span></span>  
<span data-ttu-id="069c0-111">Når du bokfører vedlikeholdskostnader fra en finanskladd, fyller du ut feltet **Vedlikeholdskode** for å registrere hva slags vedlikehold som er utført, for eksempel rutineservice eller reparasjon.</span><span class="sxs-lookup"><span data-stu-id="069c0-111">When you post maintenance costs from a general journal, you fill in the **Maintenance Code** field to record what kind of maintenance has been performed, such as routine service or repair.</span></span>
1. <span data-ttu-id="069c0-112">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Vedlikehold** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="069c0-112">In the top right corner, choose the **Search for Page or Report** icon, enter **Maintenance**, and then choose the related link.</span></span>
2. <span data-ttu-id="069c0-113">I **Vedlikehold**-vinduet definerer du koder for ulike typer vedlikeholdsarbeid.</span><span class="sxs-lookup"><span data-stu-id="069c0-113">In the **Maintenance** window, set up codes for different types of maintenance work.</span></span>

## <a name="to-set-up-maintenance-expense-accounts"></a><span data-ttu-id="069c0-114">Slik definerer du utgiftskonti for vedlikehold</span><span class="sxs-lookup"><span data-stu-id="069c0-114">To set up maintenance expense accounts</span></span>  
<span data-ttu-id="069c0-115">Du må først angi et kontonummer i vinduet **Bokf.grupper - aktiva** for å kunne bokføre vedlikeholdskostnader.</span><span class="sxs-lookup"><span data-stu-id="069c0-115">To post maintenance costs, you must first enter an account number in the **FA Posting Groups** window.</span></span>
1. <span data-ttu-id="069c0-116">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Bokf.grupper - aktiva** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="069c0-116">In the top right corner, choose the **Search for Page or Report** icon, enter **FA Posting Groups**, and then choose the related link.</span></span>
2. <span data-ttu-id="069c0-117">Fyll ut feltet **Konto for vedlikeholdsutgifter** for hver enkelt bokføringsgruppe.</span><span class="sxs-lookup"><span data-stu-id="069c0-117">Fill in the **Maintenance Expense Account** field for each posting group.</span></span>

<span data-ttu-id="069c0-118">**Merk** Hvis du vil definere at vedlikeholdskostnader fordeles til avdelinger eller prosjekter, må du definere en fordelingsnøkkel.</span><span class="sxs-lookup"><span data-stu-id="069c0-118">**Note**: To define that maintenance costs are allocated to departments or projects, set up an allocation keys.</span></span> <span data-ttu-id="069c0-119">Se [Definere generelle aktivafunksjoner](fa-how-setup-general.md) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="069c0-119">For more information, see [How to: Set Up General Fixed Assets Features](fa-how-setup-general.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="069c0-120">Se også</span><span class="sxs-lookup"><span data-stu-id="069c0-120">See Also</span></span>
[<span data-ttu-id="069c0-121">Definere aktiva</span><span class="sxs-lookup"><span data-stu-id="069c0-121">Set Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="069c0-122">Administrere aktiva</span><span class="sxs-lookup"><span data-stu-id="069c0-122">Manage Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="069c0-123">Finans</span><span class="sxs-lookup"><span data-stu-id="069c0-123">Finance</span></span>](finance-setup.md)  
[<span data-ttu-id="069c0-124">Velkommen til Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="069c0-124">Welcome to Dynamics NAV</span></span>](across-get-started.md)

