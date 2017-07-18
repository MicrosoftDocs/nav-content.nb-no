---
title: Periodisere inntekter og utgifter
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
ms.openlocfilehash: 865bc307e8635b5a5aba11b5bc2e2e448c05e769
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-defer-revenues-and-expenses"></a>Periodisere inntekter og utgifter
Hvis du føre inn en inntekt eller en utgift i en annen periode enn perioden som transaksjonen ble bokført, kan du bruke funksjonaliteten til å periodisere automatisk inntekter og utgifter etter en angitt tidsplan.

Hvis du vil fordele inntekter eller utgifter på de aktuelle regnskapsperiodene, konfigurerer du en periodiseringsmal for ressursen, varen eller finanskontoen, som det vil bli bokført inntekt eller utgift for. Når du bokfører det aktuelle salgs- eller kjøpsdokumentet, periodiseres inntekter eller utgifter til de aktuelle regnskapsperiodene i henhold til en tidsplan for periodisering som styres av innstillingene i malen for periodisering og bokføringsdatoen.

## <a name="to-set-up-a-gl-account-for-deferral"></a>Slik definerer du finanskonti for periodisering
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kontoplan** og velger deretter den relaterte koblingen.
2. Velg handlingen **Ny**.
3. Fyll ut feltene som er nødvendige for å opprette en finanskonto for periodiserte inntekter. Hvis du vil ha mer informasjon, kan du se [Økonomimodulen og kontoplanen](finance-setup-general-ledger.md).
3. Gjenta trinn 2 og 3 for å opprette en ny finanskonto for periodiserte utgifter.

For begge typer periodisering velger du **Balanse** i **Type**-feltet og gir navn til kontoene, for eksempel "Ikke tjent inntekt" for periodisert inntekt og "Ubetalte utgifter" for periodiserte utgifter.

## <a name="to-set-up-a-deferral-template"></a>Slik definerer du mal for periodisering
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Maler for periodisering** og velger deretter den relaterte koblingen.
2. Velg handlingen **Ny**.
3. Fyll ut feltene etter behov.
4. I **Beregningsmetode**-feltet angi du hvordan **Beløp**-feltet beregnes for hver periode i vinduet **Tidsplan for periodisering**. Du kan velge mellom følgende alternativer:
    - **Lineær**: De periodiske periodiseringsbeløpene beregnes etter antall perioder, distribuert i henhold til periodelengde.
    - **Lik per periode**: De periodiske periodiseringsbeløpene beregnes etter antall perioder, distribuert jevnt på perioder.
    - **Dager per periode**: De periodiske periodiseringsbeløpene beregnes etter antall dager i perioden.
    - **Brukerdefinert**: De periodiske periodiseringsbeløpene beregnes ikke. Du må manuelt fylle ut Beløp-feltet for hver periode i vinduet Tidsplan for periodisering. Hvis du vil ha mer informasjon, kan du se avsnittet Slik endrer du en tidsplan for periodisering fra en salgsfaktura.

5. I **Periodebeskr.** -feltet angir du en beskrivelse som vises i poster for periodiseringsbokføringen. Du kan angi plassholderkodene nedenfor en for vanlige verdier som skal settes inn automatisk når periodebeskrivelsen vises.
    - %1 = Dagnummeret for periodebokføringsdatoen
    - %2 = Ukenummeret for periodebokføringsdatoen
    - %3 = Månedsnummeret for periodebokføringsdatoen
    - %4 = Månedsnavnet for periodebokføringsdatoen
    - %5 = Regnskapsperiodenavnet for periodebokføringsdatoen
    - %6 = Regnskapsåret for periodebokføringsdatoen

Eksempel: Bokføringsdatoen er 06.02.2016. Hvis du angir "Utgifter periodisert for %4 %6", blir beskrivelsen som vises "Utgifter periodisert for februar 2016".

## <a name="to-assign-a-deferral-template-to-an-item"></a>Slik tilordner du en mal for periodisering til en vare
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Maler for periodisering** og velger deretter den relaterte koblingen.
2. Åpne kortet for varen som inntekter eller utgifter skal periodiseres for til regnskapsperiodene da varen ble solgt eller kjøpt.
3. I feltet **Standard mal for periodisering** , velger du den aktuelle malen for periodisering.

## <a name="to-change-a-deferral-schedule-from-a-sales-invoice"></a>Slik endrer du en tidsplan for periodisering fra en salgsfaktura
**Merk**: Trinnene i denne fremgangsmåten er den samme som når du endrer en tidsplan for periodisering, for utgifter, fra en kjøpsfaktura.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Salgsfakturaer** og velger deretter den relaterte koblingen.
2. Opprett en salgsfaktura for en vare som er tilordnet en mal for periodisering. Hvis du vil ha mer informasjon, kan du se [Fakturere salg](sales-how-invoice-sales.md).

    Legg merke til at så snart du angir varen (eller ressursen eller finanskontoen) på fakturalinjen, fylles **Periodiseringskode**-feltet ut med koden til den tildelte malen for periodisering.
3. Velg handlingen **Tidsplan for periodisering**.
4. I vinduet **Tidsplan for periodisering** endrer du innstillingene på hodet eller verdiene på linjen, for eksempel for å periodisere beløpet til en ekstra regnskapsperiode.
5. Velg handlingen **Beregn tidsplan**.
6. Velg **OK**-knappen. Tidsplanen for periodisering oppdateres for salgsfakturaen. Relaterte malen for periodisering forblir uendret.

## <a name="to-preview-how-deferred-revenues-or-expenses-will-be-posted-to-the-general-ledger"></a>Slik forhåndsviser du hvordan periodiserte inntekter eller utgifter skal bokføres i finans
**Merk**: Trinnene i denne fremgangsmåten er de samme som når du forhåndsviser hvordan periodisering av utgiften bokføres.

1. I vinduet **Salgsfaktura** velger du handlingen **Forhåndsvis bokføring**.
2. I vinduet **Forhåndsvisning av bokføring** velger du **Finanspost**-handlingen og deretter handlingen **Vis relaterte poster**.

Finansposter som skal posteres til den angitte periodiseringskontoen, for eksempel Ikke tjent inntekt, er merket med beskrivelsen du skrev inn i **Periodebeskr.** -feltet i malen for periodisering, for eksempel "Utgifter periodisert for februar 2016".

## <a name="to-review-posted-deferrals-in-the-sales-deferral-summary-report"></a>Slik ser du gjennom bokførte periodiseringer i rapporten Periodiseringssammendrag for Salg
**Merk**: Trinnene i denne fremgangsmåten er de samme som når du ser gjennom rapporten Periodiseringssammendrag for Salg.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Periodiseringssammendrag for Salg** og velger deretter den relaterte koblingen.
2. I vinduet **Periodiseringssammendrag for Salg** i **Saldo per**-feltet, angir du den siste datoen du vil se periodiserte inntekter for.
3. Velg **Forhåndsvisning**-knappen.

## <a name="see-also"></a>Se også
[Finans](finance-setup.md)  
[Definere kjerneprosesser for økonomi](finance-setup-setup-finance-setup.md)  
[Arbeide med finanskladder](ui-work-general-journals.md)

