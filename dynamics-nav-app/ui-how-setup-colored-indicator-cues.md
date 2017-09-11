---
title: Definere en farget indikator for bunke-ikoner
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
ms.openlocfilehash: 38cd904d0cf22374eac430d035e6ea6d205bcab8
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---
    
# <a name="how-to-set-up-a-colored-indicator-on-cues"></a><span data-ttu-id="9cf46-102">Definere en farget indikator for bunke-ikoner</span><span class="sxs-lookup"><span data-stu-id="9cf46-102">How to: Set Up a Colored Indicator on Cues</span></span>
<span data-ttu-id="9cf46-103">Du kan definere bunke-ikoner som vises på **Hjem**-siden med en indikator som endrer farge basert på dataverdiene i bunke-ikonene.</span><span class="sxs-lookup"><span data-stu-id="9cf46-103">You can set up Cues that appear on the **Home** page to include an indicator that changes color based on the data values in the Cues.</span></span> 

<span data-ttu-id="9cf46-104">Indikatoren vises som en farget linje langs øverste kant av bunkeflisen.</span><span class="sxs-lookup"><span data-stu-id="9cf46-104">The indicator appears as a colored bar along the top border of the Cue tile.</span></span> <span data-ttu-id="9cf46-105">Den gir et visuelt signal om statusen for aktiviteten for bunke-ikonet, som kan angi fordelaktige eller ufordelaktige tilstander som ber brukeren om å gjøre noe.</span><span class="sxs-lookup"><span data-stu-id="9cf46-105">It provides a visual signal of the status of the Cue's activity, which can indicate favorable or unfavorable conditions to prompt the user to take action.</span></span> <span data-ttu-id="9cf46-106">Hvis det for eksempel vises pågående salgsfakturaer på et bunke-ikon, kan du angi at indikatoren skal være grønn (fordelaktig) når antall pågående salgsfakturaer er under 10, og at den skal være rød (ufordelaktig) når det totale antallet er over 20.</span><span class="sxs-lookup"><span data-stu-id="9cf46-106">For example, if a Cue displays ongoing sales invoices, you can set up the indicator to appear green (favorable) when total number of ongoing sales invoices is below 10, and appears red (unfavorable) when the total is greater than 20.</span></span>

<span data-ttu-id="9cf46-107">Du bruker vinduet **Oppsett for bunke-ikon** til å definere indikatorer for alle bunke-ikonene som er tilgjengelige i selskapsdatabasen.</span><span class="sxs-lookup"><span data-stu-id="9cf46-107">From the **Cue Setup** window, you set up indicators for all the Cues that are available in the company database.</span></span>

<span data-ttu-id="9cf46-108">Hvis du vil definere indikatoren, kan du angi opptil to terskelverdier som definerer tre områder med dataverdier (lav, middels og høy) som du kan bruke en annen farge (eller stil) med.</span><span class="sxs-lookup"><span data-stu-id="9cf46-108">To set up the indicator, you specify up to two threshold values that define three ranges of data values (low, middle, and high) to which you can apply a different color (or style).</span></span>

## <a name="to-set-up-colored-indicators-on-cues"></a><span data-ttu-id="9cf46-109">Slik definerer du fargede indikatorer for bunke-ikoner</span><span class="sxs-lookup"><span data-stu-id="9cf46-109">To set up colored indicators on Cues</span></span>
1. <span data-ttu-id="9cf46-110">Under **Aktiviteter** på **Hjem**-siden, velger du **Definer bunke-ikoner**.</span><span class="sxs-lookup"><span data-stu-id="9cf46-110">Under **Activities** on your **Home** page, choose **Set Up Cues**.</span></span>  
<span data-ttu-id="9cf46-111">Vinduet **Oppsett for bunke-ikon** vises.</span><span class="sxs-lookup"><span data-stu-id="9cf46-111">The **Cue Setup** window appears.</span></span> <span data-ttu-id="9cf46-112">Vinduet viser indikatorer som er definert for bunke-ikoner.</span><span class="sxs-lookup"><span data-stu-id="9cf46-112">The window lists the indicators that are currently setup up on Cues.</span></span>
2. <span data-ttu-id="9cf46-113">Hvis du vil endre en indikator, redigerer du feltene og endrer for eksempel verdier for forskjellige terskler.</span><span class="sxs-lookup"><span data-stu-id="9cf46-113">To modify an indicator, edit the fields and modify, for example, the values for the different thresholds.</span></span>  

<span data-ttu-id="9cf46-114">Tabellen nedenfor viser fargene som tilsvarer alternativene i feltene **Stil for nedre område**, **Stil for midterste område** og **Stil for øvre område**.</span><span class="sxs-lookup"><span data-stu-id="9cf46-114">The following table lists the colors that correspond to the options of the **Low Range Style**, **Middle Range Style**, and **High Range Style** fields.</span></span>

|<span data-ttu-id="9cf46-115">Alternativ</span><span class="sxs-lookup"><span data-stu-id="9cf46-115">Option</span></span>|<span data-ttu-id="9cf46-116">Farge</span><span class="sxs-lookup"><span data-stu-id="9cf46-116">Color</span></span>|
|------|-----|
|<span data-ttu-id="9cf46-117">**Ingen**</span><span class="sxs-lookup"><span data-stu-id="9cf46-117">**None**</span></span>|<span data-ttu-id="9cf46-118">Ingen farge (samme farge som bunkeflisen</span><span class="sxs-lookup"><span data-stu-id="9cf46-118">No color (same color as the Cue tile</span></span>|
|<span data-ttu-id="9cf46-119">**Fordelaktig**</span><span class="sxs-lookup"><span data-stu-id="9cf46-119">**Favorable**</span></span>|<span data-ttu-id="9cf46-120">Grønn</span><span class="sxs-lookup"><span data-stu-id="9cf46-120">Green</span></span>|
|<span data-ttu-id="9cf46-121">**Ufordelaktig**</span><span class="sxs-lookup"><span data-stu-id="9cf46-121">**Unfavorable**</span></span>|<span data-ttu-id="9cf46-122">Rød</span><span class="sxs-lookup"><span data-stu-id="9cf46-122">Red</span></span>|
|<span data-ttu-id="9cf46-123">**Tvetydig**</span><span class="sxs-lookup"><span data-stu-id="9cf46-123">**Ambiguous**</span></span>|<span data-ttu-id="9cf46-124">Gul</span><span class="sxs-lookup"><span data-stu-id="9cf46-124">Yellow</span></span>|
|<span data-ttu-id="9cf46-125">**Underordnet**</span><span class="sxs-lookup"><span data-stu-id="9cf46-125">**Subordinate**</span></span>|<span data-ttu-id="9cf46-126">Grå</span><span class="sxs-lookup"><span data-stu-id="9cf46-126">Gray</span></span>|

## <a name="see-also"></a><span data-ttu-id="9cf46-127">Se også</span><span class="sxs-lookup"><span data-stu-id="9cf46-127">See Also</span></span>
[<span data-ttu-id="9cf46-128">Arbeide med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="9cf46-128">Work with Dynamics NAV</span></span>](ui-work-product.md)


