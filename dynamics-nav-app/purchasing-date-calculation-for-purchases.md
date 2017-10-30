---
title: "Beregne dato for kjøp"
description: "Programmet beregner automatisk datoen du må bestille en vare på for å ha den på lager på en bestemt dato. Dette er datoen da du kan forvente at varer som ble bestilt på en bestemt dato, vil være tilgjengelig for plukking."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/10/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3f3f87311f0971b2901852a9aa0c766c6c806190
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="date-calculation-for-purchases"></a>Beregne dato for kjøp
[!INCLUDE[d365fin](includes/d365fin_md.md)] beregner automatisk datoen du må bestille en vare på for å ha den på lager på en bestemt dato. Dette er datoen da du kan forvente at varer som ble bestilt på en bestemt dato, vil være tilgjengelig for plukking.  

Hvis du angir en ønsket mottaksdato på et bestillingshode, er den beregnede bestillingsdatoen datoen bestillingen må foretas for at du skal kunne motta varene på ønsket dato. Deretter beregnes datoen da varene er tilgjengelige for plukking, og denne angis i feltet **Forventet mottaksdato**.  

Hvis du ikke angir en ønsket mottaksdato, brukes bestillingsdatoen på linjen som utgangspunkt for beregning av datoen du kan forvente å motta varene på, samt datoen som varene er tilgjengelige for plukking på.  

## <a name="calculating-with-a-requested-receipt-date"></a>Beregne med en ønsket mottaksdato  
Hvis det finnes en ønsket mottaksdato på bestillingslinjen, brukes denne datoen som utgangspunkt for følgende beregninger.  

- ønsket mottaksdato - beregning av leveringstid = bestillingsdato  
- ønsket mottaksdato + inngående lagerhåndteringstid + sikkerhetsleveringstid = forventet mottaksdato  

Hvis du angir en ønsket mottaksdato i bestillingshodet, kopieres denne datoen til tilsvarende felt på alle linjene. Du kan endre denne datoen på hvilken som helst av linjene, eller du kan fjerne datoen fra linjen.  

## <a name="calculating-without-a-requested-delivery-date"></a>Beregne uten en ønsket leveringsdato  
Hvis du angir en bestillingslinje uten en ønsket leveringsdato, fylles feltet **Ordredato** på linjen ut med datoen i feltet **Ordredato** i bestillingshodet. Dette er enten den angitte datoen eller arbeidsdatoen. Følgende datoer beregnes deretter for bestillingslinjen, med utgangspunkt i bestillingsdatoen.  

- bestillingsdato + beregning av leveringstid = planlagt mottaksdato  
- planlagt mottaksdato + inngående lagerhåndteringstid + sikkerhetsleveringstid = forventet mottaksdato  

Hvis du endrer bestillingsdatoen på linjen, som når varene ikke er tilgjengelige hos leverandøren før på en senere dato, beregner de aktuelle datoene på linjen automatisk på nytt.  

Hvis du endrer bestillingsdatoen i hodet, så kopieres denne datoen til feltet **Ordredato** på alle linjene, og alle de aktuelle datofeltene beregnes deretter på nytt.  

## <a name="see-also"></a>Se også  
 [Beregne dato for salg](sales-date-calculation-for-sales.md)   
 [Beregne ordrebekreftelsesdatoer](sales-how-to-calculate-order-promising-dates.md)  
 [Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

