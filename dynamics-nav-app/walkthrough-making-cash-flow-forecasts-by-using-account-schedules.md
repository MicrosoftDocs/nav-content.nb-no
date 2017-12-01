---
title: "Gjennomgang - Lage kontantstrømprognoser ved å bruke kontoskjemaer"
description: "Denne gjennomgangen beskriver hvordan du kan bruke kontoskjemaer til å lage kontantstrømprognoser. Kontoskjemaer utfører beregninger som ikke kan utføres direkte i diagrammet over kontantstrømkontoer. I kontoskjemaer kan du definere delsummer for kontantstrømmottak og -utbetalinger. Disse delsummene kan inkluderes i nye totalsummer som deretter kan brukes til å lage kontantstrømprognoser."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 72e2c2ab540ce53dc747792c3d1fa93ec87282f8
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="walkthrough-making-cash-flow-forecasts-by-using-account-schedules"></a>Gjennomgang: Lage kontantstrømprognoser ved å bruke kontoskjemaer
Denne gjennomgangen beskriver hvordan du kan bruke kontoskjemaer til å lage kontantstrømprognoser. Kontoskjemaer utfører beregninger som ikke kan utføres direkte i diagrammet over kontantstrømkontoer. I kontoskjemaer kan du definere delsummer for kontantstrømmottak og -utbetalinger. Disse delsummene kan inkluderes i nye totalsummer som deretter kan brukes til å lage kontantstrømprognoser.  

## <a name="about-this-walkthrough"></a>Denne gjennomgangen  
Denne gjennomgangen beskriver følgende oppgaver:  

- Definere et nytt navn for kontantstrømkontoskjema.  
- Definere kontoskjemalinjer.  
- Definere et nytt kolonneoppsett.  
- Tilordne et kolonneoppsett til et kontoskjema.  
- Vise og skrive ut kontantstrømprognosen.  

### <a name="prerequisites"></a>Forutsetninger  
For å fullføre denne gjennomgangen må du gjøre følgende:  

- [!INCLUDE[d365fin](includes/d365fin_md.md)] installert.  
- Forslagslinjene for kontantstrøm registreres.  

## <a name="roles"></a>Roller  
Denne gjennomgangen viser oppgaver som utføres av følgende brukerrolle:  

- Kontrollør  

## <a name="story"></a>Hovedscenario  
Ken er kontrollør i CRONUS og utarbeider månedlige kontantstrømprognoser. Han tar med finans, salg, kjøp og aktiva i prognosen, og deretter viser han den til ØKDIR Sara.  

## <a name="setting-up-a-new-account-schedule-name"></a>Definere et nytt kontoskjemanavn  
Et kontoskjema består av et navn på kontoskjemaet for kontantstrøm med en rekke linjer og et kolonneoppsett.  

### <a name="to-set-up-a-new-account-schedule-name"></a>Slik definerer du et nytt kontoskjemanavn  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Kontoskjemaer**, og velg deretter den relaterte koblingen.  
2.  Velg **Ny** i vinduet **Kontoskjemanavn** for å opprette et nytt navn for kontantstrømkontoskjema..  
3.  I **Navn**-feltet angir du **Prognose**.  
4.  I **Beskrivelse**-feltet angir du **Kontantstrømprognose**.  
5.  La feltene **Standard kolonneoppsett** og **Analysevisningsnavn** være tomme.  

## <a name="setting-up-account-schedule-lines"></a>Definere kontoskjemalinjer  
Etter at et kontoskjemanavn er angitt, definerer Ken hver linje som vises i kontoskjemaet for kontantstrøm. Ken definerer linjer som kan vises i rapporter, i tillegg til linjer som bare er til beregningsformål.  

### <a name="to-set-up-account-schedule-lines"></a>Definere kontoskjemalinjer  

1.  Velg det nye kontoskjemanavnet for **Prognose** du har opprettet, i vinduet **Kontoskjemanavn**. I fanebladet **Hjem**, under **Prosess**, velger du **Rediger kontoskjema**.  
2.  I vinduet **Kontoskjema** angir du hver linje nøyaktig, som vist i tabellen nedenfor.  

    > [!NOTE]  
    >  Du kan bruke funksjonen **Sett inn kontantstrømkonti** til raskt å merke kontantstrømkontoene i kontantstrømkontoplanen og kopiere dem til kontoskjemalinjer.  

    |Radnr.|Beskrivelse|Sammentellingstype|Sammentelling|Radtype|Beløpstype|Vis|  
    |-------|-----------|-------------|--------|--------|---  ------|----| |C10|Beløp|Bevegelse|Poster|Nettobeløp|Alltid|  
    |C20|Beløp til dato|Saldo per dato|Poster|Nettobeløp|Alltid|  
    |C30|Helt regnskapsår|Helt regnskapsår|Poster|Nettobeløp Beløp|Alltid|  

4.  Velg **OK**.  

## <a name="assigning-the-column-layout-to-the-account-schedule-name"></a>Tilordne kolonneoppsettet til kontoskjemanavnet  
Ken er nå klar til å tilordne kolonneoppsettet til kontoskjemanavnet.  

### <a name="to-assign-the-column-layout-to-the-account-schedule-name"></a>Slik tilordner du kolonneoppsettet til kontoskjemanavnet:  

1.  I vinduet **Kontoskjemanavn** velger du **Prognose** i **Navn**-feltet.  
2.  Velg kolonneoppsettet **Kontantstrøm** i feltet **Standard kolonneoppsett** for å bruke det som standard kolonneoppsett.  

### <a name="to-view-and-print-the-cash-flow-forecast"></a>Slik viser og skriver du ut kontantstrømprognosen:  
1.  Velg **Oversikt**-handlingen i vinduet **Kontoskjemanavn** for å vise kontantstrømprognosen.  
2.  I vinduet **Kto.skjemaoversikt** kan du velge et beløp og deretter vise kontantstrømprognosepostene som utgjør beløpet. I tillegg kan du vise formelen som brukes til å beregne beløpet. Du kan også filtrere beløpene etter dato og dimensjon.  
3.  Velg **Skriv ut**-handlingen for å skrive ut kontantstrømprognosen.  

## <a name="see-also"></a>Se også  
 [Arbeide med kontoskjemaer](bi-how-work-account-schedule.md)   
 [Gjennomgang av forretningsprosesser](walkthrough-business-process-walkthroughs.md)  
 [Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

