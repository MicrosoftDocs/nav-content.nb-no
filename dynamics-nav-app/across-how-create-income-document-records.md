---
title: Opprette innkommende dokumentposter
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
ms.openlocfilehash: e91c4570ff60d991974ac6afd16ba3bc3e73e44f
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-create-incoming-document-records"></a><span data-ttu-id="c5e2b-102">Opprette innkommende dokumentposter</span><span class="sxs-lookup"><span data-stu-id="c5e2b-102">How to: Create Incoming Document Records</span></span>
<span data-ttu-id="c5e2b-103">I vinduet **Inngående dokumenter** kan du bruke forskjellige funksjoner til å se gjennom utgiftskvitteringer, behandle OCR-oppgaver og konvertere inngående dokumentfiler, manuelt eller automatisk, til de aktuelle dokumentene eller kladdelinjene.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-103">In the **Incoming Documents** window, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="c5e2b-104">De eksterne filene kan tilknyttes på et hvilket som helst tidspunkt i prosessen, inkludert bokførte dokumenter og resulterende leverandør, kunde- og finansposter.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-104">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span>

<span data-ttu-id="c5e2b-105">Hvis du vil registrere et eksternt dokument i Dynamics NAV, må du først opprette eller fullføre en innkommende dokumentpost.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-105">To record an external document in Dynamics NAV, you must first create or complete an incoming document record.</span></span> <span data-ttu-id="c5e2b-106">Du kan gjøre dette manuelt, eller du kan ta et bilde av det eksterne dokumentet og deretter opprette den inngående dokumentposten med bildefilen som vedlegg.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-106">You can do this manually, or you can take a photo of the external document and then create the incoming document record with the image file attached.</span></span>

<span data-ttu-id="c5e2b-107">Før du kan bruke funksjonen for inngående dokumenter, må du utføre den nødvendige konfigurasjonen.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-107">Before you can use the Incoming Documents feature, you must perform the required setup.</span></span> <span data-ttu-id="c5e2b-108">Hvis du vil ha mer informasjon, kan du se [Konfigurere inngående dokumenter](across-how-setup-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="c5e2b-108">For more information, see [How to: Set Up Incoming Documents](across-how-setup-income-documents.md).</span></span>

## <a name="to-approve-or-reject-an-incoming-document"></a><span data-ttu-id="c5e2b-109">Slik godkjenner eller avviser du et innkommende dokument</span><span class="sxs-lookup"><span data-stu-id="c5e2b-109">To approve or reject an incoming document</span></span>
<span data-ttu-id="c5e2b-110">Hvis du vil tillate brukere å opprette fakturaer eller finanskladdelinjer fra innkommende dokumentposter med mindre de er godkjent, kan du definere godkjennere som må godkjenne postene før de kan behandles.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-110">If you do want to allow users to create invoices or general journal lines from incoming document records unless they are approved, you can set up approvers who must approve the records before they can be processed.</span></span>

1. <span data-ttu-id="c5e2b-111">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Inngående dokumenter** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-111">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="c5e2b-112">Velg linjen med dokumentet som du vil godkjenne eller avvise, og velg deretter handlingen **Godkjenn** eller **Avvis**.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-112">Select the line with the document that you want to approve or reject, and then choose the **Approve** or **Reject** actions.</span></span>

<span data-ttu-id="c5e2b-113">Hvis du godkjenner den inngående dokumentposten, merkes det av for **Frigitt** på linjen for det inngående dokumentet.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-113">If you approve the incoming document record, the **Released** check box on the incoming document line is selected.</span></span> <span data-ttu-id="c5e2b-114">Brukeren som for eksempel er ansvarlig for å opprette kjøpsfakturaer, kan fortsette å behandle posten.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-114">The user in charge of creating, for example, purchase invoices can proceed to process the record.</span></span>

## <a name="to-create-an-incoming-document-record-by-taking-a-photo"></a><span data-ttu-id="c5e2b-115">Slik oppretter du en innkommende dokumentpost ved å ta et bilde</span><span class="sxs-lookup"><span data-stu-id="c5e2b-115">To create an incoming document record by taking a photo</span></span>
<span data-ttu-id="c5e2b-116">**Merk**: Fremgangsmåten nedenfor gjelder bare for nettbrett og telefoner med Dynamics NAV-klienter.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-116">**Note**: The following procedure only applies to the Dynamics NAV Tablet and Phone clients.</span></span>

1. <span data-ttu-id="c5e2b-117">I appfeltet velger du **Opprett innkommende dokument fra kamera**-flisen, og gå deretter til trinn 4.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-117">On the app bar, choose the **Create Incoming Document from Camera** tile, and then go to step 4.</span></span>
2. <span data-ttu-id="c5e2b-118">Alternativt kan du velge Alternativer-knappen i appfeltet, velge **Innkommende dokumenter**, og deretter velge **Alle**.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-118">Alternatively, on the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span></span>
3. <span data-ttu-id="c5e2b-119">I vinduet **Inngående dokumenter** velger du ellipseknappen, og deretter velger du **Opprett fra kamera**.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-119">In the **Incoming Documents** window, choose the ellipsis button, and then choose **Create from Camera**.</span></span> <span data-ttu-id="c5e2b-120">Kameraet på tavle-PC-en eller telefon er aktivert.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-120">The camera on the tablet or phone is activated.</span></span>
4. <span data-ttu-id="c5e2b-121">Ta et bilde av et dokument, for eksempel et kjøpsmottak, som du vil behandle som et innkommende dokument, og velg deretter **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-121">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span></span>

<span data-ttu-id="c5e2b-122">En ny innkommende dokumentpost opprettes med bildet vedlagt.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-122">A new incoming document record is created, with the image attached.</span></span>

## <a name="to-attach-an-image-to-an-incoming-document-record-by-taking-a-photo"></a><span data-ttu-id="c5e2b-123">Slik legger du ved et bilde i en innkommende dokumentpost ved å ta et bilde</span><span class="sxs-lookup"><span data-stu-id="c5e2b-123">To attach an image to an incoming document record by taking a photo</span></span>
<span data-ttu-id="c5e2b-124">**Merk**: Fremgangsmåten nedenfor gjelder bare for nettbrett og telefoner med Dynamics NAV-klienter.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-124">**Note**: The following procedure only applies to the Dynamics NAV Tablet and Phone clients.</span></span>

1. <span data-ttu-id="c5e2b-125">Velg Alternativer-knappen i appfeltet, velg **Innkommende dokumenter**, og velg deretter **Alle**.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-125">On the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span></span>
2. <span data-ttu-id="c5e2b-126">Åpne kortet for en eksisterende innkommende dokumentpost.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-126">Open the card for an existing incoming document record.</span></span>
3. <span data-ttu-id="c5e2b-127">I vinduet **Inngående dokument** velger du ellipseknappen, og deretter velger du **Legg ved bilde fra kamera**.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-127">In the **Incoming Document** window, choose the ellipsis button, and then choose **Attach Image from Camera**.</span></span> <span data-ttu-id="c5e2b-128">Kameraet på tavle-PC-en eller telefon er aktivert.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-128">The camera on the tablet or phone is activated.</span></span>
4. <span data-ttu-id="c5e2b-129">Ta et bilde av et dokument, for eksempel et kjøpsmottak, som du vil behandle som et innkommende dokument, og velg deretter **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-129">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span></span>

<span data-ttu-id="c5e2b-130">Bildet legges ved den innkommende dokumentposten.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-130">The image is attached to the incoming document record.</span></span>

## <a name="to-create-an-incoming-document-record-manually"></a><span data-ttu-id="c5e2b-131">Slik oppretter du en innkommende dokumentpost manuelt:</span><span class="sxs-lookup"><span data-stu-id="c5e2b-131">To create an incoming document record manually</span></span>
1. <span data-ttu-id="c5e2b-132">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Inngående dokumenter** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-132">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="c5e2b-133">Velg handlingen **Opprett fra fil**.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-133">Choose the **Create from File** action.</span></span>  
3. <span data-ttu-id="c5e2b-134">I **Sett inn fil**-vinduet velger du en fil og deretter **Åpne**.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-134">In the **Insert File** window, select a file, and then choose **Open**.</span></span>

    <span data-ttu-id="c5e2b-135">Filen legges ved automatisk.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-135">The file is automatically attached.</span></span>
4. <span data-ttu-id="c5e2b-136">Du kan også velge handlingen **Ny**.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-136">Alternatively, choose the **New** action.</span></span>
5. <span data-ttu-id="c5e2b-137">Hvis du vil legge ved en fil, velger du handlingen **Legg ved fil**.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-137">To attach a file, choose the **Attach File** action.</span></span>
6. <span data-ttu-id="c5e2b-138">I vinduet **Sett inn fil** velger du filen som representerer det innkommende dokumentet, og deretter velger du **Åpne**- knappen.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-138">In the **Insert File** window, select the file that represents the incoming document in question, and then choose the **Open** button.</span></span>
7. <span data-ttu-id="c5e2b-139">Fyll ut feltene etter behov i vinduet **Inngående dokument**.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-139">In the **Incoming Document** window, fill in the fields as necessary.</span></span> <span data-ttu-id="c5e2b-140">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="c5e2b-140">Choose a field to read a short description of the field or link to more information.</span></span>

##<a name="see-also"></a><span data-ttu-id="c5e2b-141">Se også</span><span class="sxs-lookup"><span data-stu-id="c5e2b-141">See Also</span></span>  
[<span data-ttu-id="c5e2b-142">Behandle inngående dokumenter</span><span class="sxs-lookup"><span data-stu-id="c5e2b-142">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="c5e2b-143">Inngående dokumenter</span><span class="sxs-lookup"><span data-stu-id="c5e2b-143">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="c5e2b-144">Håndtere kjøp</span><span class="sxs-lookup"><span data-stu-id="c5e2b-144">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="c5e2b-145">Arbeide med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="c5e2b-145">Work With Dynamics NAV</span></span>](ui-work-product.md)

