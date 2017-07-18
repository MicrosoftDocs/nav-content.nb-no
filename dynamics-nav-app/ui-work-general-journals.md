---
title: Arbeide med finanskladder
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 2dc2b22fbc0ff70addd16ca14e8c5416c49915e7
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="work-with-general-journals"></a>Arbeide med finanskladder
DU bruker finanskladder til å bokføre finanstransaksjoner til finanskonti og andre konti, for eksempel bank-, kunde- og leverandørkonti. Bokføring med en finanskladd oppretter alltid poster på finanskonti. Dette gjelder selv om en kladdelinje for eksempel bokføres på en kundekonto, ettersom en post bokføres til en finanssamlekonto via en bokføringsgruppe.

Opplysningene du angir i en kladd, er midlertidige og kan endres mens de fortsatt befinner seg i kladden. Når du bokfører kladden, overføres opplysningene til poster i individuelle konti, der de ikke kan endres. Du kan imidlertid oppheve utligningen av bokførte poster, og du kan bokføre tilbakeførings- eller korrigeringsposter.

## <a name="journal-templates-and-batches"></a>Kladdemaler og kladder
Det finnes flere finanskladdemaler. Hver kladdemal er representert av et eget vindu med bestemte funksjoner og feltene som er nødvendige for å støtte disse funksjonene, for eksempel vinduet **Betalingsavstemmingskladd** for å behandle betalinger og **Betalingskladd** for å betale leverandører.

Du kan definere dine egne personlige kladder som en kladd for hver enkelt kladdemal. Du kan for eksempel definere din egen kladd for betalingskladden som har personlig oppsett og innstillinger.

**Merk**: Et eksempel på en personlig innstilling som du kan definere i finanskladden, er å få systemet til å hjelpe deg med å fylle ut beløpsfelt. Hvis du merker av for **Foreslå motkontobeløp** på linjen for den kladden i vinduet **Finanskladder**, vil deretter for eksempel **Beløp**-feltet på finanskladdelinjer for samme dokumentnummer, automatisk forhåndsutfylles med verdien som kreves for balansere dokumentet. Hvis du vil ha mer informasjon, kan du se [La Dynamics NAV foreslå verdier](ui-let-system-suggest-values.md).

## <a name="main-accounts-and-balancing-accounts"></a>Hovedkontoer og motkontoer
Hvis du har definert standard motkonti for kladdene, vil motkontoen bli fylt ut automatisk når du fyller ut **Kontonr.**-fetet. . Hvis ikke, fyller du ut **Kontonr.** -feltet og **Motkontonr.** -feltet manuelt. Et positivt beløp i **Beløp**-feltet debiteres hovedkontoen og krediteres motkontoen. Et negativt beløp krediteres hovedkontoen og debiteres motkontoen.

**Merk**: Mva beregnes separat for hovedkontoen og motkontoen, så de kan bruke ulike mva-prosentsatser.

## <a name="recurring-journals"></a>Gjentakelseskladder
En gjentakende kladd er en finanskladd med bestemte felt for håndtering av transaksjoner du bokfører ofte, med få eller ingen endringer. Hvis du bruker disse feltene for gjentatte transaksjoner, kan du bokføre både faste og variable beløp. Du kan også angi automatiske tilbakeføringsposter for dagen etter bokføringsdatoen, og bruke fordelingsnøkler med de gjentakende postene.

## <a name="see-also"></a>Se også
[Bruke fordelingsnøkler i finanskladder](ui-how-use-allocation-keys-general-journals.md)  
[Finans](finance-setup.md)  
[Arbeide med Dynamics NAV](ui-work-product.md)

