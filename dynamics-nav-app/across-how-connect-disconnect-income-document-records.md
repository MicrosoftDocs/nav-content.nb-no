---
title: "Koble til og fra inngående dokumentposter fra dokumenter og poster"
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
ms.openlocfilehash: fece4e6e38075db6d394c71418fda82a7aa082e1
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-connect-and-disconnect-incoming-document-records-from-documents-and-entries"></a>Koble til og fra inngående dokumentposter fra dokumenter og poster
Du kan lagre eksterne forretningsdokumenter i Dynamics NAV ved å knytte dokumentfilene til de relaterte inngående dokumentpostene. Hvis dokumentet, for eksempel en kjøpsfaktura, ikke ble opprettet som en innkommende dokumentpost, kan du likevel opprette og koble en innkommende dokumentpost til det senere. Du kan også knytte inngående dokumentfiler til bokførte kjøps- og salgsdokumenter og til leverandør-, kunde- og finansposter ved hjelp av faktaboksen **Inngående dokumentfiler**, for eksempel i vinduet **Bokførte kjøpsfakturaer** og **Leverandørposter**.

Fra vinduene **Kontoplan** og **Finansposter** kan du bruke søkefunksjonen til å finne finansposter for bokførte kjøps- og salgsdokumenter som ikke har innkommende dokumentposter, og deretter sentralt koble eksisterende poster eller opprette nye med vedlagte dokumentfiler. Hvis du vil ha mer informasjon, kan du se [Finne bokførte dokumenter uten innkommende dokumentposter](across-how-find-posted-documents-without-income-document-records.md).

De følgende fremgangsmåtene viser hvordan du knytter en fil til en eksisterende kjøpsfaktura som ikke ble opprettet fra en innkommende dokumentpost, og hvordan du knytter en fil til en leverandørpost. Å knytte en en fil til bokførte kjøps- eller salgsdokumenter fungerer på en lignende måte.

## <a name="to-create-and-connect-an-incoming-document-record-from-a-purchase-invoice"></a>Slik oppretter og kobler du en innkommende dokumentpost fra en kjøpsfaktura:
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kjøpsfakturaer** og velger deretter den relaterte koblingen.
2. Velg linjen for en kjøpsfaktura du vil knytte en fil til, og velg deretter handlingen **Opprett inngående dokument fra fil**.
3. Du kan eventuelt velge linjen for en kjøpsfaktura du vil knytte en fil til, og deretter velge handlingen **Tilknytt fil**.
4. I vinduet **Sett inn fil** velger du filen som representerer det innkommende dokumentet, og deretter velger du **Åpne**- knappen.

## <a name="to-create-and-connect-an-incoming-document-record-from-a-vendor-ledger-entry"></a>Slik oppretter og kobler du en innkommende dokumentpost fra en leverandørpost:
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Leverandørposter** og velger deretter den relaterte koblingen.
2. Velg en linje for en leverandørpost du vil knytte en fil til, og velg deretter handlingen **Opprett inngående dokument fra fil**.
3. Du kan eventuelt velge en linje for en leverandørpost du vil knytte en fil til, og deretter velge handlingen **Tilknytt fil**.
4. I vinduet **Sett inn fil** velger du filen som representerer det innkommende dokumentet, og deretter velger du **Åpne**- knappen.

## <a name="to-remove-a-connection-from-an-incoming-document-record-to-a-posted-document"></a>Slik fjerner du tilkoblingen fra en innkommende dokumentpost til et bokført dokument:
Du kan fjerne filvedlegg fra ikke-bokførte dokumenter når som helst ved å slette den relaterte innkommende dokumentposten. Hvis dokumentet er bokført, må du først fjerne tilkoblingen fra den innkommende dokumentposten.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Inngående dokumenter** og velger deretter den relaterte koblingen.
2. Velg linjen for en inngående dokumentpost som er koblet til et bokført dokument du vil fjerne, og velg deretter handlingen **Fjern referanse til post**.

Tilkoblingen til det bokførte dokumentet fjernes. Nå kan du fortsette med å koble en annen innkommende dokumentpost til det bokførte dokumentet, som beskrevet i dette emnet.

## <a name="see-also"></a>Se også  
[Behandle inngående dokumenter](across-process-income-documents.md)  
[Inngående dokumenter](across-income-documents.md)  
[Håndtere kjøp](purchasing-manage-purchasing.md)  
[Arbeide med Dynamics NAV](ui-work-product.md)

