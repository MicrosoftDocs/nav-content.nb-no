---
title: Aktiver kundebetalinger gjennom PayPal
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 15f30a03c3e7ccc865ef527a707794c2c6428b2f
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-enable-customer-payments-through-paypal"></a><span data-ttu-id="05bb6-102">Aktiver kundebetalinger gjennom PayPal#</span><span class="sxs-lookup"><span data-stu-id="05bb6-102">How to: Enable Customer Payments Through PayPal#</span></span>
<span data-ttu-id="05bb6-103">Som et alternativ til å samle inn betalinger via bankoverføring eller kredittkort, kan du tilby kundene å betale du gjennom sin PayPal-konto.</span><span class="sxs-lookup"><span data-stu-id="05bb6-103">As an alternative to collecting payments through bank transfer or credit cards, you can offer your customers to pay you through their PayPal account.</span></span>

<span data-ttu-id="05bb6-104">Når en kunde velger PayPal-koblingen på en salgsfaktura eller et salgsordredokument, vises tjenestesiden deres for PayPal-kontoen med betalingsdetaljer for salget.</span><span class="sxs-lookup"><span data-stu-id="05bb6-104">When a customer chooses the PayPal link on a sales invoice or sales order document, the service page for their PayPal account appears showing the payment details for the sale.</span></span> <span data-ttu-id="05bb6-105">Kunden kan deretter betale fakturaen på samme måte som andre PayPal-betalinger.</span><span class="sxs-lookup"><span data-stu-id="05bb6-105">The customer can then pay the invoice as any other PayPal payment.</span></span>

<span data-ttu-id="05bb6-106">Hvis du vil aktivere kundebetalinger gjennom PayPal, må du gjøre følgende:</span><span class="sxs-lookup"><span data-stu-id="05bb6-106">To enable customer payments through PayPal, you must do the following:</span></span>

1. <span data-ttu-id="05bb6-107">Definere PayPal Payments Standard som en betalingstjeneste i vinduet **Betalingstjenester**.</span><span class="sxs-lookup"><span data-stu-id="05bb6-107">Set up PayPal Payments Standard as a payment service in the **Payments Services** window.</span></span>
2. <span data-ttu-id="05bb6-108">Velg PayPal Payments Standard i feltet **Betalingstjeneste** på det aktuelle salgsdokumentet.</span><span class="sxs-lookup"><span data-stu-id="05bb6-108">Select PayPal Payments Standard in the **Payment Service** field on the sales document in question.</span></span>

<span data-ttu-id="05bb6-109">PayPal Payments Standard-tjenesten er installert som en utvidelse for Dynamics NAV og er klar til å aktiveres.</span><span class="sxs-lookup"><span data-stu-id="05bb6-109">The PayPal Payments Standard service is installed as an extension to Dynamics NAV and ready to enabled.</span></span> <span data-ttu-id="05bb6-110">Hvis du vil ha mer informasjon, kan du se [Tilpasse Dynamics NAV ved hjelp av utvidelser ](ui-extensions.md).</span><span class="sxs-lookup"><span data-stu-id="05bb6-110">For more information, see [Customizing Dynamics NAV Using Extensions ](ui-extensions.md).</span></span>

## <a name="to-enable-the-paypal-payments-standard-service"></a><span data-ttu-id="05bb6-111">Aktivere PayPal Payments Standard-tjenesten</span><span class="sxs-lookup"><span data-stu-id="05bb6-111">To enable the PayPal Payments Standard service</span></span>
1. <span data-ttu-id="05bb6-112">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Betalingstjenester** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="05bb6-112">In the top right corner, choose the **Search for Page or Report** icon, **Payment Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="05bb6-113">I vinduet **Betalingstjenester** velger du handlingen **Ny**.</span><span class="sxs-lookup"><span data-stu-id="05bb6-113">In the **Payment Services** window, choose the **New** action.</span></span>
3. <span data-ttu-id="05bb6-114">Velg **PayPal Standard**, og lukk deretter vinduet.</span><span class="sxs-lookup"><span data-stu-id="05bb6-114">Select **PayPal Standard**, and then close the window.</span></span>
4. <span data-ttu-id="05bb6-115">I vinduet **Betalingstjenester** velger du handlingen **Oppsett**.</span><span class="sxs-lookup"><span data-stu-id="05bb6-115">In the **Payment Services** window, choose the **Setup** action.</span></span>
5. <span data-ttu-id="05bb6-116">Fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="05bb6-116">Fill in the fields as necessary.</span></span> <span data-ttu-id="05bb6-117">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="05bb6-117">Choose a field to read a short description of the field or link to more information.</span></span>

    <span data-ttu-id="05bb6-118">**Merk**: Merk av for **Inkluder alltid i dokumenter** hvis hyperkoblingen for PayPal-betalingstjenesten alltid skal vises på salgsdokumentene når betaling via PayPal er aktivert.</span><span class="sxs-lookup"><span data-stu-id="05bb6-118">**Note**: Select the **Always Include on Documents** check box if the hyperlink for the PayPal payment service should always be visible on sales documents where payment through PayPal is enabled.</span></span>

6. <span data-ttu-id="05bb6-119">Lukk vinduet.</span><span class="sxs-lookup"><span data-stu-id="05bb6-119">Close the window.</span></span>

## <a name="to-select-paypal-payments-standard-on-a-sales-invoice"></a><span data-ttu-id="05bb6-120">Velge PayPal Payments Standard på en salgsfaktura</span><span class="sxs-lookup"><span data-stu-id="05bb6-120">To select PayPal Payments Standard on a sales invoice</span></span>
1. <span data-ttu-id="05bb6-121">Velg handlingen **Salgsfakturaer** på Hjem-siden.</span><span class="sxs-lookup"><span data-stu-id="05bb6-121">On the Home page, choose **Sales Invoices**.</span></span>
2. <span data-ttu-id="05bb6-122">Åpne salgsfakturaen som du vil aktivere PayPal-betalinger for.</span><span class="sxs-lookup"><span data-stu-id="05bb6-122">Open the sales invoice that you want to enable PayPal payments for.</span></span>
3. <span data-ttu-id="05bb6-123">I feltet **Betalingstjeneste** velger du PayPal Payments Standard.</span><span class="sxs-lookup"><span data-stu-id="05bb6-123">In the **Payment Service** field, choose PayPal Payments Standard.</span></span>

<span data-ttu-id="05bb6-124">**Merk**: Feltet **Betalingstjeneste** vises bare hvis PayPal Payments Standard-tjenesten er aktivert.</span><span class="sxs-lookup"><span data-stu-id="05bb6-124">**Note**: The **Payment Service** field is only visible if the PayPal Payments Standard service is enabled.</span></span>   

## <a name="see-also"></a><span data-ttu-id="05bb6-125">Se også</span><span class="sxs-lookup"><span data-stu-id="05bb6-125">See Also</span></span>  
[<span data-ttu-id="05bb6-126">Definere salg</span><span class="sxs-lookup"><span data-stu-id="05bb6-126">Set Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="05bb6-127">Håndtere salg</span><span class="sxs-lookup"><span data-stu-id="05bb6-127">Manage Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="05bb6-128">Tilpasse Dynamics NAV ved hjelp av utvidelser</span><span class="sxs-lookup"><span data-stu-id="05bb6-128">Customizing Dynamics NAV Using Extensions</span></span>](ui-extensions.md)

