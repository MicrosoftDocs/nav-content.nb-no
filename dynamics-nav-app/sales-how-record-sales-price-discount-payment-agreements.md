---
title: Registrere salgspriser og rabatter
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
ms.openlocfilehash: 2d6438108fb2c36bb6f0d44efddc053bd628d068
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-record-sales-prices-and-discounts"></a>Registrere salgspriser og rabatter
De ulike pris- og rabattavtalene som gjelder ved salg til ulike kunder, må defineres slik at de avtalte reglene og verdiene brukes på salgsdokumenter du oppretter for kundene.

Når det gjelder priser, kan du sette inn en spesialsalgspris på salgslinjer hvis en bestemt kombinasjon av kunde, vare, minste antall, enhet, eller start-/sluttdato finnes.

Når det gjelder rabatter, kan du opprette og bruke to typer salgsrabatter:

|Rabattype |Beskrivelse |
|--------------|------------|
|**Salgslinjerabatt**|Et rabattbeløp som settes inn på salgslinjer hvis en bestemt kombinasjon av kunde, vare, minste antall, enhet, eller start-/sluttdato finnes. Dette fungerer på samme måte som for salgspriser.|
|**Fakturarabatt**|En prosentrabatt som trekkes fra dokumenttotalen hvis beløpet for alle linjer på et salgsdokument overskrider et bestemt minimumsbeløp.|

Ettersom salgspriser og salgslinjerabatter er basert på en kombinasjon av vare og kunde, kan du også utføre denne konfigurasjon fra varekortet for varen der reglene og verdiene skal brukes.

## <a name="to-set-up-a-sales-price-for-a-customer"></a>Definere salgspriser for en kunde
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kunder** og velger deretter den relaterte koblingen.
2. Åpne det aktuelle kundekortet, og velg deretter handlingen **Priser**.

    Feltet **Salgstype** er forhåndsutfylt med **Kunde**, og feltet **Salgskode** er forhåndsutfylt med kundenummeret.
3. Fyll ut feltene på linjen etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
4. Fyll ut en linje for hver kombinasjon som gir en spesialsalgspris for kunden.

## <a name="to-set-up-a-sales-line-discount-for-a-customer"></a>Definere en salgslinjerabatt for en kunde
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kunder** og velger deretter den relaterte koblingen.
2. Åpne det aktuelle kundekortet, og velg deretter handlingen **Linjerabatter**.

    Feltet **Salgstype** er forhåndsutfylt med **Kunde**, og feltet **Salgskode** er forhåndsutfylt med kundenummeret.
3.  Fyll ut feltene på linjen etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
4. Fyll ut en linje for hver kombinasjon som gir en salgslinjerabatt for kunden.

## <a name="to-set-up-an-invoice-discount-for-a-customer"></a>Definere en fakturarabatt for en kunde
Når du har bestemt hvilke kunder som skal gis fakturarabatter, angir du fakturarabattkode på kundekortet og definerer betingelsene for hver kode.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kunder** og velger deretter den relaterte koblingen.
2. Åpne kundekortet for kunden som skal ha fakturarabatter.
3. I feltet **Fakturarabattkode** velger du en kode for de aktuelle fakturarabattbetingelsene som skal brukes til å beregne fakturarabatter for kunden.

    **Merk**: Fakturarabattkoder representeres av eksisterende kundekort. Dette lar deg raskt tilordne fakturarabattbetingelsene til kunder ved å velge navnet på en annen kunde som har de samme betingelsene.

    Fortsett å definere nye betingelser for salgsfakturarabatt.
4. I vinduet **Kundekort** velger du handlingen **Fakturarabatter**. Vinduet **Kundefakturarabatter** åpnes.
5. I feltet **Valutakode** angir du koden til en valuta som fakturarabattbetingelsene på linjen gjelder for. La feltet stå tomt for å definere betingelser for fakturarabatt i USD.
6. I **Minimumsbeløp**-feltet angir du hva som er minstebeløpet for at det skal gis rabatt i en faktura.
7. I **Rabatt-%**-feltet angir du fakturarabatten prosentvis av fakturabeløpet.
8. Gjenta trinn 5 til 7 for hver valuta som kunden vil motta en forskjellig fakturarabatt for.

Fakturarabatten er nå definert og tilordnet til den aktuelle kunden. Når du velger kundekoden i **Fakturarabattkode**-feltet på andre kundekort, tilordnes den samme fakturarabatten til kundene.

## <a name="see-also"></a>Se også  
[Definere salg](sales-setup-sales.md)  
[Håndtere salg](sales-manage-sales.md)

