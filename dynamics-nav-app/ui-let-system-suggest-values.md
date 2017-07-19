---
title: "La Dynamics NAV foreslå verdier"
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
ms.openlocfilehash: 889d0aa5da36d7a4b7e2be1d796ac95e74aaaaf6
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="letting-dynamics-nav-suggest-values"></a>La Dynamics NAV foreslå verdier
Dynamics NAV kan hjelpe deg med å fullføre oppgaver raskere og mer riktig ved å forhåndsutfylle felt eller hele linjer med data som du ellers måtte beregne og skrive inn selv. Selv om slik automatisk dataregistrering alltid er riktig, kan du endre den senere ved behov.

Funksjonalitet som angir feltverdiene for deg tilbys vanligvis for oppgaver der du skriver inn store mengder transaksjonsdata og vil unngå feil og spare tid. Dette emnet inneholder et utvalg av slik funksjonalitet. Flere avsnitt vil bli lagt til i fremtidige oppdateringer av Dynamics NAV.

## <a name="the-suggest-balancing-amount-check-box-in-the-general-journal-batches-window"></a>Avmerkingsboksen **Foreslå motkontobeløp** i vinduet **Finanskladder**
Når du for eksempel angir finanskladdlinjer for flere utgifter som alle må bokføres til samme bankkonto, kan du få **Beløp**-feltet på bankkontolinjen oppdateres automatisk til beløpet som balanserer utgiftene, hver gang du angir en ny kladdelinje for en utgift. Hvis du vil ha mer informasjon om hvordan du arbeider med finanskladder, kan du se [Arbeid med finanskladder](ui-work-general-journals.md).

### <a name="to-have-the-amount-field-on-balancing-general-journal-lines-filled-automatically"></a>Fylle ut **Beløp**-feltet automatisk på finanskladdlinjer for motkonto
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Finanskladder** og velger deretter den relaterte koblingen.
2. På linjen for din foretrukne finanskladd kan du merke av for **Foreslå motkontobeløp**.
3. Åpne finanskladden, og fortsett med å registrere og bokføre transaksjoner ved hjelp av funksjonen som er beskrevet for automatisk registrering av en feltverdi.       

Hvis du vil ha informasjon om hvordan du konfigurerer en personlig finanskladd, for eksempel for håndtering av utgifter, kan du se [Arbeide med finanskladder](ui-work-general-journals.md).

## <a name="the-automatically-fill-date-received-field-in-the-payment-registration-window"></a>Feltet **Fyll ut mottaksdato automatisk** i vinduet **Betalingsregistrering**
Vinduet **Betalingsregistrering** viser utestående innkommende betalinger som linjer som representerer salgsdokumenter der et beløp er forfalt til betaling. Hvis du vil ha mer informasjon om utligning av kundebetalinger, kan du se [Avstemme kundebetalinger manuelt fra en liste over ubetalte salgsdokumenter](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md)

De viktigste handlingene i vinduet er å merke av for **Betaling utført** og fylle ut feltet **Mottatt den**. Du kan definere at Dynamics NAV automatisk angir arbeidsdatoen i feltet **Mottatt den** når du merker av for **Betaling utført**.

### <a name="to-have-the-date-received-field-in-the-payment-registration-window-filled-automatically"></a>Fylle ut feltet **Mottatt den** automatisk i vinduet **Betalingsregistrering**
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Betalingsregistreringsoppsett** og velger deretter den relaterte koblingen.
2. Merk av for **Fyll ut mottaksdato automatisk**.
3. Åpne vinduet **Betalingsregistrering**, og fortsett med å behandle inngående kundebetalinger ved hjelp av funksjonen som er beskrevet for automatisk registrering av en feltverdi.

## <a name="see-also"></a>Se også
[Arbeide med Dynamics NAV](ui-work-product.md)  
[Finans](Finance.md)

