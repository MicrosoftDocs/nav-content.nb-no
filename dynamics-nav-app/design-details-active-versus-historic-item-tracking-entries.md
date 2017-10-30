---
title: Designdetaljer - Aktive kontra historiske varesporingsposter
description: "Når deler av et dokumentlinjeantall bokføres, overføres bare dette bestemte antallet til varepostene og varesporingsnumrene. Du vil imidlertid ha tilgang til all relevant varesporingsinformasjon direkte fra den aktive dokumentlinjen. Det vil si at ikke bare vil du se postene som er knyttet til restantallet, men du vil også ha informasjon om enhetene som er bokført. Når du viser eller endrer vinduet **Varesporingslinjer**, vises det samlede innholdet i **Sporingsspesifikasjon**-tabellen (T336) og **Reservasjonspost**-tabellen (T337) i en midlertidig versjon av T336. Dette sikrer at historiske og aktive varesporingsdata er tilgjengelige som ett element."
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
ms.openlocfilehash: 315b5317c2ac3e2cd6a56bd243e30d4e3445a6ec
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-active-versus-historic-item-tracking-entries"></a>Designdetaljer: Aktive kontra historiske varesporingsposter
Når deler av et dokumentlinjeantall bokføres, overføres bare dette bestemte antallet til varepostene og varesporingsnumrene. Du vil imidlertid ha tilgang til all relevant varesporingsinformasjon direkte fra den aktive dokumentlinjen. Det vil si at ikke bare vil du se postene som er knyttet til restantallet, men du vil også ha informasjon om enhetene som er bokført. Når du viser eller endrer vinduet **Varesporingslinjer**, vises det samlede innholdet i **Sporingsspesifikasjon**-tabellen (T336) og **Reservasjonspost**-tabellen (T337) i en midlertidig versjon av T336. Dette sikrer at historiske og aktive varesporingsdata er tilgjengelige som ett element.  

 Tabellen nedenfor viser hvordan T336 og T337 brukes i et scenario med kjøp. Tallene i fet representerer verdier som brukeren angir manuelt i vinduet **Varesporingslinjer**.  

 Trinn 1: Opprett en bestillingslinje med sju stykker med varesporingsnumre.  

||**Antall (lagerenhet)**|**Ant. som skal håndt.**|**Ant. som skal fakt. (l.enh.)**|**Håndtert antall (l.enh.)**|**Fakturert antall (l.enh.)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|**T337**|7|0|0|0|0|  
|**T336**|0|0|0|0|0|  

 Trinn 2: Motta fire stykker.  

||**Antall (lagerenhet)**|**Ant. som skal håndt.**|**Ant. som skal fakt. (l.enh.)**|**Håndtert antall (l.enh.)**|**Fakturert antall (l.enh.)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|Vinduet **Varesporingslinjer**|7|**4**|**0**|0|0|  
|**T337**|3|0|0|0|0|  
|**T336**|4|0|0|4|0|  

 Trinn 3: Motta to stykker, og fakturer to stykker.  

||**Antall (lagerenhet)**|**Ant. som skal håndt.**|**Ant. som skal fakt. (l.enh.)**|**Håndtert antall (l.enh.)**|**Fakturert antall (l.enh.)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|Vinduet **Varesporingslinjer**|7|**2**|**2**|4|0|  
|**T337**|1|0|0|0|0|  
|**T336**|6|0|0|6|2|  

 Trinn 4: Motta ett stykk.  

||**Antall (lagerenhet)**|**Ant. som skal håndt.**|**Ant. som skal fakt. (l.enh.)**|**Håndtert antall (l.enh.)**|**Fakturert antall (l.enh.)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|Vinduet **Varesporingslinjer**|7|**1**|**0**|6|2|  
|**T336**|7|0|0|7|2|  

 Fakturere 5 enheter.  

||**Antall (lagerenhet)**|**Ant. som skal håndt.**|**Ant. som skal fakt. (l.enh.)**|**Håndtert antall (l.enh.)**|**Fakturert antall (l.enh.)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|Vinduet **Varesporingslinjer**|7|0|**5**|7|2|  
|**T336**|7|0|0|7|7|  

## <a name="see-also"></a>Se også  
 [Designdetaljer: Varesporing](design-details-item-tracking.md)   
 [Designdetaljer: Vindu for varesporingslinjer](design-details-item-tracking-lines-window.md)

