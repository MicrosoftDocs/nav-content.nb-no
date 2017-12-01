---
title: Definere statuser for serviceordrer og reparasjoner
description: "Du må definere ni alternativer for reparasjonsstatus som identifiserer fremdriften av reparasjon og vedlikehold på servicevarer i serviceordrer."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d7dbc4cfc06d4c74476a04512bd368a0ab26f837
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-statuses-for-service-orders-and-repairs"></a>Definere statuser for serviceordrer og reparasjoner
Du må definere ni alternativer for reparasjonsstatus som identifiserer fremdriften av reparasjon og vedlikehold på servicevarer i serviceordrer. Du må definerer minst ni alternativer for reparasjonsstatus som identifiserer situasjoner eller handlinger som er iverksatt under vedlikehold av servicevarer.  

Du kan angi prioritetsnivå for alternativene for serviceordrestatus. De fire prioritetene er Høy, Middels høy, Middels lav og Lav.  
  
Når du endrer reparasjonsstatusen til en servicevare i en serviceordre, oppdateres serviceordrestatusen. Reparasjonsstatusen til hver enkelt servicevare er knyttet til serviceordrestatusen. Hvis servicevarene er koblet til to eller flere alternativer for serviceordrestatus, velges serviceordrestatusen med høyest prioritet.  

## <a name="to-set-up-a-repair-status"></a>Slik definerer du reparasjonsstatus  
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Reparasjonsstatus**, og velg deretter den relaterte koblingen. 2. Opprett en ny reparasjonsstatus.  
3. Fyll ut feltene **Kode** og **Beskrivelse**.  
4. I **Serviceordrestatus**-feltet velger du ordrestatusen å knytte reparasjonsstatusen til. **Prioritet**-feltet viser prioriteten til serviceordrestatusen du har valgt.  
5. Velg en reparasjonsstatus. Du kan bare velge én.  
6. Velg feltet **Bokføring tillatt** hvis du vil kunne bokføre serviceordrer som omfatter servicevarer, med reparasjonsstatusen.  
7. Merk av for **I kø-status tillatt** for å tillate manuell endring av alternativet for serviceordrestatusen til alternativet **I kø** i serviceordrer som omfatter servicevarer med denne reparasjonsstatusen.  
8. Merk av for **I arbeid-status tillatt**, **Ferdig-status tillatt**og **Avvent-status tillatt**på samme måte.
  
## <a name="to-set-up-service-status-priorities"></a>Slik definerer du servicestatusprioritet  
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Serviceordrestatus**, og velg deretter den relaterte koblingen.  
2. Velg serviceordrestatusen du vil angi en prioritet for.  
3. I feltet **Prioritet** velger du prioriteten du vil ha for denne serviceordrestatusen. Gjenta dette trinnet for hver status.  
  
## <a name="see-also"></a>Se også  
[Forstå serviceordre- og reparasjonsstatus]()  
[Konfigurere servicehåndtering](service-setup-service.md)  

