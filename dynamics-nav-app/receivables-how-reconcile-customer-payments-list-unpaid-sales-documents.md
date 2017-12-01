---
title: Utligne betalinger mot ubetalte salgsdokumenter
description: "Du utligner beløp betalt av kunder mot relaterte salgsdokumenter og bokfører betalingen for å oppdatere kunde-, finans- og bankposter."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment process, cash receipts, customer payment
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c39a45d513ef6d5f6d4da7a052888a051d9f06d6
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-reconcile-customer-payments-manually-from-a-list-of-unpaid-sales-documents"></a>Avstemme kundebetalinger manuelt fra en liste over ubetalte salgsdokumenter
Når kundene har utført betalinger til nettbankkontoen din, må du utligne hvert beløp betalt til det tilknyttede salgsdokumentet, og deretter bokføre betalingen for å oppdatere postene for kunde, finans og bank.

> [!NOTE]  
>   Du kan utføre de samme oppgavene, inkludert leverandørbetalinger, i vinduet **Betalingsavstemmingskladd** ved hjelp av funksjoner for import av bankkontoutdrag, automatisk utligning og bankkontoavstemming. Hvis du vil ha mer informasjon, kan du se [Avstemme betalinger ved hjelp av automatisk utligning](receivables-how-reconcile-payments-auto-application.md).

Vinduet **Betalingsregistrering** er utformet for å støtte deg i oppgaver som omfatter å balansere interne konti ved hjelp av de faktiske kontanttallene for å sikre effektiv innkreving av betalinger fra kunder. Med dette betalingsbehandlingsverktøyet kan du raskt kontrollere og bokføre enkelt- eller engangsbetalinger, behandle rabatterte betalinger og søke etter bestemte ubetalte dokumenter som blir betalt.

Betalinger for ulike kunder som har ulike betalingsdatoer, må bokføres som individuelle betalinger. Betalinger for den samme kunden, som har samme betalingsdato, kan bokføres som en engangsbetaling. Dette er nyttig, for eksempel når en kunde har foretatt en enkeltbetaling som dekker flere salgsfakturaer.

## <a name="to-set-up-the-payment-registration-journal"></a>Slik definerer du betalingsregistreringsjournalen:
Fordi du kan bokføre forskjellige betalingstyper til forskjellige motkonti, må du velge en motkonto i vinduet **Betalingsregistreringsoppsett** før du starter behandlingen av kundebetalinger. Hvis du alltid bokfører til den samme motkontoen, kan du angi denne kontoen som standard og unngå dette trinnet hver gang du åpner vinduet **Betalingsregistrering**.  

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Betalingsregistreringsoppsett**, og velg deretter den relaterte koblingen.

    Du kan også gå til vinduet **Betalingsregistrering** og velge handlingen **Oppsett**.    
2. Fyll ut feltene i vinduet **Betalingsregistreringsoppsett**. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til relatert informasjon.  

## <a name="to-reconcile-payments-individually"></a>Avstemme betalinger enkeltvis
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Betalingsregistrering**, og velg deretter den relaterte koblingen.  
2. Merk av for **Betaling utført** på linjen som representerer det bokførte dokumentet som en betaling er utført for.

    Hvis det er merket av for **Fyll ut mottaksdato automatisk** i vinduet **Betalingsregistreringsoppsett**, angis arbeidsdatoen i feltet **Mottatt den**.  
3. I feltet **Mottatt den** angir du datoen da betalingen ble mottatt. Denne datoen kan være forskjellig fra arbeidsdatoen.  
4. I feltet **Beløp mottatt** angir du beløpet som er betalt.

    For fullstendige betalinger er dette det samme som beløpet i **Restbeløp** på linjen. For delbetalinger er dette lavere enn beløpet i **Restbeløp** på linjen.    
5. Gjenta trinn 2 til 4 for andre linjer som representerer bokførte dokumenter som betalinger er utført for.  
6. Velg handlingen **Bokfør betalinger**.  

Betalingsinformasjonen bokføres for dokumenter som vises som linjer der det er merket av for **Betaling utført** .  

Betalingsposter bokføres til finans-, bank- og kundekonti. Hver betaling brukes på det relaterte bokførte salgsdokumentet.  

## <a name="to-reconcile-lump-payments"></a>Avstemme engangsbetalinger
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Betalingsregistrering**, og velg deretter den relaterte koblingen.
2. Merk av for **Betaling utført** på linjene som representerer bokførte dokumenter for den samme kunden som en engangsbetaling er utført for.  

    > [!NOTE]  
>   Kunden **Navn**-feltet må være det samme på alle linjer som bokføres som en engangsbetaling.  

    Hvis det er merket av for **Fyll ut mottaksdato automatisk** i vinduet **Betalingsregistreringsoppsett**, fylles arbeidsdatoen ut i feltet **Mottatt den**.  
3. I feltet **Mottatt den** angir du datoen da betalingen ble mottatt. Denne datoen kan være forskjellig fra arbeidsdatoen.  

    > [!NOTE]  
>   Denne datoen må være den samme på alle linjene som skal bokføres som en engangsbetaling.  
4. I feltet **Beløp mottatt** angir du beløpene på flere linjer som summerer opp engangsbetalingsbeløpet.  

    > [!TIP]  
>   Prøv å bokføre så mange fullstendige betalinger som mulig med engangsbeløpet. Angi beløp som er det samme som beløpet i feltet **Restbeløp**, på så mange linjer som mulig.  
5. Gjenta trinn 2 til 4 for andre linjer som representerer bokførte dokumenter for samme kunde som det er utført en engangsbetaling for.  
6. Velg handlingen **Bokfør som engangsbetaling**. Den angitte betalingsinformasjonen bokføres for dokumenter som vises som linjer der det er merket av for **Betaling utført** .  

Betalingsposter bokføres til finans-, bank- og kundekonti. Hver betaling brukes på det relaterte bokførte salgsdokumentet.  

Hvis en betaling i banken ikke er representert av en linje i vinduet **Betalingsregistrering**, kan det være fordi det tilknyttede dokumentet ennå ikke er bokført. I det tilfellet kan du bruke en søkefunksjon til raskt å finne dokumentet og bokføre det for å behandle betalingen. Hvis du vil ha mer informasjon, kan du se delen "Slik finner du et bestemt salgsdokument som ikke er fullstendig fakturert".  

Hvis en betaling i banken ikke er representert av noen dokumenter i [!INCLUDE[d365fin](includes/d365fin_md.md)], kan du åpne en forhåndsutfylt finanskladd fra vinduet **Betalingsregistrering** for å bokføre betalingen direkte til motkontoen uten å bruke betalingen på et dokument. Alternativt kan du registrere betalingen i kladden til opprinnelsen til betalingen er fastsatt. Hvis du vil ha mer informasjon, kan du se avsnittet "Registrere eller bokføre betalinger manuelt uten et relatert dokument".  

## <a name="to-process-customer-payments-with-discounts-manually"></a>Behandle kundebetalinger med rabatter manuelt
Hvis du har avtalt en kontantrabatt med kunden, kan betalingsbeløpene være lavere enn fakturabeløpene hvis betalingen finner sted før den avtalte rabattdatoen.  

De følgende fremgangsmåtene beskriver fire forskjellige måter for bokføring av rabatterte betalinger i vinduet **Betalingsregistreringer**.  

* Betalingsbeløpet er det samme som det gjenstående rabattbeløpet, og betalingsdatoen er før rabattdatoen. Du bokfører betalingen som den er.  
* Betalingsbeløpet er det samme som det gjenstående rabattbeløpet, men betalingsdatoen er etter rabattdatoen. Du bokfører betalingen som delvis. Dokumentet forblir åpen for å hente/betale det gjenstående beløpet. Alternativt angir du rabattdatoen senere for å tillate fullstendig betaling.  
* Betalingsbeløpet er lavere enn det gjenstående rabattbeløpet. Du bokfører betalingen som delvis. Dokumentet forblir åpen for å hente/betale det gjenstående beløpet.  
* Betalingsbeløpet er større enn det gjenstående rabattbeløpet. Du bokfører betalingene som de er. Bare det gjenstående beløpet bokføres. Tilleggsbeløpet krediteres til kunden.  

### <a name="to-process-a-payment-amount-that-is-equal-to-the-discounted-amount-and-where-the-payment-date-is-before-the-discount-date"></a>Slik behandler du et betalingsbeløp som er det samme som rabattbeløpet, og der betalingsdatoen er før rabattdatoen:
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Betalingsregistrering**, og velg deretter den relaterte koblingen.  
2. Angi betalingsbeløpet i feltet **Beløp mottatt**. Beløpet er det samme som beløpet i feltet **Restbeløp etter rabatt**.

    Det merkes automatisk av for **Betaling utført**, og **Mottatt den** fylles ut med arbeidsdatoen.    
3. Angi betalingsdato i feltet **Mottatt den**. Datoen er før datoen i feltet **Kont.rabattdato**.
4. Kontroller at **Restbeløp**-feltet inneholder null (0).  
5. Velg handlingen **Bokfør betalinger** for å bokføre full betaling til finans-, bank- og kundekonti.

### <a name="to-process-a-payment-amount-that-is-equal-to-the-discounted-amount-but-where-the-payment-date-is-after-the-discount-date"></a>Slik behandler du et betalingsbeløp som er det samme som rabattbeløpet, men der betalingsdatoen er etter rabattdatoen:
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Betalingsregistrering**, og velg deretter den relaterte koblingen.  
2. Angi betalingsbeløpet i feltet **Beløp mottatt**. Beløpet er det samme som beløpet i feltet **Restbeløp etter rabatt**.

    Det merkes automatisk av for **Betaling utført**, og **Mottatt den** fylles ut med arbeidsdatoen.
3. I feltet **Mottatt den** angir du en betalingsdato er etter datoen i feltet **Kont.rabattdato**. Datofelt endres til rød skrift, og en feilmelding vises nederst i vinduet.

    > [!TIP]  
>   Hvis du vil gjøre et unntak og gi rabatten selv om betalingen er sen, følger du disse trinnene:
4. Velg handlingen **Detaljer**.  
5. I vinduet **Betalingsregistreringsdetaljer**, i feltet **Kont.rabattdato** i hurtigfanen **Kontantrabatt**, skriver du inn en dato som er etter datoen i feltet **Mottatt den** i vinduet **Betalingsregistrering**.  

    Feilmeldingen og rød skrift forsvinner, og du kan fortsette å behandle den rabatterte betalingen.    
6. Kontroller at **Restbeløp**-feltet viser beløpet som gjenstår å betale for det fullstendige fakturabeløpet.  
7. Velg handlingen **Bokfør betalinger** for å bokføre den delvise betalingen til finans-, bank- og kundekonti.  

Det tilknyttede dokumentet forblir åpent.

### <a name="to-process-a-payment-that-is-lower-than-the-remaining-discounted-amount"></a>Slik behandler du en betaling som er lavere enn det gjenstående rabattbeløpet:
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Betalingsregistrering**, og velg deretter den relaterte koblingen.  
2. Angi betalingsbeløpet i feltet **Beløp mottatt**. Beløpet er lavere enn beløpet i feltet **Restbeløp etter rabatt**.

    Det merkes automatisk av for **Betaling utført**, og **Mottatt den** fylles ut med arbeidsdatoen.  
3. Angi betalingsdato i feltet **Mottatt den**. Datoen er før datoen i feltet **Kont.rabattdato**.
4. Kontroller at **Restbeløp**-feltet viser beløpet som gjenstår å betale for det fullstendige rabattbeløpet.  
5. Velg handlingen **Bokfør betalinger** for å bokføre den delvise betalingen til finans-, bank- og kundekonti.  

Det tilknyttede dokumentet forblir åpent.

### <a name="to-process-a-payment-that-is-more-than-the-remaining-discounted-amount"></a>Slik behandler du en betaling som er større enn det gjenstående rabattbeløpet:
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Betalingsregistrering**, og velg deretter den relaterte koblingen.  
2. Angi betalingsbeløpet i feltet **Beløp mottatt**. Beløpet er større enn beløpet i feltet **Restbeløp etter rabatt**.  

    Det merkes automatisk av for **Betaling utført**, og **Mottatt den** fylles ut med arbeidsdatoen.    
3. Angi betalingsdato i feltet **Mottatt den**. Datoen er før datoen i feltet **Kont.rabattdato**.
4. Kontroller at **Restbeløp**-feltet inneholder null (0).  
5. Velg handlingen **Bokfør betalinger** for å bokføre full betaling til finans-, bank- og kundekonti.  

Det tilknyttede dokumentet lukkes, og kunden blir kreditert med det overflødige betalingsbeløpet.  

## <a name="to-find-a-specific-sales-document-that-is-not-fully-invoiced"></a>Slik finner du et bestemt salgsdokument som ikke er fullstendig fakturert:
**Betalingsregistrering**-vinduet støtter deg i oppgaver som er nødvendige for å balansere interne konti med faktiske kontanttall, for å sikre effektiv innkreving fra kunder og betaling ved forfall til leverandører. Den viser utestående innkommende betalinger som linjer som representerer salgsdokumentene der et beløp er forfalt til betaling.  

Vanligvis når en betaling er gjort i banken eller på annen måte, er relaterte salgs- eller kjøpsdokumenter representert som en linje i vinduet **Betalingsregistrering** fordi det aktuelle dokumentet venter på at betalingen skal bokføres mot det utestående beløpet. Noen ganger er imidlertid ikke en utført betaling representert av en linje i vinduet **Betalingsregistrering**, vanligvis fordi det aktuelle dokumentet ikke er fullstendig fakturabokført.

I vinduet **Dokumentsøk** kan du søke blant dokumenter som ikke er fullstendig fakturert. Du kan søke basert på ett eller flere av følgende kriterier:  

* Dokumentnummer  
* Beløp eller beløpområde  

Fremgangsmåten nedenfor forklarer hvordan du søker etter et bestemt dokument ved å bruke begge søkevilkårene.  

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Betalingsregistrering**, og velg deretter den relaterte koblingen.
2. Med pekeren på en av linjene, velger du handlingen **Søk i dokumenter**.
3. I vinduet **Dokumentsøk** skriver du inn en søkeverdi i feltet **Bilagsnr.**.  

    > [!NOTE]  
>   Verdien du angir i dette feltet, er omsluttet med skjulte jokertegn. Dette betyr at funksjonen søker etter alle bilagsnumre som inneholder den angitte verdien.    
4. I feltet **Beløp** angir du det bestemte beløpet som finnes i dokumentet du vil finne.  
5. I feltet **Beløpstoleranse-%** angir du en prosentverdi for å definere området for beløp som du vil søke etter for å finne det åpne dokumentet.  

    Hvis du skriver inn 10, søkes det etter beløp i et område mellom ti prosent lavere og ti prosent høyere enn verdien i feltet **Beløp**.    
6. Velg handlingen **Søk**.  

Søkefunksjonen søker blant dokumenter som ikke er fullstendig fakturert, basert på de angitte kriteriene.  

Hvis ett eller flere dokumenter samsvarer med søkekriteriene, åpnes vinduet **Dokumentsøkeresultat** for å vise linjer som representerer disse dokumentene. Hver linje inneholder et bilagsnummer, beskrivelse og beløp, slik at du enkelt kan finne et bestemt dokument, for eksempel basert på informasjon på bankkontoutdraget.  

Hvis en betaling i banken ikke er representert av noen dokumenter i [!INCLUDE[d365fin](includes/d365fin_md.md)], kan du åpne en forhåndsutfylt finanskladd fra vinduet **Betalingsregistrering** for å bokføre betalingen direkte til motkontoen uten å bruke betalingen på et dokument. Alternativt kan du registrere betalingen i kladden til opprinnelsen til betalingen er fastsatt.  

## <a name="to-record-or-post-a-payment-without-a-related-document"></a>Slik registrerer eller bokfører du en betaling uten et relatert dokument:
Hvis en betaling i banken ikke er representert av noen dokumenter i [!INCLUDE[d365fin](includes/d365fin_md.md)], kan du åpne en forhåndsutfylt finanskladdlinje fra vinduet **Betalingsregistrering** for å bokføre betalingen direkte til motkontoen uten å bruke betalingen på et dokument. Alternativt kan du registrere betalingen i kladden til opprinnelsen til betalingen er klarlagt.  

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Betalingsregistrering**, og velg deretter den relaterte koblingen.  

Fortsett med å registrere en udokumentert betaling.  

1. Velg handlingen **Finanskladd**.  

    Vinduet **Finanskladd** åpnes med én linje som er forhåndsutfylt med motkontoen for kladden som er definert i vinduet **Betalingsregistreringsoppsett**.  
2. Fyll ut resten av feltene på finanskladdelinjen, for eksempel beløpet og kundenummeret eller annen informasjon fra bankkontoutdraget. Hvis du vil ha mer informasjon, kan du se [Bokføre transaksjoner direkte i Finans](finance-how-post-transactions-directly.md).  

Du kan bokføre kladdelinjen for å oppdatere totalsummen på motkontoen. Du kan eventuelt la kladdelinjen være upostert, og kanskje tilføye den med en merknad om at betalingen trenger mer analyse.  

Hvis du ikke bokfører kladdelinjen, øker verdien i feltet **Ikke-bokført saldo** nederst i vinduet **Betalingsregistrering**.  

## <a name="see-also"></a>Se også
[Håndtere fordringer](receivables-manage-receivables.md)  
[Salg](sales-manage-sales.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

