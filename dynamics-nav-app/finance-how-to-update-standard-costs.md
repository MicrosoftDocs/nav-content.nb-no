---
title: Oppdatere standardkost
description: "Du må regelmessig oppdatere standardkostnadene for komponenter og opprullere de nye kostnadene til den overordnede varen."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/09/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: dd2bb16af611be7f7720fdf07eb65fd268aba039
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-update-standard-costs"></a>Oppdatere standardkost
Du må regelmessig oppdatere standardkostnadene for komponenter og opprullere de nye kostnadene til den overordnede varen. Prosessen består vanligvis av følgende fire trinn:  

1.  Oppdatere kost på komponent- og kapasitetsnivået. Hvis du vil ha mer informasjon, se kjørselen **Foreslå standardkost for vare**.  
2.  Konsolider og rull opp komponent- og kapasitetskost for å beregne samlet produksjons- eller monteringskost for varene.  
3.  Implementere standardkostnadene som angis når du kjører de forrige kjørslene. Standardkostnadene trer ikke i kraft før de blir implementert. Hvis du vil ha mer informasjon, se Implementer endringer i standardkost.  
4.  Implementere endringene for å oppdatere **Enhetskost**-feltet på varekortet og utføre revaluering av lager. Hvis du vil ha mer informasjon, kan du se [Revaluere beholdning](inventory-how-revalue-inventory.md).  

Hvis du vil ha mer informasjon, kan du se [Om beregning av standardkost](finance-about-calculating-standard-cost.md).  
## <a name="to-update-standard-costs"></a>Slik oppdaterer du standardkost  
1.  Kjør kjørselen **Juster kostverdi - vareposter**.  
2.  Kjør kjørselen **Bokfør lagerkost i Finans**.  
3.  Åpne **Standardkost - forslag**, og bruk én eller flere av følgende funksjoner:  

    1.  Kjør kjørselen **Foreslå standardkost for vare**.  
    2.  Gå gjennom resultatene, og foreta nødvendige endringer.  
    3.  Kjør kjørselen **Foreslå standardkost for kapasitet**.  
    4.  Gå gjennom resultatene, og foreta nødvendige endringer.
    5. Kjør kjørselen **Oppruller standardkost**.
    6.  Gå gjennom resultatene, og foreta nødvendige endringer.
    7.  Kjør kjørselen **Implementer endringer i standardkost**.  
4.  Gå gjennom og bokfør vinduet **Revalueringskladd**, som er fylt ut med poster fra tidligere trinn i denne fremgangsmåten.  

## <a name="see-also"></a>Se også  
 [Om beregning av standardkost](finance-about-calculating-standard-cost.md)   
 [Administrere lagerkostnader](finance-manage-inventory-costs.md)   
 [Designdetaljer: Kostmetoder](design-details-costing-methods.md) [[Finans](finance.md)  
 [Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

