---
title: "Skrive ut remitteringsønske"
description: "Du kan hjelpe leverandørene med å utføre avstemminger ved å skrive ut remitteringsønsker før du bokfører en utbetalingskladd, og etter at du har bokført en betaling."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/26/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 71c84b4a7bad83e6008c0fa34f908e133b014a59
ms.contentlocale: nb-no
ms.lasthandoff: 10/26/2017

---

#<a name="how-to-print-remittance-advice"></a>Skrive ut remitteringsønske
Du kan skrive ut et remitteringsønske før du bokfører en utbetalingskladd, og etter at du har bokført en betaling. Remitteringsønsket viser leverandørfakturanumrene, noe som hjelper leverandører å utføre avstemminger.

##<a name="to-print-remittance-advice"></a>Skrive ut remitteringsønske
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Betalingskladder**, og velg deretter den relaterte koblingen.  
2. I **Betalingskladd**-vinduet velger du betalingen som remitteringsønsket skal skrives ut for.  
3. Velg handlingen **Skrive ut remitteringsønske**.  
4. Velg aktuelle filtre i kjørselen **Remitteringsønske – Kladd**, på hurtigfanen **Finanskladdelinje**.  
  
    >[!Note]
    > Du kan filtrere ved hjelp av leverandørens eksterne dokumentnummer for å samsvare betalinger med fakturaer.

5. Velg aktuelle filtre i hurtigfanen **Leverandør**.  
6. Velg **Skriv ut** hvis du vil skrive ut rapporten, eller **Forhåndsvisning** hvis du vil se rapporten nå.  

## <a name="using-remittance-advice-reports"></a>Bruke remitteringsønskerapporter
Tabellen nedenfor beskriver rapportene som kan brukes ved remitteringsønsker:

|Rapport|Description|
|----|----|
|Remitteringsønske – Kladderapport|Denne rapporten viser hvilke dokumenter som er inkludert i betalingen. For finanskladdelinjer kan du angi hvilken kladdemal og kladd remitteringsønsket vil bli skrevet ut fra, datoen for første aktiviteten som skal skrives ut, og du kan filtrere etter et bilagsnummer. Ved leverandører kan du bestemme leverandørnumrene som skal inngå i rapporten. |
|Remitteringsønske – Postrapport| Denne rapporten viser hvilke dokumenter som er inkludert i betalingen. Du kan definere innhold i rapporten ved å definere filtre. Du kan angi flere felt på fanebladet ved å velge **Felt**-feltet. For leverandørposter kan du angi hvilke leverandører som skal tas med i rapporten, datoen for første aktiviteten som skal skrives ut, valuta, og løpenummeret som skal tas med. |

> [!Note]
> Remitteringsønske - Kladderapport støtter ikke scenarier med valutautligning eller betalingstoleranser. Hvis du vil ha mer informasjon, kan du se [Aktivere utligning av kundeposter i forskjellige valutaer](finance-how-enable-application-ledger-entries-different-currencies.md).

> [!Tip]
> Hvis du vil ha mer informasjon om hvordan du arbeider med rapporter, kan du se [Vise testrapporter før bokføring](ui-how-view-test-reports-posting.md), [Arbeide med rapporter](ui-work-report.md), og [Søke etter, filtrere og sortere data](ui-enter-criteria-filters.md).

##<a name="see-also"></a>Se også  
[Velkommen til Dynamics NAV](across-get-started.md)
