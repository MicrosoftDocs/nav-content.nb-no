---
title: Designdetaljer - Beholdningsperioder
description: "Tilbakedaterte transaksjoner eller kostnadsjusteringer påvirker ofte saldoer og lagerverdier for regnskapsperioder som kan anses som avsluttet. Dette kan ha en negativ virkning på nøyaktig rapportering, særlig i globale selskaper. Du kan bruke Lagerperioder-funksjonen til å unngå slike problemer, ved å åpne eller lukke lagerperioder for å begrense bokføring i en angitt tidsperiode."
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 1dd508ee887b28b1696746444145eff6f2bd7ebe
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-inventory-periods"></a>Designdetaljer: Beholdningsperioder
Tilbakedaterte transaksjoner eller kostnadsjusteringer påvirker ofte saldoer og lagerverdier for regnskapsperioder som kan anses som avsluttet. Dette kan ha en negativ virkning på nøyaktig rapportering, særlig i globale selskaper. Du kan bruke Lagerperioder-funksjonen til å unngå slike problemer, ved å åpne eller lukke lagerperioder for å begrense bokføring i en angitt tidsperiode.  

 En lagerperiode er en bestemt periode, angitt av en sluttdato, der du bokfører lagertransaksjoner. Når du lukker en lagerperiode, kan ingen verdiendringer bokføres i den lukkede periode. Dette omfatter nye verdibokføringer, forventede eller fakturerte bokføringer, endring av eksisterende verdier og kostjusteringer. Du kan imidlertid framdels bruke på en åpen varepost som er i en lukket periode. Hvis du vil ha mer informasjon, kan du se [Designdetaljer: Vareutligning](design-details-item-application.md).  

 For å sikre at alle transaksjonsposter i en lukket periode er endelige, må følgende betingelser oppfylles før en lagerperiode kan lukkes:  

-   Alle utgående vareposter i perioden må avsluttes (ingen negativ beholdning).  
-   Alle varekostnader i perioden må justeres.  
-   Alle frigitte og ferdige produksjonsordrer i perioden må kostnadsjusteres.  

 Når du lukker en lagerperiode, opprettes en lagerperiode ved hjelp av nummeret på den siste varejournalen i lagerperioden. I tillegg registreres klokkeslett, dato og brukerkode i lagerperiodeposten for brukeren som lukker perioden. Ved hjelp av denne informasjonen med siste varejournalen for forrige periode, kan du se hvilke lagertransaksjonene som bokført i lagerperioden. Det er også mulig å åpne lagerperioder på nytt hvis du må bokføre i en lukket periode. Når du åpner en lagerperiode på nytt, blir det opprettet en lagerperiodepost.  

## <a name="see-also"></a>Se også  
 [Designdetaljer: Kostberegning for beholdning](design-details-inventory-costing.md) [Administrere lagerkostnader](finance-manage-inventory-costs.md) [Finans](finance.md)  
 [Arbeide med Dynamics NAV](ui-work-product.md)

