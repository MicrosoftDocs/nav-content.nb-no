---
title: "Designdetaljer - Holde seg under overflytnivået"
description: "Når Maks.ant. og Fast gjenbest.ant. brukes, fokuserer planleggingssystemet bare på den beregnede beholdningen i den angitte tidsperioden. Dette betyr at planleggingssystemet kan foreslå overflødig forsyning når endring av negativt behov eller positiv forsyning skjer utenfor den angitte tidsperioden."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: bd4d3a9abb6b13ba305abf8ad437294e94b67318
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-staying-under-the-overflow-level"></a>Designdetaljer: Holde seg under overflytnivået
Når Maks.ant. og Fast gjenbest.ant. brukes, fokuserer planleggingssystemet bare på den beregnede beholdningen i den angitte tidsperioden. Dette betyr at planleggingssystemet kan foreslå overflødig forsyning når endring av negativt behov eller positiv forsyning skjer utenfor den angitte tidsperioden. Hvis det derfor blir foreslått en overflødig forsyning, vil planleggingssystemet beregne antallet forsyningen skal reduseres til (eller slettes) for å unngå overflødig forsyning. Dette antallet kalles "overflyt nivået." Overflyt formidles som en planleggingslinje med handlingen **Endre ant. (reduksjon)** eller **Avbryt** og følgende advarsel:  

*Viktig: Den beregnede beholdningen [xx] er høyere enn overflytnivået [xx] på forfallsdatoen [xx].*  

![Lageroverflytnivå](media/supplyplanning_2_overflow1_new.png "supplyplanning_2_overflow1_new")  

##  <a name="calculating-the-overflow-level"></a>Beregne overflytnivået  
Overflytnivået beregnes på ulike måter avhengig av planleggingsoppsettet.  

### <a name="maximum-qty-reordering-policy"></a>Gjenbestillingsprinsippet Maks.ant  
Overflytnivå = Maks. beholdning  

> [!NOTE]  
>  Hvis det finnes et minimumsordreantall, blir det lagt til som følger: Overflytnivå = Maksimumsbeholdning + Min. bestillingsantall.  

### <a name="fixed-reorder-qty-reordering-policy"></a>Gjenbestillingsprinsippet for Fast gjenbest.ant.  
Overflytnivå = Gjenbestillingsantall + Gjenbestillingspunkt  

> [!NOTE]  
>  Hvis minimumsordreantallet er høyere enn gjenbestillingspunktet, vil dette erstatte slik: Overflytnivå = Gjenbestillingsantall + Min. bestillingsantall  

### <a name="order-multiple"></a>Bestillingsfaktor  
Hvis det finnes en bestillingsfaktor, vil den justere overflytnivået for gjenbestillingsprinsippene Maks.ant og Fast gjenbest.ant.  

##  <a name="creating-the-planning-line-with-overflow-warning"></a>Opprette planleggingslinjen med overflytadvarsel  
Når en eksisterende forsyning fører til at den beregnede beholdningen blir høyere enn overflytnivået på slutten av en tidsperiode, opprettes en planleggingslinje. For å advare om den potensielt overflødige forsyningen vises en advarsel på planleggingslinjen, feltet **Godta handlingsmelding** er ikke valgt og handlingsmeldingen er enten Avbryt eller Endre ant.  

### <a name="calculating-the-planning-line-quantity"></a>Beregne antall for planleggingslinjen  
Antall for planleggingslinje = Gjeldende forsyningsantall - (Beregnet beholdning – Overflytnivå)  

> [!NOTE]  
>  Som med alle advarselslinjer vil alle maksimum/minimum ordreantall eller bestillingsfaktor bli ignorert.  

### <a name="defining-the-action-message-type"></a>Angi handlingsmeldingstype  

-   Hvis planleggingslinjeantall er større enn 0, er handlingsmeldingen Endre ant.  
-   Hvis planleggingslinjeantall er lik eller mindre enn 0, er handlingsmeldingen Avbryt  

### <a name="composing-the-warning-message"></a>Skrive advarselsmeldingen  
Hvis det oppstår overflyt, viser vinduet **Ikke-sporede planleggingselementer** en advarsel med følgende informasjon:  

-   Det beregnede beholdningsnivået som utløste advarselen  
-   Det beregnede overflytnivået  
-   Forfallsdatoen for forsyningshendelsen.  

Eksempel: "Den beregnede beholdningen 120 er høyere enn overflytnivået 60 28.01.11."  

## <a name="scenario"></a>Scenario  
I dette scenariet endrer en kunde en ordre fra 70 til 40 enheter mellom to planleggingskjøringer. Overflytfunksjonen trer i kraft for å redusere kjøpet som ble foreslått for det første salgsantallet.  

### <a name="item-setup"></a>Vareoppsett  

|Gjenbestillingsprinsipp|Maks.ant.|  
|-----------------------|------------------|  
|Maks. bestillingsantall|100|  
|Gjenbestillingspunkt|50|  
|Beholdning|80|  

### <a name="situation-before-sales-decrease"></a>Situasjonen før salgsreduksjon  

|Hendelse|Endre ant.|Beregnet lager|  
|-----------|-----------------|-------------------------|  
|Dag én|Ingen|80|  
|Salg|-70|10|  
|Slutten av tidsperioden|Ingen|10|  
|Foreslå ny bestilling|+90|100|  

### <a name="situation-after-sales-decrease"></a>Situasjonen etter salgsreduksjon  

|Endre|Endre ant.|Beregnet lager|  
|------------|-----------------|-------------------------|  
|Dag én|Ingen|80|  
|Salg|-40|40|  
|Kjøp|+90|130|  
|Slutten av tidsperioden|Ingen|130|  
|Foreslå å redusere bestilling<br /><br /> ordre fra 90 til 60|-30|100|  

### <a name="resulting-planning-lines"></a>Resulterende planleggingslinjer  
 Én planleggingslinje (advarsel) blir opprettet for å redusere kjøpet med 30 fra 90 til 60, for å holde den beregnede beholdningen på 100 i henhold til overflytnivået.  

![Planlegg i henhold til overflytnivå](media/nav_app_supply_planning_2_overflow2.png "nav_app_supply_planning_2_overflow2")  

> [!NOTE]  
>  Uten overflytsfunksjonen vises det ingen advarsel hvis det beregnede beholdningsnivået er over maksimumsbeholdningen. Dette kan føre til en overflødig forsyning på 30.  

## <a name="see-also"></a>Se også  
[Designdetaljer: Gjenbestillingsprinsipper](design-details-reordering-policies.md)   
[Designdetaljer: Planleggingsparametere](design-details-planning-parameters.md)   
[Designdetaljer: Håndtere gjenbestillingsprinsipper](design-details-handling-reordering-policies.md)   
[Designdetaljer: Forsyningsplanlegging](design-details-supply-planning.md)

