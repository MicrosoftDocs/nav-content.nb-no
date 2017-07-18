---
title: "Administrere skyldige beløp"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 50a68e1eaf0d6057420635f85b473639e39caa5a
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="manage-payables"></a>Administrere skyldige beløp
Det er en sentral aktivitet i håndtering av leverandørgjeld å betale leverandører. Du kan bruke funksjoner til å automatisk fylle ut vinduet **Betalingskladd** med betalingslinjer for forfalte kjøpsfakturaer. Hvis du raskt vil utføre involvert banktransaksjoner, kan du eksportere flere betalingskladdelinjer til en fil, som du deretter laste opp til banken for behandling. Du kan også betale med sjekk, inkludert å overføre sjekker som elektroniske betalinger.

En annen vanlig oppgave er å utligne utgående betalinger mot deres relaterte leverandørposter og dermed lukke de beslektede kjøpsfakturaene eller kjøpskreditnotaene som betalt. Du kan utføre dette arbeidet i vinduet **Betalingsavstemmingskladd** ved å importere en bankkontoutdragsfil for hurtig å registrere betalinger i Dynamics NAV. En funksjon for automatisk utligning utligner betalingene til deres tilknyttede åpne leverandør- eller kundeposter, basert på datasamsvar mellom betalingstekst og postinformasjonen. Du kan bruke ulike funksjoner til å se gjennom og endre automatiske utligninger før du bokfører kladden. Du kan velge å lukke alle åpne bankposter relatert til de utlignede postene når du bokfører kladden. Dette betyr at bankkontoen avstemmes automatisk når alle betalinger er utlignet.

Du kan også bruke utgående betalinger manuelt i vinduet **Betalingskladd** eller fra de relaterte leverandørpostene.

Tabellen nedenfor beskriver en sekvens av oppgaver i leverandørgjeld, og har koblinger til emnene som beskriver dem.

|Hvis du vil |Se |
|---|----|
|Generere forfalte leverandørbetalinger prioritert i henhold til kontantrabatter og forfalte straffegebyrer. Du kan også eksportere betalingene til en bankfil ved bokføring.|[Foreta betalinger](payables-make-payments.md)|
|Utligne leverandørbetalinger automatisk på ubetalte kjøpsfakturaer ved å importere en bankkontoutdragsfil.|[Bruke betalinger automatisk og avstemme bankkonti](receivables-apply-payments-auto-reconcile-bank-accounts.md)|
|Utligne leverandørbetalinger på ubetalte fakturaer manuelt.|[Utligne leverandørbetalinger manuelt](payables-how-apply-purchase-transactions-manually.md)|

## <a name="see-also"></a>Se også
[Håndtere kjøp](purchasing-manage-purchasing.md)  
[Håndtere fordringer](receivables-manage-receivables.md)  
[Arbeide med Dynamics NAV](ui-work-product.md)  
[På tvers av forretningsområder](ui-across-business-areas.md)

