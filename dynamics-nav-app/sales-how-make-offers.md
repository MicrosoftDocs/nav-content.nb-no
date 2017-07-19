---
title: Gi tilbud
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
ms.openlocfilehash: e126c755a9121c3a91f3af72f3f1ae14702a4701
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-make-offers"></a>Gi tilbud
Du kan opprette et tilbud for å registrere tilbudet til en kunde om å selge bestemte produkter på bestemte leverings- og betalingsbetingelser. Du kan sende tilbudet til kunden for å formidle tilbudet. Du kan sende dokumentet i e-post som et PDF-vedlegg. Du kan også få brødteksten i e-posten forhåndsutfylt med et sammendrag av tilbudet. Hvis du vil ha mer informasjon, kan du se [Sende dokumenter i e-post](ui-how-send-documents-email.md).

Mens du forhandler med kunden, kan du endre og sende tilbudet på nytt så ofte som nødvendig. Når kunden godkjenner tilbudet, kan du konvertere tilbudet til en salgsfaktura eller ordre som du behandler salget i. Hvis du vil ha mer informasjon, kan du se [Fakturere salg](sales-how-invoice-sales.md) eller [Selge produkter](sales-how-sell-products.md).

Produkter kan være både varer og tjenester. Hvis du vil ha mer informasjon, kan du se [Registrere nye produkter](inventory-how-register-new-products.md). Tilbudsprosessen er den samme for begge produkttyper.

**Merk**: I Dynamics NAV brukes ordet “vare” for å referere til et produkt.

Du kan fylle kundefelt i tilbudet på to måter, avhengig av om kunden allerede er registrert.

## <a name="to-create-a-sales-quote"></a>Slik oppretter du et tilbud
1. Velg handlingen **Tilbud** på Hjem-siden.  
2. I feltet **Kunde** angir du navnet på en eksisterende kunde.

    Andre felt i **Tilbud**-vinduet fylles nå med standardinformasjon for den valgte kunden. Hvis kunden ikke er registrert, følger du denne fremgangsmåten:

3. I feltet **Kunde** angir du navnet på den nye kunden.
4. Klikk **Ja**-knappen i dialogboksen for å registrere den nye kunden.
5. I vinduet **Velg en mal for en ny kunde** velger du en mal som du vil basere det nye kundekortet på, og deretter velger du **OK**-knappen.
6. Det åpnes et nytt kundekort som er forhåndsutfylt med informasjon om den valgte kundemalen. **Navn**-feltet er forhåndsutfylt med det nye kundenavnet du skrev inn i salgsfakturaen i salgsfakturaen.
7. Fortsette med å fylle ut resten av feltene på kundekortet. Hvis du vil ha mer informasjon, kan du se [Registrere nye kunder](sales-how-register-new-customers.md).  
8. Når du har fullført kundekortet, velger du **OK**-knappen for å gå tilbake til **Tilbud** -vinduet.

    Flere felt i tilbudet er nå fylt ut med informasjon du har angitt på det nye kundekortet.
9. Fyll ut resten av feltene vinduet **Tilbud** etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.

    Du kan nå begynne å fylle ut tilbudslinjene med lagervarer eller tjenester du vil tilby til kunden.

    **Merk**: Hvis du har definert gjentakende salgslinjer for kunden, for eksempel en månedlig etterfyllingsordre, kan du sette inn disse linjene på tilbudet ved å velge handlingen **Hent gjentakende salgslinjer**.
10. I hurtigfanen **Linjer**, i **Varenr.** -feltet, angir du nummeret for en lagervare eller service.
11. I feltet **Antall** angir du hvor mange varer som skal tilbys.

    **Merk**: For varer av typen Tjeneste er antallet en tidsenhet, for eksempel timer, som angitt i feltet **Enhetskode** på linjen.

    Feltet **Linjebeløp** oppdateres for å vise verdien i feltet **Salgspris** multiplisert med verdien i feltet **Antall**.

    Prisen og linjebeløpene vises med eller uten mva, avhengig av hva du valgte i feltet **Priser inkludert merverdiavgift** på kundekortet.
12. I feltet **Linjerabatt-%** angir du en prosent hvis du vil gi kunden en rabatt på produktet. Verdien i feltet **Linjebeløp** oppdateres tilsvarende.

    **Merk**: Hvis du har konfigurert varepriser i hurtigfanen **Salgspriser og salgslinjerabatter** i kunde- eller varekortet, oppdateres prisen og beløpet på tilbudslinjen automatisk hvis de avtalte priskriteriene er oppfylt. Hvis du vil ha mer informasjon, kan du se [Registrere avtaler om salgspris, rabatt og betaling](sales-how-record-sales-price-discount-payment-agreements.md).
13. Hvis du vil legge til en kommentar om tilbudslinjen som kunden kan se på tilbudsutskriften, skriver du en tekst i **Beskrivelse**-feltet på en tom linje.  
14. Gjenta trinn 10 til 13 for hver vare som du vil tilby til kunden.

    Totaler under linjene beregnes automatisk når du oppretter eller endrer linjer.
15. I feltet **Fakturarabattbeløp** angir du et beløp som skal trekkes fra verdien som vises i feltet **Totalt inkl. mva.**.

    **Merk**: Hvis du har definert fakturarabatter for kunden, settes den angitte prosentverdien automatisk inn i feltet **Fakturarabatt %** hvis kriteriene er oppfylt, og det relaterte beløpet settes inn i feltet **Fakturarabattbeløp før mva.**. Hvis du vil ha mer informasjon, kan du se [Registrere avtaler om salgspris, rabatt og betaling](sales-how-record-sales-price-discount-payment-agreements.md).
16. Når tilbudslinjene er fullført, kan du velge handlingen **E-post** eller **Skriv ut**.

    Hvis du velger handlingen **E-post**, blir en PDF-fil lagt ved automatisk i en e-post til kunden. Du kan opprette e-postmeldingen med et sammendrag av tilbudet. Hvis du vil ha mer informasjon, kan du se [Sende dokumenter i e-post](ui-how-send-documents-email.md).
17. Hvis kunden godtar tilbudet, velger du handlingen **Lag faktura** eller **Lag ordre**.

Tilbudet er fjernet fra databasen. Det opprettes en salgsfaktura eller ordre basert på informasjonen i tilbudet der du kan behandle salget. I **Tilbudsnr.** -feltet på salgsfakturaen eller ordren kan du se nummeret på salgstilbudet den ble laget fra. Hvis du vil ha mer informasjon, kan du se [Fakturere salg](sales-how-invoice-sales.md) eller [Selge produkter](sales-how-sell-products.md).

## <a name="see-also"></a>Se også  
[Håndtere salg](sales-manage-sales.md)  
[Definere salg](sales-setup-sales.md)  
[Sende dokumenter i e-post](ui-how-send-documents-email.md)  
[Arbeide med Dynamics NAV](ui-work-product.md)

