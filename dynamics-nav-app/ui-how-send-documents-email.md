---
title: Sende dokumenter i e-post
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: e4476c2ab903001017dcd6c8bdaa84892ba79c9e
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-send-documents-by-email"></a>Sende dokumenter i e-post
For å formidle innholdet i forretningsdokumenter raskt til dine forretningspartnere, for eksempel betalingsinformasjon for salgsdokumenter for kunder, kan du bruke funksjonen Rapportoppsett til å definere dokumentspesifikt innhold som blir satt inn automatisk i brødteksten i e-post.

Hvis du vil aktivere e-postmeldinger fra Dynamics NAV, starter du det assisterte oppsettet **Konfigurer e-post** på Hjem-siden.

Du kan sende nesten alle dokumenttyper som vedlegg i e-postmeldinger direkte fra vinduet som viser dokumentet. I tillegg til vedlegget kan du definere dokumentspesifikke brødtekster for e-post med kjerneinformasjon fra dokumentet, som innledes med standardtekst som hilser e-postmottakeren og introduserer det aktuelle dokumentet. For å tilby kundene å betale for salg med elektroniske betalingstjenester, for eksempel PayPal, kan du også sette inn PayPal-informasjonen og -hyperkoblingen i brødteksten i e-posten.

Fra alle dokumenter som støttes starter du sending i e-post ved å velge handlingen **Send** på bokførte dokumenter, eller handlingen **Bokfør og send** på dokumenter som ikke er bokført.

Hvis **E-post**-feltet i vinduet **Send dokument til** er satt til **Ja (spør om innstillinger)**, vil vinduet **Send e-post** åpnes forhåndsutfylte med kontaktpersonen i **Til**-feltet og dokumentet vedlagt som en PDF-fil. I **Brødtekst**-feltet kan du angi tekst manuelt eller du kan la feltet fylles ut med en dokumentspesifikk brødtekst for e-post, som du har definert.

Fremgangsmåten nedenfor beskriver hvordan du konfigurerer rapporten **Salg - faktura** til bruk for dokumentspesifikke brødtekster for e-post når du sender bokførte salgsfakturaer i e-post.

## <a name="to-set-up-a-document-specific-email-body-for-sales-invoices"></a>Konfigurere en dokumentspesifikk brødtekst for e-post for salgsfakturaer
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Rapportvalg - salg** og velger deretter den relaterte koblingen.
2. I vinduet **Rapportvalg - salg**, i **Bruk**-feltet, velger du **Faktura**.
3. På en ny linje i **-Rapport-ID**-feltet, velger du for eksempel standardrapport 1306.
4. Merk av for **Bruk for brødtekst i e-post**.
5. Velg feltet **Oppsett-ID for brødtekst i e-post**, og velg deretter ett av oppsettene som er tilgjengelige i vinduet **Egendefinerte rapportoppsett**.
6. Rapportoppsett definerer stilen og innholdet i selve brødteksten i e-posten, inkludert standardteksten som kommer foran kjerneinformasjonen i dokumentet i brødteksten i e-post.
7. Hvis du vil vise eller redigere oppsettet som brødteksten i e-post er basert på, går du til vinduet **Egendefinerte rapportoppsett** og velger handlingen **Rediger oppsett**.
8. Hvis du vil tilby kundene å betale for salg med elektroniske, kan du konfigurere de relaterte betalingstjenestene, for eksempel PayPal, og deretter også sette inn PayPal-informasjonen og -hyperkoblingen i brødteksten i e-posten. Hvis du vil ha mer informasjon, kan du se [Aktivere kundebetalinger via PayPal](sales-how-enable-customer-payments-paypal.md).
9. Velg **OK**-knappen.

Nå når du for eksempel velger Send-handlingen i vinduet **Bokført salgsfaktura**, vil brødteksten i e-posten inneholde dokumentinformasjonen fra rapport 1306 foran standardteksten i henhold til rapportoppsettet du valgte i trinn 5.

Fremgangsmåten nedenfor beskriver hvordan du sender en bokført salgsfaktura som en e-postmelding med dokumentet vedlagt som en PDF-fil og en dokumentspesifikk brødtekst i e-posten.
## <a name="to-send-documents-by-email"></a>Sende dokumenter i e-post
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Bokførte salgsfakturaer** og velger deretter den relaterte koblingen.
2. Velg den relevante salgsfakturaen, og velg handlingen **Send**. Vinduet **Send dokument til** åpnes.
3. I feltet **E-post** velger du **Ja (spør om innstillinger)**. Hvis du vil ha mer informasjon, kan du se [Definere en profil for dokumentsending](sales-how-setup-document-send-profiles.md).
4. Velg **OK**-knappen. Vinduet **Send e-post** åpnes.
5. Angi en gyldig e-postadresse i **Til**-feltet. Standardverdien er kundens e-postadresse.
6. Angi en e-postadresse i **Kopi**-feltet for å sende en kopi av e-postmeldingen til en annen mottaker.
7. Angi en e-postadresse i **Blindkopi**-feltet for å sende kopi av e-postmeldingen til en annen mottaker uten at e-postadressen og navnet vises for andre mottakere.
8. Angi en beskrivende emnetekst i **Emne**-feltet. Standardverdien er kundenavnet og fakturanummeret.
9. Den genererte fakturaen legges som standard ved som en PDF-fil i **Vedlegg**-feltet. Velg oppslagsknappen for å åpne filen eller legge ved en annen.
10. Skriv inn en kort melding til mottakeren i **Tekst**-feltet.

    Hvis en dokumentspesifikke brødtekst i e-post er konfigurert i vinduet **Rapportvalg - salg**, fylles **Brødtekst**-feltet ut automatisk. Hvis du vil ha mer informasjon, kan du se avsnittet “Konfigurere en dokumentspesifikk brødtekst for e-post for salgsfakturaer” i dette emnet.
11. Merk av for **Rediger i Outlook Web App** for å åpne e-postmeldingen i e-postappen for Office 365.
12. Velg **OK**-knappen for å sende e-postmeldingen.

**Merk**: Hvis du ikke vil angi postinnstillinger hver gang du sender et dokument i e-post, kan du velge alternativet **Ja (bruk standardinnstillinger)** i E-post-feltet i vinduet **Sende dokument til**. I så fall åpnes ikke vinduet **Send e-post**. Se trinn 4. Hvis du vil ha mer informasjon, kan du se [Definere en profil for dokumentsending](sales-how-setup-document-send-profiles.md).

## <a name="see-also"></a>Se også  
[Arbeide med Dynamics NAV](ui-work-product.md)  
[Fakturere salg](sales-how-invoice-sales.md)

