---
title: Definere bransjegrupper for kontaktselskaper
description: Beskriver hvordan du definerer en bransjegruppe og tilordner den til et kontaktselskap, for eksempel detaljistbransjen eller bilbransjen.
documentationcenter: 
author: jswymer
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 62d946155cb65a3e976771bc5029878893bd4797
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-industry-groups-for-contact-companies"></a><span data-ttu-id="6befe-103">Definere bransjegrupper for kontaktselskaper</span><span class="sxs-lookup"><span data-stu-id="6befe-103">How to: Set Up Industry Groups for Contact Companies</span></span>
<span data-ttu-id="6befe-104">Du bruker bransjegrupper for å angi hvilken bransje kontaktene tilhører, for eksempel detaljistbransjen eller bilbransjen.</span><span class="sxs-lookup"><span data-stu-id="6befe-104">You use industry groups to indicate the type of industry to which your contacts belong, for example, the retail industry or the automobile industry.</span></span>

<span data-ttu-id="6befe-105">Bruk av bransjegrupper på kontakter er en totrinnsprosess.</span><span class="sxs-lookup"><span data-stu-id="6befe-105">Using industry groups on contacts is a two-step process.</span></span> <span data-ttu-id="6befe-106">Først må definere du koden for bransjegruppen.</span><span class="sxs-lookup"><span data-stu-id="6befe-106">First, you define the industry group code.</span></span> <span data-ttu-id="6befe-107">Du trenger bare utføre dette trinnet én gang for hver bransjegruppe.</span><span class="sxs-lookup"><span data-stu-id="6befe-107">You only have to perform this step one time for each industry group.</span></span> <span data-ttu-id="6befe-108">Når du har en kode for bransjegruppe, kan du begynne å tilordne koden til kontaktselskaper.</span><span class="sxs-lookup"><span data-stu-id="6befe-108">Once you have an industry group code, you can start to assign the code to contact companies.</span></span>

> [!NOTE]  
>   <span data-ttu-id="6befe-109">Hvis du planlegger å synkronisere kontaktene med leverandører, kunder eller bankkonti i andre deler av programmet, bør du definere en forretningsforbindelse for disse.</span><span class="sxs-lookup"><span data-stu-id="6befe-109">If you plan to synchronize your contacts with vendors, customers, or bank accounts in other parts of the application, you may want to set up a business relation for them.</span></span>

## <a name="to-define-an-industry-group-code"></a><span data-ttu-id="6befe-110">Definere en kode for bransjegruppe</span><span class="sxs-lookup"><span data-stu-id="6befe-110">To define an industry group code</span></span>
<span data-ttu-id="6befe-111">Koden for bransjegruppen definerer typen eller kategorien for gruppen, for eksempel REKLAME for reklame, eller PRESSE, for TV og radio.</span><span class="sxs-lookup"><span data-stu-id="6befe-111">The industry group code defines the type or category of the group, such as ADVERT for advertising, or PRESS, for TV and radio.</span></span> <span data-ttu-id="6befe-112">Du kan ha flere koder for bransjegruppe.</span><span class="sxs-lookup"><span data-stu-id="6befe-112">You can have several industry group codes.</span></span> <span data-ttu-id="6befe-113">Hvis du vil definere bransjegrupper, bruker du vinduet **Bransjegrupper**.</span><span class="sxs-lookup"><span data-stu-id="6befe-113">To define the industry groups, you use the **Industry Groups** window.</span></span>

1. <span data-ttu-id="6befe-114">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bransjegrupper**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="6befe-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Industry Groups**, and then choose the related link.</span></span>
2. <span data-ttu-id="6befe-115">Velg handlingen **Ny**, og fyll ut en kode og en beskrivelse.</span><span class="sxs-lookup"><span data-stu-id="6befe-115">Choose the **New** action, and fill in a code and description.</span></span> <span data-ttu-id="6befe-116">Koden kan bestå av opptil 11 tegn, og kan inneholde en kombinasjon av tall og bokstaver.</span><span class="sxs-lookup"><span data-stu-id="6befe-116">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span></span>

## <span data-ttu-id="6befe-117"><a name="AssignIndustryGroupContact"></a> Tilordne bransjegrupper til en kontakt</span><span class="sxs-lookup"><span data-stu-id="6befe-117"><a name="AssignIndustryGroupContact"></a> To assign industry groups to a contact</span></span>
<span data-ttu-id="6befe-118">Du kan ikke tilordne bransjegrupper til en kontaktperson, bare selskaper.</span><span class="sxs-lookup"><span data-stu-id="6befe-118">You cannot assign industry groups to a contact person - only companies.</span></span>

1. <span data-ttu-id="6befe-119">Åpne kontakten.</span><span class="sxs-lookup"><span data-stu-id="6befe-119">Open the contact.</span></span>
2. <span data-ttu-id="6befe-120">Velg handlingen **Selskap**, og deretter handlingen **Bransjegrupper**.</span><span class="sxs-lookup"><span data-stu-id="6befe-120">Choose the **Company** action, and then the **Industry Groups** action.</span></span> <span data-ttu-id="6befe-121">Vinduet **Kontaktbransjegrupper** åpnes.</span><span class="sxs-lookup"><span data-stu-id="6befe-121">The **Contact Industry Groups** window opens.</span></span>
3. <span data-ttu-id="6befe-122">Velg bransjegruppen du vil tilordne, i feltet **Bransjegruppe - kode**.</span><span class="sxs-lookup"><span data-stu-id="6befe-122">In the **Industry Groups Code** field, select the industry groups you want to assign.</span></span>

<span data-ttu-id="6befe-123">Gjenta disse trinnene hvis du vil tilordne flere bransjegrupper.</span><span class="sxs-lookup"><span data-stu-id="6befe-123">Repeat these steps to assign as many industry groups as you want.</span></span> <span data-ttu-id="6befe-124">Du kan også tilordne bransjegrupper fra kontaktlisten ved å følge samme fremgangsmåte.</span><span class="sxs-lookup"><span data-stu-id="6befe-124">You can also assign industry groups from the contact list by following the same procedure.</span></span>

<span data-ttu-id="6befe-125">Antallet bransjegrupper du har tilordnet kontakten, vises i feltet **Ant. bransjegrupper** i inndelingen **Segmentering** i vinduet **Kontakt**.</span><span class="sxs-lookup"><span data-stu-id="6befe-125">The number of industry groups that you have assigned to the contact is displayed in the **No. of Industry Groups** field in the **Segmentation** section in the **Contact** window.</span></span>

<span data-ttu-id="6befe-126">Når du har tilordnet bransjegrupper til kontaktene, kan du bruke disse opplysningene til å velge kontakter for segmentene.</span><span class="sxs-lookup"><span data-stu-id="6befe-126">After you have assigned industry groups to your contacts, you can use this information to select contacts for your segments.</span></span> <span data-ttu-id="6befe-127">Hvis du vil ha mer informasjon, kan du se [Legge til kontakter i segmenter](marketing-add-contact-segment.md).</span><span class="sxs-lookup"><span data-stu-id="6befe-127">For more information, see [How to: Add Contacts to Segments](marketing-add-contact-segment.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="6befe-128">Se også</span><span class="sxs-lookup"><span data-stu-id="6befe-128">See Also</span></span>
[<span data-ttu-id="6befe-129">Opprette kontaktselskaper</span><span class="sxs-lookup"><span data-stu-id="6befe-129">Creating Contact Companies</span></span>](marketing-create-contact-companies.md)  
<span data-ttu-id="6befe-130">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6befe-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

