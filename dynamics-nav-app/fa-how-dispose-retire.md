---
title: Avhende eller trekke tilbake aktiva
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
ms.openlocfilehash: 795bb23e7c0b46be095b2bbdfe7705b3d7b1e4ee
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-dispose-of-or-retire-fixed-assets"></a><span data-ttu-id="9f441-102">Avhende eller trekke tilbake aktiva</span><span class="sxs-lookup"><span data-stu-id="9f441-102">How to: Dispose of or Retire Fixed Assets</span></span>
<span data-ttu-id="9f441-103">Når du selger eller på annen måte avhender et aktiva, må salgsverdien bokføres for å beregne og registrere tap eller vinning.</span><span class="sxs-lookup"><span data-stu-id="9f441-103">When you sell or otherwise dispose of a fixed asset, the disposal value must be posted to calculate and record the gain or loss.</span></span> <span data-ttu-id="9f441-104">En salgspost må være den siste posten som bokføres for et aktiva.</span><span class="sxs-lookup"><span data-stu-id="9f441-104">A disposal entry must be the last entry posted for a fixed asset.</span></span> <span data-ttu-id="9f441-105">Du kan bokføre mer enn én salgspost for aktiva som er delvis solgt.</span><span class="sxs-lookup"><span data-stu-id="9f441-105">For partially disposed fixed assets, you can post more than one disposal entry.</span></span> <span data-ttu-id="9f441-106">Summen av alle bokførte salgsbeløp må være et kreditbeløp.</span><span class="sxs-lookup"><span data-stu-id="9f441-106">The total of all posted disposal amounts must be a credit amount.</span></span>

 <span data-ttu-id="9f441-107">**Merk**: Hvis du bytter ut et aktiva med et annet, må du registrere både salget av det gamle aktivaet og innkjøpet av det nye (anskaffelsen).</span><span class="sxs-lookup"><span data-stu-id="9f441-107">**NOTE**: If you trade in a fixed asset for another one, you must record both the sale of the old asset (disposal) and the purchase of the new one (acquisition).</span></span> <span data-ttu-id="9f441-108">Hvis du vil ha mer informasjon, se [Anskaffe aktiva](fa-how-acquire.md).</span><span class="sxs-lookup"><span data-stu-id="9f441-108">For more information, see [How to: Acquire Fixed Assets](fa-how-acquire.md).</span></span>

## <a name="to-post-a-disposal-from-the-fixed-asset-gl-journal"></a><span data-ttu-id="9f441-109">Slik bokfører du et salg fra aktivafinanskladden:</span><span class="sxs-lookup"><span data-stu-id="9f441-109">To post a disposal from the fixed asset G/L journal</span></span>  
1. <span data-ttu-id="9f441-110">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktivafinanskladder** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="9f441-110">In the top right corner, choose the **Search for Page or Report** icon, enter **FA G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="9f441-111">Opprett en innledende kladdelinje, og fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="9f441-111">Create an initial journal line and fill in the fields as necessary.</span></span> <span data-ttu-id="9f441-112">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="9f441-112">Choose a field to read a short description of the field or link to more information.</span></span>
3. <span data-ttu-id="9f441-113">I feltet **Aktivabokf.type** velger du **Salg**.</span><span class="sxs-lookup"><span data-stu-id="9f441-113">In the **FA Posting Type** field, select **Disposal**.</span></span>
4. <span data-ttu-id="9f441-114">Velg **Sett inn aktivamotkonto**.</span><span class="sxs-lookup"><span data-stu-id="9f441-114">Choose the **Insert FA Bal. Account** action.</span></span> <span data-ttu-id="9f441-115">En ny kladdelinje opprettes for motkontoen som er satt opp for salgsbokføring.</span><span class="sxs-lookup"><span data-stu-id="9f441-115">A second journal line is created for the balancing account that is set up for disposal posting.</span></span>

    <span data-ttu-id="9f441-116">**Merk**: Trinn 4 fungerer bare hvis du har definert følgende: I vinduet **Kort for bokf.grp.- aktiva** for bokføringsgruppen for aktivaet, inneholder **Konto for salg**-feltet finansdebetkontoen og **Motkonto for salg**-feltet inneholder finanskontoen du vil bokføre motposter for oppskrivning til.</span><span class="sxs-lookup"><span data-stu-id="9f441-116">**Note**: Step 4 only works if you have set up the following: In the **FA Posting Group Card** window for the posting group of the fixed asset, the **Disposal Account** field contains the general ledger debit account and the **Disposal Bal. Account** field contains the general ledger account to which you want to post balancing entries for appreciation.</span></span> <span data-ttu-id="9f441-117">Hvis du vil ha mer informasjon, kan du se "Definere bokføringsgrupper for aktiva" i [Definere generell aktivainformasjon](fa-how-setup-general.md).</span><span class="sxs-lookup"><span data-stu-id="9f441-117">For more information, see the "To set up fixed asset posting groups" section in [How to: Set Up General Fixed Asset Information](fa-how-setup-general.md).</span></span>
5. <span data-ttu-id="9f441-118">Velg handlingen **Bokfør**.</span><span class="sxs-lookup"><span data-stu-id="9f441-118">Choose the **Post** action.</span></span>

<span data-ttu-id="9f441-119">Hvis du selger eller på avhender deler av et aktiva, må du dele opp aktivaet før du kan registrere salgstransaksjonen.</span><span class="sxs-lookup"><span data-stu-id="9f441-119">If you sell or dispose of part of a fixed asset, you must split up the asset before you can record the disposal transaction.</span></span> <span data-ttu-id="9f441-120">Hvis du vil ha mer informasjon, se [Overføre, dele opp eller kombinere aktiva](fa-how-trans-split-combine.md).</span><span class="sxs-lookup"><span data-stu-id="9f441-120">For more information, see [How to: Transfer, Split, or Combine Fixed Assets](fa-how-trans-split-combine.md).</span></span>

## <a name="to-view-disposal-ledger-entries"></a><span data-ttu-id="9f441-121">Slik viser du salgsposter</span><span class="sxs-lookup"><span data-stu-id="9f441-121">To view disposal ledger entries</span></span>  
<span data-ttu-id="9f441-122">Når du selger eller avhender et aktiva, bokføres salgsverdien til finans der du kan se resultatet.</span><span class="sxs-lookup"><span data-stu-id="9f441-122">When you sell or dispose of a fixed asset, the disposal value is posted to the general ledger where you can view the result.</span></span>   

1. <span data-ttu-id="9f441-123">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktiva** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="9f441-123">In the top right corner, choose the **Search for Page or Report** icon, enter **Fixed Assets**, and then choose the related link.</span></span>  
2. <span data-ttu-id="9f441-124">Velg aktivaet du vil vise poster for, og velg deretter **Avskrivningstablåer**.</span><span class="sxs-lookup"><span data-stu-id="9f441-124">Select the fixed asset that you want to view entries for, and then choose the **Depreciation Books** action.</span></span>
3. <span data-ttu-id="9f441-125">Velg avskrivningstablået du vil vise poster for, og velg deretter **Poster**.</span><span class="sxs-lookup"><span data-stu-id="9f441-125">Select the depreciation book that you want to view entries for, and then choose the **Ledger Entries** action.</span></span>
4. <span data-ttu-id="9f441-126">Velg en linje med **Salg** i **Bokføringskategori, aktiva**-feltet, og velg deretter **Naviger**.</span><span class="sxs-lookup"><span data-stu-id="9f441-126">Select a line with **Disposal** in the **FA Posting Category** field, and then choose the **Navigate** action.</span></span>  
5. <span data-ttu-id="9f441-127">I **Naviger**-vinduet velger du finanspostlinjen og deretter **Vis**.</span><span class="sxs-lookup"><span data-stu-id="9f441-127">In the **Navigate** window, select the general ledger entry line, and then choose the **Show** action.</span></span>
<span data-ttu-id="9f441-128">**Finansposter**-vinduet åpnes der du kan se postene som er resultat av salgsbokføringen.</span><span class="sxs-lookup"><span data-stu-id="9f441-128">The **General Ledger Entries** window opens where you can see the entries that the disposal posting resulted in.</span></span>

## <a name="see-also"></a><span data-ttu-id="9f441-129">Se også</span><span class="sxs-lookup"><span data-stu-id="9f441-129">See Also</span></span>
[<span data-ttu-id="9f441-130">Administrere aktiva</span><span class="sxs-lookup"><span data-stu-id="9f441-130">Manage Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="9f441-131">Definere aktiva</span><span class="sxs-lookup"><span data-stu-id="9f441-131">Set Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="9f441-132">Finans</span><span class="sxs-lookup"><span data-stu-id="9f441-132">Finance</span></span>](finance-setup.md)  
[<span data-ttu-id="9f441-133">Velkommen til Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="9f441-133">Welcome to Dynamics NAV</span></span>](across-get-started.md)

