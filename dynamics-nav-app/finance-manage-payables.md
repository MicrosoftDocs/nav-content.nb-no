---
title: "Behandle leverandørgjeld"
description: "Oversikt over hvordan Dynamics NAV hjelper deg å behandle leverandørgjeld, inkludert leverandørbetalinger, kreditorer, gjeld og forfalt saldo."
documentationcenter: 
author: bholtorf
manager: edupont
editor: 
ms.prod: dynamics-nav-2018
ms.workload: na
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: article
ms.search.keywords: vendor payment, creditor, debt, balance due, AP
ms.date: 06/02/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 698cb92c4209f2675fda3a4b2280ab8afad0c9cc
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="managing-payables"></a>Administrere skyldige beløp
[!INCLUDE[d365fin_long](includes/d365fin_long_md.md)] har det du trenger for å effektivt administrere leverandører.  

## <a name="payments"></a>Betalinger
Det er enkelt å prioritere betalinger, vurdere straffer for forfalte betalinger og håndtere rabatter for tidlige betalinger.

Du kan registrere betalinger i en finanskladd og deretter skrive ut sjekker før bokføring av utbetalingskladden.

Du kan utligne betalinger mot lukkede fakturaer når du bokfører betalingen, eller etter at du har bokført betalingen. **Utligningsmetode** angitt for leverandøren (på **leverandørkortet**) bestemmer om du utligner betalingen manuelt eller automatisk. Du kan alltid utligne transaksjoner manuelt. Hvis utligningsmetoden for leverandøren er **Saldo** og du ikke angir et dokument som betalingen skal utlignes mot, vil betalingen imidlertid bli utlignet mot den eldste åpne posten for leverandøren.

## <a name="suggest-vendor-payments"></a>Betalingsforslag - leverandør
[!INCLUDE[d365fin](includes/d365fin_md.md)] kan foreslå ulike utbetalinger til leverandører, for eksempel betalinger som snart forfaller eller betalinger hvor en rabatt er tilgjengelig. Betalingsforslaget kan ta hensyn til et beløp du angir som tilgjengelige betalingsbeløp og berettigelse til kontantrabatter.

## <a name="issue-checks"></a>Utstede sjekker
[!INCLUDE[d365fin](includes/d365fin_md.md)] lar deg utstede sjekker til leverandører manuelt og elektronisk. Du kan gjøre begge deler i **Utbetalingskladder**-vinduet, der du kan kansellere sjekker og vise sjekkposter.

## <a name="export-payments-to-a-bank-file"></a>Eksportere betalinger til en bankfil
Når du er klar til betale en leverandør, kan du fra vinduet **Betalingskladd** eksportere en fil med betalingsinformasjonen fra kladdelinjene. Du kan deretter laste opp filen til nettbanken for å behandle pengeoverføringene.

Hvis du ikke vil bokføre en utbetalingskladdelinje for en eksportert betaling, for eksempel fordi du venter på at banken skal bekrefte transaksjonen, kan du bare slette kladdelinjen. Når du senere oppretter en utbetalingskladdelinje for å betale restbeløpet på fakturaen, viser feltet **Totalt eksportert beløp** hvor mye av betalingsbeløpet som allerede er eksportert. Du kan også finne detaljert informasjon om det eksporterte totalbeløpet ved å velge knappen **Poster i kredittoverføringsreg.**

Hvis du venter med å bokføre innbetalinger til etter at banken bekrefter at den har behandlet transaksjoner, er det to måter å unngå ved et uhell på nytt eksport betalinger for åpne dokumenter:  

* I en betalingskladd med foreslåtte betalingslinjer kan du sortere etter kolonnen **Lest ut til betalingsfil** eller **Totalt eksportert beløp**, og deretter slette betalingsforslag for åpne fakturaer som allerede er betalt og du ikke ønsker å betale.

    **Merk:** Det kan være du må legge til disse kolonnene i oversikten. Hvis du vil ha mer informasjon, kan du se [Brukertilpasning](ui-user-personalization.md).  
* Du kan også merke av for **Hopp over eksporterte betalinger** i kjørselen **Betalingsforslag - leverandør**, der du angir hvilke betalinger som skal inkluderes i utbetalingskladden, hvis du ikke vil sette inn kladdelinjer for betalinger som allerede er eksportert.

## <a name="see-also"></a>Se også
[Betalingsmåter](finance-payment-methods.md)  
[Finans](finance.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

