---
title: Opprette plasseringer fra interne plasseringer
description: "Når varer er plassert, og før de blir plukket for å oppfylle behovene i en produksjonsordre eller følgeseddel, blir de lagret i lageret som en del av tilgjengelig lager."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 970b9b9046018b0dcea5b9996d10e19e444a7639
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-pick-and-put-away-without-a-source-document"></a>Plukke og plassere uten et kildedokument.
Når varer er plassert, og før de blir plukket for å oppfylle behovene i en produksjonsordre eller følgeseddel, blir de lagret i lageret som en del av tilgjengelig lager.  

Det kan oppstå situasjoner der varer må tas ut av plukkhyller midlertidig, for eksempel for å tjene som demonstrasjonsmodeller i en salgspresentasjon. Disse elementene eies fortsatt av firmaet og er en del av beholdningen, men er ikke tilgjengelige for plukking. De er registrert i en spesiell hylle som du oppretter for dette formålet. Teknisk sett er varene på lageret, men fysisk kan de være i et konferanserom eller demonstrasjonsrom.  

I andre situasjoner kan produksjonsenheten få uventet behov for noen få deler til en prosess. Du kan plukke varer for produksjonshyllen ved hjelp av den interne plukken. Når prosessen er over og avgangen er opprettet, bokfører du forbruket av varene og tømmer produksjonshyllen, som i sin tur reduserer antallet av varen i din lokasjon.  

På samme måte kan varer returneres til lageret for plassering. Varene kan ha vært tatt ut av det tilgjengelige lageret for en produksjonsordre og så ikke blitt brukt i det hele tatt. For å få dem til å bli en del av det tilgjengelige lageret igjen, må de plasseres i hyllen.  

Med **Intern plassering** kan du utføre plasseringer uten å måtte referere til et bestemt kildedokument. Du kan enkelt sette opp all den informasjonen du trenger til å opprette en lagerinstruksjon for plassering.  

> [!NOTE]  
>  Hvis du ikke bruker intern plukking og intern plassering, kan disse justeringene utføres med metodene for å flytte varer fra hylle til hylle eller for å bokføre antallsjusteringer i en hylle.  
>   
>  Når lokasjonen bruker lagerstyring, og derfor bruker hylletyper, kan du ikke manuelt flytte varer til eller fra en hylle av hylletypen RECEIVE, fordi varer som er i en slik hylle må registreres som plassert før de blir en del av det tilgjengelige lageret.  

## <a name="to-create-an-internal-pick"></a>Opprette en intern plukking  
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Intern plukk**, og velg deretter den relaterte koblingen.  
2.  Fyll ut feltet **Nr.** feltet og feltet **Til hylle-kode** i hurtigfanen **Generelt**. Feltet **Til hylle-kode** angir hyllen som du vil hente varene fra. Til produksjonsformål ville denne hyllen være den inngående produksjonshyllen eller den åpne produksjonshyllen. Til andre formål velger du en Til hylle-kode for en hylletype som ikke brukes til plukking, sannsynligvis en hylle for oppsamling, levering eller spesielle formål.  
3.  Velg en vare i feltet **Varenr.**, og fyll ut antallene du vil plukke.  
4. Velg handlingen **Opprett plukk**. En plukkinstruksjon er nå klar til utføring av en lageransatt.  

## <a name="to-create-an-internal-put-away"></a>Opprette en intern plassering  
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Intern plukk**, og velg deretter den relaterte koblingen.  
2.  Fyll ut feltet **Nr.** og **Fra hylle-kode** i hurtigfanen **Generelt**. Feltet **Fra hylle-kode** angir hyllen der varene som blir returnert til lageret, kanskje fra produksjon, er plassert.  
3.  Fyll ut varenumrene og antallene på linjene.  
4.  Velg handlingen **Opprett plassering**. En plasseringsinstruksjon er nå klar til utføring av en lageransatt.  

## <a name="see-also"></a>Se også  
[Lagerstyring](warehouse-manage-warehouse.md)  
[Lager](inventory-manage-inventory.md)  
[Definere lagerstyring](warehouse-setup-warehouse.md)     
[Monteringsstyring](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyring](design-details-warehouse-management.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

