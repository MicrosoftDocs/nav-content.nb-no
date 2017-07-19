---
title: Definere eller endre kontoplanen
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 48cd91958545b40b2ab0c5e48442fc874845af5b
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="set-up-or-change-the-chart-of-accounts"></a>Definere eller endre kontoplanen
Kontoplanen viser finanskontoene som lagrer dine økonomiske data. Dynamics NAV inneholder en standard kontoplan som er klar til å støtte forretningsvirksomheten din.
Du kan imidlertid endre standardkontoene, og du kan legge til nye kontoer.  

## <a name="adding-or-changing-accounts"></a>Legge til eller endre kontoer
For hver kontoplan kan du åpne finanskontoen og legge til eller endre innstillinger.

**Merk**: Du kan slette en finanskonto. Før du sletter den, må imidlertid følgende være oppfylt:  
- Saldo på kontoen må være null.  
- Feltet **Tillat sletting av finanskto. før** må være satt i vinduet **Finansoppsett**, og kontoen kan ikke ha finansposter på eller etter denne datoen.  
- Hvis feltet **Kontroller finanskontobruk** er valgt i vinduet **Finansoppsett**, må ikke kontoen brukes i bokføringsgrupper eller bokføringsoppsett.  

Dynamics NAV hindrer deg i å slette en finanskonto som lagrer data som er nødvendige i kontoplanen.  

##<a name="see-also"></a>Se også  
[Økonomimodulen og kontoplanen](finance-setup-general-ledger.md)  
[Håndtere bankkonti](bank-manage-bank-accounts.md)  
[Dimensjoner](finance-setup-dimensions.md)  
[Arbeide med GIFI-koder i Canada](ca-finance-setup-work-GiFI-codes.md)

