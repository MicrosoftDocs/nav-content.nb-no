---
title: "Finne bokførte dokumenter uten innkommende dokumentposter"
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
ms.openlocfilehash: eca38d238361a9ac50aac117199fa97fbba4374f
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-find-posted-documents-without-incoming-document-records"></a><span data-ttu-id="56128-102">Finne bokførte dokumenter uten innkommende dokumentposter</span><span class="sxs-lookup"><span data-stu-id="56128-102">How to: Find Posted Documents without Incoming Document Records</span></span>
<span data-ttu-id="56128-103">Fra vinduene **Kontoplan** og **Finansposter** kan du bruke søkefunksjonen til å finne finansposter for bokførte kjøps- og salgsdokumenter som ikke har innkommende dokumentposter, og deretter sentralt koble eksisterende poster eller opprette nye med vedlagte dokumentfiler.</span><span class="sxs-lookup"><span data-stu-id="56128-103">From the **Chart of Accounts** and **General Ledger Entries** windows, you can use a search function to find general ledger entries for posted purchase and sales documents that do not have incoming document records and then centrally link to existing records or create new ones with attached document files.</span></span>

## <a name="to-find-posted-documents-without-incoming-document-records"></a><span data-ttu-id="56128-104">Slik finner du bokførte dokumenter uten innkommende dokumentposter:</span><span class="sxs-lookup"><span data-stu-id="56128-104">To find posted documents without incoming document records</span></span>
1. <span data-ttu-id="56128-105">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kontoplan** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="56128-105">In the top right corner, choose the **Search for Page or Report** icon, enter **Chart of Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="56128-106">Velg en linje for en finanskonto som du vil vise bokførte kjøps- og salgsdokumenter for uten innkommende dokumentposter, og velg deretter handlingen **Bokførte dokumenter uten inngående dokument**.</span><span class="sxs-lookup"><span data-stu-id="56128-106">Select a line for a G/L account for whose general ledger entries you want to see posted purchase and sales documents without incoming document records, and then choose the **Posted Documents without Incoming Document** action.</span></span>
3. <span data-ttu-id="56128-107">Du kan også velge handlingen **Poster**.</span><span class="sxs-lookup"><span data-stu-id="56128-107">Alternatively, choose the **Ledger Entries** action.</span></span>
4. <span data-ttu-id="56128-108">I vinduet **Finansposter** velger du handlingen **Bokførte dokumenter uten inngående dokumenter**.</span><span class="sxs-lookup"><span data-stu-id="56128-108">In the **General Ledger Entries** window, choose the **Posted Documents without Incoming Documents** action.</span></span>

<span data-ttu-id="56128-109">Vinduet **Bokførte dokumenter uten innkommende dokument** åpnes med bokførte kjøps- og salgsdokumenter uten innkommende dokumentposter representert av finansposter på finanskontoen som du åpnet vinduet for.</span><span class="sxs-lookup"><span data-stu-id="56128-109">The **Posted Documents without Incoming Document** window opens showing posted purchase and sales documents without incoming document records represented by general ledger entries on the G/L account that you opened the window for.</span></span> <span data-ttu-id="56128-110">Vinduet kan vise maksimalt 1000 linjer.</span><span class="sxs-lookup"><span data-stu-id="56128-110">The window can show a maximum of 1000 lines.</span></span> <span data-ttu-id="56128-111">Som standard inneholder derfor feltet **Datofilter** et filter som begrenser linjene til poster med bokføringsdatoer fra begynnelsen av regnskapsperioden til arbeidsdatoen.</span><span class="sxs-lookup"><span data-stu-id="56128-111">By default, the **Date Filter** field therefore contains a filter that limits the lines to entries with posting dates from the beginning of the accounting period to the work date.</span></span>

## <a name="to-connect-found-documents-to-existing-incoming-document-records"></a><span data-ttu-id="56128-112">Slik kobler du dokumenter som blir funnet, til eksisterende innkommende dokumentposter:</span><span class="sxs-lookup"><span data-stu-id="56128-112">To connect found documents to existing incoming document records</span></span>
1. <span data-ttu-id="56128-113">I vinduet **Bokførte dokumenter uten inngående dokument** velger du linjen for et bokført dokument du vil koble til en eksisterende innkommende dokumentpost, og deretter velger du handlingen **Velg inngående dokument**.</span><span class="sxs-lookup"><span data-stu-id="56128-113">In the **Posted Documents without Incoming Document** window, select the line for a posted document that you want to connect to an existing incoming document record, and then choose the **Select Incoming Document** action.</span></span>
2. <span data-ttu-id="56128-114">I vinduet **Inngående dokumenter** velger du den innkommende dokumentposten som du vil koble til det bokførte dokumentet som ble funnet, og deretter velger du **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="56128-114">In the **Incoming Documents** window, select the incoming document record that you want to connect to posted document found, and then choose the **OK** button.</span></span>
3. <span data-ttu-id="56128-115">I vinduet **Bokførte dokumenter uten inngående dokument** er den valgte inngående dokumentposten nå koblet til det bokførte dokumentet, som du kan se i faktaboksen **Filer for inngående dokument**.</span><span class="sxs-lookup"><span data-stu-id="56128-115">In the **Posted Documents without Incoming Document** window, the selected incoming document record is now connected to the posted document, as you can see in the **Incoming Document Files** FactBox.</span></span>

<span data-ttu-id="56128-116">Hvis en relevant innkommende dokumentpost ikke finnes i vinduet **Inngående dokumenter** , kan du opprette den.</span><span class="sxs-lookup"><span data-stu-id="56128-116">If a relevant incoming document record does not exist in the **Incoming Documents** window, then you can create it.</span></span> <span data-ttu-id="56128-117">Hvis du vil ha mer informasjon, kan du se [Opprette innkommende dokumentposter](across-how-create-income-document-records.md).</span><span class="sxs-lookup"><span data-stu-id="56128-117">For more information, see [How to: Create Incoming Document Records](across-how-create-income-document-records.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="56128-118">Se også</span><span class="sxs-lookup"><span data-stu-id="56128-118">See Also</span></span>  
[<span data-ttu-id="56128-119">Behandle inngående dokumenter</span><span class="sxs-lookup"><span data-stu-id="56128-119">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="56128-120">Inngående dokumenter</span><span class="sxs-lookup"><span data-stu-id="56128-120">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="56128-121">Håndtere kjøp</span><span class="sxs-lookup"><span data-stu-id="56128-121">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="56128-122">Arbeide med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="56128-122">Work With Dynamics NAV</span></span>](ui-work-product.md)

