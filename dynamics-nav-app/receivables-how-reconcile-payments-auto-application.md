---
title: Avstemme betalinger ved hjelp av automatisk utligning
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
ms.openlocfilehash: bde263424bb8e5b60d2c9a139ddc8bfef0a90062
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-reconcile-payments-using-automatic-application"></a>Avstemme betalinger ved hjelp av automatisk utligning
Vinduet **Betalingsavstemmingskladd** angir inngående eller utgående betalinger som er registrert som transaksjoner på nettbankkontoen, og som du kan utligne mot de relaterte åpne kunde-, leverandør og bankkontopostene. Linjene i kladden fylles ut ved å importere et bankkontoutdrag som bankfeed eller fil.

En betalingsavstemmingskladd er knyttet til én bankkonto i Dynamics NAV som gjenspeiler nettbankkontoen der betalingstransaksjonene registreres. Alle åpne bankposter relatert til den utlignede kunden- eller leverandørposter lukkes når du velger handlingen **Bokfør betalinger og avstem bankkonto**. Dette betyr at bankkontoen automatisk avstemmes for betalinger du bokfører med kladden.

Hvis du vil importere bankkontoutdrag som bankfeeder, må du først aktivere bankfeedtjenesten Envestnet Yodlee og deretter knytte bankkontoen til den relaterte nettbankkontoen. Betalingsavstemmingskladden oppdager deretter automatisk bankfeeder når du velger handlingen **Importer banktransaksjoner**. I tillegg kan du konfigurere en bankkonto til automatisk å importere nye bankkontoutdragsfeeder hver time. Transaksjoner for betalinger som allerede er bokført som utlignet og/eller avstemt vil ikke bli importert. Hvis du vil ha mer informasjon, kan du se [Konfigurere bankfeedservicen Envestnet Yodlee](bank-how-setup-bank-statement-service.md)

**Merk**: The Envestnet Yodlee Bank Feeds-tjenesten eller en annen leverandørs bankfeedtjeneste, er kanskje ikke tilgjengelig i systemet. Hvis du vil bruke en bankfeedtjeneste til å importere bankkontoutdrag, kontakter du Microsoft-partneren din.

Med handlingen **Tilordne tekst til konto** kan du definere tilordninger mellom tekst på betalinger og bestemte debet-, kredit- og motkonti, slik at slike betalinger bokføres på de angitte kontiene når du bokfører kladden for betalingsavstemming. Se trinn 9. Hvis du vil ha mer informasjon, kan du se [Tilordne tekst på gjentakende betalinger til kontoer for automatisk avstemming](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md)

Det finnes liknende funksjon hvis du vil avstemme overskytende beløp på linjene for betalingsavstemmingskladd på ad hoc-basis. Hvis du vil ha mer informasjon, kan du se [Avstemme betalinger som ikke kan utlignes.](receivables-how-reconcile-payments-cannot-apply-auto.md)

Du bruker **Utlign automatisk**-funksjonen enten automatisk når du importerer en bankfil eller feed med betalingstransaksjoner eller aktiverer den, for å utligne betalinger mot tilknyttede åpne poster basert på avstemming av data på en kladdelinje mot data i én eller flere åpne poster.

På kladdelinjer der en betaling er utlignet automatisk mot én eller flere åpne poster, har **Konfidensintervall**-feltet en verdi mellom Lav og Høy for å angi kvaliteten på datasamsvaret som den foreslåtte betalingsutligningen er basert på. I tillegg blir **Kontotype**- og **Kontonr.** -feltet fylt ut med informasjon om kunden eller leverandøren som den bokførte betalingen utlignes for. Hvis du har definert en tekst-til-kontotilordning, kan den automatiske utligningen føre til verdien **Høy – tekst-til-kontotilordning** for samsvarskonfidens.

For hver kladdelinje som representerer en betaling i vinduet **Betalingsavstemmingskladd**, kan du åpne vinduet **Betalingsutligning** hvis du vil vise alle åpne kandidatposter for betalingen og detaljert informasjon for hver post om datasamsvaret som en betalingsutligning er basert på. Her kan du manuelt utligne betalinger som ble utlignet automatisk mot feil oppføring, eller utligne betalinger på nytt. Hvis du vil ha mer informasjon, kan du se [Se gjennom eller utligne betalinger etter automatisk utligning](receivables-how-review-apply-payments-auto-application.md).

**Merk**: Du kan starte import av banktransaksjoner samtidig som du åpner vinduet **Betalingsavstemmingskladd** for en eksisterende kladd for betalingsavstemming i vinduet **Kladder for betalingsavstemming**. Følgende prosedyre beskriver hvordan du importerer banktransaksjoner til vinduet **Betalingsavstemmingskladd** etter at du har opprettet en ny kladd.

## <a name="to-reconcile-payments-using-automatic-application"></a>Avstemme betalinger ved hjelp av automatisk utligning
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Betalingsavstemmingskladder** og velger deretter den relaterte koblingen.
2. Hvis du vil arbeide i en ny kladd for betalingsavstemming, velger du handlingen **Ny kladd**.
3. I vinduet **Betalingsbankkonto - oversikt** velger du bankkontoen du vil utligne betalinger for, og deretter velger du **OK**-knappen.
Vinduet **Betalingsavstemmingskladd** åpnes forberedt for den valgte bankkontoen.
4. Velg handlingen **Importer banktransaksjoner**.
Hvis bankkontoen for den valgte kladden ikke er konfigurert for import av banktransaksjoner, åpnes en dialogboks som er til hjelp når du skal fylle ut de aktuelle feltene.
5. Velg filen som inneholder banktransaksjoner for betalingene du vil avstemme, i vinduet **Velg en fil som skal importeres**, og velg deretter **Åpne**-knappen.  
6. Hvis tjenesten for bankkontoutdrag er aktivert, angir du datointervallet for bankkontoutdrag som skal importeres i vinduet **Filtrering av bankkontoutdrag**, som åpnes automatisk.

    Vinduet **Betalingsavstemmingskladd** fylles ut med linjer for betalinger som representerer banktransaksjoner i det importerte bankkontoutdraget.

    På linjer for betalinger som er utlignet automatisk mot de tilknyttede åpne postene, har **Konfidensintervall**-feltet en verdi mellom **Lav** og **Høy** for å angi kvaliteten på datasamsvaret som den foreslåtte betalingsutligningen er basert på. I tillegg blir **Kontotype**- og **Kontonr.** -feltet fylt ut med informasjon om kunden eller leverandøren som den bokførte betalingen utlignes for.
7. Velg en kladdelinje, og velg deretter handlingen **Utlign manuelt** for å se gjennom betalingen manuelt i vinduet **Betalingsutligning**. Hvis du vil ha mer informasjon, kan du se [Se gjennom eller utligne betalinger etter automatisk utligning](receivables-how-review-apply-payments-auto-application.md).

    Når du er ferdig med den manuelle utligningen, inneholder **Konfidensintervall**-feltet på kladdelinjen du har behandlet manuelt, **Godtatt**.
8. Velg en kladdelinje med opphevet utligning for en gjentakende innbetaling eller utgift, for eksempel kjøp av drivstoff til en bil, og velg deretter Tilordne tekst til konto under Se gjennom i kategorien Hjem. Hvis du vil ha mer informasjon, kan du se [Tilordne tekst på gjentakende betalinger til kontoer for automatisk avstemming](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md)
9. Når du er ferdig med å tilordne betalingstekst til kontoer, velger du handlingen **Utlign manuelt**.
10. Når du er sikker på at alle betalinger i kladdelinjene er riktig utlignet eller satt til direkte bokføring, velger du handlingen **Bokfør**.

Når du bokfører kladden for betalingsavstemming, lukkes de utlignede åpne postene, og de relaterte kunde-, leverandør- eller finanskontiene oppdateres. De angitte kunde-, leverandør- og finanskontiene oppdateres for betalinger på kladdelinjer basert på tekst-til-kontotilordning. Det opprettes bankkontoposter for alle kladdelinjene. Hvis du velger handlingen **Bokfør betalinger og avstem bankkonto**, vil alle åpne bankposter relatert til den utlignede kunden- eller leverandørposter lukkes. Dette betyr at bankkontoen automatisk avstemmes for betalinger du bokfører med kladden.

Du kan sammenligne verdien i feltet **Saldo på bankkonto etter bokføring** med verdien i feltet **Utdrag - sluttsaldo** for å spore når bankkontoen avstemmes basert på betalinger som du bokfører.

**Merk**: Hvis du vil avstemme en bankkonto fra vinduet **Betalingsavstemmingskladd** , må du bruke vinduet **Bankkontoavstemming**. Hvis du vil ha mer informasjon, kan du se [Avstemme bankkonti separat](bank-how-reconcile-bank-accounts-separately.md).

## <a name="see-also"></a>Se også
[Håndtere fordringer](receivables-manage-receivables.md)  
[Håndtere salg](sales-manage-sales.md)

