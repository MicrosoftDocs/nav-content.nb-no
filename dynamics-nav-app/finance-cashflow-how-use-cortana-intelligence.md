---
title: "Prediktive kontantstrømprognoser"
author: bholtorf
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f657509fc2195674db81f47bc5ae31b7ba1aa40e
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-make-predictive-cash-flow-forecasts"></a>Prediktive kontantstrømprognoser
Kontantstrømprognoser hjelper deg med å sikre at selskapet har nok kontanter til å dekke sine økonomiske forpliktelser, og er nyttig for å identifisere justeringer. Hvis du for eksempel har et kontantoverskudd, kan du betale ned litt gjeld, og du verdsetter en tidlig advarsel hvis tidsfrister nærmer seg. 

Cortana Intelligence bruker Azure Machine Learning-tjenesten for å gjøre pålitelige, prediktive prognoser. Prognoser fra Cortana Intelligence kan for eksempel hjelpe deg med å forutse, og unngå, kontantunderskudd. Tjenesten kombinerer historisk informasjon med gjeldende bokføringer for kunde og leverandør, inkludert bokføringer med forfallsdatoer som er i fremtiden. Disse omfatter:
* Bestillinger
* Ordrer
* Bokførte salgs og kjøpsfakturaer
* Kreditnotaer

## <a name="before-you-start"></a>Før du begynner  
Det er noen ting du må gjøre før du kan bruke Cortana Intelligence for kontantstrømprognoser: 
* Hvis du ikke allerede bruker kontantstrømprognoser, må du konfigurere:
    * Én eller flere oppsett i **Kontantstrømoppsett**. 
    * Kontoer for leverandører, kunder, salgsordrer og bestillinger. Cortana Intelligence bruker bokføringene i disse kontoene.
    * Én eller flere kontantstrømprognoser i **Kontantstrømprognose**. Husk å ta med bestillinger, salgsordrer, kunder og leverandører som kilde.  
    Hvis du vil ha mer informasjon, kan du søke etter _kontantstrømprognoser_ i hjelpesystemet. 
* Kjenn URL-API og API-nøkkel som skal brukes for webtjenesten for prediksjonsanalyse.  
    Du kan bruke Azure Machine Learning eller en annen tjeneste, hvis du har en. En offentlig modell kalt _Forecasting Model for Microsoft Dynamics NAV_ er også tilgjengelig på Internett i Cortana Intelligence Gallery. Hvis du vil bruke modellen, følger du denne fremgangsmåten:

    1. Åpne en nettleser, og gå til [Cortana Intelligence Gallery](https://go.microsoft.com/fwlink/?linkid=828352)
    2. Søk etter _Forecasting Model for Microsoft Dynamics NAV_, og åpne deretter modellen i Azure Machine Learning Studio.
    3. Bruke Microsoft-kontoen til å registrere deg for et arbeidsområde, og kopier deretter modellen.
    4. Kjør modellen, og publisere den som en webtjeneste.
    5. Noter URL-API og API-nøkkel. Du vil bruke disse legitimasjonene når du konfigurerer Cortana Intelligence i Microsoft Dynamics NAV.  

* Vurdere hvor ofte du vil beregne prognosen. Azure Machine Learning-tjenesten har begrensninger med hensyn til bruk. Hvis du for eksempel har mange varer, kan det være bedre å beregne sjeldnere. 
* Vær tilordnet rollesenteret for regnskapsfører. 

## <a name="set-up-cortana-intelligence"></a>Konfigurer Cortana Intelligence
Du kan bruke en assistert oppsettsveiledning til å definere kontantstrømprognoser. Veiledningen hjelper deg med å angi informasjon, for eksempel hvor ofte prognosen skal oppdateres, kontoene som den skal baseres på, informasjon om når du betaler skatt, og om du vil bruke Cortana Intelligence.  

Hvis du allerede bruker kontantstrømprognoser og bare vil aktivere Cortana Intelligence, kan du også bruke en manuell prosess. Når du logger på, viser en melding på et blått felt øverst i arbeidsområdet. Hvis du vil definere Cortana Intelligence umiddelbart, kan du velge **Ja,takk**. Meldingen viser bare én gang. Hvis du lukker den, kan du bruke den manuelle prosessen for å definere Cortana Intelligence.  

**Tips:** Ta hensyn til lengden på periodene som tjenesten vil bruke i beregningene. Jo mer data du angir, jo mer nøyaktig vil forutsigelsene være. Vær også oppmerksom på store avvik i perioder. De vil også ha innvirkning på forutsigelser. Hvis Cortana Intelligence ikke finner nok data eller dataene varierer mye, vil ikke tjenesten utføre en forutsigelse. 

Slik bruker du den assisterte oppsettsveiledningen:
1. I rollesenter for regnskapsfører, under diagrammet **Kontantstrømprognose**, velger du handlingen **Åpne assistert oppsett**.
2. Fyll ut feltene etter behov i hvert trinn av veiledningen.

Slik bruker du en manuell prosess:
1. Søk etter **Kontantstrømoppsett**, og velg deretter den relaterte koblingen.
2. Vis hurtigfanen **Cortana Intelligence**, og fyll deretter ut feltene etter behov.

## <a name="turn-on-cortana-intelligence-for-cash-flow-forecasts"></a>Aktivere Cortana Intelligence for kontantstrømprognoser
1. Søk etter **Kontantstrømprognoser**, og velg deretter den relaterte koblingen.
2. Velg handlingen **Kontantstrømforslag**.
3. På siden **Kontantstrømforslag** velger du handlingen **Foreslå forslagslinjer**.  
4. Under **Kildetyper som skal inkluderes**, merker du av for **Cortana Intelligence-prognose**.

## <a name="investigate-a-cash-flow-forecast"></a>Undersøke en kontantstrømprognose
Hvis du vil undersøke dataene bak prognosen, inkludert avviket, velger du kolonnen **Cortana Intelligence**. Den første raden i tabellen viser avviket. De andre radene er ordnet etter kildedokument.  

Du kan for eksempel se hvordan prognosen:    
* Håndterer bekreftede salg og innkjøp 
* Trekker fra tilgodehavende og legger til skyldig beløp
* Hopper over dupliserte salgsordrer og bestillinger

## <a name="see-also"></a>Se også  
[Arbeide med Dynamics NAV](ui-work-product.md)

