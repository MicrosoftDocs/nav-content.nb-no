---
title: Fakturere salg
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
ms.openlocfilehash: cba338ec6469ea0ac22f024571664a718988e827
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-invoice-sales"></a>Fakturere salg

Du kan opprette en salgsfaktura eller ordre for å registrere avtalen med en kunde om å selge bestemte produkter på bestemte leverings- og betalingsbetingelser.

**Merk**: Du må bruke ordrer hvis salgsprosessen krever at du kan sende deler av et bestillingsantall, for eksempel fordi det fullstendige antallet ikke er tilgjengelig samtidig. Hvis du selger varer ved å levere direkte fra leverandøren til kunden, som en direkte levering, må du også å bruke ordrer. Hvis du vil ha mer informasjon, kan du se [Foreta direkte leveringer](sales-how-drop-shipment.md). I alle andre henseender fungerer ordrer på samme måte som salgsfakturaer. Hvis du vil ha mer informasjon, kan du se [Selge produkter](sales-how-sell-products.md).

Du kan forhandle med kunden ved først å opprette et tilbud, som du kan konvertere til en salgsfaktura når dere blir enige om salget. Hvis du vil ha mer informasjon, kan du se [Gi tilbud](sales-how-make-offers.md).

Etter at kunden har bekreftet avtalen, for eksempel etter en tilbudsprosess, bokfører du salgsfakturaen for å opprette relatert antall og verdiposter i systemet. Når du bokfører salgsfakturaen, kan du også sende dokumentet som et PDF-vedlegg i e-post. Du kan få brødteksten i e-posten forhåndsutfylt med et sammendrag av fakturaen og betalingsinformasjonen, for eksempel en kobling til PayPal. Hvis du vil ha mer informasjon, kan du se [Sende dokumenter i e-post](ui-how-send-documents-email.md).

I forretningsmiljøer der kunden må betale før produkter leveres, for eksempel i detaljhandel, må du vente til mottak av betalingen før du leverer produktene. I de fleste tilfeller kan du behandle innkommende betalinger noen uker etter levering ved å utligne betalingene mot deres tilknyttede bokførte, ubetalte salgsfakturaer. Hvis du vil ha mer informasjon, kan du se [Avstemme betalinger ved hjelp av automatisk utligning](receivables-how-reconcile-payments-auto-application.md).

Hvis den bokførte salgsfakturaen er betalt, må du opprette en salgskreditnota for å reversere salget. Hvis du vil ha mer informasjon, kan du se [Behandle ordrereturer eller annulleringer](sales-how-process-sales-returns-cancellations.md).

Produkter kan være både varer og tjenester. Hvis du vil ha mer informasjon, kan du se [Registrere nye produkter](inventory-how-register-new-products.md). Salgsfakturaprosessen er den samme for begge produkttyper.

**Merk**: I Dynamics NAV brukes ordet “vare” for å referere til et produkt.

Du kan fylle kundefelt i salgsfakturaen på to måter, avhengig av om kunden allerede er registrert.

## <a name="to-create-a-sales-invoice"></a>Slik oppretter du en salgsfaktura
1. Velg handlingen **Salgsfaktura** på Hjem-siden.  
3. I feltet **Kunde** angir du navnet på en eksisterende kunde.

    Andre felt i **Salgsfaktura**-vinduet fylles nå med standardinformasjon for den valgte kunden. Hvis kunden ikke er registrert, følger du denne fremgangsmåten:
4. I feltet **Kunde** angir du navnet på den nye kunden.
5. Klikk **Ja**-knappen i dialogboksen for å registrere den nye kunden.
6. I vinduet **Velg en mal for en ny kunde** velger du en mal som du vil basere det nye kundekortet på, og deretter velger du **OK**-knappen.
7. Det åpnes et nytt kundekort som er forhåndsutfylt med informasjon om den valgte kundemalen. **Navn**-feltet er forhåndsutfylt med det nye kundenavnet du skrev inn i salgsfakturaen i salgsfakturaen.
8. Fortsette med å fylle ut resten av feltene på kundekortet. Hvis du vil ha mer informasjon, kan du se [Registrere nye kunder](sales-how-register-new-customers.md).  
9. Når du har fullført kundekortet, velger du **OK**-knappen for å gå tilbake til **Salgsfaktura** -vinduet.

    Flere felt i salgsfakturen er nå fylt ut med informasjon du har angitt på det nye kundekortet.
10. Fyll ut resten av feltene vinduet **Salgsfaktura** etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.

    Du kan nå begynne å fylle ut salgsfakturalinjene med lagervarer eller tjenester du vil selge til kunden.

    Hvis du har definert gjentakende salgslinjer for kunden, for eksempel en månedlig etterfyllingsordre, kan du sette inn disse linjene på fakturaen ved å velge handlingen **Hent gjentakende salgslinjer**.
11. Angi nummeret på en vare eller tjeneste i **Vare**-feltet i hurtigfanen **Linjer**.  
12. I feltet **Antall** angir du hvor mange varer som skal selges.

    **Merk**: For varer av typen Tjeneste er antallet en tidsenhet, for eksempel timer, som angitt i feltet **Enhetskode** på linjen.

    Feltet **Linjebeløp** oppdateres for å vise verdien i feltet **Salgspris** multiplisert med verdien i feltet **Antall**.

    Prisen og linjebeløpene vises med eller uten mva, avhengig av hva du valgte i feltet **Priser inkludert merverdiavgift** på kundekortet.
13. I feltet **Linjerabatt-%** angir du en prosent hvis du vil gi kunden en rabatt på produktet. Verdien i feltet **Linjebeløp** oppdateres tilsvarende.

    Hvis du har konfigurert varepriser i hurtigfanen **Salgspriser og salgslinjerabatter** i kunde- eller varekortet, oppdateres prisen og beløpet på tilbudslinjen automatisk hvis de avtalte priskriteriene er oppfylt. Hvis du vil ha mer informasjon, kan du se [Registrere avtaler om salgspris, rabatt og betaling](sales-how-record-sales-price-discount-payment-agreements.md).
14. Hvis du vil legge til en kommentar om tilbudslinjen som kunden kan se på tilbudsutskriften, skriver du en tekst i **Beskrivelse**-feltet på en tom linje.  
15. Gjenta trinn 10 til 13 for hver vare som du vil tilby til kunden.

    Totaler under linjene beregnes automatisk når du oppretter eller endrer linjer.
16. I feltet **Fakturarabattbeløp** angir du et beløp som skal trekkes fra verdien som vises i feltet **Totalt inkl. mva.**.

    Hvis du har definert fakturarabatter for kunden, settes den angitte prosentverdien automatisk inn i feltet **Fakturarabatt %** hvis kriteriene er oppfylt, og det relaterte beløpet settes inn i feltet **Fakturarabattbeløp før mva.**. Hvis du vil ha mer informasjon, kan du se [Registrere avtaler om salgspris, rabatt og betaling](sales-how-record-sales-price-discount-payment-agreements.md).
17. Når salgsfakturalinjene er fullført, kan du velge handlingen **Bokfør og send**.

Dialogboksen **Bokfør og send bekreftelse** åpnes, og viser den foretrukne sendemetoden for kunden. Du kan endre sendemetoden ved å velge oppslagsknappen for feltet **Send dokument til**. Hvis du vil ha mer informasjon, kan du se [Definere en profil for dokumentsending](sales-how-setup-document-send-profiles.md).

Beslektet element og kundeposter opprettes nå i systemet, og salgsfakturaen skrives ut som et PDF-dokument. Salgsfakturaen fjernes fra listen over salgsfakturaer og erstattes med et nytt dokument i listen over bokførte salgsfakturaer.

## <a name="see-also"></a>Se også  
[Håndtere salg](sales-manage-sales.md)  
[Definere salg](sales-setup-sales.md)  
[Lager](inventory-manage-inventory.md)    
[Sende dokumenter i e-post](ui-how-send-documents-email.md)  
[Arbeide med Dynamics NAV](ui-work-product.md)

