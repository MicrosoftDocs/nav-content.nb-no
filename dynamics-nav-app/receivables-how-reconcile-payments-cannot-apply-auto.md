---
title: Avstemme betalinger som ikke kan utlignes automatisk
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
ms.openlocfilehash: f9fd7c2958aaa359d2f6af5dde2e8be81349e900
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-reconcile-payments-that-cannot-be-applied-automatically"></a>Avstemme betalinger som ikke kan utlignes automatisk
Noen ganger må du å håndtere betalinger til din bankkonto som ikke kan utlignes mot en relatert åpen kunde-, leverandør- eller bankkontopost. Årsakene kan være at det ikke finnes dokumenter i Dynamics NAV som betalingen kan utlignes mot, eller at det tilknyttede dokumentet i Dynamics NAV har et annet beløp enn transaksjonsbeløpet, for eksempel på grunn av valutaveksling. I vinduet **Betalingsavstemmingskladd** vises alle transaksjonsbeløp for betalinger som ennå ikke er utlignet i **Differanse** -feltet, inkludert beløp som ikke kan brukes på grunn av årsaker som nevnt ovenfor.

Betalinger som ikke kan brukes, kan vises på linjer for betalingsavstemmingskladd på følgende forskjellige måter:

- Verdien i **Differanse**-feltet er lik verdien i **Transaksjonsbeløp** -feltet, som angir at ingen del av betalingen kan utlignes mot en relatert åpne kunde-, leverandør- eller bankkontopost.

- Verdien i **Differanse**-feltet er lavere enn verdien i **Transaksjonsbeløp** -feltet, som angir at ingen del av betalingen kan utlignes mot en relatert åpne kunde-, leverandør- eller bankkontopost. Den gjenværende delen av betalingen kan ikke utlignes og må avstemmes manuelt eller ved å bokføre den direkte til en konto.

Hvis du vil avstemme slike betalinger, kan du velge Overfør differanse til konto-knappen, og deretter angir du hvilken konto beløpet i Differanse-feltet bokføres til når du bokfører betalingsavstemmingskladd.

**Merk**: Det finnes lignende funksjonalitet for å konfigurere automatisk avstemming av regelmessige betalinger som ikke kan utlignes mot relaterte åpne kunde-, leverandør- eller bankkontoposter. [Hvis du vil ha mer informasjon, kan du se Tilordne tekst på gjentakende betalinger til kontoer for automatisk avstemming](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md)

## <a name="to-reconcile-payments-that-cannot-be-applied"></a>Avstemme betalinger som ikke kan utlignes
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Betalingsavstemmingskladder** og velger deretter den relaterte koblingen.
2. Åpne en kladd for betalingsavstemming. Hvis du vil ha mer informasjon, kan du se [Avstemme betalinger ved hjelp av automatisk utligning](receivables-how-reconcile-payments-auto-application.md).
3. Velg **Overfør differanse til konto**. Vinduet **Overfør differanse til konto** 3. åpnes.
4. I **Kontotype**-feltet angir du om kontotypen som betalingsbeløpet blir bokført til.
5. I **Kontonummer** -feltet angir du kontotypen som betalingsbeløpet blir bokført til.
6. I **Beskrivelse**-feltet angir du en tekst som beskriver denne direktebetalingsbokføringen. Som standard blir teksten i **Transaksjonstekst**-feltet på linjen for betalingsavstemmingskladd, satt inn.
7. Velg **OK**-knappen.

Hvis verdien i **Differanse**-feltet er lik verdien i **Transaksjonsbeløp**-feltet når du bokfører betalingsavstemmingskladden, bokføres hele betalingen på kladdelinjen direkte til den angitte motkontoen.

Hvis verdien i **Differanse**-feltet var lavere enn verdien i **Transaksjonsbeløpet**-feltet, opprettes det en ekstra kladdelinje med samme tekst og dato og med differansen som er satt inn i **Transaksjonsbeløp**-feltet. I den opprinnelige kladdelinjen blir differansen trukket fra verdien i **Transaksjonsbeløp**-feltet, og betalingen blir brukt til den relaterte kunde-, leverandør- eller bankkontoposten. Når du bokfører betalingsavstemmingskladden, bokføres en del av betalingen som utlignet betaling. Den andre delen av betalingen posteres direkte til den angitte kontoen.

## <a name="see-also"></a>Se også
[Håndtere fordringer](receivables-manage-receivables.md)  
[Håndtere salg](sales-manage-sales.md)

