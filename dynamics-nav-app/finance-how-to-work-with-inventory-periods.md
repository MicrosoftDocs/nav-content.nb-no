---
title: Arbeide med lagerperioder
description: "Du kan kontrollere tidsrammen som brukere kan bokføre endringer i lageret, ved å definere lagerperioder."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: inventory, periods
ms.date: 08/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 289b12d39c9f67913d862cb3500cccae0b3823d2
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-work-with-inventory-periods"></a>Arbeide med lagerperioder
Lagerperioder er tidsperioder som du kan bokføre lagerendringer i. En lagerperiode defineres av datoen den slutter på, eller sluttdatoen. En lagerperiode defineres av datoen den slutter på, eller sluttdatoen. Du kan ikke bokføre eventuelle nye verdier til lageret før sluttdatoen. Hvis du har åpne vareposter i en lukket periode, det vil si positivt antall som ennå ikke er utlignet mot utgående transaksjoner, kan du fortsatt utligne utgående antall mot disse postene, selv om perioden er lukket.  

De følgende delene handler om hvordan du kan:  

* Opprett lagerperioder.  
* Lukk lagerperioder.  
* Åpne lagerperioder på nytt.  

## <a name="to-create-an-inventory-period"></a>Slik oppretter du en lagerperiode  
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Lagerperioder**, og velg deretter den relaterte koblingen.  
2. Opprett en ny linje.  
3. Angi den siste datoen i lagerperioden du vil definere, i **Sluttdato**-feltet. Når perioden er lukket, kan du ikke bokføre lagerendringer før denne datoen.  
4. Skriv inn et beskrivende navn i **Navn**-feltet. Velg **OK**.  

## <a name="closing-inventory-periods"></a>Lukke lagerperioder  
**Lukket**-feltet angir om lagerperioden er lukket eller ikke for lagerverdiendringer. Du kan ikke redigere dette feltet.  

Du kan lukke en hvilken som helst lagerperiode gitt at følgende betingelser er oppfylt:  

* Det er ingen utgående vareposter, det vil si negativ beholdning, i perioden.  
* Kostbeløpet for alle varer er justert ved hjelp av kjørselen **Juster kostverdi - vareposter**.  

Dette betyr at alle utgående transaksjonsantall, for eksempel de fra ordrer, utgående overføringer, salgsfakturaer, bestillingsreturer eller kjøpskreditnotaer, må utlignes mot eksisterende antall på lageret.  

### <a name="to-close-an-inventory-period"></a>Slik lukker du en lagerperiode:  
1. Før du lukker en lagerperiode, kjører du den satsvise jobben **Juster kostverdi – vareposter** for å sikre at alle kostjusteringer er bokført. I fanebladet **Handlinger**, under **Funksjoner** velger du **Juster kostverdi - vareposter**.  

     Kjør rapporten **Lukk lagerperiode - test** for å fastslå om det er noen åpne utgående vareposter i lagerperioden eller varer som kost ikke er justert for ennå.  
2. Velg **Lukk lagerperiode - test**.  

     Kjør kjørselen **Bokfør lagerkost i Finans** for å sikre at all kost bokføres i Finans.  
3. Velg handlingen **Bokfør lager i Finans**.  
4. I vinduet **Lagerperioder** velger du lagerperioden du vil lukke.  
5. Velg **Lukk periode**. Når lagerperioden er lukket, kan du ikke bokføre lagerendringer før sluttdatoen. Du må justere kostbeløpet for alle varer med kjørselen **Juster kostverdi - vareposter** før du lukker lagerperioden.  
6. Velg **Ja** for å bekrefte at du vil lukke perioden, eller velg **Nei** hvis du ikke vil lukke den.  
7. Lagerperioden lukkes og en bekreftelsesmelding vises når prosessen er ferdig.  

## <a name="reopening-inventory-periods"></a>Åpne lagerperioder på nytt  
Når du har lukket lagerperioden, kan du ikke slette den. Du kan imidlertid åpne den på nytt hvis du vil tillate bokføring før sluttdatoen i lagerperioden. Hvis du åpner en periode på nytt, åpnes også alle lagerperioder med sluttdatoer som er senere enn perioden du åpner på nytt.  

### <a name="to-reopen-an-inventory-period"></a>Åpne en lagerperiode på nytt  
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Lagerperioder**, og velg deretter den relaterte koblingen.  
2. Velg lagerperioden du vil åpne på nytt.  
3. Velg **Åpne periode på nytt**. Bekreft at du vil åpne perioden på nytt.  
4. Alle lagerperioder med sluttdatoer som er senere enn perioden du valgte, åpnes på nytt.  

## <a name="see-also"></a>Se også  
[Designdetaljer: Beholdningsperioder](design-details-inventory-periods.md)  
[Finans](finance.md)  
[Lager](inventory-manage-inventory.md)  
[Arbeide med Dynamics NAV](ui-work-product.md)

