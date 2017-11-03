---
title: Forholdsmessig MVA
description: "Forbedringer i den norske versjonen gjør det mulig for deg å beregne MVA når både fradragsberettiget og ikke-fradragsberettiget MVA forekommer."
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
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 83aef795964ca7cec672c929b1f899aefd03d2e8
ms.contentlocale: nb-no
ms.lasthandoff: 10/26/2017

---
# <a name="proportional-vat"></a>Forholdsmessig MVA
[!INCLUDE[navnow](../../includes/navnow_md.md)] gjør det mulig for deg å beregne MVA når både fradragsberettiget og ikke-fradragsberettiget MVA forekommer. Siden det er vanskelig å vite hvor og hvordan varen blir brukt, må du ta kontakt med norske skattemyndigheter for å finne ut om en angitt prosentandel MVA kan gå til fradrag basert på historiske data.  

## <a name="example"></a>Eksempel  
Et busselskap eier både busser og lastebiler. Når det kjøpes inn bensin, blir denne lagret i én oppbevaringstank. Når bensinen brukes i en buss som transporterer barn, er den ikke fradragsberettiget. Når bensinen brukes i en lastebil, kan den være fradragsberettiget. Avtalen mellom selskapet og de norske skattemyndighetene kan for eksempel da være at 60 % av mva. går til fradrag.  

Hvis du har en kjøpsfaktura på USD 12 500,00 basert på 25 prosent mva., og **Ja** er angitt i **Beregn forholdsmessig fradrag** i vinduet **Mva-bokføringsoppsett** og feltet **Forholdsmessig fradrags-%** er satt til **60 prosent**, går bare 60 prosent av mva. til fradrag i en kladd. Når fakturaen er bokført, er posteringene som følger:  

- Til leverandøren finanskonto - USD 12 500 (kredit)  
- Til kostkonto 4010 - USD 11 000,00 (debet)  
- Til mva-konto 2720 - USD 1 500,00 (debet)  

Vanligvis ville mva-beløpet bli USD 2 500, basert på 25 prosent mv. Imidlertid går bare 60 prosent til fradrag; mva-beløpet er derfor USD 2 500 x 60 % = USD 1 500. Beløpet på USD 1 000 som ikke er fradragsberettiget, legges til på kostkontoen. Mva-grunnlaget har tilsvarende verdier. Dette beløpet skulle ha vært USD 10 000,00, men siden bare 60 prosent går til fradrag, er grunnlaget USD 6000,00.  

Dette vil også fungere hvis transaksjonen med denne mva-kombinasjonen bokføres via en bestilling.  

> [!NOTE]  
>  Hvis denne funksjonen brukes i en bestilling som brukes til innkjøp av varer til lager, har ikke funksjonen noen innvirkning på varekostnaden. Varekostnaden legges til gjennom ikke-fradragsberettiget mva. Dette er bare tilfelle i forbindelse med finans.  

## <a name="see-also"></a>Se også  
 [Beregne forholdsmessig MVA](how-to-calculate-proportional-vat.md)   
 [Norsk mva-rapportering](norwegian-vat-reporting.md)

