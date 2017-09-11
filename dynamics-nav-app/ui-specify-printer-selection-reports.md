---
title: Angi skrivervalg for rapporter
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
ms.openlocfilehash: 56a5c1428651162293e56d71e2369fe55d291594
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---
    
# <a name="specify-printer-selection-for-reports"></a><span data-ttu-id="f9c34-102">Angi skrivervalg for rapporter</span><span class="sxs-lookup"><span data-stu-id="f9c34-102">Specify Printer Selection for Reports</span></span>
<span data-ttu-id="f9c34-103">Du kan definere rapporter slik at de må skrives ut på en bestemt skriver.</span><span class="sxs-lookup"><span data-stu-id="f9c34-103">You can set up reports so that they must be printed on a specific printer.</span></span> <span data-ttu-id="f9c34-104">Her er noen av bruksområdene for skrivervalg:</span><span class="sxs-lookup"><span data-stu-id="f9c34-104">The following are some uses of printer selection:</span></span> 

- <span data-ttu-id="f9c34-105">Du kan skrive ut rapporter på papir med et spesielt brevhode for selskapet.</span><span class="sxs-lookup"><span data-stu-id="f9c34-105">You can print reports on special company letterhead.</span></span>
- <span data-ttu-id="f9c34-106">Du kan skrive ut rapporter på ulike papirstørrelser.</span><span class="sxs-lookup"><span data-stu-id="f9c34-106">You can print reports on different paper sizes.</span></span>
- <span data-ttu-id="f9c34-107">Du kan skrive ut rapporter på standardskriveren for en bestemt ansatt.</span><span class="sxs-lookup"><span data-stu-id="f9c34-107">You can print reports on the default printer of a specified employee.</span></span>

<span data-ttu-id="f9c34-108">Du bruker vinduet **Skrivervalg** til å angi ulike verdier for å få forskjellig utskrift.</span><span class="sxs-lookup"><span data-stu-id="f9c34-108">You use the **Printer Selections** window to set different values to obtain different output.</span></span> <span data-ttu-id="f9c34-109">Hvis du angir et bestemt skrivervalg, har dette forrang over et mer generelt skrivervalg.</span><span class="sxs-lookup"><span data-stu-id="f9c34-109">If you set a specific printer selection, then it takes precedence over a more general printer selection.</span></span> <span data-ttu-id="f9c34-110">Du kan for eksempel angi et skrivervalg som har verdier i feltene **Bruker-ID**, **Rapport-ID** og **Skrivernavn**.</span><span class="sxs-lookup"><span data-stu-id="f9c34-110">For example, you can set a printer selection that has values in the **User ID**, **Report ID**, and **Printer Name** fields.</span></span> <span data-ttu-id="f9c34-111">Dette skrivervalget overstyrer skrivervalget som har tomme oppføringer i **Bruker-ID**- eller **Rapport-ID**-feltet.</span><span class="sxs-lookup"><span data-stu-id="f9c34-111">This printer selection takes precedence over a printer selection that has blank entries in the **User ID** or **Report ID** fields.</span></span> 

<span data-ttu-id="f9c34-112">Tabellen nedenfor beskriver kombinasjonen av verdier som må angis når du konfigurerer skrivervalg for en rapport.</span><span class="sxs-lookup"><span data-stu-id="f9c34-112">The following table describes the combination of values to specify when you set up printer selections for a report.</span></span>

|<span data-ttu-id="f9c34-113">Hvis du vil</span><span class="sxs-lookup"><span data-stu-id="f9c34-113">To</span></span>                                                 |<span data-ttu-id="f9c34-114">Angi følgende verdier</span><span class="sxs-lookup"><span data-stu-id="f9c34-114">Set the following values</span></span>                                             |
|---------------------------------------------------|---------------------------------------------------------------------|
|<span data-ttu-id="f9c34-115">Skrive ut en rapport på en bestemt skriver for alle brukere</span><span class="sxs-lookup"><span data-stu-id="f9c34-115">Print a report to a specific printer for all users</span></span> |<span data-ttu-id="f9c34-116">Angi verdier i feltene **Rapport-ID** og **Skrivernavn**, og la **Bruker-ID**-feltet stå tomt.</span><span class="sxs-lookup"><span data-stu-id="f9c34-116">Specify values in the **Report ID** and **Printer Name** fields and leave the **User ID** field blank.</span></span>|
|<span data-ttu-id="f9c34-117">Skrive ut alle rapporter på en bestemt skriver til en bestemt bruker</span><span class="sxs-lookup"><span data-stu-id="f9c34-117">Print all reports to a specific printer for a specific user</span></span>|<span data-ttu-id="f9c34-118">Angi verdier i feltene **Bruker-ID** og **Skrivernavn**, og la **Rapport-ID**-feltet stå tomt.</span><span class="sxs-lookup"><span data-stu-id="f9c34-118">Specify values in the **User ID** and **Printer Name** fields and leave the **Report ID** field blank.</span></span>|
|<span data-ttu-id="f9c34-119">Angi standardskriver for alle rapporter</span><span class="sxs-lookup"><span data-stu-id="f9c34-119">Set the default printer for all reports</span></span>|<span data-ttu-id="f9c34-120">Angi en verdi i **Skrivernavn**-feltet, og la feltene **Bruker-ID** og **Rapport-ID** stå tomme.</span><span class="sxs-lookup"><span data-stu-id="f9c34-120">Specify a value in the **Printer Name** field and leave the **User ID** and **Report ID** fields blank.</span></span>|
|<span data-ttu-id="f9c34-121">Skrive ut en bestemt rapport på brukerens standardskriver</span><span class="sxs-lookup"><span data-stu-id="f9c34-121">Print a specific report to the user’s default printer</span></span>|<span data-ttu-id="f9c34-122">Angi en verdi i **Rapport-ID**-feltet, og la feltene **Skrivernavn** og **Bruker-ID** stå tomme.</span><span class="sxs-lookup"><span data-stu-id="f9c34-122">Specify a value in the **Report ID** field and leave the **Printer Name** and **User ID** fields blank.</span></span>|
|<span data-ttu-id="f9c34-123">Skrive ut en bestemt rapport på en bestemt skriver til en bestemt bruker</span><span class="sxs-lookup"><span data-stu-id="f9c34-123">Print a specific report to a specific printer for a specific user</span></span>|<span data-ttu-id="f9c34-124">Angi verdier i alle tre feltene.</span><span class="sxs-lookup"><span data-stu-id="f9c34-124">Specify values in all three fields.</span></span>|

## <a name="see-also"></a><span data-ttu-id="f9c34-125">Se også</span><span class="sxs-lookup"><span data-stu-id="f9c34-125">See Also</span></span>
[<span data-ttu-id="f9c34-126">Arbeide med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="f9c34-126">Work with Dynamics NAV</span></span>](ui-work-product.md)

