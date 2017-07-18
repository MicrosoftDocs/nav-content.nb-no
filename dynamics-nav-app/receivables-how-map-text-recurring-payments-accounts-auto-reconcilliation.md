---
title: "Tilordne tekst på gjentakende betalinger til kontoer for automatisk avstemming"
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
ms.openlocfilehash: 7f9bf8b0550f7da1cced995234e15ad7aab484ba
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-map-text-on-recurring-payments-to-accounts-for-automatic-reconciliation"></a>Tilordne tekst på gjentakende betalinger til kontoer for automatisk avstemming
I vinduet **Tekst-til-konto-tilordning**, som du åpner fra vinduet **Betalingsavstemmingskladd**, kan du definere tilordninger mellom tekst på betalinger og bestemte debet-, kredit- og motkonti, slik at slike betalinger bokføres på de angitte kontiene når du bokfører kladden for betalingsavstemming.

**Merk**: Emnet gjelder også når du bruker funksjonen **Tilordne tekst til konto** fra en innkommende dokumentpost til å hjelpe med konvertering av elektroniske dokumenter som mottas fra eksterne tjenester, til dokumenter i Dynamics NAV. Hvis du vil ha mer informasjon, kan du se [Bruke OCR til å konvertere PDF- og bildefiler til elektroniske dokumenter](across-how-use-ocr-pdf-images-files.md).   

Det finnes liknende funksjon hvis du vil avstemme overskytende beløp på linjene for betalingsavstemmingskladd på ad hoc-basis. Hvis du vil ha mer informasjon, kan du se [Avstemme betalinger som ikke kan utlignes automatisk](receivables-how-reconcile-payments-cannot-apply-auto.md)

Betalinger som bokføres basert på tekst-til-kontotilordning, utlignes ikke mot åpne poster, men bokføres bare på bestemte konti, i tillegg til at de oppretter bankkontoposter. Tekst-til-kontotilordning er dermed egnet til gjentakende innbetalinger eller utgifter, for eksempel hyppige kjøp av drivstoff til bil eller bankgebyrer og renter, som regelmessig oppstår på bankkontoutdraget og ikke trenger et tilknyttet forretningsdokument. Hvis du vil ha mer informasjon, kan du se avsnittet “Eksempel – tekst-til-kontotilordning for drivstoffutgifter” i dette emnet.

**Merk**: Betalinger på avstemmingskladdelinjene settes bare til bokføring i henhold til tekst-til-kontotilordning hvis funksjonen for automatisk utligning bare kan gi samsvarskonfidensen **Lav** eller **Middels**. Hvis funksjonen for automatisk utligning gir konfidensintervallet Høy, utlignes betalingen automatisk mot én eller flere åpne poster, og betalingen bokføres ikke på kontiene som er angitt i vinduet **Tekst-til-konto-tilordning**. Samsvarskonfidensen **Høy** overstyrer med andre ord tekst-til-kontotilordning.

På en linje i betalingsavstemmingskladden der betalingen er satt til bokføring i henhold til tekst-til-kontotilordning, inneholder **Konfidensintervall**-feltet **Høy – tekst-til-kontotilordning**, og **Kontotype**- og **Kontonummer** -feltene inneholder de tilordnede kontiene.

## <a name="to-map-text-on-recurring-payments-to-accounts-for-automatic-reconciliation"></a>Tilordne tekst på gjentakende betalinger til kontoer for automatisk avstemming
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Betalingsavstemmingskladder** og velger deretter den relaterte koblingen.
2. Åpne en kladd for betalingsavstemming. Hvis du vil ha mer informasjon, kan du se [Avstemme betalinger ved hjelp av automatisk utligning](receivables-how-reconcile-payments-auto-application.md).
3. Velg handlingen **Tilordne tekst til konto**. Vinduet **Tekst-til-konto-tilordning** åpnes.
4. Skriv inn tekst som forekommer på betalinger du vil bokføre på bestemte konti uten å utligne mot en åpen post, i **Tilordningstekst**-feltet. Du kan angi opptil 50 tegn.

    **Merk**: Hvis ingen andre betalinger eller inngående dokumenter finnes med den aktuelle tilordningsteksten, vil tekst-til-konto-tilordningen skje selv når bare en del av teksten på betalingen eller det inngående dokumentet finnes som tilordningstekst.
5. I **Leverandørnr.**-feltet angir du leverandøren som innkommende dokumenter som inneholder den tilordnede teksten, blir opprettet for, eller som betalinger blir bokført til. Hvis du vil ha mer informasjon, kan du se [Bruke OCR til å konvertere PDF- og bildefiler til elektroniske dokumenter](across-how-use-ocr-pdf-images-files.md).      
6. I **Debetkontonummer** -feltet angir du kontoen som betalinger som inneholder tilordningsteksten, skal bokføres på hvis de er inngående betalinger. For innkommende betalinger er fortegnet for verdien i **Utdragsbeløp**-feltet positivt.
7. I **Kreditkontonummer** -feltet angir du kontoen som betalinger som inneholder tilordningsteksten, skal bokføres på hvis de er utgående betalinger. For utgående betalinger er fortegnet for verdien i **Utdragsbeløp**-feltet negativt.
8. Angi om betalingen skal bokføres på en finanskonto eller en kunde- eller leverandørkonto, i feltet **Saldokildetype**.
9. I **Saldokildenummer** -feltet angir du kontoen som betalingen skal bokføres på, i feltet **Saldokildetype**, avhengig av hva du du valgte i feltet .
10. Gjenta trinn 4 til og med 8 for all tekst på betalinger du vil tilordne til kontoer for direkte bokføring uten utligning.

Neste gang du importerer en bankkontoutdragsfil eller velger handlingen **Utlign automatisk** i vinduet **Betalingsavstemmingskladd**, inneholder kladdelinjene for betalinger som inneholder den angitte tilordningsteksten, de tilordnede kontiene i feltene **Kontotype** og **Kontonummer**. -feltene. Feltet **Konfidensintervall** inneholder **Høy – tekst-til-konto-tilordning**. Dette er under forutsetning av at automatiske utligningsfunksjonen bare kan gi samsvarskonfidensen **Lav** eller **Middels**.

##<a name="example-text-to-account-mapping-for-fuel-expense"></a>Eksempel: Tekst-til-konto-tilordning for drivstoffutgifter

Hvis du alltid vil bokføre drivstoffutgifter påløpt ved Shell-bensinstasjoner til finanskontoen for bensin (konto 8510), fyller du ut en linje som følger i vinduet **Tekst-til-konto-tilordning**.

|Tilordningstekst |Debetkonto Nr. |Kreditkonto Nr. |Motkonto Kildetype |Motkonto Kildenr. |
|-------------|---------------|----------------|-----------------|----------------|
|Shell |TOM |8510 |Finanskonto|TOM|

**Tips**: Hvis du vil ha mer informasjon om hvordan du arbeider med felt og kolonner, kan du se [Arbeide med Dynamics NAV](ui-work-product.md). Hvis du vil ha mer informasjon om hvordan du finner bestemte sider, kan du se [Søke](ui-search.md).

## <a name="see-also"></a>Se også
[Håndtere fordringer](receivables-manage-receivables.md)  
[Håndtere salg](sales-manage-sales.md)  
[Konfigurere bankfeedservicen Envestnet Yodlee](bank-how-setup-bank-statement-service.md)  
[Tilpasse Dynamics NAV ved hjelp av utvidelser](ui-extensions.md)

