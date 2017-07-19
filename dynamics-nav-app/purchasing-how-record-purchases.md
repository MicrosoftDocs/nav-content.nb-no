---
title: "Registrere kjøp"
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 6d1933bf1e1c9236d34d429a4da84c907df13708
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-record-purchases"></a>Registrere kjøp
Du kan opprette en kjøpsfaktura eller bestilling for å registrere kjøpskostnader og spore leverandørgjeld. Hvis du vil kontrollere en beholdning, brukes kjøpsfakturaer og bestillinger også til å oppdatere lagernivåer dynamisk, slik at du kan redusere lagerkostnadene og gi bedre kundeservice. Kjøpskostnadene, inkludert tjenesteutgifter samt lagerverdier som er resultat av bokføring av kjøpsfakturaer eller bestillinger, bidrar til fortjenestetall og andre økonomiske KPI-er på Hjem-siden.

**Merk**: Du må bruke bestillinger hvis kjøpsprosessen krever at du registrerer delvise mottak av et bestillingsantall, for eksempel fordi det fullstendige antallet ikke var tilgjengelig hos leverandøren. Hvis du selger varer ved å levere direkte fra leverandøren til kunden, som en direkte levering, må du også å bruke bestillinger. Hvis du vil ha mer informasjon, kan du se [Foreta direkte leveringer](sales-how-drop-shipment.md). I alle andre henseender fungerer bestillinger på samme måte som kjøpsfakturaer. Følgende fremgangsmåte er basert på en kjøpsfaktura. Trinnene er de samme for en bestilling.

Når du mottar lagervarene, eller når den kjøpte tjenesten er fullført, kan du bokføre kjøpsfakturaen eller bestillingen for å oppdatere lager- og økonomiposter og aktivere betaling til leverandøren i samsvar med betalingsbetingelsene. Hvis du vil ha mer informasjon, kan du se [Utføre betalinger](payables-make-payments.md).

**Forsiktig**: Ikke bokfør en kjøpsfaktura før du mottar produktene og kjenner de endelige kostnaden for kjøpet, herunder eventuelle tilleggskostnader. Hvis ikke, kan det hende at lagerverdien og fortjenestebeløpet er skjevt.

Hvis du allerede har betalt for produktene i den bokførte kjøpsfakturaen, må du opprette en kjøpskreditnota for å reversere innkjøpet. Hvis du vil ha mer informasjon, kan du se [Behandle bestillingsreturer eller annulleringer](purchasing-how-process-purchase-returns-cancellations.md).

Produkter kan være både varer og tjenester. Hvis du vil ha mer informasjon, kan du se [Registrere nye produkter](inventory-how-register-new-products.md). Kjøpsfakturaprosessen er den samme for begge produkttyper.



Du kan fylle leverandørfelt i kjøpsfakturaen på to måter, avhengig av om leverandøren allerede er registrert.

## <a name="to-create-a-purchase-invoice"></a>Slik oppretter du en kjøpsfaktura:
1. Velg handlingen **Kjøpsfaktura** på Hjem-siden.  
2. I feltet **Leverandør** angir du navnet på en eksisterende kunde.

    Andre felt i **Kjøpsfaktura**-vinduet fylles nå med standardinformasjon for den valgte leverandøren. Hvis leverandøren ikke er registrert, følger du denne fremgangsmåten:
3. I feltet **Leverandør** angir du navnet på den nye leverandøren.
4. Klikk **Ja**-knappen i dialogboksen for å registrere den nye leverandøren.
5. I vinduet **Velg en mal for en ny leverandør** velger du en mal som du vil basere det nye leverandørkortet på, og deretter velger du **OK**-knappen.
6. Det åpnes et nytt leverandørkort som er forhåndsutfylt med informasjon om den valgte leverandørmalen. **Navn**-feltet er forhåndsutfylt med det nye leverandørnavnet du skrev inn i kjøpsfakturaen.
7. Fortsette med å fylle ut resten av feltene på leverandørkortet. Hvis du vil ha mer informasjon, kan du se [Registrere nye leverandører](purchasing-how-register-new-vendors.md).  
8. Når du har fylt ut leverandørkortet, velger du **OK**-knappen for å gå tilbake til **Kjøpsfaktura**-vinduet.

    Flere felt i **Kjøpsfaktura**-vinduet er fylt ut med informasjon du har angitt på det nye leverandørkortet.
9. Fyll ut resten av feltene vinduet **Kjøpsfaktura** etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.

    Du kan nå begynn å fylle ut kjøpsfakturalinjene med lagervarer eller tjenester du har kjøpt fra leverandøren.

    **Merk**: Hvis du har definert gjentakende bestillingslinjer for leverandøren, for eksempel en månedlig etterfyllingsordre, kan du sette inn disse linjene på fakturaen ved å velge handlingen **Hent gjentakende bestillingslinjer**.
10. I hurtigfanen **Linjer**, i **Varenr.** -feltet, angir du nummeret for en lagervare eller service.
11. I feltet **Antall** angir du hvor mange varer som skal kjøpes.

    **Merk**: For varer av typen **Service** er antallet en tidsenhet, for eksempel timer, som angitt i feltet **Enhetskode** på linjen.

    Feltet **Linjebeløp** oppdateres for å vise verdien i feltet **Direkte enhetskost** multiplisert med verdien i feltet **Antall**.

    Prisen og linjebeløpet vises med eller uten mva, avhengig av hva du valgte i feltet **Priser inkludert merverdiavgift** på leverandørkortet.
12. I feltet **Fakturarabattbeløp** angir du et beløp som skal trekkes fra verdien som vises i feltet **Totalt inkl. mva.** nederst på fakturaen.

    **Merk**: Hvis du har definert fakturarabatter for leverandøren, settes den angitte prosentverdien automatisk inn i feltet **Leverandørfakturarabatt-%** hvis kriteriene er oppfylt, og det relaterte beløpet settes inn i feltet **Fakturarabattbeløp**.
13. Velg **Bokfør** når du mottar innkjøpte varer eller tjenester.

Kjøpet gjenspeiles nå i lager- og økonomiposter, og leverandørbetalingen aktiveres. Kjøpsfakturaen fjernes fra listen over kjøpsfakturaer og erstattes med et nytt dokument i listen over bokførte kjøpsfakturaer.

## <a name="see-also"></a>Se også  
[Håndtere kjøp](purchasing-manage-purchasing.md)  
[Definere kjøp](purchasing-setup-purchasing.md)  
[Fremgangsmåte: Kjøpe produkter for salg](purchasing-how-purchase-products-sale.md)  
[Registrere nye leverandører](purchasing-how-register-new-vendors.md)  
[Klargjøre direkte leveringer](sales-how-drop-shipment.md)  
[Arbeide med Dynamics NAV](ui-work-product.md)

