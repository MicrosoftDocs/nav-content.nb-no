---
title: Bruke betalinger automatisk og avstemme bankkonti
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
ms.openlocfilehash: 11df387c16e19421090531fd03c209103b9989d9
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="apply-payments-automatically-and-reconcile-bank-accounts"></a>Bruke betalinger automatisk og avstemme bankkonti
Du må regelmessig avstemme bankkontoene og samlekontoene for kunder og leverandører i Dynamics NAV ved å utligne betalinger som er registrert på bankkontoen, mot de tilknyttede ubetalte fakturaene og kreditnotaene eller andre åpne poster i Dynamics NAV.

Du kan utføre denne oppgaven i vinduet **Betalingsavstemmingskladd** ved å importere en bankkontoutdragsfil eller feed for hurtig å registrere betalinger i Dynamics NAV. En funksjon for automatisk utligning utligner betalingene til deres tilknyttede åpne kunde- eller leverandørposter, basert på datasamsvar mellom betalingstekst og postinformasjonen. Du kan se gjennom og endre automatiske utligninger før du bokfører kladden. Du kan velge å lukke alle åpne bankposter relatert til de utlignede postene når du bokfører kladden. Dette betyr at bankkontoen avstemmes automatisk når alle betalinger er utlignet.

Hvis du vil aktivere import av bankkontoutdrag som en bankfeed, må du først konfigurere og aktivere bankfeedtjenesten Envestnet Yodlee og deretter knytte bankkontoene til relaterte nettbankkonti. Hvis du vil ha mer informasjon, kan du se [Konfigurere bankfeedservicen Envestnet Yodlee](bank-how-setup-bank-statement-service.md)

**Merk**: The Envestnet Yodlee Bank Feeds-tjenesten eller en annen leverandørs bankfeedtjeneste, er kanskje ikke tilgjengelig i systemet. Hvis du vil bruke en bankfeedtjeneste til å importere bankkontoutdrag, kontakter du Microsoft-partneren din.

Du kan også bruke konverteringstjenesten for bankdata til å konvertere en bankkontoutdragsfil i hvilket som helst format, til en datastrøm du kan importere til Dynamics NAV. Hvis du vil ha mer informasjon, kan du se [Konfigurere konverteringstjenesten for bankdata](bank-how-setup-bank-data-conversion-service.md)

Tabellen nedenfor beskriver en sekvens av oppgaver, og har koblinger til emnene som beskriver dem.

|Hvis du vil |Se |
|---|----|
|Utligne betalinger mot åpne kunde- eller leverandørposter ved å importere et bankkontoutd, og avstemme bankkontoen når alle betalingene er utlignet. | [Avstemme betalinger ved hjelp av automatisk utligning](receivables-how-reconcile-payments-auto-application.md) |
|Utlign betalinger manuelt ved å vise detaljert informasjon om samsvarende data og forslag til åpne kandidatposter som betalinger kan utlignes mot. | [Se gjennom eller utligne betalinger etter automatisk utligning](receivables-how-review-apply-payments-auto-application.md)
|Løse betalinger som ikke kan utlignes automatisk på de tilknyttede åpne postene, for eksempel fordi beløpene er forskjellige, eller fordi en relatert post ikke finnes. | [Avstemme betalinger som ikke kan utlignes automatisk](receivables-how-reconcile-payments-cannot-apply-auto.md)
|Koble tekst på betalinger til bestemte kunde-, leverandør- eller finanskontoer for alltid å bokføre gjentakende innbetalinger eller utgifter på disse kontoene når det ikke finnes noen dokumenter å utligne dem på.| [Tilordne tekst på gjentakende betalinger til kontoer for automatisk avstemming](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md)|

## <a name="see-also"></a>Se også
[Håndtere fordringer](receivables-manage-receivables.md)  
[Håndtere salg](sales-manage-sales.md)

