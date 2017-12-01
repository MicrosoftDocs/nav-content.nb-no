---
title: Bruke utvidelsen QuickBooks Datamigrering
description: "Beskriver hvordan du bruker utvidelsen til å overføre kunder, leverandører, varer og konti fra QuickBooks Online til Dynamics NAV."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, QuickBooks, import
ms.date: 05/24/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ff8f8f0c529966fc108d2d4c86e2d0681b1fc005
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---

# <a name="the-quickbooks-online-data-migration-extension-for-dynamics-nav"></a>Utvidelsen QuickBooks Online Datamigrering for Dynamics NAV
Utvidelsen er inkludert i den assisterte oppsettsveiledningen **Datamigrering** for å hjelpe deg å overføre viktige forretningsdata fra QuickBooks Online til [!INCLUDE[d365fin](includes/d365fin_md.md)]. Dette er for eksempel praktisk når virksomheten er i vekst og du har besluttet å oppgradere appen for forretningsdrift ved å begynne å bruke [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="what-data-can-i-import-from-quickbooks-online"></a>Hvilke data kan jeg importere fra QuickBooks Online?
Du kan importere følgende data fra QuickBooks Online til [!INCLUDE[d365fin](includes/d365fin_md.md)]:  

* Kunder
* Leverandører
* Varer
* Kontoplan 
* Startsaldotransaksjon i Finans
* Beholdningsantall for lagervarer
* Åpne dokumenter for kunder og leverandører, for eksempel fakturaer, kreditnotaer og betalinger

Vi overfører bare hele beløp på salgs- og kjøpsdokumenter. Vi oppdaterer ikke delvis betalte beløp. Hvis en kunde for eksempel har betalt 300 av totalt 500 kroner på en salgsfaktura, overfører vi hele beløpet på 500. Hvis du har mottatt delbetalinger, må du oppdatere disse manuelt før eller etter at du har overført data. Vi anbefaler at du utligner utestående transaksjoner før du overfører, bare for å gjøre ting enklere senere.

> [!NOTE]  
>   Vi overfører ikke bestillinger eller ordrer.

## <a name="before-you-start"></a>Før du begynner
En viktig del av overføringen er å angi kontiene som transaksjonene skal overføres til. Det er lurt å planlegge denne tilordningen før du overfører data. Kontiene der du for eksempel bokfører transaksjoner for følgende:  
  
* Salg av varer eller tjenestene til kunder.
* Kjøp av varer eller tjenester fra leverandører.  
* Justeringer i Finans.  

[!INCLUDE[d365fin](includes/d365fin_md.md)] krever at det er tilordnet kontonumre til finanskonti. Kontroller at kontonumre er tilordnet til kontiene i QuickBooks Online.

Hvis transaksjoner i QuickBooks Online har mva-beløp, må du definere en mva-konto for mva-jurisdiksjonene i [!INCLUDE[d365fin](includes/d365fin_md.md)] før du kan bokføre transaksjoner.

## <a name="how-do-i-start-using-the-extension"></a>Hvordan begynner jeg å bruke utvidelsen?
Det er enkelt å komme i gang. Alt du trenger å gjøre, er å kjøre den assisterte oppsettsveiledningen **Datamigrering**. Slik gjør du det:

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Assistert oppsett**, og velg deretter **Overfør forretningsdata**.
2. Følg instruksjonene for hvert trinn i den assisterte oppsettsveiledningen.

## <a name="what-do-i-do-after-i-migrate-data"></a>Hva gjør jeg etter at jeg har overført dataene?
Etter at du har overført dataene, har transaksjoner statusen **Ikke bokført**, slik at du kan se gjennom dem og foreta justeringer. Hvis du vil se gjennom transaksjonene, går du til siden der de vanligvis er. Hvis du for eksempel vil se gjennom ikke-bokførte salgsfakturaer, går du til siden **Salgsfakturaer**. Hvis du vil se gjennom utbetalingskladder, går du til siden **Utbetalingskladder**.   

Det er enkelte bestemte ting du bør gjøre:

* Hvis transaksjonene i QuickBooks Online hadde påslags- eller rabattbeløp, må du legge til beløpene manuelt i de relaterte transaksjonene i [!INCLUDE[d365fin](includes/d365fin_md.md)] før du bokfører dem.
* Hvis du bruker merverdiavgift (mva), må du kanskje legge til en bokføringsgruppe for firma og en varebokføringsgruppe i bokføringsoppsettet, slik at du kan bokføre mva-beløp.
* Kontroller startsaldoene for konti i Finans. QuickBooks Online lagrer ikke gjeldende saldo for alle konti, så du må kanskje rette startsaldoer.

## <a name="see-also"></a>Se også
[Importere forretningsdata fra andre økonomisystemer](upload-data.md)  
[Tilpasse [!INCLUDE[d365fin](includes/d365fin_md.md)] ved hjelp av utvidelser](ui-extensions.md)  

