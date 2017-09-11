---
title: Registrere en nye produkter
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
ms.openlocfilehash: df84a4d3e15035cd956c7612a12069844f5601d2
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-register-new-products"></a><span data-ttu-id="7485f-102">Registrere en nye produkter</span><span class="sxs-lookup"><span data-stu-id="7485f-102">How to: Register New Products</span></span>

<span data-ttu-id="7485f-103">Produktene er grunnlaget for virksomheten din, varer eller tjenester som du handler med.</span><span class="sxs-lookup"><span data-stu-id="7485f-103">Products are the basis of your business, the goods or services that you trade in.</span></span> <span data-ttu-id="7485f-104">Hvert produkt må være registrert som et varekort.</span><span class="sxs-lookup"><span data-stu-id="7485f-104">Each product must be registered as an item card.</span></span>

<span data-ttu-id="7485f-105">**Merk**: I Dynamics NAV brukes ordet “vare” for å referere til et produkt.</span><span class="sxs-lookup"><span data-stu-id="7485f-105">**Note**: In Dynamics NAV, a product is referred to using the term “item”.</span></span>

<span data-ttu-id="7485f-106">Varekort inneholder informasjonen som er nødvendig for å kjøpe, lagre, selge, levere og gjøre rede for produkter.</span><span class="sxs-lookup"><span data-stu-id="7485f-106">Item cards hold the information that is required to buy, store, sell, deliver, and account for products.</span></span>

<span data-ttu-id="7485f-107">Varekortet kan være av typen Beholdning eller Tjeneste for å angi om produktet er en fysisk enhet eller arbeidstidsenhet.</span><span class="sxs-lookup"><span data-stu-id="7485f-107">The item card can be of type Inventory or Service to specify if the product is a physical unit or labor time unit.</span></span> <span data-ttu-id="7485f-108">Bortsett fra noen av feltene som er relatert til de fysiske aspektene av en vare, fungerer alle felt på et varekort på samme måte for lagervarer og tjenester.</span><span class="sxs-lookup"><span data-stu-id="7485f-108">Apart from some fields that relate to the physical aspects of an item, all fields on an item card function in the same way for inventory items and services.</span></span> <span data-ttu-id="7485f-109">Hvis du vil ha mer informasjon om hvordan du selger en vare, kan du se [Selge produkter](sales-how-sell-products.md) eller [Fakturere salg](sales-how-invoice-sales.md).</span><span class="sxs-lookup"><span data-stu-id="7485f-109">For more information about selling an item, see [How to: Sell Products](sales-how-sell-products.md) or [How to: Invoice Sales](sales-how-invoice-sales.md).</span></span>

<span data-ttu-id="7485f-110">**Merk**: Hvis det finnes varemaler for ulike varetyper, vises et vindu når du oppretter et nytt kundekort der du kan velge en passende mal.</span><span class="sxs-lookup"><span data-stu-id="7485f-110">**Note**: If item templates exist for different item types, then a window appears when you create a new item card from where you can select an appropriate template.</span></span> <span data-ttu-id="7485f-111">Hvis det bare finnes én varemal, brukes alltid denne malen i nye varekort.</span><span class="sxs-lookup"><span data-stu-id="7485f-111">If only one item template exists, then new item cards always use that template.</span></span>

## <a name="to-create-a-new-item-card"></a><span data-ttu-id="7485f-112">Opprette et nytt varekort</span><span class="sxs-lookup"><span data-stu-id="7485f-112">To create a new item card</span></span>
1. <span data-ttu-id="7485f-113">På Hjem-siden velger du handlingen **Varer** for å åpne listen over eksisterende varer.</span><span class="sxs-lookup"><span data-stu-id="7485f-113">On the Home page, choose the **Items** action to open the list of existing items.</span></span>  
2. <span data-ttu-id="7485f-114">I vinduet **Varer** velger du handlingen **Ny**.</span><span class="sxs-lookup"><span data-stu-id="7485f-114">In the **Items** window, choose the **New** action.</span></span>

    <span data-ttu-id="7485f-115">Hvis det bare finnes én varemal, åpnes et nytt varekort med noen felt som er fylt ut med informasjon fra malen.</span><span class="sxs-lookup"><span data-stu-id="7485f-115">If only one item template exists, then a new item card opens with some fields filled with information from the template.</span></span>
3. <span data-ttu-id="7485f-116">I vinduet **Velg en mal for en ny vare** velger du malen som du vil bruke for det nye varekortet.</span><span class="sxs-lookup"><span data-stu-id="7485f-116">In the **Select a template for a new item** window, choose the template that you want to use for the new item card.</span></span>
4. <span data-ttu-id="7485f-117">Velg **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="7485f-117">Choose the **OK** button.</span></span> <span data-ttu-id="7485f-118">Det åpnes et nytt varekort med noen felt som er fylt ut med informasjon fra malen.</span><span class="sxs-lookup"><span data-stu-id="7485f-118">A new item card opens with some fields filled with information from the template.</span></span>
5. <span data-ttu-id="7485f-119">Fortsette med å fylle ut eller endre feltet på varekortet etter behov.</span><span class="sxs-lookup"><span data-stu-id="7485f-119">Proceed to fill or change fields on the item card as necessary.</span></span> <span data-ttu-id="7485f-120">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="7485f-120">Choose a field to read a short description of the field or link to more information.</span></span>

<span data-ttu-id="7485f-121">I hurtigfanen **Salgspriser** kan du vise spesialpriser eller rabatter som skal gis for varen hvis bestemte kriterier oppfylles, for eksempel kunde, minimumsordreantall eller sluttdato.</span><span class="sxs-lookup"><span data-stu-id="7485f-121">On the **Sales Prices** FastTab, you can view special prices or discounts that you grant for the item if certain criteria are met, such as customer, minimum order quantity, or ending date.</span></span> <span data-ttu-id="7485f-122">Hver rad representerer en spesialpris eller linjerabatt.</span><span class="sxs-lookup"><span data-stu-id="7485f-122">Each row represents a special price or line discount.</span></span> <span data-ttu-id="7485f-123">Hver kolonne representerer et vilkår som må brukes for å garantere spesialprisen du angir i feltet **Enhetspris**, eller linjerabatten du angir i feltet **Linjerabatt-%**.</span><span class="sxs-lookup"><span data-stu-id="7485f-123">Each column represents a criterion that must apply to warrant the special price that you enter in the **Unit Price** field, or the line discount that you enter in the **Line Discount %** field.</span></span> <span data-ttu-id="7485f-124">Hvis du vil ha mer informasjon, kan du se [Registrere avtaler om salgspris, rabatt og betaling](sales-how-record-sales-price-discount-payment-agreements.md).</span><span class="sxs-lookup"><span data-stu-id="7485f-124">For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).</span></span>

<span data-ttu-id="7485f-125">Varen er nå registrert, og varekortet er klart til å brukes på kjøps- og salgsdokumenter.</span><span class="sxs-lookup"><span data-stu-id="7485f-125">The item is now registered, and the item card is ready to be used on purchase and sales documents.</span></span>

<span data-ttu-id="7485f-126">Hvis du vil bruke dette varekortet som en mal når du oppretter nye varekort, kan du lagre det som en mal.</span><span class="sxs-lookup"><span data-stu-id="7485f-126">If you want to use this item card as a template when you create new item cards, you can save it as a template.</span></span> <span data-ttu-id="7485f-127">Hvis du vil ha mer informasjon, kan du se følgende avsnitt:</span><span class="sxs-lookup"><span data-stu-id="7485f-127">For more information, see the following section.</span></span>

## <a name="to-save-the-item-card-as-a-template"></a><span data-ttu-id="7485f-128">Lagre varekortet som en mal</span><span class="sxs-lookup"><span data-stu-id="7485f-128">To save the item card as a template</span></span>
1. <span data-ttu-id="7485f-129">I vinduet **Varekort** velger du handlingen **Lagre som mal**.</span><span class="sxs-lookup"><span data-stu-id="7485f-129">In the **Item Card** window, choose the **Save as Template** action.</span></span> <span data-ttu-id="7485f-130">**Varemal**  -vinduet åpnes og viser varekortet som en mal.</span><span class="sxs-lookup"><span data-stu-id="7485f-130">The **Item Template** window opens showing the item card as a template.</span></span>
2. <span data-ttu-id="7485f-131">Fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="7485f-131">Fill in the fields as necessary.</span></span> <span data-ttu-id="7485f-132">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="7485f-132">Choose a field to read a short description of the field or link to more information.</span></span>
3. <span data-ttu-id="7485f-133">Hvis du vil bruke dimensjoner i maler, velger du handlingen **Dimensjoner**.</span><span class="sxs-lookup"><span data-stu-id="7485f-133">To reuse dimensions in templates, choose the **Dimensions** action.</span></span> <span data-ttu-id="7485f-134">**Dimensjonsmaler**-vinduet åpnes med alle dimensjonskoder som er definert for varen.</span><span class="sxs-lookup"><span data-stu-id="7485f-134">The **Dimension Templates** window opens showing any dimension codes that are set up for the item.</span></span>
4. <span data-ttu-id="7485f-135">Rediger eller angi dimensjonskoder som skal gjelde for nye varekort som opprettes ved hjelp av malen.</span><span class="sxs-lookup"><span data-stu-id="7485f-135">Edit or enter dimension codes that will apply to new item cards created by using the template.</span></span>
5. <span data-ttu-id="7485f-136">Når du har fullført den nye varemalen, kan du velge **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="7485f-136">When you have completed the new item template, choose the **OK** button.</span></span>

<span data-ttu-id="7485f-137">Varemalen legges til i listen over varemaler, slik at du kan bruke den til å opprette nye varekort.</span><span class="sxs-lookup"><span data-stu-id="7485f-137">The item template is added to the list of item templates, so that you can use it to create new item cards.</span></span>

## <a name="see-also"></a><span data-ttu-id="7485f-138">Se også</span><span class="sxs-lookup"><span data-stu-id="7485f-138">See Also</span></span>
  [<span data-ttu-id="7485f-139">Håndtere lager</span><span class="sxs-lookup"><span data-stu-id="7485f-139">Manage Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="7485f-140">  [Håndtere kjøp](purchasing-manage-purchasing.md)</span><span class="sxs-lookup"><span data-stu-id="7485f-140">  [Manage Purchasing](purchasing-manage-purchasing.md)</span></span>  
<span data-ttu-id="7485f-141">  [Håndtere salg](sales-manage-sales.md)</span><span class="sxs-lookup"><span data-stu-id="7485f-141">  [Manage Sales](sales-manage-sales.md)</span></span>

