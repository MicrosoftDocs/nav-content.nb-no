---
title: Salgs- og lagerprognose
author: edupont04
ms.custom: na
ms.date: 09/23/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 765527ed4f4800acec20f0abbd4374e95c9c36dc
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="sales-and-inventory-forecast-for-dynamics-nav"></a>Salgs- og lagerprognose for Dynamics NAV
Lagerstyring er en avveining mellom kundeservice og håndtering av kostnader. På den ene siden krever en lav beholdning mindre arbeidskapital, men på den annen side kan tomme lagre føre til tapt salg. Salgs- og lagerprognose-utvidelsen forutsier mulig salg ved hjelp av historiske data og gir en tydelig oversikt over forventet tomt lager. Basert på prognosen hjelper utvidelsen med å opprette etterfyllingsforespørsler til leverandørene og sparer deg for tid.  

## <a name="setting-up-forecasting"></a>Sette opp prognoser
I Dynamics NAV må du konfigurere tilkoblingen til Azure ML (Azure Machine Learning). Hvis du vil ha mer informasjon, kan du se [Registrere Dynamics NAV i Azure-administrasjonsportalen](ui-how-register-dynamics-nav-azure.md). Når du har opprette tilkoblingen, kan du konfigurere prognosen til å bruke en annen type periode å rapportere etter, for eksempel endre fra prognose etter måned til prognose etter kvartal. Du kan også velge antall perioder som prognosene skal beregnes for, avhengig av hvor detaljert du vil at prognosen skal være. Vi foreslår at du lager månedlige prognoser, og med en 12 måneders horisont for prognosen.  

## <a name="using-the-forecasts"></a>Bruke prognosene
Utvidelsen bruker Azure ML-funksjoner for å forutse fremtidige salg basert på din salgshistorikk for å unngå for liten lagerbeholdning. Når du for eksempel velger en vare i **Varer**-vinduet, viser diagrammet i **Vareprognose**-ruten beregnet salg av denne varen i den kommende perioden. På denne måten kan du se om det er sannsynlig at du snart går tom for varen på lageret.  

Du kan også bruke utvidelsen til å foreslå når lageret bør fylles på. Hvis du for eksempel oppretter en bestilling for Fabrikam fordi du vil kjøpe deres nye skrivebordsstol, foreslår Salgs- og lagerprognose-utvidelsen at du også fyller på med LONDON-svingstolen som du vanligvis kjøper fra denne leverandøren. Dette er fordi utvidelsen forutsier at du vil gå tom for LONDON-svingstolen i løpet av de neste to månedene, og at du kanskje vil bestille flere stoler allerede nå.  

## <a name="see-also"></a>Se også
[Håndtere salg](sales-manage-sales.md)  
[Håndtere lager](inventory-manage-inventory.md)  
[Tilpasse Dynamics NAV ved hjelp av utvidelser](ui-extensions.md)  
[Registrere Dynamics NAV i Azure-administrasjonsportalen](ui-how-register-dynamics-nav-azure.md)  

