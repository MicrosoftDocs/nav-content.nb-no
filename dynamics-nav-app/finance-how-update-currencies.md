---
title: Oppdatere valutakurser
description: Hvis du vil bruke flere valutaer i virksomheten, kan du definere en kode for hver valuta og bruke en ekstern valutakurstjeneste, for eksempel Yahoo.
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies, Yahoo
ms.date: 07/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 50603747629eee61f9bdaed900dcfc0dfc96ab3b
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-update-currency-exchange-rates"></a>Oppdatere valutakurser
Du må definere en kode for hver valuta du bruker hvis du kjøper eller selger i andre valutaer enn din lokale valuta, har kundekonti eller leverandørkonti i andre valutaer, eller registrerer finanstransaksjoner i forskjellige valutaer.  

Ettersom selskaper har drift i stadig flere land/regioner, blir det også stadig viktigere at de kan vurdere eller rapportere økonomien i mer enn én valuta. Programmet støtter bruk av flere valutaer. I programmet blir Finans definert ved hjelp av den lokale valutaen (NOK), og en annen valuta blir definert som tilleggsvaluta, med en tilordnet gjeldende valutakurs.  

 Når du angir en ny valuta som tilleggsrapporteringsvaluta, registrerer [!INCLUDE[d365fin](includes/d365fin_md.md)] beløp automatisk i både NOK og denne tilleggsrapporteringsvalutaen i alle finansposter og andre poster, for eksempel mva-poster. Når finanspostbeløp beregnes i en tilleggsrapporteringsvaluta, brukes informasjonen fra **Valutakurser**-vinduet til å finne den relevante valutakursen i programmet.  

> [!WARNING]  
>  Funksjonen for tilleggsrapporteringsvaluta må IKKE brukes som grunnlag for oversettelse av årsregnskap. Den er ikke et verktøy som kan utføre oversettelse av årsregnskap fra utenlandske datterselskaper som en del av en selskapskonsolidering. Funksjonen for tilleggsrapporteringsvaluta gir bare muligheten til å utarbeide rapporter i en annen valuta, som om denne valutaen var selskapets lokale valuta.

## <a name="adjusting-exchange-rates"></a>Justere valutakurser  
Ettersom valutakursene varierer konstant, må tilleggsvalutaangivelser i systemet justeres jevnlig. Hvis disse justeringene ikke utføres, kan beløp som er regnet om fra utenlandske valutaer (eller tilleggsvalutaer) og bokført i NOK i Finans, være villedende. I tillegg må daglige poster som bokføres før en daglig valutakurs angis i programmet, oppdateres etter at informasjonen om den daglige valutakursen er angitt. Kjørselen Juster valutakurser brukes til å justere valutakursene for bokførte kunde-, leverandør- og bankkontoposter. Den kan også oppdatere tilleggsrapporteringsvalutabeløp i finansposter.  

## <a name="displaying-reports-and-amounts-in-the-additional-reporting-currency"></a>Vise rapporter og beløp i tilleggsrapporteringsvalutaen  
Bruk av en tilleggsrapporteringsvaluta kan hjelpe rapporteringsprosessen for et selskap i følgende tilfeller:  

- Selskaper som ikke holder til i EU-land/-regioner, men som har transaksjoner som i stor grad foregår med selskaper i EU-land/-regioner. I dette tilfellet ønsker ikke-EU-selskapet kanskje også å rapportere i euro, slik at økonomirapportene gir større mening for handelspartnerne i EU.  

- Selskaper som også vil vise rapporter i en valuta som er mer brukt internasjonalt enn den lokale valutaen.  

Flere rapporter i Finans-modulen er basert på finansposter. Hvis du vil vise økonomidataene i rapporten i tilleggsrapporteringsvalutaen, merker du ganske enkelt av for **Vis beløp i tilleggsrapp.valuta** i det relevante finansrapportvinduet.  

## <a name="to-set-up-a-currency-exchange-rate-service"></a>Slik konfigurerer du en valutakurstjeneste
Du kan bruke en ekstern tjeneste for å holde valutakurser oppdatert. Tjenesten Yahoo-valutakurser er forhåndsinstallert og klar til å aktiveres.

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Valutakurstjenester**, og velg deretter den relaterte koblingen.
2. Velg handlingen **Ny**.
3. I vinduet **Valutakurstjeneste** fyller du ut feltene etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Merk av for **Aktivert** for å aktivere tjenesten.

## <a name="to-update-currency-exchange-rates-through-a-service"></a>Oppdatere valutakurser via en tjeneste
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Valutaer**, og velg deretter den relaterte koblingen.
2. Velg **Oppdater valutakurser**.

Verdien i **Valutakurs**-feltet i **Valutaer**-vinduet oppdateres med den nyeste valutakursen.

## <a name="see-also"></a>Se også
[Avslutte år og perioder](year-close-years-periods.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

