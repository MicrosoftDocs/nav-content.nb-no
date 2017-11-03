---
title: Designdetaljer - Lukke behov og forsyning
description: "Når balanseringsprosessene for forsyning er utført, er det tre mulige sluttsituasjoner."
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
ms.openlocfilehash: 337fdb4c625e17e72f4adb692cbf0f2729ae96b7
ms.contentlocale: nb-no
ms.lasthandoff: 10/26/2017

---
# <a name="design-details-closing-demand-and-supply"></a>Designdetaljer: Lukke behov og forsyning
Når balanseringsprosessene for forsyning er utført, er det tre mulige sluttsituasjoner:  

-   Nødvendig antall og dato for behovshendelsene er dekket, og planleggingen for dem kan lukkes. Forsyningshendelsen er fortsatt åpen og kan kanskje dekke neste behov, slik at balanseringsprosessen kan starte på nytt med den gjeldende forsyningshendelsen og neste behov.  

-   Forsyningsordren kan ikke endres slik at den dekker alle behov. Behovshendelsen er fortsatt åpen, med et ikke-dekket antall som kan dekkes av neste forsyningshendelse. Gjeldende forsyningshendelse blir dermed lukket, slik at balanseringen kan starte på nytt med det gjeldende behovet og neste forsyningshendelse.  

-   All etterspørsel er dekket. Det er ingen etterfølgende etterspørsel (eller det er ingen etterspørsel i det hele tatt). Hvis det finnes overskuddsforsyning, kan den reduseres (eller avbrytes) og deretter lukkes. Det kan hende det finnes flere forsyningshendelser videre i kjeden, og de må også avbrytes.  

 Til slutt oppretter planleggingssystemet en ordresporingskoblingen mellom forsyning og behov.  

## <a name="creating-the-planning-line-suggested-action"></a>Opprette planleggingslinjen (foreslått handling)  
 Hvis det foreslås en handling, Ny, Endre antall, Tidsplanlegg på nytt, Tidsplanlegg på nytt og endre antallet eller Avbryt, for å endre forsyningsordren, oppretter planleggingssystemet en planleggingslinje i planleggingsforslaget. Planleggingslinjen opprettes på grunn av ordresporing, ikke bare når forsyningshendelsen lukkes, men også hvis behovshendelsen lukkes, selv om forsyningshendelsen fremdeles er åpen og kan endres når neste behovshendelse behandles. Dette betyr at når planleggingslinjen først opprettes, kan den endres på nytt.  

 Du kan minimere databasetilgang ved håndtering av produksjonsordrer ved å vedlikeholde planleggingslinjen på tre nivåer og samtidig prøve å utføre det minst krevende vedlikeholdsnivået:  

-   Opprett bare planleggingslinjen med gjeldende forfallsdato og antall, men uten ruting og komponenter.  

-   Inkluder ruting: Den planlagte ruten settes opp, herunder beregning av start- og sluttdatoer og -klokkeslett. Dette er krevende når det gjelder databasetilgang. For å fastslå slutt- og forfallsdatoene blir det kanskje nødvendig å beregne dette selv om forsyningshendelsen ikke er lukket (når det gjelder planlegging fremover).  

-   Ta med stykklisteutfoldelse: Dette kan vente til like før forsyningshendelsen lukkes.  

 Med dette avsluttes beskrivelsene av hvordan behov og forsyning lastes, prioriteres og balanseres av planleggingssystemet. I integrering med denne aktiviteten for forsyningsplanlegging, må systemet sikre at nødvendig lagernivå opprettholdes for hver planlagt vare i henhold til sine gjenbestillingsprinsippene.  

## <a name="see-also"></a>Se også  
 [Designdetaljer: Balansere behov og forsyning](design-details-balancing-demand-and-supply.md)   
 [Designdetaljer: Sentrale begreper for planleggingssystemet](design-details-central-concepts-of-the-planning-system.md)   
 [Designdetaljer: Forsyningsplanlegging](design-details-supply-planning.md)

