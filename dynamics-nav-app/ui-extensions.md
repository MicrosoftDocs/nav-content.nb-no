---
title: Tilpasse Dynamics NAV ved hjelp av utvidelser
author: edupont04
ms.custom: na
ms.date: 09/23/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: cc832772a255c7c801a7b956c74da827caca3765
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---

# <a name="customizing-dynamics-nav-using-extensions"></a><span data-ttu-id="929a7-102">Tilpasse Dynamics NAV ved hjelp av utvidelser</span><span class="sxs-lookup"><span data-stu-id="929a7-102">Customizing Dynamics NAV Using Extensions</span></span>
<span data-ttu-id="929a7-103">Du kan endre Dynamics NAV ved å installere utvidelser som for eksempel legger til funksjonalitet, endrer virkemåte eller gir deg tilgang til nye elektroniske tjenester.</span><span class="sxs-lookup"><span data-stu-id="929a7-103">You can change Dynamics NAV by installing extensions that add functionality, change behavior, or give you access to new online services, for example.</span></span>
<span data-ttu-id="929a7-104">Når du starter Dynamics NAV for første gang, er noen utvidelser allerede installert for deg.</span><span class="sxs-lookup"><span data-stu-id="929a7-104">When you first launch Dynamics NAV, some extensions are already installed for you.</span></span> <span data-ttu-id="929a7-105">Over tid gjøres flere utvidelser tilgjengelig for deg, og du kan deretter velge om du vil bruke utvidelsen eller ikke.</span><span class="sxs-lookup"><span data-stu-id="929a7-105">Over time, more extensions can be made available to you, and you can then choose if you want to use the extension or not.</span></span>

<span data-ttu-id="929a7-106">Microsoft tilbyr for eksempel en utvidelse som kan gi integrering med PayPal Payments Standard.</span><span class="sxs-lookup"><span data-stu-id="929a7-106">For example, Microsoft provides an extension that provides integration with PayPal Payments Standard.</span></span> <span data-ttu-id="929a7-107">Denne utvidelsen er installert som standard.</span><span class="sxs-lookup"><span data-stu-id="929a7-107">This extension is installed by default.</span></span>
<span data-ttu-id="929a7-108">Hvis en annen utvidelse gjøres tilgjengelig som gir integrasjon med en annen betalingstjenesten, kan du installere den nye utvidelsen og deretter velger hvilke av de to tjenestene du vil bruke.</span><span class="sxs-lookup"><span data-stu-id="929a7-108">But if another extension is made available that offers integration with another payment service, you can install the new extension and then choose which of the two services to use.</span></span>  

<span data-ttu-id="929a7-109">Du administrerer utvidelsene i vinduet **Administrasjon av utvidelse**.</span><span class="sxs-lookup"><span data-stu-id="929a7-109">You manage the extensions in the **Extension Management** window.</span></span> <span data-ttu-id="929a7-110">Du kan gå til dette vinduet fra Hjem.</span><span class="sxs-lookup"><span data-stu-id="929a7-110">You can access this window from Home.</span></span> <span data-ttu-id="929a7-111">I øvre høyre hjørne kan du også velge ikonet **Søk etter side eller rapport**, angi **Utvidelse** og deretter velge den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="929a7-111">Alternatively, choose the **Search for Page or Report** icon in the top right corner, enter **Extension**, and then choose the related link.</span></span>   

## <a name="installing-an-extension"></a><span data-ttu-id="929a7-112">Installere en utvidelse</span><span class="sxs-lookup"><span data-stu-id="929a7-112">Installing an Extension</span></span>
<span data-ttu-id="929a7-113">Hvis nye filtyper blir gjort tilgjengelig for deg fordi de har blitt publisert til serveren, vil de vises i vinduet **Administrasjon av utvidelse**.</span><span class="sxs-lookup"><span data-stu-id="929a7-113">If new extensions are made available to you because they have been published to your server, they will be shown in the **Extension Management** window.</span></span> <span data-ttu-id="929a7-114">Herfra kan du velge å installere og avinstallere utvidelser.</span><span class="sxs-lookup"><span data-stu-id="929a7-114">From here, you can choose to install and uninstall extensions.</span></span>  

<span data-ttu-id="929a7-115">Hvis du velger en utvidelse, kan du lese om hva utvidelsen gjør, og du kan få tilgang til hjelp for utvidelsen for å finne ut mer.</span><span class="sxs-lookup"><span data-stu-id="929a7-115">If you choose an extension, you can read about what the extension does, and you can access Help for the extension to learn more.</span></span> <span data-ttu-id="929a7-116">Når du skaffer en utvidelse, må du godta vilkårene for bruk.</span><span class="sxs-lookup"><span data-stu-id="929a7-116">When you choose to get an extension, you must agree to the terms of use.</span></span>  

<span data-ttu-id="929a7-117">Når du installerer en utvidelse, må du kanskje konfigurere den, for eksempel angi en konto for bruk med utvidelsen **PayPal Payments Standard for Dynamics NAV**.</span><span class="sxs-lookup"><span data-stu-id="929a7-117">When you install an extension, you might have to set it up, such as specifying an account for use with the **PayPal Payments Standard for Dynamics NAV** extension.</span></span>
<span data-ttu-id="929a7-118">Andre utvidelser legger for eksempel ganske enkelt til felt på en eksisterende side, eller de legger til en ny side.</span><span class="sxs-lookup"><span data-stu-id="929a7-118">Other extensions simply add fields to an existing page, or they add a new page, for example.</span></span>   

<span data-ttu-id="929a7-119">Hvis du avinstallerer en utvidelse og du deretter ombestemmer deg, kan du installere den på nytt.</span><span class="sxs-lookup"><span data-stu-id="929a7-119">If you uninstall an extension, and you then change your mind, you can install it again.</span></span> <span data-ttu-id="929a7-120">Når du avinstallerer en utvidelse som du har brukt, beholdes dataene, slik at hvis du installerer utvidelsen på nytt, er dataene fremdeles tilgjengelige.</span><span class="sxs-lookup"><span data-stu-id="929a7-120">When you uninstall an extension that you have been using, the data is preserved so that if you install the extension again, your data is still available.</span></span>  

<span data-ttu-id="929a7-121">Microsoft tilbyr følgende utvidelser:</span><span class="sxs-lookup"><span data-stu-id="929a7-121">Microsoft provides the following extensions:</span></span>  
- [<span data-ttu-id="929a7-122">PayPal Payments Standard</span><span class="sxs-lookup"><span data-stu-id="929a7-122">PayPal Payments Standard</span></span>](ui-extensions-paypal-payments-standard.md)  
- [<span data-ttu-id="929a7-123">Salgs- og lagerprognose</span><span class="sxs-lookup"><span data-stu-id="929a7-123">Sales and Inventory Forecast</span></span>](ui-extensions-sales-forecast.md)  

<span data-ttu-id="929a7-124">Det finnes også andre utvidelser som standard, avhengig av landet/regionen.</span><span class="sxs-lookup"><span data-stu-id="929a7-124">Other extensions are also available by default, depending on your country/region.</span></span>

## <a name="see-also"></a><span data-ttu-id="929a7-125">Se også</span><span class="sxs-lookup"><span data-stu-id="929a7-125">See Also</span></span>  
[<span data-ttu-id="929a7-126">Aktiver kundebetalinger gjennom PayPal</span><span class="sxs-lookup"><span data-stu-id="929a7-126">How to: Enable Customer Payment Through PayPal</span></span>](sales-how-enable-customer-payments-paypal.md)  
[<span data-ttu-id="929a7-127">Velkommen til Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="929a7-127">Welcome to Dynamics NAV</span></span>](across-get-started.md)  

