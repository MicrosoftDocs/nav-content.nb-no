---
title: Opprette en produksjonsprognose
description: Du kan opprette salgs- og produksjonsprognoser i vinduet **Produksjonsprognose**.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 106e75dbe6f1fca00ba09a19eeafb965fa83f4ea
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-a-production-forecast"></a>Opprette en produksjonsprognose
Du kan opprette salgs- og produksjonsprognoser i **Produksjonsprognose**-vinduet.  

Prognosefunksjonalitet brukes til å opprette forventet behov. Faktisk behov opprettes basert på ordrer og produksjonsordrer. Under oppretting av MPS (Master Production Schedule) nettoberegnes prognosen mot salgs- og produksjonsordrer. *Komponenten*-alternativet på prognosen bestemmer hvilken kravtype som skal tas i betraktning i nettoavregningsprosessen. Hvis prognosen er for en salgsvare, nettoberegnes prognosen bare mot ordrer. Hvis det er for komponenter, nettoberegnes prognosen bare mot produksjonsordrekomponenter.  

Prognoser gir selskapet muligheten til å lage "hva om"-scenarier og å planlegge for og dekke behov effektivt og kostnadseffektivt. Nøyaktige prognoser kan være av avgjørende betydning for nivået av kundetilfredshet når det gjelder ordrebekreftelsesdatoer og punktlig levering.  

## <a name="sales-forecasts-and-production-forecasts"></a>Salgsprognoser og produksjonsprognoser  
Prognosefunksjonaliteten i programmet kan brukes til å opprette salgs- eller produksjonsprognoser, kombinert eller uavhengig av hverandre. De fleste selskaper som produserer varer til ordrer, har for eksempel ikke ferdige varer på lager siden hver vare produseres når den bestilles av kunden. Å kunne forutse ordrer (via salgsprognoser) er avgjørende for å oppnå en rimelig gjennomløpstid for de ferdige varene (via produksjonsprognoser). Komponentdeler med lange leveringstider kan for eksempel forsinke produksjonen hvis de ikke er bestilt eller på lager.  

-   Salgsprognosen er salgsavdelingens beste antakelse om hva som kommer til å bli solgt i fremtiden, og angis etter vare og etter periode. Salgsprognosen er imidlertid ikke alltid tilstrekkelig for produksjon.  
-   Produksjonsprognosen er produksjonsplanleggerens beregning av hvor mange sluttvarer og avledede halvfabrikata som skal produseres i bestemte perioder for å oppfylle salgsprognosen.  

I de fleste tilfeller endrer produksjonsplanleggeren salgsprognosen slik at den passer til produksjonsbetingelsene, men fortsatt oppfyller salgsprognosen.  

Du oppretter prognoser manuelt i vinduet **Produksjonsprognose**. Det kan finnes flere prognoser i systemet, og de skilles med navn og type. Du kan kopiere og redigere prognoser etter behov. Merk at bare én prognose er gyldig for planleggingsformål om gangen.  

Prognosen består av poster med varenummer, prognosedato og prognoseantall. Prognosen for en vare dekker en periode, som defineres av prognosedatoen og prognosedatoen til den neste (senere) prognoseposten. Fra en planleggingssynsvinkel må prognoseantallet være tilgjengelig ved begynnelsen av behovsperioden.  

Du må angi en prognose som *Salgsvare*, *Komponent* eller *Begge*. Prognosetypen *Salgsvare* brukes til salgsprognoser. Du oppretter produksjonsprognosen ved å bruke *Komponent*-typen. Prognosetypen *Begge* brukes bare til å gi planleggeren en oversikt over både salgsprognosen og produksjonsprognosen. Hvis du velger dette alternativet, kan ikke prognosepostene redigeres. Når du angir disse prognosetypene her, kan du bruke det samme forslaget til å angi en salgsprognose slik du angir en produksjonsprognose, og til å vise begge prognosene samtidig. Merk at systemet behandler de ulike inndataene (salg og produksjon) på ulike måter ved beregning av planlegging, basert på vare og produksjonsoppsett.  

## <a name="component-forecast"></a>Komponentprognose  
Komponentprognosen kan ses på som en prognose for en valgfri enhet i forbindelse med en overordnet vare. Dette kan for eksempel være nyttig hvis planleggeren kan anslå behovet for komponenten.  

Siden komponentprognosen er utformet for å definere valgfrie enheter for en overordnet vare, skal komponentprognosen være lik eller mindre enn salgsvareprognoseantallet. Hvis komponentprognosen er større enn salgsvareprognosen, behandler systemet avviket mellom disse to prognosetypene som uavhengig behov.  

## <a name="forecasting-periods"></a>Prognoseperioder  
 Prognoseperioden er gyldig fra sin egen startdato frem til startdatoen for den neste prognosen. I tidsintervallvinduet kan du velge mellom flere alternativer for å sette inn behovet på en bestemt dato i en periode. Det anbefales derfor at du ikke endrer prognoseperiodeomfanget med mindre du vil flytte alle prognoseposter til startdatoen i denne perioden.  

## <a name="forecast-by-locations"></a>Prognose etter lokasjoner  
Det kan angi i produksjonsoppsettet om. Merk imidlertid at hvis du viser lokasjonsbaserte prognoser isolert, kan det hende at den samlede prognosen ikke er representativ.

## <a name="to-create-a-production-forecast"></a>Slik oppretter du en produksjonsprognose

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Produksjonsprognose**, og velg deretter den relaterte koblingen.  
2.  På hurtigfanen **Generelt** velger du en prognose i feltet **Navn på prod.prognose**. Det kan finnes flere prognoser, og de skilles med navn og prognosetype.  
3.  I **Lokasjonsfilter**-feltet velger du lokasjonen som denne prognosen skal brukes på.  
4.  Velg **Salgsvare**, **Komponent** eller **Begge** i **Prognosetype**-feltet. Hvis du velger **Salgsvare** eller **Komponent**, kan du redigere antallet etter periode. Hvis du velger **Begge**, kan du ikke redigere antallet, men du kan velge rullegardinpilen og vise postene for produksjonsprognose.  
5.  Angi et **Datofilter** hvis du vil begrense mengden data som vises.  
6.  På hurtigfanen **Matrise for produksjonsprognose** angir du de prognostiserte antallene for **Salgsvare**- eller **Komponent**-prognose for de ulike periodene.  
7.  På hurtigfanen **Matrisealternativer** angir du tidsintervallet i **Vis etter**-feltet for å endre perioden som vises i hver kolonne. Du kan velge mellom følgende intervaller: **Dag**, **Uke**, **Måned**, **Kvartal**, **År** eller **Regnskapsperiode**, som definert i Økonomistyring.  

    > [!NOTE]  
    >  Du bør vurdere hvilket tidsintervall du vil bruke i fremtidige prognoser, slik at det blir konsekvent. Når du angir et prognoseantall, er det gyldig den første dagen i tidsintervallet du velger. Hvis du for eksempel velger en måned, angir du prognoseantallet på den første dagen i måneden. Hvis du velger et kvartal, angir du prognoseantallet på den første dagen i den første måneden i kvartalet.  

8.  I **Vis som**-feltet velger du hvordan de prognostiserte antallene skal vises for tidsintervallet. Hvis du velger **Bevegelse**, vises nettoendringen i saldo for tidsintervallet. Hvis du velger **Saldo per dato**, viser vinduet saldoen per den siste dagen i tidsintervallet.  

> [!NOTE]  
>  Du kan også redigere en eksisterende prognose. Velg **Kopier produksjonsprognose** i vinduet **Matrise for produksjonsprognose**, og fyll ut **Produksjonsprognose**-vinduet med en eksisterende prognose. Deretter kan du redigere antall etter behov.  

## <a name="see-also"></a>Se også  
[Definere produksjon](production-configure-production-processes.md)  
[Produksjon](production-manage-manufacturing.md)    
[Lager](inventory-manage-inventory.md)  
[Innkjøp](purchasing-manage-purchasing.md)  
[Designdetaljer: Forsyningsplanlegging](design-details-supply-planning.md)   
[Anbefalte fremgangsmåter for oppsett: Forsyningsplanlegging](setup-best-practices-supply-planning.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

