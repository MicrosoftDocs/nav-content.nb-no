---
title: Korrigere forskudd
description: "Du kan foreta en korrigering i en ordre etter at du har bokført en forskuddsfaktura for ordren. Du kan legge til nye linjer på en ordre etter at du har utstedt et forskudd, og deretter kan du bokføre en ny forskuddsfaktura, men du kan ikke slette en linje fra en ordre etter at et forskudd er fakturert for linjen."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c39223940880514f9a59eae96e88182e19db2b5e
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-correct-prepayments"></a>Korrigere forskudd
Du kan foreta en korrigering i en ordre etter at du har bokført en forskuddsfaktura for ordren. Du kan legge til nye linjer på en ordre etter at du har utstedt et forskudd, og deretter kan du bokføre en ny forskuddsfaktura, men du kan ikke slette en linje fra en ordre etter at et forskudd er fakturert for linjen.  

## <a name="to-correct-a-prepayment"></a>Slik korrigerer du et forskudd
Følgende fremgangsmåte viser hvordan du utsteder en forskuddskreditnota som kansellerer alle fakturerte forskudd for en ordre.  
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Ordrer**, og velg deretter den relaterte koblingen.  
2. Åpne den aktuelle ordren.
3. Velg **Forskuddsbetaling**, og velg deretter **Bokfør kreditnota for forskudd** eller **Bokfør og skriv ut forskuddsfaktura**.  
4. I vinduet **Salgskreditnota** fortsette med å korrigere de aktuelle postene, for en salgskreditnota. Hvis du vil ha mer informasjon, kan du se [Behandle ordrereturer eller annulleringer](sales-how-process-sales-returns-cancellations.md).     

    > [!NOTE]  
    > For å redusere beløpet i **Linjebeløp**-feltet må du først øke forskuddsprosenten på linjen slik at verdien i feltet **Linjebeløp for forskudd** ikke blir lavere enn verdien i feltet **Fakturert forskuddsbeløp**.

5. Når du skal opprette en forskuddsfaktura for nye linjer i en salgskreditnota, velger du **Forskuddsbetaling** og velger deretter **Bokfør forskuddsfaktura** eller **Bokfør og skriv ut forskuddsfaktura**.  
6. Du kan utstede en ny forskuddsfaktura ved å øke forskuddsbeløpet på én eller flere linjer og bokføre forskuddsfakturaen. Det opprettes en ny faktura for differansen mellom forskuddsbeløpene som er fakturert, og de nye forskuddsbeløpene.  

## <a name="see-also"></a>Se også  
[Fakturere forskuddsbetalinger](finance-invoice-prepayments.md)  
[Gjennomgang: konfigurere og fakturere salgsforskudd](walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
[Finans](finance.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

