---
title: Selge produkter
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
ms.openlocfilehash: e45d67005364f7d45817d917ccaeab219b6f8446
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-sell-products"></a>Selge produkter
Du kan opprette en ordre eller salgsfaktura for å registrere avtalen med en kunde om å selge bestemte produkter på bestemte leverings- og betalingsbetingelser.

**Merk**: Du bruker ordrer hvis salgsprosessen krever at du kan sende deler av et bestillingsantall, for eksempel fordi det fullstendige antallet ikke er tilgjengelig samtidig. Hvis du selger varer ved å levere direkte fra leverandøren til kunden, som en direkte levering, må du også å bruke ordrer. Hvis du vil ha mer informasjon, kan du se [Foreta direkte leveringer](sales-how-drop-shipment.md). I alle andre henseender fungerer ordrer på samme måte som salgsfakturaer. Hvis du vil ha mer informasjon, kan du se [Fakturere salg](sales-how-invoice-sales.md).

Du kan forhandle med kunden ved først å opprette et tilbud, som du kan konvertere til en ordre når dere blir enige om salget. Hvis du vil ha mer informasjon, kan du se [Gi tilbud](sales-how-make-offers.md).

Etter at kunden har bekreftet avtalen, for eksempel etter en tilbudsprosess, kan du sende en ordrebekreftelse for å registrere din forpliktelse til å levere produktene som avtalt.

Når du leverer produkter, helt eller delvis, kan du bokføre ordren som levert eller som levert og fakturert for å opprette de beslektede vare- og kundepostene i systemet. Når du bokfører ordren, kan du også sende dokumentet som et PDF-vedlegg i e-post. Du kan få brødteksten i e-posten forhåndsutfylt med et sammendrag av ordren og betalingsinformasjonen, for eksempel en kobling til PayPal. Hvis du vil ha mer informasjon, kan du se [Sende dokumenter i e-post](ui-how-send-documents-email.md).

I forretningsmiljøer der kunden må betale før produkter leveres, for eksempel i detaljhandel, må du vente til mottak av betalingen før du leverer produktene. I de fleste tilfeller kan du behandle innkommende betalinger noen uker etter levering ved å utligne betalingene mot deres tilknyttede bokførte, ubetalte salgsfakturaer. Hvis du vil ha mer informasjon, kan du se [Avstemme betalinger ved hjelp av automatisk utligning](receivables-how-reconcile-payments-auto-application.md).

Hvis den bokførte salgsfakturaen er betalt, må du opprette en salgskreditnota for å reversere salget. Hvis du vil ha mer informasjon, kan du se [Behandle ordrereturer eller annulleringer](sales-how-process-sales-returns-cancellations.md).

Produkter kan være både varer og tjenester. Hvis du vil ha mer informasjon, kan du se [Registrere nye produkter](inventory-how-register-new-products.md). Ordreprosessen er den samme for begge produkttyper.

**Merk**: I Dynamics NAV brukes ordet “vare” for å referere til et produkt.

Du kan fylle kundefelt i ordren på to måter, avhengig av om kunden allerede er registrert.

## <a name="to-create-a-sales-order"></a>Opprette en ordre
1. Velg handlingen **Ordre** på Hjem-siden.  
2. I feltet **Kunde** angir du navnet på en eksisterende kunde.

    Andre felt i **Ordre**-vinduet fylles nå med standardinformasjon for den valgte kunden. Hvis kunden ikke er registrert, følger du denne fremgangsmåten:

3. I feltet **Kunde** angir du navnet på den nye kunden.
4. Klikk **Ja**-knappen i dialogboksen for å registrere den nye kunden.  
5. I vinduet **Velg en mal for en ny kunde** velger du en mal som du vil basere det nye kundekortet på, og deretter velger du **OK**-knappen.

    Det åpnes et nytt kundekort som er forhåndsutfylt med informasjon om den valgte kundemalen. **Navn**-feltet er forhåndsutfylt med det nye kundenavnet du skrev inn i salgsfakturaen i ordren.
6. Fortsette med å fylle ut resten av feltene på kundekortet. Hvis du vil ha mer informasjon, kan du se [Registrere nye kunder](sales-how-register-new-customers.md).  
7. Når du har fullført kundekortet, velger du **OK**-knappen for å gå tilbake til **Ordre** -vinduet.

    Flere felt i ordren er nå fylt ut med informasjon du har angitt på det nye kundekortet.
8. Fyll ut resten av feltene vinduet **Ordre** etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.

    Du kan nå begynne å fylle ut ordrelinjene med lagervarer eller tjenester du vil selge til kunden.

    Hvis du har definert gjentakende salgslinjer for kunden, for eksempel en månedlig etterfyllingsordre, kan du sette inn disse linjene på ordren ved å velge handlingen **Hent gjentakende salgslinjer**.
9. Angi nummeret på en vare eller tjeneste i **Vare**-feltet i hurtigfanen **Linjer**.  
10. I feltet **Antall** angir du hvor mange varer som skal selges.

    **Merk**: For varer av typen Tjeneste er antallet en tidsenhet, for eksempel timer, som angitt i feltet **Enhetskode** på linjen.

    Feltet **Linjebeløp** oppdateres for å vise verdien i feltet **Salgspris** multiplisert med verdien i feltet **Antall**.

    Prisen og linjebeløpene vises med eller uten mva, avhengig av hva du valgte i feltet **Priser inkludert merverdiavgift** på kundekortet.
11. I feltet **Linjerabatt-%** angir du en prosent hvis du vil gi kunden en rabatt på produktet. Verdien i feltet **Linjebeløp** oppdateres tilsvarende.

    Hvis du har konfigurert varepriser i hurtigfanen **Salgspriser og salgslinjerabatter** i kunde- eller varekortet, oppdateres prisen og beløpet på tilbudslinjen automatisk hvis de avtalte priskriteriene er oppfylt. Hvis du vil ha mer informasjon, kan du se [Registrere avtaler om salgspris, rabatt og betaling](sales-how-record-sales-price-discount-payment-agreements.md).
12. Hvis du vil legge til en kommentar om tilbudslinjen som kunden kan se på tilbudsutskriften, skriver du en tekst i **Beskrivelse**-feltet på en tom linje.  
13. Gjenta trinn 10 til 13 for hver vare som du vil tilby til kunden.

    Totaler under linjene beregnes automatisk når du oppretter eller endrer linjer.
14. I feltet **Fakturarabattbeløp** angir du et beløp som skal trekkes fra verdien som vises i feltet **Totalt inkl. mva.**.

    Hvis du har definert fakturarabatter for kunden, settes den angitte prosentverdien automatisk inn i feltet **Fakturarabatt %** hvis kriteriene er oppfylt, og det relaterte beløpet settes inn i feltet **Fakturarabattbeløp før mva.**. Hvis du vil ha mer informasjon, kan du se [Registrere avtaler om salgspris, rabatt og betaling](sales-how-record-sales-price-discount-payment-agreements.md).
15. Hvis du vi sende bare en del av ordreantallet, kan du angi antallet i den feltet **Levere (antall)**. Verdien kopieres til feltet **Fakturer (antall)**.
16. Hvis du vi fakturere bare en del av det sendte antallet, kan du angi antallet i den feltet **Fakturer (antall)**. Antallet må være lavere enn verdien i feltet **Levere (antall)**.   
17. Når ordrelinjene er fullført, kan du velge handlingen **Bokfør og send**.
Dialogboksen **Bokfør og send bekreftelse** åpnes, og viser den foretrukne sendemetoden for kunden.

Du kan endre sendemetoden ved å velge oppslagsknappen for feltet **Send dokument til**. Hvis du vil ha mer informasjon, kan du se [Definere en profil for dokumentsending](sales-how-setup-document-send-profiles.md).

Beslektet element og kundeposter opprettes nå i systemet, og ordren skrives ut som et PDF-dokument. Når ordren er fullstendig bokført, fjernes fra listen over ordrer og erstattes med nye dokumenter i listen over bokførte salgsfakturaer og oversikten over bokførte følgesedler.

## <a name="see-also"></a>Se også  
[Håndtere salg](sales-manage-sales.md)  
[Definere salg](sales-setup-sales.md)  
[Lager](inventory-manage-inventory.md)  
[Sende dokumenter i e-post](ui-how-send-documents-email.md)  
[Arbeide med Dynamics NAV](ui-work-product.md)

