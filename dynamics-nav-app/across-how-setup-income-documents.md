---
title: "Konfigurere inngående dokumenter"
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
ms.openlocfilehash: d55329b571e4c59d4821a86a39362ea58480b86a
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-set-up-incoming-documents"></a><span data-ttu-id="a1a46-102">Konfigurere inngående dokumenter</span><span class="sxs-lookup"><span data-stu-id="a1a46-102">How to: Set Up Incoming Documents</span></span>
<span data-ttu-id="a1a46-103">Hvis du oppretter finanskladdelinjer fra innkommende dokumentposter, må du angi hvilken kladdemal og kladd som skal brukes i vinduet **Oppsett for inngående dokumenter**.</span><span class="sxs-lookup"><span data-stu-id="a1a46-103">If you create general journal lines from incoming document records, you must specify in the **Incoming Documents Setup** window which journal template and batch to use.</span></span>

<span data-ttu-id="a1a46-104">Hvis du ikke vil at brukerne skal opprette fakturaer eller finanskladdelinjer fra innkommende dokumentposter med mindre dokumentene først er godkjent, må du definere godkjennere i vinduet **Godkjennere for inngående dokumenter**.</span><span class="sxs-lookup"><span data-stu-id="a1a46-104">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up approvers in the **Incoming Document Approvers** window.</span></span>

<span data-ttu-id="a1a46-105">Hvis du vil gjøre om PDF- og bildefiler til elektroniske dokumenter som du kan konvertere til, for eksempel kjøpsfakturaer i Dynamics NAV, må du først sette opp OCR-funksjonen og aktivere tjenesten.</span><span class="sxs-lookup"><span data-stu-id="a1a46-105">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside Dynamics NAV, you must first set up the OCR feature and enable the service.</span></span>

<span data-ttu-id="a1a46-106">Når funksjonen for inngående dokumenter er konfigurert, kan du bruke forskjellige funksjoner til å se gjennom utgiftskvitteringer, behandle OCR-oppgaver og konvertere inngående dokumentfiler, manuelt eller automatisk, til de aktuelle dokumentene eller kladdelinjene.</span><span class="sxs-lookup"><span data-stu-id="a1a46-106">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="a1a46-107">De eksterne filene kan tilknyttes på et hvilket som helst tidspunkt i prosessen, inkludert bokførte dokumenter og resulterende leverandør, kunde- og finansposter.</span><span class="sxs-lookup"><span data-stu-id="a1a46-107">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span> <span data-ttu-id="a1a46-108">Hvis du vil ha mer informasjon, kan du se [Behandle inngående dokumenter](across-process-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="a1a46-108">For more information, see [How to: Process Incoming Documents](across-process-income-documents.md).</span></span>

## <a name="to-set-up-the-incoming-documents-feature"></a><span data-ttu-id="a1a46-109">Slik konfigurerer du funksjonen for inngående dokumenter:</span><span class="sxs-lookup"><span data-stu-id="a1a46-109">To set up the Incoming Documents feature</span></span>
1. <span data-ttu-id="a1a46-110">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Oppsett for inngående dokumenter** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="a1a46-110">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="a1a46-111">Fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="a1a46-111">Fill in the fields as necessary.</span></span> <span data-ttu-id="a1a46-112">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="a1a46-112">Choose a field to read a short description of the field or link to more information.</span></span>

## <a name="to-set-up-approvers-of-incoming-document-records"></a><span data-ttu-id="a1a46-113">Slik definerer du godkjennere av inngående dokumentposter:</span><span class="sxs-lookup"><span data-stu-id="a1a46-113">To set up approvers of incoming document records</span></span>
1. <span data-ttu-id="a1a46-114">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Oppsett for inngående dokumenter** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="a1a46-114">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="a1a46-115">I vinduet **Oppsett for inngående dokumenter** velger du handlingen **Godkjennere**.</span><span class="sxs-lookup"><span data-stu-id="a1a46-115">In the **Incoming Documents Setup** window, choose the **Approvers** action.</span></span>

    <span data-ttu-id="a1a46-116">Vinduet **Godkjennere for inngående dokumenter** viser alle brukerne som er definert i Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="a1a46-116">The **Incoming Document Approvers** window shows all users that are set up in your Dynamics NAV .</span></span>  
3. <span data-ttu-id="a1a46-117">Velg én eller flere brukere som kan godkjenne et innkommende dokument før det kan opprettes en relatert dokument- eller kladdelinje.</span><span class="sxs-lookup"><span data-stu-id="a1a46-117">Select one or more users that can approve an incoming document before a related document or journal line can be created.</span></span>

<span data-ttu-id="a1a46-118">Når godkjennere er definert i vinduet **Godkjennere for inngående dokumenter**, er det bare disse brukerne som kan godkjenne et inngående dokument hvis det er merket av for **Krev godkjenning for opprettelse** i vinduet **Oppsett for inngående dokumenter**.</span><span class="sxs-lookup"><span data-stu-id="a1a46-118">When approvers have been set up in the **Incoming Document Approvers** window, only those users can approve an incoming document if the **Require Approval To Create** check box in the **Incoming Documents Setup** window is selected.</span></span>

<span data-ttu-id="a1a46-119">**Merk**: Dette godkjenningsoppsettet er ikke relatert til arbeidsflyter for godkjenning.</span><span class="sxs-lookup"><span data-stu-id="a1a46-119">**Note**: This approval setup is not related to approval workflows.</span></span> <span data-ttu-id="a1a46-120">Hvis du vil ha mer informasjon, kan du se [Bruke arbeidsflyter for godkjenning](across-how-use-approval-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="a1a46-120">For more information, see [How to: Use Approval Workflows](across-how-use-approval-workflows.md).</span></span>

## <a name="to-set-up-an-ocr-service"></a><span data-ttu-id="a1a46-121">Slik definerer du en OCR-tjeneste:</span><span class="sxs-lookup"><span data-stu-id="a1a46-121">To set up an OCR service</span></span>
1. <span data-ttu-id="a1a46-122">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Oppsett for OCR-tjeneste** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="a1a46-122">In the top right corner, choose the **Search for Page or Report** icon, enter **OCR Service Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="a1a46-123">Fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="a1a46-123">Fill in the fields as necessary.</span></span> <span data-ttu-id="a1a46-124">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="a1a46-124">Choose a field to read a short description of the field or link to more information.</span></span>


## <a name="to-encrypt-your-login-information"></a><span data-ttu-id="a1a46-125">Slik krypterer du påloggingsinformasjonen:</span><span class="sxs-lookup"><span data-stu-id="a1a46-125">To encrypt your login information</span></span>
<span data-ttu-id="a1a46-126">Det anbefales at du beskytter påloggingsinformasjonen du angir i vinduet **Oppsett for OCR-tjeneste**.</span><span class="sxs-lookup"><span data-stu-id="a1a46-126">It is recommended that you protect the logon information that you enter in the **OCR Service Setup** window.</span></span> <span data-ttu-id="a1a46-127">Du kan kryptere data på serveren ved å generere nye eller importere eksisterende krypteringsnøkler du aktiverer på serverforekomsten som kobler til databasen.</span><span class="sxs-lookup"><span data-stu-id="a1a46-127">You can encrypt data on the server by generating new or importing existing encryption keys that you enable on the server instance that connects to the database.</span></span>

1. <span data-ttu-id="a1a46-128">I vinduet **Oppsett for OCR-tjeneste** velger du handlingen **Krypteringsadministrasjon**.</span><span class="sxs-lookup"><span data-stu-id="a1a46-128">In the **OCR Service Setup** window, choose the **Encryption Management** action.</span></span>
2. <span data-ttu-id="a1a46-129">I vinduet **Administrasjon av datakryptering** aktiverer du kryptering av dataene.</span><span class="sxs-lookup"><span data-stu-id="a1a46-129">In the **Data Encryption Management** window, enable encryption of your data.</span></span>

## <a name="see-also"></a><span data-ttu-id="a1a46-130">Se også</span><span class="sxs-lookup"><span data-stu-id="a1a46-130">See Also</span></span>  
[<span data-ttu-id="a1a46-131">Behandle inngående dokumenter</span><span class="sxs-lookup"><span data-stu-id="a1a46-131">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="a1a46-132">Inngående dokumenter</span><span class="sxs-lookup"><span data-stu-id="a1a46-132">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="a1a46-133">Håndtere kjøp</span><span class="sxs-lookup"><span data-stu-id="a1a46-133">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="a1a46-134">Arbeide med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="a1a46-134">Work With Dynamics NAV</span></span>](ui-work-product.md)

