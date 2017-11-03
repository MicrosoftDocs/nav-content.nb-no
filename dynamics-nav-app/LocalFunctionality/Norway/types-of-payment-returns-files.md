---
title: Typer betalingsreturfiler
description: 'Forbedringer i den norske versjonen omfatter to typer importerbare betalingsreturfiler:'
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 0c89f6e63ffa8438f88b3ca02ee36b2182f11bcc
ms.contentlocale: nb-no
ms.lasthandoff: 10/26/2017

---
# <a name="types-of-payment-returns-files"></a>Typer betalingsreturfiler
[!INCLUDE[navnow](../../includes/navnow_md.md)]omfatter to typer importerbare betalingsreturfiler:  

- Mottaksreturer  
- Avregningsreturer  

Du kan også velge å ikke bruke returfiler ved å velge feltet **Returfiler brukes ikke** i **remitteringsavtalen**-tabellen. Se [Sette opp remitteringsavtaler](how-to-set-up-remittance-agreements.md) for mer informasjon.  

## <a name="receipt-returns"></a>Mottaksreturer  
Mottaksreturen mottas fra banken etter at du har sendt remitteringsfilen til banken. Når data leses inn, vises informasjon om hvor mange fakturaer som blir korrekt mottatt og hvor mange som mottas med feilmelding. Når du har importert en mottaksretur, blir statusen for betalingene i vinduet **Ventekladd** satt til **Godkjent**.  

> [!NOTE]  
>  Du kan også motta en avvist retur fra banken. Hvis remitteringen avvises, mottar du ingen avregningsretur.  

## <a name="settlement-returns"></a>Avregningsreturer  
Avregningsreturen mottas fra banken etter at betalingen er utført. Når dataene leses inn, vises informasjon om antall oppgjorte fakturaer.  

Følgende skjer når avregningsreturen leses inn:  

- Betalingsstatusen i tabellen **Ventekladd** settes til **Avregnet**.  
- Det overføres informasjon fra vinduet **Ventekladd** til innbetalingskladden.  
- Det opprettes en motkonto for hver transaksjon.  
- Det settes inn bilagsnumre for hver transaksjon.  

## <a name="exchange-rates-by-settlement"></a>Valutakurser ved oppgjør  
Ved oppgjør håndteres valutakurser på følgende måter:  

- Betaling fra en konto i lokal valuta - Hvis en betaling i en annen valuta utføres fra en konto i NOK, flagger banken avregningsreturen med en advarsel om hvilken vekslingskurs som benyttes mellom NOK og valutaen som benyttes for betalingen.  

- Betaling fra en valutakonto - Hvis betalingen utføres fra en valutakonto, benyttes vekslingskursen for denne valutaen og NOK. Dette fordi banken ikke informerer systemet om valutakursen.  

## <a name="warnings-on-settlement-returns"></a>Advarsler i avregningsreturer  
Det kan forekomme advarsler når avregningsreturen leses inn. Innbetalingskladdelinjer med advarsler er merket med et symbol. Hvis du vil vite mer om advarselen, kan du åpne vinduet **Avregningsopplysninger**.  

## <a name="see-also"></a>Se også  
 [Elektroniske betalinger til leverandører i Norge](electronic-payments-to-vendors-in-norway.md)   
 [Sette opp remitteringsavtaler](how-to-set-up-remittance-agreements.md)   
 [Opprette remitteringskontoer](how-to-create-remittance-accounts.md)   
 [Angi leverandører for remittering](how-to-set-up-vendors-for-remittance.md)   
 [Mottakerreferansekoder](recipient-reference-codes.md)   
 [Opprette remitteringsforslag](how-to-create-remittance-suggestions.md)   
 [Opprette manuelle remitteringsoppdrag](how-to-create-manual-remittance-payments.md)   
 [Definere betalingslinjeinformasjon](how-to-set-up-payment-line-information.md)   
 [Kontrollere remitteringsoppdrag](how-to-test-remittance-payments.md)   
 [Eksportere remitteringsoppdrag](how-to-export-remittance-payments.md)   
 [Importere betalingsreturdata](how-to-import-payment-return-data.md)   
 [Slette remitteringsoppdrag](how-to-delete-remittance-payment-orders.md)   
 [Remitteringsfeil](remittance-errors.md)   
 [Vise remitteringsfeilkoder](how-to-view-remittance-error-codes.md)   
 [Annullere betalinger](how-to-cancel-payments.md)

