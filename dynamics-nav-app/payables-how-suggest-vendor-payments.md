---
title: "Foreslå leverandørbetalinger"
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
ms.openlocfilehash: 11bfba9f279f6bd84c5d169f6f97fd48759bc6df
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-suggest-vendor-payments"></a>Foreslå leverandørbetalinger
I vinduet **Betalingskladd** kan du bruke en funksjon til å foreslå betalingslinjer i henhold til dine innstillinger, for eksempel betalinger som forfaller snart eller betalinger der kontantrabatt er tilgjengelig.

Hvis du vil dra full nytte funksjonen Betalingsforslag - leverandør, må du først prioritere leverandørene. Hvis du vil ha mer informasjon, kan du se [Prioritere leverandører](purchasing-how-prioritize-vendors.md).

Leverandørposter som er merket med **Avvent** tas ikke med i kjørselen.  

**Viktig**: Hvis du vil dra nytte av kontantrabatter og få angitt et disponibelt beløp, brukes beløpet først til prioriterte forfalte leverandørposter i prioritetsrekkefølge, deretter til forfalte leverandørposter som ikke er prioritert, og til slutt til åpne leverandørposter med rett til kontantrabatter, sortert etter leverandørnummer.

## <a name="to-use-the-suggest-vendor-payments-function"></a>Bruke funksjonen Betalingsforslag - leverandør
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Betalingskladder** og velger deretter den relaterte koblingen.
2. Åpne den aktuelle kladden, og velg deretter handlingen **Betalingsforslag - leverandør**.
3. Fyll ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
4. Velg **OK**-knappen.

## <a name="to-insert-the-due-date-as-posting-date-on-payment-journal-lines"></a>Sette inn forfallsdato som bokføringsdato på betalingskladdelinjer
Når du bruker kjørselen **Betalingsforslag - leverandør** til å opprette betalingslinjer for leverandørene, kan du fylle ut to spesialfelt for å sikre at de genererte linjene bruker forfallsdatoen til å beregne bokføringsdatoen. Disse feltene er **Beregn bokføringsdato fra forfallsdato for utligningsbilag** og **Forskyvning av forfallsdato for utligningsbilag**.

**Viktig**: Du kan ikke bruke feltet **Beregn bokføringsdato fra forfallsdato for utligningsbilag** sammen med feltet **Søk etter kontantrabatter** eller feltet **Summer per leverandør**. Årsaken er at hvis bokføringsdatoen er basert på forfallsdatoen, kan det hende at en del kontantrabatt ikke beregnes på riktig måte, fordi bokføringsdatoen kan komme etter kontantrabattdatoen.
Hvis den beregnede bokføringsdatoen er passert, vil bokføringsdatoen også bli flyttet til arbeidsdatoen og det vil vises en advarsel.

Du kan også opprette betalingslinjer manuelt ved å bruke forfallsdatoen til å beregne bokføringsdatoen. Når du har utlignet leverandørposter, kan du bruke handlingen **Beregn bokføringsdato**. Dett vil oppdatere bokføringsdatoen på kladdelinjen med forfallsdatoen for den tilknyttede kjøpsfakturaen. Hvis du vil ha mer informasjon, kan du se [Utligne kjøpstransaksjoner manuelt](payables-how-apply-purchase-transactions-manually.md).  

**Merk**: Hvis kjøpsfakturaen er forfalt, vil bokføringsdatoen bli satt til arbeidsdatoen, og skriftfargen på linjen endres til rød.

## <a name="see-also"></a>Se også
[Administrere skyldige beløp](payables-manage-payables.md)  
[Foreta betalinger](payables-make-payments.md)  
[Arbeide med finanskladder](ui-work-general-journals.md)

