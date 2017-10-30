---
title: "Definere fordelingskilde og -mål"
description: "Hver fordeling består av en fordelingskilde og ett eller flere fordelingsmål. Fordelingskilden fastsetter hvilke kostnader som blir fordelt. Fordelingsmålene fastsetter hvor kostnadene skal fordeles."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 91adabefc3e0b4a69b24b34a084f89c17711d573
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-allocation-source-and-targets"></a>Definere fordelingskilde og -mål
Hver fordeling består av en fordelingskilde og ett eller flere fordelingsmål. Fordelingskilden fastsetter hvilke kostnader som blir fordelt. Fordelingsmålene fastsetter hvor kostnadene skal fordeles.  

## <a name="to-set-up-cost-allocations"></a>Definere kostfordelinger  
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Kostfordeling**, og velg deretter den relaterte koblingen.  
2.  I vinduet **Kostfordeling** velger du **Rediger**.  
3.  Angi en ID for fordelingskilde i **ID**-feltet.  
4.  Definer et nivå som et tall mellom 1 og 99 i **Nivå**-feltet. Fordelingsbokføringen vil følge rekkefølgen på nivåene.  
5.  Angi en kosttype for å definere hvilke kosttyper som skal fordeles, i feltet **Kosttypeområde**. Hvis all kost for en kosttype fordeles, defineres ikke område.  
6.  Angi et kostsenter sammen med kostnadene skal fordeles, i feltet **Kostsenterkode**.  
7.  Angi et kostobjekt sammen med kostnadene skal fordeles, i feltet **Kostobjektkode**. Feltet blir som oftest stående tomt, fordi kostobjekter sjelden fordeles på andre kostobjekter.  
8.  Angi en kosttype feltet **Krediter til kosttype**. Fordelt kost krediteres til kildekosttypen. Kreditposten bokføres til kostnadstypen som er gitt her.  
9. På hurtigfanen **Linjer** definerer du tildelingsmålene. På den første linjen angir du en kosttype i feltet **Målkosttype**. Det definerer hvilken kosttype fordelingen debiteres.  
10. På den første linjen angir du første fordelingsmålet i feltet **Målkostsenter** eller **Målkostobjekt**. Disse to feltene definerer hvilket kostsenter eller kostobjekt fordelingen debiteres til. Du kan bare fylle ut ett av disse feltene, og ikke begge.  
11. Gjenta de samme trinnene på den andre linjen for å definere ytterligere fordelingsmål.  
12. Når du har satt opp fordelingsmål og -kilder, velger du **Beregn fordelingsnøkkel** for å beregne totale andelsverdier.  

> [!NOTE]  
>  Merk av for **Blokkert** for å deaktivere tildelingsoppsettet.  

## <a name="see-also"></a>Se også  
[Gjøre rede for kostnader](finance-manage-cost-accounting.md)  
 [Angi filtre for dynamisk fordelingsgrunnlag](finance-setting-filters-for-dynamic-allocation-bases.md)   
 [Eksempelscenario: Definere statiske fordelinger basert på fordelingsgrad](finance-scenario-example-defining-static-allocations-based-on-allocation-ratio.md)   
 [Eksempelscenario: Definere dynamiske fordelinger basert på solgte varer](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md)   
 [Definere og fordele kostnader](finance-define-and-allocate-costs.md)   
 [Terminologi i kostregnskap](finance-terminology-in-cost-accounting.md)  
 [Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

