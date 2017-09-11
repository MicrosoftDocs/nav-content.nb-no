---
title: Definere salgssykluser for salgsmuligheter og syklusfaser
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 756e9b2f33fe66cd4c2b4e26ca4390683bd087af
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---
# <a name="how-to-set-up-opportunity-sales-cycles-and-cycle-stages"></a><span data-ttu-id="66f1a-102">Definere salgssykluser for salgsmuligheter og syklusfaser</span><span class="sxs-lookup"><span data-stu-id="66f1a-102">How to: Set Up Opportunity Sales Cycles and Cycle Stages</span></span>
<span data-ttu-id="66f1a-103">Før du kan begynne å bruke salgsmuligheter, må du definere salgssykluser og salgssyklusfaser.</span><span class="sxs-lookup"><span data-stu-id="66f1a-103">Before you can start using sales opportunities, you must set up sales cycles and sales cycle stages.</span></span> <span data-ttu-id="66f1a-104">En salgssyklus består av en serie med faser som går fra den første kontakten til avslutningen av et salg.</span><span class="sxs-lookup"><span data-stu-id="66f1a-104">A sales cycle is made up of a series of stages that go from the initial contact to the closing of a sale.</span></span> <span data-ttu-id="66f1a-105">Hver fase kan ha bestemte krav som må oppfylles, for eksempel at et tilbud er påkrevd, før en salgsmulighet kan gå til neste fase.</span><span class="sxs-lookup"><span data-stu-id="66f1a-105">Each stage can have certain requirements that must be met, such as requiring a sales quote, before an opportunity can go to the next stage.</span></span> <span data-ttu-id="66f1a-106">Du kan også angi om en fase kan utelates.</span><span class="sxs-lookup"><span data-stu-id="66f1a-106">You can also specify whether a stage can be skipped.</span></span> <span data-ttu-id="66f1a-107">Du kan definere så mange salgssykluser du trenger, og du kan definere så mange salgssyklusfaser som nødvendig i en salgssyklus.</span><span class="sxs-lookup"><span data-stu-id="66f1a-107">You can setup as many sales cycles as you need, and you can set up as many sales cycle stages as necessary within a sales cycle.</span></span>

<span data-ttu-id="66f1a-108">Implementering av salgssykluser for salgsmulighet innebærer å definere salgssykluskode, definere de ulike syklusfasene, og deretter tilordne syklusen til salgsmuligheter.</span><span class="sxs-lookup"><span data-stu-id="66f1a-108">Implementing opportunity sales cycles involves setting up the sales cycle code, defining the different stages of the cycle, and then assigning the cycle to opportunities.</span></span>

## <a name="to-set-up-an-opportunity-sales-cycle-code"></a><span data-ttu-id="66f1a-109">Definere salgssykluskode for salgsmulighet</span><span class="sxs-lookup"><span data-stu-id="66f1a-109">To set up an opportunity sales cycle code</span></span>
1. <span data-ttu-id="66f1a-110">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Salgssykluser** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="66f1a-110">In the top right corner, choose the **Search for Page or Report** icon, enter **Sales Cycles**, and then choose the related link.</span></span> <span data-ttu-id="66f1a-111">Vinduet **Salgssykluser** åpnes, og det viser alle eksisterende salgssykluser.</span><span class="sxs-lookup"><span data-stu-id="66f1a-111">The **Sales Cycles** window opens, and lists all the existing sales cycles.</span></span>
2. <span data-ttu-id="66f1a-112">Velg handlingen **Ny**, og fyll ut feltene.</span><span class="sxs-lookup"><span data-stu-id="66f1a-112">Choose the **New** action, and fill in the fields.</span></span>

<span data-ttu-id="66f1a-113">Gjenta disse trinnene for å konfigurere så mange salgssykluser som du vil.</span><span class="sxs-lookup"><span data-stu-id="66f1a-113">Repeat these steps to set up as many sales cycles as you want.</span></span> <span data-ttu-id="66f1a-114">Etter at du har definert salgssykluser for salgsmuligheter, bør du definere ulike faser i hver enkelt syklus.</span><span class="sxs-lookup"><span data-stu-id="66f1a-114">After you have set up opportunity sales cycles, you may want to set up the different stages within each cycle.</span></span>

## <a name="to-define-opportunity-sales-cycle-stages"></a><span data-ttu-id="66f1a-115">Definere salgssyklusfaser for salgsmulighet</span><span class="sxs-lookup"><span data-stu-id="66f1a-115">To define opportunity sales cycle stages</span></span>
1. <span data-ttu-id="66f1a-116">I vinduet **Salgssykluser** velger du salgssyklusen for salgsmuligheten du vil definere faser for, og deretter velger du handlingen **Faser**.</span><span class="sxs-lookup"><span data-stu-id="66f1a-116">In the **Sales Cycles** window, select the opportunity sales cycle for which you want to set up stages, and then choose the **Stages** action.</span></span> <span data-ttu-id="66f1a-117">Vinduet **Salgssyklusfaser** åpnes.</span><span class="sxs-lookup"><span data-stu-id="66f1a-117">The **Sales Cycle Stages** window opens.</span></span>
2. <span data-ttu-id="66f1a-118">Velg handlingen **Ny** for å angi en ny fase i salgssyklusen.</span><span class="sxs-lookup"><span data-stu-id="66f1a-118">Choose the **New** action to enter a new stage in the sales cycle.</span></span>

<span data-ttu-id="66f1a-119">Gjenta disse trinnene hvis du vil definere flere faser i salgssyklusen.</span><span class="sxs-lookup"><span data-stu-id="66f1a-119">Repeat these steps to set up as many stages as you want within the sales cycle.</span></span>

## <a name="to-assign-stage-cycle-to-an-opportunity"></a><span data-ttu-id="66f1a-120">Tilordne fasesyklus til en salgsmulighet</span><span class="sxs-lookup"><span data-stu-id="66f1a-120">To assign stage cycle to an opportunity</span></span>
<span data-ttu-id="66f1a-121">Når du legger til fasesyklusen for salgsmulighet, kan du begynne å legge til salgsmuligheter og deretter tilordne fasesyklusen til salgsmuligheter ved å bruke feltet **Salgssykluskode**.</span><span class="sxs-lookup"><span data-stu-id="66f1a-121">After you add the opportunities stage cycle, you can start to add sales opportunities, and then assign the stage cycle to opportunities by setting the **Sales Cycle Code** field.</span></span> <span data-ttu-id="66f1a-122">Hvis du vil ha mer informasjon, kan du se [Opprette salgsmuligheter](marketing-how-create-opportunities.md).</span><span class="sxs-lookup"><span data-stu-id="66f1a-122">For more information, see [How to: Create Sales Opportunities](marketing-how-create-opportunities.md).</span></span>

##<a name="see-also"></a><span data-ttu-id="66f1a-123">Se også</span><span class="sxs-lookup"><span data-stu-id="66f1a-123">See Also</span></span>  
[<span data-ttu-id="66f1a-124">Behandle salgsmuligheter</span><span class="sxs-lookup"><span data-stu-id="66f1a-124">Processing Sales Opportunities</span></span>](marketing-processing-sales-opportunities.md)  
[<span data-ttu-id="66f1a-125">Håndtere salg</span><span class="sxs-lookup"><span data-stu-id="66f1a-125">Manage Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="66f1a-126">Arbeide med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="66f1a-126">Working with Dynamics NAV</span></span>](ui-work-product.md)

