---
title: Eksportere Positive Pay-filer
description: "Du kan sikre at banken bare innfrir validerte sjekker og beløp, ved å eksportere en Positive Pay-fil som inneholder leverandør-og betalingsinformasjon."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: check, clearing
ms.date: 06/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: bf09817e318b5338da0358f829ea2ed1edde9d67
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-export-a-positive-pay-file"></a>Eksportere en Positive Pay-fil
For å sørge for at banken bare innfrir validerte sjekker og beløp, kan du eksportere en Positive Pay-fil med relevant leverandørinformasjon, sjekknummer og betalingskonto, som du deretter sender til banken for referanse når du behandler betalinger.

[!INCLUDE[d365fin](includes/d365fin_md.md)] er forhåndskonfigurert til å støtte Positive Pay-filer for Bank of America og City Bank.

## <a name="to-set-up-a-bank-account-for-positive-pay"></a>Slik definerer du en bankkonto for Positive Pay
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bankkonti**, og velg deretter den relaterte koblingen.
2. Åpne kortet for bank du vil bruke Positive Pay for.
3. Angi POSPAYBANK i feltet **Kode for eksport for Positive Pay**.
4. Lukk vinduet.

## <a name="to-export-a-positive-pay-file"></a>Slik eksporterer du en Positive Pay-fil
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bankkonti**, og velg deretter den relaterte koblingen.
2. Velg bankkontoen som du vil eksportere en Positive Pay-fil for.
3. Velg **Eksport for Positive Pay**.

    Vinduet **Eksport for Positive Pay** åpnes med betalinger som er gjort for bankkontoen siden den forrige datoen for opplasting, som vist i feltene **Dato for siste oppdatering** og **Klokkeslett for siste oppdatering**.
4. I feltet **Dato for frist for oppdatering** field angir du en dato, og betalinger blir ikke inkludert i den eksporterte filen før denne datoen.
5. Velg handlingen **Eksporter**.
6. I **Eksporter fil**-vinduet velger du **Lagre**-knappen, og deretter lagrer du filen på en passende plassering.
7. Last opp filen til det elektroniske bankområdet.
8. Skriv ned eller kopier bekreftelsesnummeret som vises når filopplastingen er vellykket.

Vise eksporterte Positive Pay-poster

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bankkonti**, og velg deretter den relaterte koblingen.
2. Velg bankkontoen som du vil vise Positive Pay-eksportposter for.
3. Velg **Poster for Positive Pay**.

    I vinduet **Poster for Positive Pay** kan du se alle Positive Pay-eksportpostene for bankkontoen.
4. I feltet **Bekreftelsesnummer** angir du bekreftelsesnummeret som du får når opplastingen av filen til banken er vellykket, for hver post for eksport.
5. For å vise de relaterte betalingslinjene, velger du **Detaljer for poster for Positive Pay**.

Eksportere Positive Pay-filer på nytt

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bankkonti**, og velg deretter den relaterte koblingen.
2. Velg bankkontoen som du vil eksportere Positive Pay-filer på nytt for.
3. Velg **Poster for Positive Pay**.
4. Velg linjen for Positive Pay-eksportfilen som du vil eksportere på nytt.
5. I vinduet **Poster for Positive Pay** velger du **Eksporter Positive Pay til fil på nytt**.

## <a name="see-also"></a>Se også
[Finans](finance.md)  
[Konfigurere finans](finance-setup-finance.md)  
[Arbeide med finanskladder](ui-work-general-journals.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

