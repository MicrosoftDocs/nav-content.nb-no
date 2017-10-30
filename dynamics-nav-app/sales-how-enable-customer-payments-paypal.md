---
title: Aktiver kundebetalinger gjennom PayPal
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 15f30a03c3e7ccc865ef527a707794c2c6428b2f
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-enable-customer-payments-through-paypal"></a>Aktiver kundebetalinger gjennom PayPal#
Som et alternativ til å samle inn betalinger via bankoverføring eller kredittkort, kan du tilby kundene å betale du gjennom sin PayPal-konto.

Når en kunde velger PayPal-koblingen på en salgsfaktura eller et salgsordredokument, vises tjenestesiden deres for PayPal-kontoen med betalingsdetaljer for salget. Kunden kan deretter betale fakturaen på samme måte som andre PayPal-betalinger.

Hvis du vil aktivere kundebetalinger gjennom PayPal, må du gjøre følgende:

1. Definere PayPal Payments Standard som en betalingstjeneste i vinduet **Betalingstjenester**.
2. Velg PayPal Payments Standard i feltet **Betalingstjeneste** på det aktuelle salgsdokumentet.

PayPal Payments Standard-tjenesten er installert som en utvidelse for Dynamics NAV og er klar til å aktiveres. Hvis du vil ha mer informasjon, kan du se [Tilpasse Dynamics NAV ved hjelp av utvidelser](ui-extensions.md).

## <a name="to-enable-the-paypal-payments-standard-service"></a>Aktivere PayPal Payments Standard-tjenesten
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Betalingstjenester** og velger deretter den relaterte koblingen.  
2. I vinduet **Betalingstjenester** velger du handlingen **Ny**.
3. Velg **PayPal Standard**, og lukk deretter vinduet.
4. I vinduet **Betalingstjenester** velger du handlingen **Oppsett**.
5. Fyll ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.

    **Merk**: Merk av for **Inkluder alltid i dokumenter** hvis hyperkoblingen for PayPal-betalingstjenesten alltid skal vises på salgsdokumentene når betaling via PayPal er aktivert.

6. Lukk vinduet.

## <a name="to-select-paypal-payments-standard-on-a-sales-invoice"></a>Velge PayPal Payments Standard på en salgsfaktura
1. Velg handlingen **Salgsfakturaer** på Hjem-siden.
2. Åpne salgsfakturaen som du vil aktivere PayPal-betalinger for.
3. I feltet **Betalingstjeneste** velger du PayPal Payments Standard.

**Merk**: Feltet **Betalingstjeneste** vises bare hvis PayPal Payments Standard-tjenesten er aktivert.   

## <a name="see-also"></a>Se også  
[Definere salg](sales-setup-sales.md)  
[Håndtere salg](sales-manage-sales.md)  
[Tilpasse Dynamics NAV ved hjelp av utvidelser](ui-extensions.md)

