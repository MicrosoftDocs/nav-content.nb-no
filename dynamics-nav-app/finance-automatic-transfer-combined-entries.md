---
title: "Automatisk overføring og sammensatte poster"
description: "I kostnadsregnskap kan du overføre finansposter til en kosttype ved å bruke en kombinert bokføring. Du kan angi om en kosttype mottar kombinerte poster i feltet **Kombiner poster** i kosttypedefinisjonen. Tabellen nedenfor beskriver de ulike alternativene."
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
ms.openlocfilehash: 638fc123d4113695d70102a94b9fce0bff6b43fa
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="automatic-transfer-and-combined-entries"></a>Automatisk overføring og sammensatte poster
I kostnadsregnskap kan du overføre finansposter til en kosttype ved å bruke en kombinert bokføring. Du kan angi om en kosttype mottar kombinerte poster i feltet **Kombiner poster** i kosttypedefinisjonen. Tabellen nedenfor beskriver de ulike alternativene.  

|Kombiner poster|Beskrivelse|  
|---------------------|-----------------|  
|Ingen|Hver finanspost overføres individuelt til tilsvarende kosttype.|  
|Dag|Finansposter med samme bokføringsdato overføres som én post til tilsvarende kosttype.|  
|Måned|Alle finansposter som har samme kalendermåned, overføres som én post til den tilsvarende kosttypen.|  

> [!IMPORTANT]  
>  Hvis du har merket av for **Overfør automatisk fra Finans** i vinduet **Kostregnskapsoppsett**, oppdaterer [!INCLUDE[d365fin](includes/d365fin_md.md)] kostregnskapet etter hver bokføring i finans. Kombinerte poster er ikke mulig.  

## <a name="see-also"></a>Se også  
 [Overføre finansposter til kostposter](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md)   
 [Kriterier for overføring av finansposter til kostposter](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md)   
 [Resultater av overføringen](finance-results-of-the-transfer.md)   
 [Overføre og bokføre kostposter](finance-transfer-and-post-cost-entries.md)  
 [Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

