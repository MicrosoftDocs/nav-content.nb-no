---
title: "Registrere kjøpspriser og rabatter"
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
ms.openlocfilehash: f99bb0aeef2c25048b0da3e0476ae2d612bff562
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

#<a name="how-to-record-purchase-prices-and-discounts"></a>Registrere kjøpspriser og rabatter
De forskjellige pris- og rabattavtaler som gjelder når du kjøper fra forskjellige leverandører, må defineres slik at avtalte regler og verdier brukes på kjøpsdokumenter du oppretter for leverandørene.

Når det gjelder priser, kan du sette inn en spesialkjøpspris på bestillingslinjer hvis en bestemt kombinasjon av leverandør, vare, minste antall, enhet, eller start-/sluttdato finnes.

Når det gjelder rabatter, kan du opprette og bruke to typer kjøpsrabatter:

|Rabattype |Beskrivelse |
|--------------|------------|
|**Bestillingslinjerabatt**|Et rabattbeløp som settes inn på bestillingslinjer hvis en bestemt kombinasjon av leverandør, vare, minste antall, enhet, eller start-/sluttdato finnes. Dette fungerer på samme måte som for innkjøpspriser.|
|**Fakturarabatt**|En prosentrabatt som trekkes fra dokumenttotalen hvis beløpet for alle linjer på et kjøpsdokument overskrider et bestemt minimumsbeløp.|

Ettersom bestillingslinjerabatter og kjøpspriser er basert på en kombinasjon av vare og leverandør, kan du også angi denne konfigurasjonen fra varekortet, der regler og verdier er definert. Hvis du vil ha mer informasjon, kan du se [Registrere nye produkter](inventory-how-register-new-products.md).

## <a name="to-set-up-a-special-purchase-price-for-a-vendor"></a>Definere en spesialkjøpspris for en leverandør
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Leverandører** og velger deretter den relaterte koblingen.
2. Åpne det aktuelle leverandørkortet, og velg deretter handlingen **Priser**.

    **Kjøpstype**-feltet er forhåndsutfylt med **Leverandør**, og **Kjøpskode**-feltet er forhåndsutfylt med leverandørnummeret.
3. Fyll ut feltene på linjen etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
4. Fylle ut en linje for hver kombinasjon som leverandøren gir deg en bestillingslinjerabatt for.

## <a name="to-set-up-a-line-discount-for-a-vendor"></a>Definere en linjerabatt for en leverandør
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Leverandører** og velger deretter den relaterte koblingen.
2. Åpne det aktuelle leverandørkortet, og velg deretter handlingen **Linjerabatter**.

    **Kjøpstype**-feltet er forhåndsutfylt med **Leverandør**, og **Kjøpskode**-feltet er forhåndsutfylt med leverandørnummeret.
3. Fyll ut feltene på linjen etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
4. Fylle ut en linje for hver kombinasjon som leverandøren gir deg en bestillingslinjerabatt for.

## <a name="to-set-up-an-invoice-discount-for-a-vendor"></a>Definere en fakturarabatt for en leverandør
Når leverandøren har informert deg om hvilke linjerabatter som gis, angir du fakturarabattkoden på leverandørkortet og definerer betingelsene for hver kode.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Leverandører** og velger deretter den relaterte koblingen.
2. Åpne leverandørkortet for leverandøren som skal ha fakturarabatter.
3. I feltet **Fakturarabattkode** velger du en kode for de aktuelle fakturarabattbetingelsene som skal brukes til å beregne fakturarabatter for leverandøren.

    **Merk**: Fakturarabattkoder representeres av eksisterende leverandørkort. Dette lar deg raskt tilordne fakturarabattbetingelsene til leverandører ved å velge navnet på en annen leverandører som har de samme betingelsene.

    Fortsett å definere nye betingelser for kjøpsfakturarabatt.
4. I vinduet **Leverandørkortet** velger du handlingen **Fakturarabatter**. Vinduet **Levrd./fakt.-rabatter** åpnes.
5. I feltet **Valutakode** angir du koden til en valuta som fakturarabattbetingelsene på linjen gjelder for. La feltet stå tomt for å definere betingelser for fakturarabatt i USD.
6. I **Minimumsbeløp**-feltet angir du hva som er minstebeløpet for at det skal gis rabatt i en faktura.
7. I **Rabatt-%**-feltet angir du fakturarabatten prosentvis av fakturabeløpet.
8. Gjenta trinn 5 til 7 for hver valuta som leverandøren vil motta en forskjellig fakturarabatt for.

Fakturarabatten er nå definert og tilordnet til den aktuelle leverandøren. Når du velger leverandørkoden i **Fakturarabattkode**-feltet på andre leverandørkort, tilordnes den samme fakturarabatten til leverandøren.

## <a name="see-also"></a>Se også  
[Definere kjøp](purchasing-setup-purchasing.md)  
[Håndtere kjøp](purchasing-manage-purchasing.md)

