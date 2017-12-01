---
title: Definere hylletyper
description: "Du kan dirigere vareflyten gjennom hyller som du har definert for bestemte lageraktiviteter. Du gir hver hylle de grunnleggende flytaktivitetene, og du definerer måten en hylles skal brukes på ved å tilordne den en hylletype."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 406f9e1a325c791fb19558e13db5ace93fdc8e31
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-bin-types"></a>Definere hylletyper
Du kan dirigere vareflyten gjennom hyller som du har definert for bestemte lageraktiviteter. Du gir hver hylle de grunnleggende flytaktivitetene, og du definerer måten en hylles skal brukes på ved å tilordne den en hylletype.  

Det finnes åtte hylletyper. Du kan velge å bruke alle de åtte mulige hylletypene i lageret, eller du kan velge å bruke bare hylletypene MOTTAK, PLASSPLUKK, LEVERING og KK. Med disse fire hylletypene kan det gis forslag som støtter flyten, og du kan registrere beholdningsavvik.  

## <a name="to-set-up-the-bin-types-you-want-to-use"></a>Slik setter du opp de hylletypene du vil bruke  
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Hylletyper**, og velg deretter den relaterte koblingen.  
2.  I vinduet **Hylletyper** oppretter du en kode på 10 tegn for hver hylletype.  
3.  Velg hvilke aktiviteter som kan utføres med hver hylletype.  

> [!NOTE]  
>  Hylletyper er tilgjengelig bare når du bruker lagerstyring for lokasjonen.  

Hylletypen fastslår bare hvordan en hylle skal brukes i behandlingen av flyten gjennom lageret. Du kan alltid overstyre forslagene for et hvilket som helst lagerdokument, og du kan flytte varene inn i eller ut av en hvilken som helst hylle ved å utføre en lagerflytting.  

Nedenfor finner du en liste over de hylletypene du kan opprette.  

|Hylletype|Beskrivelse|  
|------------------|---------------------------------------|  
|MOTTA|Varer som er registrert som bokførte mottak, men som ennå ikke er plassert.|  
|SHIP|Varer som er plukket for lagerleveringslinjer, men som ennå ikke er bokført som levert.|  
|PUT AWAY|Vanligvis varer som skal lagres i store enheter, men som du ikke vil opprette tilgang til for plukking. I og med at disse hyllene ikke brukes til plukking, verken for produksjonsordrer eller følgesedler, kan bruk av en hylle av typen Plassere være begrenset, men hylletypen kan være nyttig hvis du har kjøpt et stort antall varer. Hyller av denne typen bør alltid ha en lav hylleprioritering, slik at, når mottatte varer plasseres, andre PUTPICK-hyller med høyere prioritering som er fast knyttet til varen, plasseres først. Hvis du bruker denne hylletypen, må du regelmessig etterfylle hyllene slik at varene som er lagret i disse hyllene, også blir tilgjengelige i hyller av typen PUTPICK eller PICK.|  
|PICK|Varer som bare skal brukes til plukking, for eksempel for varer med en snarlig utløpsdato som du har flyttet til denne typen hylle. Du bør alltid gi disse hyllene en høy hylleprioritering slik at de foreslås for plukking først.|  
|PUTPICK|Varer i hyller som er foreslått både for plasserings- og plukkfunksjoner. Hyller av denne typen har forskjellige hylleprioriteringer. Du kan sette opp masselagringshyllene som denne typen hylle med lave hylleprioriteringer sammenlignet med dine vanlige plukkhyller eller hyller i forhåndsplukkingsområder.|  
|KK|Denne hyllen brukes til lagerjusteringer hvis du angir denne hyllen på lokasjonskortet i feltet **Hyllekode for justering**. Du kan også sette opp hyller av denne typen for defekte varer og varer som blir kontrollert. Du kan flytte varer til denne typen hylle hvis du vil gjøre dem utilgjengelig for den vanlige vareflyten.<br /><br /> **Obs!** I motsetning til alle andre hylletyper er det ikke merket av for noen av varehåndteringsalternativene for **KK**-hylletypen som standard. Dette angir at alt innhold du plasserer i en KK-hylle er utelukket fra vareflyter.|  

## <a name="see-also"></a>Se også
[Lagerstyring](warehouse-manage-warehouse.md)  
[Lager](inventory-manage-inventory.md)  
[Definere lagerstyring](warehouse-setup-warehouse.md)     
[Monteringsstyring](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyring](design-details-warehouse-management.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

