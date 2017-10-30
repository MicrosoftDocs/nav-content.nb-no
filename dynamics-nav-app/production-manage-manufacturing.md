---
title: "Utføre produksjon"
description: "Når behov er planlagt og materialer er utstedt i henhold til produksjonsstykklistene, kan de faktiske produksjonsoperasjonene startes og kjøres i rekkefølgen definert i produksjonsordreruten."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/26/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 1d3e6b49626aaf60f398b9f9cf8a656bd3dc4946
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="manufacturing"></a>Produksjon
Når behov er planlagt og materialer er utstedt i henhold til produksjonsstykklistene, kan de faktiske produksjonsoperasjonene startes og kjøres i rekkefølgen definert i produksjonsordreruten.  

En viktig del av produksjonsutførelsen, sett fra systemets side, er å bokføre produksjonsavgang i databasen for å rapportere fremdrift, og å oppdatere beholdningen med de ferdige varene. Avgang kan bokføres manuelt ved å fylle ut og bokføre kladdelinjer etter produksjonsoperasjoner. Det kan også gjøres automatisk ved å bruke lagertrekk fremover. Materialforbruk blir da bokført automatisk samtidig med avgang når produksjonsordren endres til Ferdig.  

Som et alternativ til kladden for massebokføring av avgang for flere produksjonsordrer, kan du bruke **Produksjonskladd**-vinduet til å bokføre forbruk og/eller avgang for én produksjonsordrelinje.

Før du kan begynne å produsere varer, må du gjøre ulike oppsett, for eksempel arbeidssentre, ruter og produksjonsstykklister. Hvis du vil ha mer informasjon, kan du se [Definere produksjon](production-configure-production-processes.md).

Tabellen nedenfor beskriver en sekvens av oppgaver, og har koblinger til emnene som beskriver dem.   

|**Hvis du vil**|**Se**|  
|------------|-------------|  
|Forstå hvordan produksjonsordrer fungerer.|[Om produksjonsordrer](production-about-production-orders.md)|
|Opprett produksjonsordrer manuelt.|[Opprette produksjonsordrer](production-how-to-create-production-orders.md)|
|Sett ut alle eller utvalgte operasjoner i en produksjonsstykkliste til en underleverandør.|[Underleveranse av produksjon](production-how-to-subcontract-manufacturing.md)|
|Registrere og bokføre produksjonsavgang, i tillegg til material- og tidsforbruk, for én enkelt frigitt produksjonsordrelinje.|[Slik bokfører du forbruk og avgang for én frigitt produksjonsordrelinje](production-how-to-register-consumption-and-output.md)|  
|Massebokfør antall komponenter som brukes per operasjon i en kladd som kan behandle flere planlagte produksjonsordrer.|[Massebokføre forbruk](production-how-to-post-consumption.md)|
|Bokfør antall ferdigstilte varer og tiden som brukes per operasjon i en kladd som kan behandle flere frigitte produksjonsordrer.|[Slik: kjørselen Bokfør avgang og operasjonstid](production-how-to-post-output-quantity.md)|  
|Bokføre antallet varer som er produsert i hver fullført operasjon, og som ikke kvalifiserer som ferdigvare, men som vraket materiale.|[Slik bokfører du vrak](production-how-to-post-scrap.md)|
|Vise belastningen for produksjonen som et resultat av planlagte og frigitte produksjonsordrer.|[Vise belastning på arbeidssentre og produksjonsressurser](production-how-to-view-the-load-on-work-centers.md)|      
|Bruke **Kapasitetskladd**-vinduet til å bokføre brukt kapasitet som ikke er tilordnet til en produksjonsordre, for eksempel vedlikeholdsarbeid.|[Bokføre kapasiteter](production-how-to-post-capacities.md)|  
|Beregne og justere kost for ferdige produksjonsvarer og forbrukte komponenter for økonomisk avstemming.|[Om fullførte produksjonsordrekostnader](finance-about-finished-production-order-costs.md)|  

## <a name="see-also"></a>Se også  
[Definere produksjon](production-configure-production-processes.md)  
[Planlegging](production-planning.md)      
[Lager](inventory-manage-inventory.md)  
[Innkjøp](purchasing-manage-purchasing.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

