---
title: Lagrede innstillinger i rapporter
author: jswymer
ms.custom: na
ms.date: 09/26/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 0f11d862315c8ecd160cd18afb0a72a2d684b9b2
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---
# <a name="saved-settings-on-reports"></a>Lagrede innstillinger i rapporter
Avhengig av hvilken rapport som skal kjøres, kan det vises en side som lar deg angi bestemte alternativer og filtre for å endre dataene som er inkludert i den genererte rapporten. Denne siden kalles rapportforespørselssiden. En rapport kan inneholde en eller flere *lagrede innstillinger* som du kan bruke på rapporten fra forespørselssiden. *Lagrede innstillinger* er i hovedsak forhåndsdefinerte alternativer og filtre. Lagrede innstillinger er en rask og pålitelig metode for å generere konsekvent rapporter som inneholder de riktige dataene.

Du kan se de lagrede innstillingene som er tilgjengelige for en rapport i delen **Lagrede innstillinger** i rapportforespørselssiden.

## <a name="to-apply-saved-settings-to-a-report"></a>Slik bruker du lagrede innstillinger på en rapport
1.  Åpne rapporten.

    Rapportforespørselssiden vises.    
2.  I delen **Lagrede innstillinger** på siden, setter du **Navn**-feltet til de lagrede innstillingene du vil bruke.

    Delen **Lagrede innstillinger** vises bare hvis rapporten er kjørt tidligere eller hvis det finnes eksisterende oppføringer for lagrede innstillinger. Oppføringen med lagrede innstillinger, som kalles **Sist brukte alternativer og filtre**, er alltid tilgjengelig. Disse innstillingene er verdiene for alternativet og filteret som ble brukt sist gang du kjørte rapporten.

## <a name="administer-saved-report-settings-for-users"></a>Administrere lagrede rapportinnstillinger for brukere
Hvis du har riktige tillatelser, kan du vise, opprette og endre de lagrede innstillingene for alle rapporter for alle brukere i firmaet. Du kan tilordne lagrede innstillingene for en rapport til enkeltbrukere eller alle brukerne i firmaet.

Du kan administrere lagrede innstillinger fra siden 1506 **Rapportinnstillinger**. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Rapportinnstillinger** og velger deretter den relaterte koblingen for å åpne denne siden. 

Fra siden **Rapportinnstillinger** kan du opprette en ny innstillinger fra bunnen av eller du kan kopiere og endre eksisterende innstillinger. Hvis du vil endre alternativer og filtre for en innstillingene, velger du **Rediger**-handling.

**Merknader**:
-    Funksjonen for lagrede innstillinger i rapporter gjelder bare når SaveValues-egenskapen for forespørselssiden er satt til Ja. SaveValues-egenskapen angis i utviklingsmiljøet.
-    Hvis du oppretter et element for lagrede innstillinger for alle brukere, og det har samme navn som eksisterende lagrede innstillinger for en bestemt bruker, kan ikke brukeren bruke de lagrede innstillingene som er tilordnet til alle.  I feltet Lagrede innstillinger på rapportforespørselssiden, vil brukeren se to lagrede innstillingsalternativer med samme navn. Uansett hvilket alternativ som velges, vil imidlertid de brukerspesifikke lagrede innstillingene bli brukt.

## <a name="see-also"></a>Se også
[Planlegge en rapport for kjøring](ui-schedule-report.md)

