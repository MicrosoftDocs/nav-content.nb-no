---
title: "Lukke åpne vareposter som er resultat av fast utligning i varekladden"
description: "Du kan bruke feltet **Utlignet fra-post** i vinduet **Varekladd** til å opprette en fast utligning manuelt mellom en inngående transaksjon og den opprinnelige utgående transaksjonen. Du kan for eksempel bruke det til å rette den utgående transaksjonen eller behandle returen."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/09/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b0b0daad01f8108d035739e387b38af4f0311ff9
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-close-open-item-ledger-entries-resulting-from-fixed-application-in-the-item-journal"></a>Lukke åpne vareposter som er resultat av fast utligning i varekladden
Du kan bruke feltet **Utlignet fra-post** i vinduet **Varekladd** til å opprette en fast utligning manuelt mellom en inngående transaksjon og den opprinnelige utgående transaksjonen. Du kan for eksempel bruke det til å rette den utgående transaksjonen eller behandle returen. Hvis du vil ha mer informasjon, kan du se Utlignet-fra post.  

> [!IMPORTANT]  
>  Faste utligninger som gjøres på denne måten, bruker bare kostnader, ikke antallet. Den bokførte positive vareposten vil på samme måte ikke lukke den brukte utgående posten og vil selv forbli åpen. Dette gjelder også når du bokfører en fast utligning for en positiv post til en negativ post som ikke er lukket av en vanlig positiv post – da vil både den negative og den positive posten forbli åpne.  
>   
>  Dette betyr at du ikke kan lukke en lagerperiode hvis det finnes en slik post.  

Følgende fremgangsmåte viser hvordan du lukker slike poster ved å utføre to korrigerende bokføringer i varekladden.  

## <a name="to-close-open-item-ledger-entries-that-result-from-a-fixed-application-in-the-item-journal"></a>Slik lukker du åpne vareposter som er resultater fra en fast utligning i varekladden:  

1.  Bruk feltet **Utlignet-fra post** til å bokføre en oppjustering med tilsvarende antall. Dette lukker den opprinnelige negative korreksjonsposten med en fast utligning.  
2.  Bruk feltet **Utligningspost** til å bokføre en nedjustering. Dette lukker den opprinnelige positive korreksjonsposten med en fast utligning.  

## <a name="see-also"></a>Se også  
[ Fjerne varefinansposter og utligne dem på nytt](finance-how-to-remove-and-reapply-item-entries.md)  
 [Behandle ordrereturer og annulleringer](sales-how-process-sales-returns-cancellations.md)   
 [Definere lagerverdisetting og kostberegning](finance-set-up-inventory-valuation-and-costing.md)   
 [Administrere lagerkostnader](finance-manage-inventory-costs.md)   
 [Designdetaljer: Kostmetoder](design-details-costing-methods.md)

