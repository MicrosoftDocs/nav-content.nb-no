---
title: "Håndtere fordringer"
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
ms.openlocfilehash: 3f2be627dfda9720e9f31fd227164d1c27116d2c
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="manage-receivables"></a>Håndtere fordringer#
En sentral oppgave ved håndtering av kundekonto er å utligne inngående betalinger mot deres relaterte kunde- eller leverandørposter og dermed lukke de beslektede salgsfakturaene eller kjøpskreditnotaene som betalt. Når alle betalinger er utlignet, kan du avstemme bankkontoen.  

Du kan utføre denne oppgaven i vinduet **Betalingsavstemmingskladd** ved å importere en bankkontoutdragsfil eller feed for hurtig å registrere betalinger i Dynamics NAV. En funksjon for automatisk utligning utligner betalingene til deres tilknyttede åpne kunde- eller leverandørposter, basert på datasamsvar mellom betalingstekst og postinformasjonen. Du kan se gjennom og endre automatiske utligninger før du bokfører kladden. Du kan velge å lukke alle åpne bankposter relatert til de utlignede postene når du bokfører kladden. Dette betyr at bankkontoen avstemmes automatisk når alle betalinger er utlignet.

**Merk**: Du kan avstemme bankkonti som en separat oppgave i vinduet **Bankkontoavstemming**, som også støtter også sjekkposter. Hvis du vil ha mer informasjon, kan du se [Avstemme bankkonti separat](bank-how-reconcile-bank-accounts-separately.md).

Du kan også bruke betalinger i vinduet **Betalingsregistrering** ved manuelt å kontrollere betalinger mottatt som kontanter, sjekk eller banktransaksjon, mot en generert liste over ubetalte salgsdokumenter. Legg merke til at denne funksjonen bare er tilgjengelig for salgsdokumenter.

En annen metode for avstemming av betalinger er at du kan bokføre hvert mottak på relevante finans-, kunde- eller andre kontoer, ved å angi en betalingslinje i vinduet **Innbetalingskladd**. I så fall kan du bruke mottaket eller refundere til én eller flere åpne poster før du bokfører innbetalingskladden, eller du kan utligne fra de opprettede kundepostene.

En annen oppgave i håndtering av kundekonto er å samle utestående saldoer, inkludert å administrere rentenotaer og utstede purringer.

Tabellen nedenfor beskriver en sekvens av oppgaver, og har koblinger til emnene som beskriver dem.

|Hvis du vil |Se |
|---|----|
|Utligne betalinger mot åpne kunde- eller leverandørposter basert på en importert bankkontoutdragsfil eller -feed, og avstemme bankkontoen når alle betalingene er utlignet.|[Bruke betalinger automatisk og avstemme bankkonti](receivables-apply-payments-auto-reconcile-bank-accounts.md)|
|Utligne betalinger mot åpne kundeposter basert på manuell oppføring i en liste over ubetalte salgsdokumenter. | [Avstemme kundebetalinger manuelt fra en liste over ubetalte salgsdokumenter](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md)|
|Bokføre kontantmottak eller refusjoner for kunder i innbetalingskladden, og utligne mot kundeposter fra kladden eller bokførte poster. | [Avstemme kundebetalinger manuelt](receivables-how-apply-sales-transactions-manually.md) |
|Minne kundene om forfalte beløp, beregne rente og rentenotaer, og håndtere kortsiktige fordringer. | [Innkreve utestående saldi](receivables-collect-outstanding-balances.md) |

## <a name="see-also"></a>Se også
[Håndtere salg](sales-manage-sales.md)  
[Administrere skyldige beløp](payables-manage-payables.md)  
[Arbeide med Dynamics NAV](ui-work-product.md)  
[På tvers av forretningsområder](ui-across-business-areas.md)

