---
title: Designdetaljer - Prioritere ordrer
description: "Les mer om hvordan du prioriterer for å dekke både behov og forsyningskrav."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, priority, prioritize, order, sku, demand, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c01ad1bb74e01ff81f35159865eddf14e9a34910
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-prioritizing-orders"></a>Designdetaljer: Prioritere ordrer
I en gitt LFE representerer ønsket eller tilgjengelig dato den høyeste prioriteten. Behovet i dag bør håndteres før behovet i neste uke. I tillegg til denne generelle prioriteten vil planleggingssystemet også foreslå hvilken type behov som må være oppfylt før andre behov oppfylles. Det vil foreslå hvilken forsyningskilde som skal brukes før du bruker andre forsyningskilder. Dette gjøres i henhold til ordreprioriteter.  
  
Innlastet behov og forsyning bidrar til en profil for den beregnede beholdningen i henhold til følgende prioriteter:  
  
## <a name="priorities-on-the-demand-side"></a>Prioriteter på behovssiden  
1. Allerede levert: Varepost  
2. Bestillingsretur  
3. Ordre  
4. Serviceordre  
5. Produksjonskomponentbehov  
6. Monteringsordrelinje  
7. Utgående overføringsordre  
8. Rammebestilling (som ikke allerede er brukt av tilknyttede salgsordrer)  
9. Prognose (som ikke allerede er brukt av andre salgsordrer)  
  
> [!NOTE]  
>  Bestillingsreturer tas vanligvis ikke med i forsyningsplanlegging. De skal alltid reserveres fra partiet som skal returneres. Hvis den ikke er reservert, spiller bestillingsreturer en rolle i tilgjengeligheten og er høyt prioritert for å unngå at planleggingssystemet foreslår at en forsyningsordre bare skal fungere som en bestillingsretur.  
  
## <a name="priorities-on-the-supply-side"></a>Prioriteter på forsyningssiden  
1. Allerede på lager: Varepost (planleggingsfleksibilitet = ingen)  
2. Ordreretur (Planleggingsfleksibilitet = Ingen)  
3. Inngående overføringsordre  
4. Produksjonsordre  
5. Monteringsordre  
6. Bestilling  
  
## <a name="priority-related-to-the-state-of-demand-and-supply"></a>Prioritet som er knyttet til statusen for behov og forsyning  
I tillegg til prioriteter som er angitt av behov og forsyning, definerer den nåværende ordretilstanden i utføringsprosessen, en prioritet. Lageraktiviteter har for eksempel innvirkning, og det tas hensyn til statusen for salgs-, kjøps-, overførings-, monterings- og produksjonsordrer:  
  
1. Delvis behandlet (Planleggingsfleksibilitet = Ingen)  
2. Allerede i prosessen i lageret (planleggingsfleksibilitet = ingen)  
3. Frigitt – alle ordretyper (Planleggingsfleksibilitet = Ubegrenset)  
4. Fast planlagt produksjonsordre (planleggingsfleksibiliteten = ubegrenset)  
5. Planlagt/åpen – alle ordretyper (Planleggingsfleksibilitet = Ubegrenset)  
  
## <a name="see-also"></a>Se også  
[Designdetaljer: Balansere behov og forsyning](design-details-balancing-demand-and-supply.md)   
[Designdetaljer: Sentrale begreper for planleggingssystemet](design-details-central-concepts-of-the-planning-system.md)   
[Designdetaljer: Forsyningsplanlegging](design-details-supply-planning.md)
