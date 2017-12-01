---
title: Aktiver kundebetalinger gjennom PayPal
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 92b00332f3fb5adff12d518ca2af4aa4093fbf7a
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---

# <a name="how-to-enable-customer-payments-through-paypal"></a><span data-ttu-id="397f2-102">Aktiver kundebetalinger gjennom PayPal#</span><span class="sxs-lookup"><span data-stu-id="397f2-102">How to: Enable Customer Payments Through PayPal#</span></span>
<span data-ttu-id="397f2-103">Som et alternativ til å samle inn betalinger via bankoverføring eller kredittkort, kan du tilby kundene å betale du gjennom sin PayPal-konto.</span><span class="sxs-lookup"><span data-stu-id="397f2-103">As an alternative to collecting payments through bank transfer or credit cards, you can offer your customers to pay you through their PayPal account.</span></span>

<span data-ttu-id="397f2-104">Når en kunde velger PayPal-koblingen på en salgsfaktura eller et salgsordredokument, vises tjenestesiden deres for PayPal-kontoen med betalingsdetaljer for salget.</span><span class="sxs-lookup"><span data-stu-id="397f2-104">When a customer chooses the PayPal link on a sales invoice or sales order document, the service page for their PayPal account appears showing the payment details for the sale.</span></span> <span data-ttu-id="397f2-105">Kunden kan deretter betale fakturaen på samme måte som andre PayPal-betalinger.</span><span class="sxs-lookup"><span data-stu-id="397f2-105">The customer can then pay the invoice as any other PayPal payment.</span></span>

<span data-ttu-id="397f2-106">Hvis du vil aktivere kundebetalinger gjennom PayPal, må du gjøre følgende:</span><span class="sxs-lookup"><span data-stu-id="397f2-106">To enable customer payments through PayPal, you must do the following:</span></span>

1. <span data-ttu-id="397f2-107">Definere PayPal Payments Standard som en betalingstjeneste i vinduet **Betalingstjenester**.</span><span class="sxs-lookup"><span data-stu-id="397f2-107">Set up PayPal Payments Standard as a payment service in the **Payments Services** window.</span></span>
2. <span data-ttu-id="397f2-108">Velg PayPal Payments Standard i feltet **Betalingstjeneste** på det aktuelle salgsdokumentet.</span><span class="sxs-lookup"><span data-stu-id="397f2-108">Select PayPal Payments Standard in the **Payment Service** field on the sales document in question.</span></span>

<span data-ttu-id="397f2-109">PayPal Payments Standard-tjenesten er installert som en utvidelse for Dynamics NAV og er klar til å aktiveres.</span><span class="sxs-lookup"><span data-stu-id="397f2-109">The PayPal Payments Standard service is installed as an extension to Dynamics NAV and ready to enabled.</span></span> <span data-ttu-id="397f2-110">Hvis du vil ha mer informasjon, kan du se [Tilpasse Dynamics NAV ved hjelp av utvidelser](ui-extensions.md).</span><span class="sxs-lookup"><span data-stu-id="397f2-110">For more information, see [Customizing Dynamics NAV Using Extensions ](ui-extensions.md).</span></span>

## <a name="to-enable-the-paypal-payments-standard-service"></a><span data-ttu-id="397f2-111">Aktivere PayPal Payments Standard-tjenesten</span><span class="sxs-lookup"><span data-stu-id="397f2-111">To enable the PayPal Payments Standard service</span></span>
1. <span data-ttu-id="397f2-112">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Betalingstjenester** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="397f2-112">In the top right corner, choose the **Search for Page or Report** icon, **Payment Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="397f2-113">I vinduet **Betalingstjenester** velger du handlingen **Ny**.</span><span class="sxs-lookup"><span data-stu-id="397f2-113">In the **Payment Services** window, choose the **New** action.</span></span>
3. <span data-ttu-id="397f2-114">Velg **PayPal Standard**, og lukk deretter vinduet.</span><span class="sxs-lookup"><span data-stu-id="397f2-114">Select **PayPal Standard**, and then close the window.</span></span>
4. <span data-ttu-id="397f2-115">I vinduet **Betalingstjenester** velger du handlingen **Oppsett**.</span><span class="sxs-lookup"><span data-stu-id="397f2-115">In the **Payment Services** window, choose the **Setup** action.</span></span>
5. <span data-ttu-id="397f2-116">Fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="397f2-116">Fill in the fields as necessary.</span></span> <span data-ttu-id="397f2-117">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="397f2-117">Choose a field to read a short description of the field or link to more information.</span></span>

    <span data-ttu-id="397f2-118">**Merk**: Merk av for **Inkluder alltid i dokumenter** hvis hyperkoblingen for PayPal-betalingstjenesten alltid skal vises på salgsdokumentene når betaling via PayPal er aktivert.</span><span class="sxs-lookup"><span data-stu-id="397f2-118">**Note**: Select the **Always Include on Documents** check box if the hyperlink for the PayPal payment service should always be visible on sales documents where payment through PayPal is enabled.</span></span>

6. <span data-ttu-id="397f2-119">Lukk vinduet.</span><span class="sxs-lookup"><span data-stu-id="397f2-119">Close the window.</span></span>

## <a name="to-select-paypal-payments-standard-on-a-sales-invoice"></a><span data-ttu-id="397f2-120">Velge PayPal Payments Standard på en salgsfaktura</span><span class="sxs-lookup"><span data-stu-id="397f2-120">To select PayPal Payments Standard on a sales invoice</span></span>
1. <span data-ttu-id="397f2-121">Velg handlingen **Salgsfakturaer** på Hjem-siden.</span><span class="sxs-lookup"><span data-stu-id="397f2-121">On the Home page, choose **Sales Invoices**.</span></span>
2. <span data-ttu-id="397f2-122">Åpne salgsfakturaen som du vil aktivere PayPal-betalinger for.</span><span class="sxs-lookup"><span data-stu-id="397f2-122">Open the sales invoice that you want to enable PayPal payments for.</span></span>
3. <span data-ttu-id="397f2-123">I feltet **Betalingstjeneste** velger du PayPal Payments Standard.</span><span class="sxs-lookup"><span data-stu-id="397f2-123">In the **Payment Service** field, choose PayPal Payments Standard.</span></span>

<span data-ttu-id="397f2-124">**Merk**: Feltet **Betalingstjeneste** vises bare hvis PayPal Payments Standard-tjenesten er aktivert.</span><span class="sxs-lookup"><span data-stu-id="397f2-124">**Note**: The **Payment Service** field is only visible if the PayPal Payments Standard service is enabled.</span></span>   

## <a name="see-also"></a><span data-ttu-id="397f2-125">Se også</span><span class="sxs-lookup"><span data-stu-id="397f2-125">See Also</span></span>  
[<span data-ttu-id="397f2-126">Definere salg</span><span class="sxs-lookup"><span data-stu-id="397f2-126">Set Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="397f2-127">Håndtere salg</span><span class="sxs-lookup"><span data-stu-id="397f2-127">Manage Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="397f2-128">Tilpasse Dynamics NAV ved hjelp av utvidelser</span><span class="sxs-lookup"><span data-stu-id="397f2-128">Customizing Dynamics NAV Using Extensions</span></span>](ui-extensions.md)

