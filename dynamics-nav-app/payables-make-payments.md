---
title: "Oversikt over oppgaver for å behandle betalinger til leverandører"
description: "Gir en oversikt over oppgavene for å behandle betalinger til leverandører eller kreditorer, inkludert bokføring av betalingslinjene og oversikt over forfalt saldo."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, vendor payment, creditor, debt, balance due, AP
ms.date: 06/28/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 6ec19f50c70b5355c0d586b03f4d5a41733f8e3e
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="making-payments"></a>Utføre betalinger
Når du foretar betalinger til leverandører eller refusjoner til de ansatte, kan du bokføre de relaterte betalingslinjene i vinduet **Betalingskladd**. Du kan bruke funksjonen **Betalingsforslag – leverandør** til å finne leverandørbetalinger som har forfalt. Du kan også bruker rapporten **Leverandør – forfallsoversikt** til å få oversikt over leverandørbetalinger som har forfalt.

Fra betalingskladden kan du skrive ut maskinelle sjekker eller registrere når sjekker skrives. Hvis du velger **Maskinell sjekk** i feltet **Bankbetalingstype**, må eventuelle linjer som representerer sjekker skrives ut før betalingskladden kan bokføres.

Når betalingene er bokført, kan du eksportere dem til en bankfil for opplasting til banken for behandling.

Når betalingene er foretatt i banken, må du utligne dem på deres tilknyttede åpne leverandør- eller ansattposter. Du kan gjøre dette manuelt eller ved å importere en bankkontoutdragsfil og utligne betalingene automatisk. Hvis du vil ha mer informasjon, kan du se [Utligne betalinger automatisk og avstemme bankkonti](receivables-apply-payments-auto-reconcile-bank-accounts.md).

Tabellen nedenfor beskriver en sekvens av oppgaver, og har koblinger til emnene som beskriver dem.

| Til | Se |
| --- | --- |
|Bruk vinduet **Utbetalingskladd**, som er basert på finanskladden, til å bokføre betalinger til leverandører eller ansatte.|[Arbeide med finanskladder](ui-work-general-journals.md)|
| Bruke en funksjon til å foreslå leverandørbetalinger i henhold til valgte kriterier som forfallsdato, rabatt arbeidstillatelse og din likviditet. |[Foreslå leverandørbetalinger](payables-how-suggest-vendor-payments.md) |
|Refunder de ansatte for personlige utgifter under firmaaktiviteter ved å betale dem på deres bankkontoer.|[Registrere og refundere ansattes utgifter](finance-how-record-reimburse-employee-expenses.md)|
| Utstede sjekker for leverandørbetalinger, enten som utskrifter eller maskinelle sjekker. Kansellere sjekker før eller etter bokføring. |[Arbeide med sjekker](payables-how-work-checks.md) |
| Betal leverandøren kontant eller med sjekk, og bokfør betalingen når du bokfører selve fakturaen. |[Gjøre opp kjøpsfakturaer omgående](finance-how-to-settle-purchase-invoices-promptly.md) |
| Du kan sørge for at at banken bare fjerner validerte sjekker og beløp ved å sende dem en fil som inneholder informasjon om leverandør, sjekk og betaling. |[Eksportere en Positive Pay-fil](finance-how-positive-pay.md) |
|Eksporter betalinger fra vinduet **Utbetalingskladd** til en bankfil som du laster opp til banken for behandling, inkludert EFT (elektronisk pengeoverføring) i Nord-Amerika. |[Fremgangsmåte: Eksportere betalinger til en bankfil](payables-how-export-payments-bank-file.md)|  

## <a name="see-also"></a>Se også
[Administrere skyldige beløp](payables-manage-payables.md)  
[Innkjøp](purchasing-manage-purchasing.md)  
[Håndtere fordringer](receivables-manage-receivables.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

