---
title: Flytte varer
description: "Varer som er på lager, må kanskje flyttes mellom hyller for å opprettholde vareflyten gjennom lageret. Noen flyttinger skjer i direkte tilknytning til interne operasjoner, for eksempel en produksjonsordre som trenger komponenter levert eller sluttvarer plassert. Andre flyttinger skjer som ren lagerplassoptimalisering eller ad-hoc flyttinger til og fra operasjoner."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/22/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ce2e6f176d2eb13c74e54e903d284a41948d87b8
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="moving-items"></a>Flytte varer
Lageraktiviteten med å flytte varer i lageret utføres på ulike måter avhengig av hvordan lagerstyringsfunksjonene er satt opp. Kompleksiteten kan variere fra ingen lagerfunksjoner, via grunnleggende lagerkonfigurasjoner der bestilling for bestilling behandles ved hjelp av bare en eller flere aktiviteter, til avanserte oppsett der alle lageraktiviteter utføres i en styrt arbeidsflyt. Du finner mer informasjon under [Definere lagerstyring](warehouse-setup-warehouse.md).

Varer som er på én lagerlokasjon, må kanskje flyttes mellom hyller for å opprettholde vareflyten gjennom lageret. Noen flyttinger skjer i direkte tilknytning til interne operasjoner, for eksempel en produksjonsordre som trenger komponenter levert eller sluttvarer plassert. Andre flyttinger skjer som ren lagerplassoptimalisering eller ad-hoc flyttinger til og fra operasjoner.

Flytting av varer til andre lokasjoner påvirker varepostene, og dette må derfor gjøres ved hjelp av en overføringsordre. Hvis du vil ha mer informasjon, kan du se [Overføre beholdning mellom lokasjoner](inventory-how-transfer-between-locations.md).  

Andre flytteoppgaver er å etterfylle plukkhyller og åpne produksjonshyller jevnlig, og å endre informasjonen om hylleinnhold.  

 Tabellen nedenfor beskriver en sekvens av oppgaver, og har koblinger til emnene som beskriver dem.   

|**Hvis du vil**|**Se**|  
|------------|-------------|  
|Flytte varer mellom hyller i enkle lageroppsett når som helst og uten kildedokumenter.|[Flytte varer i enkle lageroppsett](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md)|
|Bruk lagerflytteforslaget til å flytte varer i avanserte lageroppsett, både for kildedokumenter og ad hoc.|[Flytte varer i avanserte lageroppsett](warehouse-how-to-move-items-in-advanced-warehousing.md)|  
|Ta med komponentvarer for interne operasjoner i grunnleggende lagerkonfigurasjoner som forespurt av kildedokumenter for disse operasjonene.|[Flytte komponenter til et operasjonsområde i enkle lageroppsett](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)|
|Planlegge hvilke hyller som skal fylles eller tømmes for å opprettholde en effektiv flyt, for eksempel planlegge tømming av et masselagringsområde før et stort mottak.|[Planlegge lagerflyttinger i forslag](warehouse-how-to-plan-warehouse-movements-in-worksheets.md)|
|Oppdatere hvor hyppig hyllene (for eksempel plukkhyller) må fylles på grunn av svingninger i etterspørsel.|[Beregne etterfylling av hylle](warehouse-how-to-calculate-bin-replenishment.md)|
|Omstrukturer lageret med nye hyllekoder og nye hylleegenskaper og flytt dem eventuelt rundt.|[Omstrukturere lagre](warehouse-how-to-restructure-warehouses.md)|  

## <a name="see-also"></a>Se også  
[Lagerstyring](warehouse-manage-warehouse.md)  
[Lager](inventory-manage-inventory.md)  
[Definere lagerstyring](warehouse-setup-warehouse.md)     
[Monteringsstyring](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyring](design-details-warehouse-management.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

