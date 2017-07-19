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
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 2bce97c76876c86a576ec6a281a306a46881027c
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-incoming-documents"></a>Konfigurere inngående dokumenter
Hvis du oppretter finanskladdelinjer fra innkommende dokumentposter, må du angi hvilken kladdemal og kladd som skal brukes i vinduet **Oppsett for inngående dokumenter**.

Hvis du ikke vil at brukerne skal opprette fakturaer eller finanskladdelinjer fra innkommende dokumentposter med mindre dokumentene først er godkjent, må du definere godkjennere i vinduet **Godkjennere for inngående dokumenter**.

Hvis du vil gjøre om PDF- og bildefiler til elektroniske dokumenter som du kan konvertere til, for eksempel kjøpsfakturaer i Dynamics NAV, må du først sette opp OCR-funksjonen og aktivere tjenesten.

Når funksjonen for inngående dokumenter er konfigurert, kan du bruke forskjellige funksjoner til å se gjennom utgiftskvitteringer, behandle OCR-oppgaver og konvertere inngående dokumentfiler, manuelt eller automatisk, til de aktuelle dokumentene eller kladdelinjene. De eksterne filene kan tilknyttes på et hvilket som helst tidspunkt i prosessen, inkludert bokførte dokumenter og resulterende leverandør, kunde- og finansposter. Hvis du vil ha mer informasjon, kan du se [Behandle inngående dokumenter](across-process-income-documents.md).

## <a name="to-set-up-the-incoming-documents-feature"></a>Slik konfigurerer du funksjonen for inngående dokumenter:
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Oppsett for inngående dokumenter** og velger deretter den relaterte koblingen.
2. Fyll ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.

## <a name="to-set-up-approvers-of-incoming-document-records"></a>Slik definerer du godkjennere av inngående dokumentposter:
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Oppsett for inngående dokumenter** og velger deretter den relaterte koblingen.  
2. I vinduet **Oppsett for inngående dokumenter** velger du handlingen **Godkjennere**.

    Vinduet **Godkjennere for inngående dokumenter** viser alle brukerne som er definert i Dynamics NAV.  
3. Velg én eller flere brukere som kan godkjenne et innkommende dokument før det kan opprettes en relatert dokument- eller kladdelinje.

Når godkjennere er definert i vinduet **Godkjennere for inngående dokumenter**, er det bare disse brukerne som kan godkjenne et inngående dokument hvis det er merket av for **Krev godkjenning for opprettelse** i vinduet **Oppsett for inngående dokumenter**.

**Merk**: Dette godkjenningsoppsettet er ikke relatert til arbeidsflyter for godkjenning. Hvis du vil ha mer informasjon, kan du se [Bruke arbeidsflyter for godkjenning](across-how-use-approval-workflows.md).

## <a name="to-set-up-an-ocr-service"></a>Slik definerer du en OCR-tjeneste:
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Oppsett for OCR-tjeneste** og velger deretter den relaterte koblingen.
2. Fyll ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.


## <a name="to-encrypt-your-login-information"></a>Slik krypterer du påloggingsinformasjonen:
Det anbefales at du beskytter påloggingsinformasjonen du angir i vinduet **Oppsett for OCR-tjeneste**. Du kan kryptere data på serveren ved å generere nye eller importere eksisterende krypteringsnøkler du aktiverer på serverforekomsten som kobler til databasen.

1. I vinduet **Oppsett for OCR-tjeneste** velger du handlingen **Krypteringsadministrasjon**.
2. I vinduet **Administrasjon av datakryptering** aktiverer du kryptering av dataene.

## <a name="see-also"></a>Se også  
[Behandle inngående dokumenter](across-process-income-documents.md)  
[Inngående dokumenter](across-income-documents.md)  
[Håndtere kjøp](purchasing-manage-purchasing.md)  
[Arbeide med Dynamics NAV](ui-work-product.md)

