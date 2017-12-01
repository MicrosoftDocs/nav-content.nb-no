---
title: Opprett en salgsfaktura eller ordre
description: "Beskriver hvordan du oppretter en sluttseddel, eller en salgsfaktura eller ordre, for å registrere avtalen med en kunde om å selge produkter i samsvar med bestemte betingelser."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bill, sale, invoice, order
ms.date: 10/11/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7da07d1491fde4e555ea259f61babc02664094a8
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-invoice-sales"></a>Fakturere salg
Du kan opprette en salgsfaktura eller ordre for å registrere avtalen med en kunde om å selge bestemte produkter på bestemte leverings- og betalingsbetingelser.  

Det er et par scenarier der du må bruke en ordre i stedet for en salgsfaktura:  

* Hvis du trenger å levere bare en del av en bestillingsantall, for eksempel fordi det fullstendige antallet ikke er på lager.  
* Hvis du selger varer som leverandøren gir deg direkte til kunden, kjent som direkte levering. Hvis du vil ha mer informasjon, kan du se [Foreta direkte leveringer](sales-how-drop-shipment.md).  

I alle andre henseender fungerer ordrer og salgsfakturaer på samme måte. Hvis du vil ha mer informasjon, kan du se [Selge produkter](sales-how-sell-products.md).

Du kan forhandle med kunden ved først å opprette et tilbud, som du kan konvertere til en salgsfaktura når dere blir enige om salget. Hvis du vil ha mer informasjon, kan du se [Gi tilbud](sales-how-make-offers.md).

Hvis kunden bestemmer seg for å kjøpe, kan du bokføre salgsfaktura for å lage relaterte antall og verdiposter. Når du bokfører salgsfakturaen, kan du også sende dokumentet som et PDF-vedlegg i e-post. Du kan få brødteksten i e-posten forhåndsutfylt med et sammendrag av fakturaen og betalingsinformasjonen, for eksempel en kobling til PayPal. Hvis du vil ha mer informasjon, kan du se [Sende dokumenter i e-post](ui-how-send-documents-email.md).

I forretningsmiljøer der kunden må betale før produkter leveres, for eksempel i detaljhandel, må du vente til mottak av betalingen før du leverer produktene. I de fleste tilfeller kan du behandle innkommende betalinger noen uker etter levering ved å utligne betalingene mot deres tilknyttede bokførte, ubetalte salgsfakturaer. Hvis du vil ha mer informasjon, kan du se [Avstemme betalinger ved hjelp av automatisk utligning](receivables-how-reconcile-payments-auto-application.md).

Du kan enkelt korrigere eller annullere en bokført salgsfaktura før den er betalt. Dette er for eksempel praktisk hvis du vil rette en skrivefeil, eller hvis kunden ber om en endring tidlig i ordreprosessen. Hvis du vil ha mer informasjon, kan du se [Korrigere eller annullere ubetalte salgsfakturaer](sales-how-correct-cancel-sales-invoice.md). Hvis den bokførte salgsfakturaen er betalt, må du opprette en salgskreditnota for å reversere salget. Hvis du vil ha mer informasjon, kan du se [Behandle ordrereturer eller annulleringer](sales-how-process-sales-returns-cancellations.md).

Du kan fylle kundefelt i salgsfakturaen på to måter, avhengig av om kunden allerede er registrert. Se trinn 2 og 3 i fremgangsmåten nedenfor.

## <a name="to-create-a-sales-invoice"></a>Slik oppretter du en salgsfaktura
1. Velg handlingen **Salgsfaktura** på Hjem-siden.  
2. I feltet **Kunde** angir du navnet på en eksisterende kunde.

   Andre felt i **Salgsfaktura**-vinduet inneholder nå standardinformasjon for den valgte kunden. Hvis kunden ikke er registrert, følger du denne fremgangsmåten:
3. I feltet **Kunde** angir du navnet på den nye kunden.
4. Klikk **Ja**-knappen i dialogboksen for å registrere den nye kunden.
5. I vinduet **Velg en mal for en ny kunde** velger du en mal som du vil basere det nye kundekortet på, og deretter velger du **OK**-knappen.
6. Det åpnes et nytt kundekort som viser informasjon om den valgte kundemalen. Fyll ut feltene som gjenstår. Hvis du vil ha mer informasjon, kan du se [Registrere nye kunder](sales-how-register-new-customers.md).  
7. Når du har fullført kundekortet, velger du **OK**-knappen for å gå tilbake til **Salgsfaktura** -vinduet.

   Flere felt i salgsfakturen er nå fylt ut med informasjon du har angitt på det nye kundekortet.  
8. Fyll ut resten av feltene vinduet **Salgsfaktura** etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

Du er nå klar til å fylle ut linjene salgsfaktura for produktene du selger til kunden eller for noen transaksjon med kunden som du vil registrere i en finanskonto.   

Hvis du har definert gjentakende salgslinjer for kunden, for eksempel en månedlig etterfyllingsordre, kan du sette inn disse linjene på ordren ved å velge handlingen **Hent gjentakende salgslinjer**.  
9. På **Linjer**-hurtigfanen i **Type**-feltet velger du typen produkt, tillegg eller transaksjon som du vil legge til for kunden med salgslinjen.
10. I **Nr.** velger du en post skal bokføres, i henhold til verdien i **Type**-feltet.

 La feltet **Nr.** stå tomt i følgende tilfeller: – Hvis linjen er for en kommentar. Skriv inn kommentaren i **Beskrivelse**-feltet.
 - Hvis linjen er for en katalogvare. Velg handlingen **Velg katalogvarer**. Hvis du vil ha mer informasjon, kan du se [Arbeide med katalogvarer](inventory-how-work-nonstock-items.md).

11. I **Antall**-feltet angir du hvor mange enheter av produktet, gebyret eller transaksjonen som linjen skal registrere for kunden.  

    Verdien i **Linjebeløp**-feltet beregnes som *salgspris* x *antall*.  

    Prisen og linjebeløpene er med eller uten mva, avhengig av hva du valgte i feltet **Priser inkludert merverdiavgift** på kundekortet.  
12. Hvis du vil gi en rabatt, skriver du inn en prosentandel i feltet **Linjerabatt-%**. Verdien i feltet **Linjebeløp** oppdateres tilsvarende.  

    Hvis du har konfigurert varepriser i hurtigfanen **Salgspriser og salgslinjerabatter** i kunde- eller varekortet, oppdateres prisen og beløpet på salgslinjen automatisk hvis de avtalte priskriteriene er oppfylt. Hvis du vil ha mer informasjon, kan du se [Registrere avtaler om salgspris, rabatt og betaling](sales-how-record-sales-price-discount-payment-agreements.md).  
13. Gjenta trinn 9 til 12 for hver hvert produkt eller gebyr som du vil selge til kunden.  

    Totaler under linjene beregnes automatisk når du oppretter eller endrer linjer.  
14. I feltet **Fakturarabattbeløp** angir du et beløp som skal trekkes fra verdien som vises i feltet **Totalt inkl. mva.**.

    Hvis du har definert fakturarabatter for kunden, settes den angitte prosentverdien automatisk inn i feltet **Fakturarabatt %** hvis kriteriene er oppfylt, og det relaterte beløpet settes inn i feltet **Fakturarabattbeløp før mva.**. Hvis du vil ha mer informasjon, kan du se [Registrere avtaler om salgspris, rabatt og betaling](sales-how-record-sales-price-discount-payment-agreements.md).  
15. Når salgsfakturalinjene er fullført, kan du velge handlingen **Bokfør og send**.  

Dialogboksen **Bokfør og send bekreftelse** viser kundens foretrukne metode for mottak av dokumenter. Du kan endre sendemetoden ved å velge oppslagsknappen for feltet **Send dokument til**. Hvis du vil ha mer informasjon, kan du se [Definere en profil for dokumentsending](sales-how-setup-document-send-profiles.md).

Beslektet element og kundeposter opprettes nå i systemet, og salgsfakturaen skrives ut som et PDF-dokument. Salgsfakturaen fjernes fra listen over salgsfakturaer og erstattes med et nytt dokument i listen over bokførte salgsfakturaer.

## <a name="see-also"></a>Se også
[Salg](sales-manage-sales.md)  
[Sette opp salg](sales-setup-sales.md)  
[Lager](inventory-manage-inventory.md)  
[Sende dokumenter i e-post](ui-how-send-documents-email.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

