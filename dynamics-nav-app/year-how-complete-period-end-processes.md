---
title: Avslutte perioder
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: ac1ed2d1dcf8bf780bda91fbf0a04e5c5e8d106a
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---
# <a name="close-periods"></a>Avslutte perioder
Programmet tvinger deg ikke til å avslutte perioder, men det finnes imidlertid mange aktiviteter for periodeslutt (månedsslutt) som kan utføres i programmet hvis du vil. Dette emnet inneholder en oversikt over disse prosessene og aktivitetene, som er eller ikke er nødvendig for selskapet.

## <a name="general-ledger"></a>Finans
* Angi systemomfattende og brukerspesifikke bokføringsperioder.

    Dette angir datoene som bokføringer som er tillatt mellom. Avhengig av forretningsbehovene vil du kanskje begrense brukerens bokføringsdatoområder i begynnelsen av prosessen ved periodeslutt eller senere mot slutten av perioden. Hvis du vil ha mer informasjon, kan du se [Angi bokføringsperioder](finance-setup-how-specify-posting-periods.md).
* Foreta alle nødvendige finansjusteringer.
* Oppdater og bokfør gjentakelseskladder.
<!--* Process Consolidations-->
* Kjør kontoskjemaer som følger:
  1. Åpne **Kontoskjema**-vinduet, og klikk handlingen **Skriv ut**.
  2. Fyll ut **Kontoskjema**-forespørselen, og velg handlingen **Skriv ut**.

## <a name="sales--receivables"></a>Salg
* Bokfør alle ordrer, fakturaer, kreditnotaer og ordrereturer.
* Bokfør alle innbetalingskladder.
* Oppdater og bokfør gjentakelseskladder som er relatert til salg.
* Avstem kortsiktige fordringer mot Finans.
* Kjør kjørselen **Slett fakturerte ordrer**.

## <a name="purchases--payables"></a>Kjøp
* Bokfør alle bestillinger, fakturaer, kreditnotaer og ordrereturer.
* Bokfør alle utbetalingskladder.
* Oppdater og bokfør gjentakelseskladder som er relatert til kjøp.
* Kjør rapporten **Aldersfordelt saldoliste - lev.**, og avstem leverandørgjeld mot Finans.
* Kjør kjørselen **Slett fakturerte bestillinger**.

<!-- ### Fixed Assets
* Post all maintenance costs have been posted through the fixed asset journals or invoices.
* Post adjustments.
* Post appreciation.
* Post depreciation.
* Update and post the recurring fixed asset journal.-->

<!--### Intercompany
* Process Intercompany Postings.-->

## <a name="calculate-and-process-sales-tax"></a>Beregn og behandle mva.
*  Fullfør mva-oppgaver.

## <a name="see-also"></a>Se også
[Avslutt år og perioder](year-close-years-periods.md)  
[Lukk bøker](year-close-books.md)

