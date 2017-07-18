---
title: Opprette innkommende dokumentposter
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
ms.openlocfilehash: 10ba191b197be8b98b2d5d5ab9ac4bc3baf0d82b
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-create-incoming-document-records"></a>Opprette innkommende dokumentposter
I vinduet **Inngående dokumenter** kan du bruke forskjellige funksjoner til å se gjennom utgiftskvitteringer, behandle OCR-oppgaver og konvertere inngående dokumentfiler, manuelt eller automatisk, til de aktuelle dokumentene eller kladdelinjene. De eksterne filene kan tilknyttes på et hvilket som helst tidspunkt i prosessen, inkludert bokførte dokumenter og resulterende leverandør, kunde- og finansposter.

Hvis du vil registrere et eksternt dokument i Dynamics NAV, må du først opprette eller fullføre en innkommende dokumentpost. Du kan gjøre dette manuelt, eller du kan ta et bilde av det eksterne dokumentet og deretter opprette den inngående dokumentposten med bildefilen som vedlegg.

Før du kan bruke funksjonen for inngående dokumenter, må du utføre den nødvendige konfigurasjonen. Hvis du vil ha mer informasjon, kan du se [Konfigurere inngående dokumenter](across-how-setup-income-documents.md).

## <a name="to-approve-or-reject-an-incoming-document"></a>Slik godkjenner eller avviser du et innkommende dokument
Hvis du vil tillate brukere å opprette fakturaer eller finanskladdelinjer fra innkommende dokumentposter med mindre de er godkjent, kan du definere godkjennere som må godkjenne postene før de kan behandles.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Inngående dokumenter** og velger deretter den relaterte koblingen.
2. Velg linjen med dokumentet som du vil godkjenne eller avvise, og velg deretter handlingen **Godkjenn** eller **Avvis**.

Hvis du godkjenner den inngående dokumentposten, merkes det av for **Frigitt** på linjen for det inngående dokumentet. Brukeren som for eksempel er ansvarlig for å opprette kjøpsfakturaer, kan fortsette å behandle posten.

## <a name="to-create-an-incoming-document-record-by-taking-a-photo"></a>Slik oppretter du en innkommende dokumentpost ved å ta et bilde
**Merk**: Fremgangsmåten nedenfor gjelder bare for nettbrett og telefoner med Dynamics NAV-klienter.

1. I appfeltet velger du **Opprett innkommende dokument fra kamera**-flisen, og gå deretter til trinn 4.
2. Alternativt kan du velge Alternativer-knappen i appfeltet, velge **Innkommende dokumenter**, og deretter velge **Alle**.
3. I vinduet **Inngående dokumenter** velger du ellipseknappen, og deretter velger du **Opprett fra kamera**. Kameraet på tavle-PC-en eller telefon er aktivert.
4. Ta et bilde av et dokument, for eksempel et kjøpsmottak, som du vil behandle som et innkommende dokument, og velg deretter **OK**-knappen.

En ny innkommende dokumentpost opprettes med bildet vedlagt.

## <a name="to-attach-an-image-to-an-incoming-document-record-by-taking-a-photo"></a>Slik legger du ved et bilde i en innkommende dokumentpost ved å ta et bilde
**Merk**: Fremgangsmåten nedenfor gjelder bare for nettbrett og telefoner med Dynamics NAV-klienter.

1. Velg Alternativer-knappen i appfeltet, velg **Innkommende dokumenter**, og velg deretter **Alle**.
2. Åpne kortet for en eksisterende innkommende dokumentpost.
3. I vinduet **Inngående dokument** velger du ellipseknappen, og deretter velger du **Legg ved bilde fra kamera**. Kameraet på tavle-PC-en eller telefon er aktivert.
4. Ta et bilde av et dokument, for eksempel et kjøpsmottak, som du vil behandle som et innkommende dokument, og velg deretter **OK**-knappen.

Bildet legges ved den innkommende dokumentposten.

## <a name="to-create-an-incoming-document-record-manually"></a>Slik oppretter du en innkommende dokumentpost manuelt:
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Inngående dokumenter** og velger deretter den relaterte koblingen.
2. Velg handlingen **Opprett fra fil**.  
3. I **Sett inn fil**-vinduet velger du en fil og deretter **Åpne**.

    Filen legges ved automatisk.
4. Du kan også velge handlingen **Ny**.
5. Hvis du vil legge ved en fil, velger du handlingen **Legg ved fil**.
6. I vinduet **Sett inn fil** velger du filen som representerer det innkommende dokumentet, og deretter velger du **Åpne**- knappen.
7. Fyll ut feltene etter behov i vinduet **Inngående dokument**. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.

##<a name="see-also"></a>Se også  
[Behandle inngående dokumenter](across-process-income-documents.md)  
[Inngående dokumenter](across-income-documents.md)  
[Håndtere kjøp](purchasing-manage-purchasing.md)  
[Arbeide med Dynamics NAV](ui-work-product.md)

