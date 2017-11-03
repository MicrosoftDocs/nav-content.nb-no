---
title: Aktivere kundebetalinger gjennom betalingstjenester
description: "Gjør det lettere for kundene å betale sine fakturaer ved å aktivere betalingstjenester."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: online payment
ms.date: 07/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: f56df1759d375548b7415234c9b303a49e50687d
ms.contentlocale: nb-no
ms.lasthandoff: 10/26/2017

---
# <a name="how-to-enable-customer-payments-through-payment-services"></a><span data-ttu-id="3d3c6-103">Aktivere kundebetalinger gjennom betalingstjenester</span><span class="sxs-lookup"><span data-stu-id="3d3c6-103">How to: Enable Customer Payments Through Payment Services</span></span>
<span data-ttu-id="3d3c6-104">Som et alternativ til å samle inn betalinger via bankoverføring eller kredittkort, kan kundene betale via egne kontoer med betalingstjenester, som PayPal og WorldPay.</span><span class="sxs-lookup"><span data-stu-id="3d3c6-104">As an alternative to collecting payments through bank transfer or credit cards, your customers can pay you through their account with payment services, such as PayPal and WorldPay.</span></span>  

<span data-ttu-id="3d3c6-105">Når du har aktivert en betalingstjeneste i [!INCLUDE[d365fin](includes/d365fin_md.md)], en kobling til tjenesten er tilgjengelig på salgsdokumenter som du sender via e-post til kundene dine.</span><span class="sxs-lookup"><span data-stu-id="3d3c6-105">After you enable a payment service in [!INCLUDE[d365fin](includes/d365fin_md.md)], a link to the service is available on sales documents that you send by email to your customers.</span></span> <span data-ttu-id="3d3c6-106">Kunder kan bruke koblingen for å gå til tjenesten og betale fakturaen, direkte fra salgsdokumentet.</span><span class="sxs-lookup"><span data-stu-id="3d3c6-106">Customers can use the link to go to the payment service and pay the bill, directly from the sales document.</span></span> <span data-ttu-id="3d3c6-107">Hvis du ikke vil inkludere koblingen, for eksempel kan Hvis en kunde betaler kontant, du fjerne tjenesten fra fakturaen før bokføring.</span><span class="sxs-lookup"><span data-stu-id="3d3c6-107">If you don't want to include the link, for example, if a customer will pay with cash, you can remove the payment service from the invoice before posting.</span></span>  

<span data-ttu-id="3d3c6-108">PayPal betalinger Standard og WorldPay betalinger Standard tilleggene som er installert i [!INCLUDE[d365fin](includes/d365fin_md.md)], og er klar til å aktivere.</span><span class="sxs-lookup"><span data-stu-id="3d3c6-108">The PayPal Payments Standard and WorldPay Payments Standard extensions are installed in [!INCLUDE[d365fin](includes/d365fin_md.md)], and are ready for you to enable.</span></span>  

## <a name="to-enable-a-payment-service-in-included365finincludesd365finmdmd"></a><span data-ttu-id="3d3c6-109">Slik aktiverer du en betalingstjeneste i [!INCLUDE[d365fin](includes/d365fin_md.md)]</span><span class="sxs-lookup"><span data-stu-id="3d3c6-109">To enable a payment service in [!INCLUDE[d365fin](includes/d365fin_md.md)]</span></span>
1. <span data-ttu-id="3d3c6-110">Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Betalingstjenester**, og velg deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="3d3c6-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="3d3c6-111">I vinduet **Betalingstjenester** velger du handlingen **Ny**.</span><span class="sxs-lookup"><span data-stu-id="3d3c6-111">In the **Payment Services** window, choose the **New** action.</span></span>  
3. <span data-ttu-id="3d3c6-112">Velg betalingstjenesten, og lukk deretter vinduet.</span><span class="sxs-lookup"><span data-stu-id="3d3c6-112">Select the payment service, and then close the window.</span></span>  
4. <span data-ttu-id="3d3c6-113">I vinduet **Betalingstjenester** velger du handlingen **Oppsett**.</span><span class="sxs-lookup"><span data-stu-id="3d3c6-113">In the **Payment Services** window, choose the **Setup** action.</span></span>  
5. <span data-ttu-id="3d3c6-114">Fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="3d3c6-114">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
6. <span data-ttu-id="3d3c6-115">Lukk vinduet.</span><span class="sxs-lookup"><span data-stu-id="3d3c6-115">Close the window.</span></span>  

## <a name="to-select-a-payment-service-on-a-sales-invoice"></a><span data-ttu-id="3d3c6-116">Velge en betalingstjeneste på en salgsfaktura</span><span class="sxs-lookup"><span data-stu-id="3d3c6-116">To select a payment service on a sales invoice</span></span>
1. <span data-ttu-id="3d3c6-117">Velg handlingen **Salgsfakturaer** på Hjem-siden.</span><span class="sxs-lookup"><span data-stu-id="3d3c6-117">On the Home page, choose **Sales Invoices**.</span></span>  
2. <span data-ttu-id="3d3c6-118">Åpne Salgsfaktura som du ønsker å betale ved hjelp av betalingstjenesten.</span><span class="sxs-lookup"><span data-stu-id="3d3c6-118">Open the sales invoice that you want to pay by using the payment service.</span></span>  
3. <span data-ttu-id="3d3c6-119">I feltet **Betalingstjeneste** velger du betalingstjenesten.</span><span class="sxs-lookup"><span data-stu-id="3d3c6-119">In the **Payment Service** field, choose the payment service.</span></span>  

    > [!NOTE]  
>   <span data-ttu-id="3d3c6-120">Feltet **Betalingstjeneste** er bare tilgjengelig hvis du har aktivert betalingstjenesten.</span><span class="sxs-lookup"><span data-stu-id="3d3c6-120">The **Payment Service** field is available only if you've enabled the payment service.</span></span>  

## <a name="see-also"></a><span data-ttu-id="3d3c6-121">Se også</span><span class="sxs-lookup"><span data-stu-id="3d3c6-121">See Also</span></span>  
[<span data-ttu-id="3d3c6-122">Sette opp salg</span><span class="sxs-lookup"><span data-stu-id="3d3c6-122">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="3d3c6-123">Salg</span><span class="sxs-lookup"><span data-stu-id="3d3c6-123">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="3d3c6-124">[Tilpasse [!INCLUDE[d365fin](includes/d365fin_md.md)] ved hjelp av utvidelser](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="3d3c6-124">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
<span data-ttu-id="3d3c6-125">[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="3d3c6-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

