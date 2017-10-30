---
title: "Slik massebokfører du produksjonsavgang og operasjonstider"
description: Avgangsantallet representerer arbeidsframdriften i form av det ferdige antallet.
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
ms.openlocfilehash: 266c3f52dda22133acebf6052326ab57551b2ec0
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-batch-post-output-and-run-times"></a>Slik: kjørselen Bokfør avgang og operasjonstid
Avgangsantallet representerer arbeidsframdriften i form av det ferdige antallet.  

> [!NOTE]
> Bare når du bokfører avgangsantall i den siste operasjonen, oppdateres beholdningen automatisk.  

## <a name="to-post-output-quantities-for-one-or-more-production-order-lines"></a>Slik bokfører du avgangsantall for en eller flere produksjonsordrelinjer
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Ferdigmeldingskladd**, og velg deretter den relaterte koblingen.  
2. Fyll ut feltene med produksjonsordre- og avgangsdata. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Hvis operasjonen er fullført, velger du **Ferdig**-feltet.  

    Hvis lagerlokasjonen der varene skal plasseres bruker hyller, men ikke krever plasseringsbehandling,  tildeler du en hyllekode til kladdelinjen for å angi hvor varene skal lagres på lageret Hvis du vil ha mer informasjon, kan du se [Plassere produksjonsavgang eller monteringsavgang](warehouse-how-to-put-away-production-output.md).  

4. Velg **Bokfør** for å bokføre operasjonene. Avgangsantallet bokføres. Varen kan nå leveres.  

## <a name="to-post-run-times-for-one-or-more-production-order-lines"></a>Slik bokfører du kjøretid for en eller flere produksjonsordrelinjer
Operasjonstiden representerer arbeidsframdrift i form av nødvendig arbeidstid.    

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Ferdigmeldingskladd**, og velg deretter den relaterte koblingen.  
2. Fyll ut feltene med produksjonsordre- og avgangsdata.  
3.  Hvis operasjonen er fullført, velger du **Ferdig**-feltet.  
4. Velg **Bokfør**-handlingen for å bokføre tiden som brukes per operasjon. Kapasitetsposter oppdateres for brukte arbeids- eller produksjonsressurser.

## <a name="see-also"></a>Se også  
[Produksjon](production-manage-manufacturing.md)    
[Definere produksjon](production-configure-production-processes.md)  
[Planlegging](production-planning.md)      
[Lager](inventory-manage-inventory.md)  
[Innkjøp](purchasing-manage-purchasing.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

