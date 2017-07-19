---
title: Angi skrivervalg for rapporter
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 55b48aef2bc108ced7f581f0ff6c11263ee467df
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---
    
# <a name="specify-printer-selection-for-reports"></a>Angi skrivervalg for rapporter
Du kan definere rapporter slik at de må skrives ut på en bestemt skriver. Her er noen av bruksområdene for skrivervalg: 

- Du kan skrive ut rapporter på papir med et spesielt brevhode for selskapet.
- Du kan skrive ut rapporter på ulike papirstørrelser.
- Du kan skrive ut rapporter på standardskriveren for en bestemt ansatt.

Du bruker vinduet **Skrivervalg** til å angi ulike verdier for å få forskjellig utskrift. Hvis du angir et bestemt skrivervalg, har dette forrang over et mer generelt skrivervalg. Du kan for eksempel angi et skrivervalg som har verdier i feltene **Bruker-ID**, **Rapport-ID** og **Skrivernavn**. Dette skrivervalget overstyrer skrivervalget som har tomme oppføringer i **Bruker-ID**- eller **Rapport-ID**-feltet. 

Tabellen nedenfor beskriver kombinasjonen av verdier som må angis når du konfigurerer skrivervalg for en rapport.

|Hvis du vil                                                 |Angi følgende verdier                                             |
|---------------------------------------------------|---------------------------------------------------------------------|
|Skrive ut en rapport på en bestemt skriver for alle brukere |Angi verdier i feltene **Rapport-ID** og **Skrivernavn**, og la **Bruker-ID**-feltet stå tomt.|
|Skrive ut alle rapporter på en bestemt skriver til en bestemt bruker|Angi verdier i feltene **Bruker-ID** og **Skrivernavn**, og la **Rapport-ID**-feltet stå tomt.|
|Angi standardskriver for alle rapporter|Angi en verdi i **Skrivernavn**-feltet, og la feltene **Bruker-ID** og **Rapport-ID** stå tomme.|
|Skrive ut en bestemt rapport på brukerens standardskriver|Angi en verdi i **Rapport-ID**-feltet, og la feltene **Skrivernavn** og **Bruker-ID** stå tomme.|
|Skrive ut en bestemt rapport på en bestemt skriver til en bestemt bruker|Angi verdier i alle tre feltene.|

## <a name="see-also"></a>Se også
[Arbeide med Dynamics NAV](ui-work-product.md)

