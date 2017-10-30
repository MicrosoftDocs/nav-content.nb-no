---
title: Utligne poster i ulike valutaer
description: "Du kan utligne poster i flere valutaer, for eksempel hvis du selger i én valuta og mottar betaling i en annen."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies, payment, reconcile
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f323b98472f3e2ef0f28000f8a9140b066206945
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-enable-application-of-ledger-entries-in-different-currencies"></a>Aktivere utligning av kundeposter i forskjellige valutaer
Hvis du handler fra en leverandør i én valuta og betaler i en annen valuta, kan du utligne utbetalingen mot kjøpet.

Hvis du selger til en kunde i én valuta og mottar betaling i en annen valuta, kan du også utligne betalingen mot salgsfakturaen.

Fremgangsmåten nedenfor beskriver hvordan du definerer dette for leverandørposter i vinduet **Kjøpsoppsett**. Oppsettet er det samme for kundeposter i vinduet **Salgsoppsett**.

## <a name="to-enable-application-of-vendor-ledger-entries-in-different-currencies"></a>Aktivere utligning av leverandørposter i forskjellige valutaer
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Kjøpsoppsett**, og velg deretter den relaterte koblingen.
2. I feltet **Utligning mellom valuta** velger du ett av følgende alternativer:

| Alternativ | Beskrivelse |
| --- | --- |
| Ingen |Utligning mellom valutaer er ikke tillatt. |
| ØMU |Utligning mellom ØMU-valutaer er tillatt. |
| Alle |Utligning mellom alle valutaer er tillatt. |

## <a name="to-set-up-gl-accounts-for-currency-application-rounding-differences"></a>Slik konfigurerer du finanskonti for avrundingsdifferanser ved valutautligning  
Hvis du vil utligne poster i ulike valutaer, må du opprette finanskontoer som du vil bokføre avrundingsdifferanser på.  

> [!NOTE]  
>  Du må opprette finanskontoene før du fullfører oppgaven. Hvis du vil ha mer informasjon, kan du se [Forstå finans og kontoplanen](finance-general-ledger.md).

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bokføringsgrupper - kunde**, og velg deretter den relaterte koblingen.  
2. Angi de relevante finanskontiene der avrundingsdifferanser skal bokføres, i feltene **Debetkonto for valutaavrund.** og **Kreditkonto for valutaavrund.**.  
3. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bokføringsgrupper - leverandør**, og velg deretter den relaterte koblingen.  
4. Angi de relevante finanskontiene der avrundingsdifferanser skal bokføres, i feltene **Debetkonto for valutaavrund.** og **Kreditkonto for valutaavrund.**.  

## <a name="see-also"></a>Se også
[Administrere skyldige beløp](payables-manage-payables.md)  
[Håndtere fordringer](receivables-manage-receivables.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

