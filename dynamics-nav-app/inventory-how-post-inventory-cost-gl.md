---
title: "Bokføre lagerkost i finans"
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
ms.openlocfilehash: 59815db9c7b435ff585e1174b570029a360dea6e
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-post-inventory-costs-to-the-general-ledger"></a>Bokføre lagerkost i finans   
Når du bokfører lagertransaksjoner, for eksempel følgesedler, kjøpsfakturaer eller lagerjusteringer, registreres endringene i antall og kostnader i henholdsvis varepostene og verdipostene. For å gjenspeile endringen i lagerverdien i regnskapet, må du bokføre lagerkost til de relaterte lagerkontoene i Finans.

Du kan bokføre lagerkost til finans på to måter:

- Automatisk, slik at lagerkost bokføres til Finans hver gang du bokfører en lagertransaksjon.
- Manuelt, slik at lagerkost bokføres til finans bare når du kjører en satsvis jobb.


## <a name="to-post-inventory-costs-automatically"></a>Slik bokfører du lagerkost automatisk
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Lageroppsett** og velger deretter den relaterte koblingen.
2. I vinduet **Lageroppsett** merker du av for **Automatisk kostbokføring**.

For hver lagertransaksjon du bokfører, bokføres de aktuelle verdiene i lagerkontoen, justeringskontoen og vareforbrukskontoen i Finans.

Selv om du bruker automatisk kostbokføring, må du fremdeles kjøre kjørselen Juster kostverdi - vareposter for å sikre at kostbeløpene for varer videresendes til de riktige utgående transaksjonene, for eksempel salg eller overføringer. Dette er særlig viktig i situasjoner der du selger varer før du fakturerer kjøpet av varene.

Hvis det oppstår en feil i dimensjonsoppsettet mens programmet bokfører lagerkost i Finans, slutter bokføringen med en feil.

## <a name="to-post-inventory-costs-manually"></a>Slik bokfører du lagerkost manuelt
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Bokfør lagerkost i Finans** og velger deretter den relaterte koblingen.
2. Bokfør lagerkost manuelt i Finans ved å starte kjørselen. Når du kjører denne kjørselen, opprettes finansposter på grunnlag av verdiposter. Du kan bokføre postene slik at de summeres per bokføringsgruppe.

**Merk**: Når du kjører denne kjørselen, kan det oppstå feil som har å gjøre med manglende oppsett eller inkompatibelt dimensjonsoppsett. Hvis det oppstår feil i dimensjonsoppsettet, overstyrer kjørselen disse feilene og bruker dimensjonene til verdiposten. Hvis det oppstår en annen type feil, hopper kjørselen over bokføringen av verdipostene og viser en oversikt over dem på slutten av rapporten, i en del med overskriften “Poster som er hoppet over”. Hvis du vil bokføre disse postene, må du rette opp feilene.

Hvis du vil ha en oversikt over feil før du kjører bokføringskjørselen, kan du kjøre rapporten **Bokfør lagerkost i Finans - test**. Kontrollrapporten viser en oversikt over alle feilene som har oppstått under en kontrollbokføring. Du kan deretter rette opp feilene og kjøre kjørselen for lagerkost uten å hoppe over noen poster.

Hvis du ganske enkelt vil ha en oversikt over hvilke verdier som kan bokføres i Finans, uten faktisk å utføre bokføringen, kan du kjøre kjørselen Bokfør lagerkost i Finans uten faktisk å bokføre verdiene i Finans. Du gjør dette ved å fjerne merket i Bokfør-feltet på forespørselssiden. På denne måten genereres rapporten som viser verdiene som er klare til bokføring i Finans, når du kjører kjørselen, men de bokføres ikke.

## <a name="see-also"></a>Se også
[Håndtere lager](inventory-manage-inventory.md)    
[Justere varekost](inventory-how-adjust-item-costs.md)  
[Håndtere salg](sales-manage-sales.md)  
[Håndtere kjøp](purchasing-manage-purchasing.md)

