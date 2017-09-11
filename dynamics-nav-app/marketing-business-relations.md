---
title: Definere forretningsforbindelser for kontaktselskaper
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
ms.openlocfilehash: 6616473a00e85e52648713d7e067f4b3b72caecf
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---
# <a name="set-up-business-relations-on-contact-companies"></a><span data-ttu-id="71de9-102">Definere forretningsforbindelser for kontaktselskaper</span><span class="sxs-lookup"><span data-stu-id="71de9-102">Set Up Business Relations on Contact Companies</span></span>
<span data-ttu-id="71de9-103">Du kan bruke forretningsforbindelser blir brukt til å angi hvilket forretningsforhold du har til kontaktene, for eksempel prospekter, banker, konsulenter, serviceleverandører og så videre.</span><span class="sxs-lookup"><span data-stu-id="71de9-103">You can use business relations to indicate the business relationship you have with your contacts, for example, a prospect, bank, consultant, service supplier, and so on.</span></span>

<span data-ttu-id="71de9-104">Bruk av forretningsforbindelser på kontakter er en totrinnsprosess.</span><span class="sxs-lookup"><span data-stu-id="71de9-104">Using business relations on contacts is a two-step process.</span></span> <span data-ttu-id="71de9-105">Først må definere du koden for forretningsforbindelsen.</span><span class="sxs-lookup"><span data-stu-id="71de9-105">First, you define the business relation code.</span></span> <span data-ttu-id="71de9-106">Du trenger bare utføre dette trinnet én gang for hver forretningsforbindelse.</span><span class="sxs-lookup"><span data-stu-id="71de9-106">You only have to perform this step one time for each business relation.</span></span> <span data-ttu-id="71de9-107">Når du har en kode for forretningsforbindelse, kan du begynne å tilordne koden til kontaktselskaper.</span><span class="sxs-lookup"><span data-stu-id="71de9-107">Once you have a business relation code, you can start to assign the code to contact companies.</span></span>

<span data-ttu-id="71de9-108">**Merk**: Hvis du vil synkronisere kontaktene med leverandører, kunder eller bankkonti i andre deler av applikasjonen, bør du definere en forretningsforbindelse for disse.</span><span class="sxs-lookup"><span data-stu-id="71de9-108">**Note**: If you plan to synchronize your contacts with vendors, customers, or bank accounts in other parts of the application, you may want to set up a business relation for them.</span></span>

## <a name="define-a-business-relation-code"></a><span data-ttu-id="71de9-109">Definere en kode for forretningsforbindelse</span><span class="sxs-lookup"><span data-stu-id="71de9-109">Define a Business Relation Code</span></span>
<span data-ttu-id="71de9-110">Koden for forretningsforbindelsen definerer en kategori eller type for forretningsforbindelsen, for eksempel BANK eller JURIDISK.</span><span class="sxs-lookup"><span data-stu-id="71de9-110">The business relation code defines a category or type of the business relationship, such as BANK or LAW.</span></span> <span data-ttu-id="71de9-111">Du kan ha flere forretningsforbindelseskoder.</span><span class="sxs-lookup"><span data-stu-id="71de9-111">You can have several business relation codes.</span></span> <span data-ttu-id="71de9-112">Hvis du vil definere forretningsforbindelsen, bruker du vinduet **Forretningsforbindelser**.</span><span class="sxs-lookup"><span data-stu-id="71de9-112">To define the business relation, you use the **Business Relations** window.</span></span>

1. <span data-ttu-id="71de9-113">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Forretningsforbindelser** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="71de9-113">In the top right corner, choose the **Search for Page or Report** icon, enter **Business Relations**, and then choose the related link.</span></span>
2. <span data-ttu-id="71de9-114">Velg handlingen **Ny**, og fyll ut en kode og en beskrivelse.</span><span class="sxs-lookup"><span data-stu-id="71de9-114">Choose the **New** action, and fill in a code and description.</span></span> <span data-ttu-id="71de9-115">Koden kan bestå av opptil 11 tegn, og kan inneholde en kombinasjon av tall og bokstaver.</span><span class="sxs-lookup"><span data-stu-id="71de9-115">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span></span>

## <a name="assign-business-relations-to-a-contact"></a><span data-ttu-id="71de9-116">Tilordne forretningsforbindelser til en kontakt</span><span class="sxs-lookup"><span data-stu-id="71de9-116">Assign Business Relations to a Contact</span></span>
<span data-ttu-id="71de9-117">Du kan ikke tilordne forretningsforbindelser til en kontaktperson, bare selskaper.</span><span class="sxs-lookup"><span data-stu-id="71de9-117">You cannot assign business relations to a contact person - only companies.</span></span>

1. <span data-ttu-id="71de9-118">Åpne kontakten.</span><span class="sxs-lookup"><span data-stu-id="71de9-118">Open the contact.</span></span>
2. <span data-ttu-id="71de9-119">Velg handlingen **Selskap**, og deretter handlingen **Forretningsforbindelser**.</span><span class="sxs-lookup"><span data-stu-id="71de9-119">Choose the **Company** action, and then the **Business Relations** action.</span></span>

    <span data-ttu-id="71de9-120">Vinduet **Kontaktens forretn.forbind.** åpnes.</span><span class="sxs-lookup"><span data-stu-id="71de9-120">The **Contact Business Relations** window opens.</span></span>
3. <span data-ttu-id="71de9-121">Velg forretningsforbindelsen du vil tilordne, i feltet **Forretn.forbindelseskode**.</span><span class="sxs-lookup"><span data-stu-id="71de9-121">In the **Business Relation Code** field, select the business relation you want to assign.</span></span>

<span data-ttu-id="71de9-122">Gjenta disse trinnene hvis du vil tilordne flere forretningsforbindelser.</span><span class="sxs-lookup"><span data-stu-id="71de9-122">Repeat these steps to assign as many business relations as you want.</span></span> <span data-ttu-id="71de9-123">Du kan også tilordne forretningsforbindelser fra kontaktlisten ved å følge samme fremgangsmåte.</span><span class="sxs-lookup"><span data-stu-id="71de9-123">You can also assign business relations from the contact list by following the same procedure.</span></span>

<span data-ttu-id="71de9-124">Antall forretningsforbindelser du har tilordnet kontakten, vises i feltet **Ant. forretningsforbindelser** i inndelingen **Segmentering** i vinduet **Kontakt**.</span><span class="sxs-lookup"><span data-stu-id="71de9-124">The number of business relations you have assigned to the contact is displayed in the **No. of Business Relations** field in the **Segmentation** section in the **Contact** window.</span></span>

<span data-ttu-id="71de9-125">Når du har tilordnet forretningsforbindelser til kontaktene, kan du bruke disse opplysningene til å velge kontakter for segmentene.</span><span class="sxs-lookup"><span data-stu-id="71de9-125">After you have assigned business relations to your contacts, you can use this information to select contacts for your segments.</span></span> <span data-ttu-id="71de9-126">Hvis du vil ha mer informasjon, kan du se [Legge til kontakter i segmenter](marketing-add-contact-segment.md).</span><span class="sxs-lookup"><span data-stu-id="71de9-126">For more information, see [How to: Add Contacts to Segments](marketing-add-contact-segment.md).</span></span>

##<a name="see-also"></a><span data-ttu-id="71de9-127">Se også</span><span class="sxs-lookup"><span data-stu-id="71de9-127">See Also</span></span>
[<span data-ttu-id="71de9-128">Opprette kontaktselskaper</span><span class="sxs-lookup"><span data-stu-id="71de9-128">Create Contact Companies</span></span>](marketing-create-contact-companies.md)

