---
title: Norsk mva-rapportering
description: "Forbedringer i den norske versjonen gjør det mulig for deg å beregne og rapportere mva til de norske skattemyndighetene."
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
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 81d7cd5aa0cc176ab03918e7de1812762700074c
ms.contentlocale: nb-no
ms.lasthandoff: 10/26/2017

---
# <a name="norwegian-vat-reporting"></a>Norsk mva-rapportering
[!INCLUDE[navnow](../../includes/navnow_md.md)]../../inkluderer orbedringer i den norske versjonen som gjør det mulig for deg å beregne og rapportere mva til de norske skattemyndighetene.  

Dette emnet forklarer de vanlige trinnene du skal følge når du rapporterer norsk mva.  

## <a name="print-the-trade-settlement"></a>Skrive ut omsetningsoppgaven  
Først må du må skrive ut omsetningsoppgaven. Bruk **Omsetningsoppgaven**-rapporten til å skrive ut omsetningsoppgaven som kreves av skattemyndighetene.  

Denne rapporten skriver ut detaljerte opplysninger om bokført mva i den angitte perioden. Den faktisk omsetningsoppgaven som skal rapporteres skrives ut på siste side av rapporten.  

Denne rapporten kan skrives ut så mange ganger som nødvendig. Ingen bokføring eller andre endringer utføres på dataene når du bruker denne rapporten.  

## <a name="check-the-trade-settlement"></a>Sjekk omsetningsoppgaven  
Så må du må sjekke omsetningsoppgaven. Kontroller at beløpene i omsetningsoppgaven er riktig, og foreta eventuelle justeringer.  

## <a name="post-vat"></a>Bokfør Mva.  
Hvis informasjonen i omsetningsoppgaven er riktig, er det siste trinnet å bokføre mva ved hjelp av rapporten **Beregn og Bokfør mva-oppgjør**. Det er nødvendig at du manuelt angi riktig mva-periode i feltene **Startdato** og **Sluttdato**. Vanligvis korresponderer disse datoene til perioden som tidligere er angitt i **Omsetningsoppgaven**-rapporten.  

Når du bruker denne rapporten, kan du velge å ikke bokføre hvis du vil kontrollere resultatene før du faktisk bokfører mva.  

Når du bokfører mva., opprettes den tilsvarende mva-perioden, og merkes som lukket i **Oppgjort mva-periode**-tabellen. Hvis du angir en periode som ikke svarer til én av de vanlige seks norske mva periodene, avsluttes alle periodene som berøres av den angitte periode.  

## <a name="see-also"></a>Se også  
 [Funksjonalitet som er spesifikk for norske brukere](norway-local-functionality.md)

