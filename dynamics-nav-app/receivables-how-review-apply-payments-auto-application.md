---
title: "Kontrollere automatisk utlignede betalinger og utligne betalinger på nytt manuelt"
description: "Etter at betalingene er utlignet automatisk, kan du se gjennom alle postene for en betaling og manuelt utligne de som ble uriktig utlignet, på nytt."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment process, reconcile payment, expenses, cash receipts
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 336dd02d1f29e5f80209961eae164a6faeaf65bc
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-review-or-apply-payments-manually-after-automatic-application"></a>Se gjennom eller utligne betalinger manuelt etter automatisk utligning
For hver kladdelinje som representerer en betaling i vinduet **Betalingsavstemmingskladd**, kan du åpne vinduet **Betalingsutligning** hvis du vil vise alle åpne kandidatposter for betalingen og detaljert informasjon for hver post om datasamsvaret som en betalingsutligning er basert på. Her kan du manuelt utligne betalinger som ble utlignet automatisk mot feil oppføring, eller utligne betalinger på nytt. Hvis du vil ha mer informasjon om automatisk utligning, kan du se [Avstemme betalinger ved hjelp av automatisk utligning](receivables-how-reconcile-payments-auto-application.md).

> [!IMPORTANT]  
>   Når bankkontoen du avstemmer betalinger for, er konfigurert for den lokale valutaen, vises alle åpne poster i lokal valuta i vinduet **Betalingsutligning**, inkludert åpne poster for dokumenter som opprinnelig ble fakturert i utenlandsk valuta. Betalinger som utlignes mot poster med omregnede valutaer, kan derfor bli bokført med andre beløp enn i det opprinnelige dokumentet på grunn av potensielt ulike valutakurser som henholdsvis brukes av banken og [!INCLUDE[d365fin](includes/d365fin_md.md)].

Derfor anbefaler vi at du ser etter utenlandske valutakoder i feltet **Valutakode** i vinduet **Betalingsutligning**, for å se om utligningene er basert på omregnede valutaer. Hvis du vil se gjennom det opprinnelige dokumentbeløpet i den utenlandske valutaen og se valutakursen som brukes, velger du feltet **Utligningspostnr.**, og deretter velger du rullegardinknappen for å åpne vinduet **Kundeposter** eller **Leverandørposter**.

Eventuell justering av tap og vinning på grunn av valutaomregning behandles ikke automatisk av [!INCLUDE[d365fin](includes/d365fin_md.md)].

> [!NOTE]  
>   Du kan ikke utligne poster med et annet fortegn enn fortegnet på betalingen. Hvis du for eksempel vil lukke en kreditnota med negativt fortegn og den tilknyttede fakturaen med positivt fortegn, må du først utligne kreditnotaen mot fakturaen og deretter utligne betalingen mot fakturaen med det reduserte restbeløpet.

> [!WARNING]  
>   Hvis du bruker kontantrabatter og betalingsdatoen er før forfallsdatoen for betalingen, brukes feltet **Restbeløp inkl. rabatt** i vinduet **Betalingsutligning** til avstemming. Ellers brukes verdien i **Restbeløp**-feltet. Hvis betalingen ble gjort med et rabattbeløp etter forfallsdatoen for betalingen eller hele beløpet ble betalt, men med en rabatt, blir ikke beløpet avstemt.

> [!NOTE]  
>   Du kan bare utligne en betaling mot én konto. Hvis du vil dele utligningen på flere åpne poster, for eksempel for å utligne en engangsbetaling, må de åpne postene være for samme konto. Hvis du vil ha mer informasjon, kan du se trinn 7 og 8 i fremgangsmåten i dette emnet.

## <a name="to-review-or-apply-payments-after-automatic-application"></a>Se gjennom eller utligne betalinger etter automatisk utligning
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Betalingsavstemmingskladder**, og velg deretter den relaterte koblingen.
2. Åpne kladden for betalingsavstemming for en bankkonto du vil avstemme betalinger for. Hvis du vil ha mer informasjon, kan du se [Avstemme betalinger ved hjelp av automatisk utligning](receivables-how-reconcile-payments-auto-application.md).
3. I vinduet **Betalingsavstemmingskladd** velger du en betalingsmåte som du vil se gjennom eller utligner manuelt mot én eller flere åpne poster, og velger deretter handlingen **Utlign manuelt**.
4. Merk av for **Utlignet** på linjen for den åpne posten du vil utligne betalingen mot.
5. Betalingsbeløpet, som også vises i **Transaksjonsbeløp**-feltet i vinduet **Betalingsutligning**, settes inn i **Utlignet beløp**-feltet, men du kan endre feltet, for eksempel hvis du vil utligne beløpet mot flere åpne poster.
6. Hvis du vil utligne en del av det betalte beløpet mot en annen åpen post for kontoen, for eksempel for å utligne en engangsbetaling, merker du av for **Utlignet** for linjen. Det utlignede beløpet trekkes automatisk fra transaksjonsbeløpet for å gjenspeile fordelingen på de to åpne postene.
7. Hvis du vil utligne en del av en betaling mot én eller flere åpne poster som ikke finnes i databasen, kan du opprette en ny linje under linjen for samme konto. I feltet **Utlignet beløp** angir du beløpet som skal utlignes for den nye linjen, og deretter justerer du **Utlignet beløp**-feltet på den eksisterende linjen.
8. Gjenta trinn 5, 6 eller 7 for andre åpne poster du vil utligne et fullt beløp eller et delbeløp mot.
9. Når du har sett over en betalingsutligning eller manuelt utlignet til én eller flere åpne poster, velger du handlingen **Godta utligning**.

Vinduet **Betalingsutligning** lukkes, og i vinduet **Betalingsavstemmingskladd** endres verdien i **Konfidensintervall**-feltet til **Godtatt** for å vise at du har gjennomgått eller manuelt utlignet betalingen.

## <a name="see-also"></a>Se også
[Håndtere fordringer](receivables-manage-receivables.md)  
[Salg](sales-manage-sales.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

