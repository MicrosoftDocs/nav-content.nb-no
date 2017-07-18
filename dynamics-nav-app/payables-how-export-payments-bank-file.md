---
title: Eksportere betalinger til en bankfil
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
ms.openlocfilehash: 09bdf56b3d5e76b12d868091e89232ce9c08e215
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-export-payments-to-a-bank-file"></a>Eksportere betalinger til en bankfil
Når du er klar til å utføre betalinger til leverandører ved hjelp av vinduet **Betalingskladd**, kan du eksportere en fil med betalingsinformasjonen for kladdelinjene. Du kan deretter laste opp filen til nettbanken for å behandle de relaterte pengeoverføringene.

I den generelle versjonen av Dynamics NAV er det konfigurert og koblet til en global tjenesteleverandør for å konvertere bankdata til hvilket som helst format banken krever.

**Merk**: Før du kan eksportere fra en utbetalingskladd, må du aktivere eksport på den tilhørende kladden. I tillegg må din bankkonto og leverandørens bankkonto konfigureres for elektronisk betaling. Hvis du vil ha mer informasjon, kan du se [Konfigurere konverteringstjenesten for bankdata](bank-how-setup-bank-data-conversion-service.md)

Du bruker vinduet **Kredittoverføringsregistre** til å vise betalingsfilene som er eksportert fra betalingskladden. Fra dette vinduet kan du også eksportere betalingsfiler på nytt ved tekniske feil eller endringer.

## <a name="to-export-payments-to-a-bank-file"></a>Slik eksporterer du betalinger til en bankfil:
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Betalingskladder** og velger deretter den relaterte koblingen.
2. Fyll ut utbetalingskladdelinjer, for eksempel ved hjelp av funksjonen **Betalingsforslag - leverandør**. Hvis du vil ha mer informasjon, kan du se [Betalingsforslag - leverandør](payables-how-suggest-vendor-payments.md).  
3. Når du har fullført alle betalingskladdlinjene, velger du **Eksporter betaling til fil**.

    Eventuelle feilmeldinger vises i faktaboksen **Feil i betalingsfil**, der du også kan velge en feilmelding hvis du vil ha mer informasjon. Du må løse alle feil før betalingsfilen kan eksporteres.

    **Tips**: Når du bruker funksjonen for konverteringstjeneste for bankdata, kan du få en vanlig feilmelding om at bankkontonummeret ikke har lengden som banken krever. Hvis du vil unngå eller løse feilen, må du fjerne verdien i **IBAN**-feltet i vinduet **Bankkort**, og i **Bankkontonr.** -feltet angir du deretter et bankkontonummer i formatet som banken krever.
4. I vinduet **Lagre som** angir du plasseringen som filen som blir eksportert til, og deretter velger du **Lagre**.

Bankbetalingsfilen eksporteres til plasseringen du angir, og du kan deretter laste den opp til nettbankkontoen og foreta de faktiske betalingene.

Når du får bekreftet at betalingene er behandlet i den elektroniske banken, kan du bokføre de eksporterte utbetalingskladdelinjene.

## <a name="to-plan-when-to-post-exported-payments"></a>Planlegge når du bokfører eksporterte betalinger
Hvis du ikke vil bokføre en utbetalingskladdelinje for en eksportert betaling, for eksempel fordi du venter på bekreftelse på at transaksjonen er behandlet av banken, kan du bare slette kladdelinjen. Når du senere oppretter en utbetalingskladdelinje for å betale restbeløpet på fakturaen, viser feltet **Totalt eksportert beløp** hvor mye av betalingsbeløpet som allerede er eksportert. Du kan også finne detaljert informasjon om det eksporterte totalbeløpet ved å velge knappen **Poster i kredittoverføringsreg.** for å vise mer informasjon om eksporterte betalingsfiler.

Hvis du følger en prosess der du ikke bokfører betalinger før du har fått bekreftelse på at de har blitt behandlet i banken, kan du kontrollere dette på to måter.

* I en betalingskladd med foreslåtte betalingslinjer kan du sortere etter kolonnen **Lest ut til betalingsfil** eller **Totalt eksportert beløp**, og deretter slette betalingsforslag for åpne fakturaer som allerede er betalt og du ikke ønsker å betale.
* Du kan merke av for **Hopp over eksporterte betalinger** i vinduet **Betalingsforslag - leverandør**, der du angir hvilke betalinger som skal settes inn i utbetalingskladden, hvis du ikke vil sette inn kladdelinjer for betalinger som allerede er eksportert.

Du kan vise informasjon om eksporterte betalinger ved å velge handlingen **Historikk for betalingseksport**.

## <a name="to-re-export-payments-to-a-bank-file"></a>Eksportere betalinger til en bankfil på nytt
Du kan eksportere betalingsfiler på nytt fra vinduet **Kredittoverføringsregistre**. Før du sletter eller bokfører utbetalingskladdelinjer, kan du også eksportere betalingsfilen på nytt fra vinduet **Betalingskladd**.

Hvis du har slettet eller bokført utbetalingskladdelinjer etter at du har eksportert dem, kan du eksportere samme betalingsfil på nytt fra vinduet **Kredittoverføringsregistre**. Velg linjen for bunken med kredittoverføringer du vil eksportere på nytt, og bruk handlingen **Eksporter betalinger til fil på nytt**.

## <a name="see-also"></a>Se også
[Kjøp](payables-manage-payables.md)  
[Håndtere kjøp](purchasing-manage-purchasing.md)  
[Definere kjøp](purchasing-setup-purchasing.md)

