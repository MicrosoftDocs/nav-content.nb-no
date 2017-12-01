---
title: Gjennomgang - beregne varer i arbeid for et prosjekt
description: "Med jobber kan du planlegge forbruket av selskapets ressurser og holde rede på de ulike kostnadene som er knyttet til ressursene i et bestemt prosjekt. Prosjekter omfatter forbruk av ansattes arbeidstid, maskindriftstid, lagervarer og andre typer forbruk som må spores etter hvert som et prosjekt går fremover."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ea0953192454302a83a9187cd6569905723fd150
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="walkthrough-calculating-work-in-process-for-a-job"></a>Gjennomgang: beregne varer i arbeid for et prosjekt
Med jobber kan du planlegge forbruket av selskapets ressurser og holde rede på de ulike kostnadene som er knyttet til ressursene i et bestemt prosjekt. Prosjekter omfatter forbruk av ansattes arbeidstid, maskindriftstid, lagervarer og andre typer forbruk som må spores etter hvert som et prosjekt går fremover. Hvis et prosjekt varer i en lang periode, vil du kanskje overføre disse kostene til en VIA-konto (varer i arbeid) i balansen mens prosjektet fullføres. Du kan deretter føre kost og salg i resultatregnskapskontiene når det blir aktuelt.  

## <a name="about-this-walkthrough"></a>Denne gjennomgangen  
 Denne gjennomgangen tar for seg følgende oppgaver:  

-   Beregning av VIA  
-   Valg av VIA-beregningsmetode  
-   Utelatelse av en del av et prosjekt fra VIA.  
-   Bokføring av VIA i Finans.  
-   Tilbakeføring av en VIA-bokføring  

 I hvert trinn av fremgangsmåten blir verdien av prosjekttransaksjonene beregnet, og deretter blir de flyttet til Finans. Beregnings- og bokføringstrinnene atskilles for å gjøre det enklere å se gjennom dataene og foreta endringer før bokføring i Finans. Derfor bør du sørge for at all informasjon er riktig etter at du har kjørt beregningskjørslene, og før du kjører bokføringskjørslene.  

## <a name="roles"></a>Roller  
 I denne gjennomgangen brukes Marie (medlem i prosjektgruppen) som rollefiguren.  

## <a name="prerequisites"></a>Forutsetninger  
 Før du kan utføre oppgavene i gjennomgangen, må [!INCLUDE[d365fin](includes/d365fin_md.md)] være installert på datamaskinen.  

## <a name="story"></a>Hovedscenario  
 Denne gjennomgangen fokuserer på Cronus Norge AS, et design- og konsulentfirma som designer og innreder nye infrastrukturer, for eksempel konferanserom og kontorer, med møbler, tilbehør og reoler. Mesteparten av arbeidet i CRONUS er prosjektorientert og Marie, et prosjektgruppemedlem bruker prosjekter til å ha oversikt over hvert pågående prosjekt som CRONUS har startet, og også prosjekter som er fullført. Noen av prosjektene kan være svært lange og kan kjøre over måneder. Marie kan bruke en VIA-konto til å registrere varer i arbeid og spore kostnadene i hele prosjektet.  

## <a name="calculating-wip"></a>Beregne VIA  
 CRONUS har tatt på seg et langvarig prosjekt som nå har strukket seg over rapporteringsperioder. Marie, et medlem i prosjektgruppen, beregner varene i arbeid (VIA) for å sikre at regnskapet for selskapet blir nøyaktig.  

 I løpet av denne fremgangsmåten skal Marie velge en bestemt gruppe oppgaver som skal tas med i VIA-beregningen. Hun kan angi disse linjene i kolonnen **VIA-sum** i vinduet **Prosjektoppgavelinjer**.  

 Tabellen nedenfor beskriver de tre alternativene.  

|Felt|Beskrivelse|  
|-------------------------------------|---------------------------------------|  
|**<blank>**|La stå tomt hvis jobb-aktiviteten er en del av en gruppe med aktiviteter.|  
|**I alt**|Definerer området eller gruppen med aktiviteter som er inkludert i beregningen av VIA og føringer. Alle prosjektoppgaver med **Prosjektoppgavetype** satt til **Bokføring** i gruppen, tas med i VIA-summen, med mindre feltet **VIA-sum** er satt til **Utelatt**.|  
|**Utelatt**|Gjelder bare for en oppgave der **Prosjektoppgavetype** er **Bokføring**. Oppgaven er ikke inkludert ved beregning av VIA og føring.|  

 I den følgende gjennomgangen bruker Marie metoden Kostverdi, standarden i selskapet, til å beregne VIA. Hun angir hvilken del av jobben som skal inkluderes i VIA-beregningen ved å tilordne VIA-sumverdier til forskjellige prosjektoppgavelinjer.  

### <a name="to-calculate-wip"></a>Slik beregner du VIA:  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Prosjekter**, og velg deretter den relaterte koblingen.  
2.  I **Prosjekter**-listen velger du **Klepp Datakontor A/s**-prosjektet, og velger deretter **Rediger**-handlingen. Dermed åpnes prosjektkortet i redigeringsmodus.  

     VIA kan beregnes basert på Kostverdi, Salgsverdi, Løpende eller Ved avslutning. I dette eksemplet bruker CRONUS metoden Kostverdi.  

3.  Velg **VIA-metode** på hurtigfanen **Bokføring**, og velg deretter **Kostverdi**.  
4.  Velg **Prosjektoppgavelinjer**-handlingen og angi følgende verdier i **VIA-sum**-feltet.  

     Tabellen nedenfor beskriver verdiene.  

    |Prosjektoppgavenr.|Feltet VIA-sum|  
    |------------------|----------------------|  
    |1130|Utelatt|  
    |1190|I alt|  
    |1210|Utelatt|  
    |1310|Utelatt|  

5.  Velg **VIA**-handlingen, og velg deretter **Beregn VIA**-handlingen.  
6.  Du kan velge prosjektet du vil beregne VIA for, på kortet **Beregn VIA for prosjekt**. Velg **Klepp Datakontor A/S** i **Nr.**-feltet i hurtigfanen **Prosjekt** .  
7.  I **Bokføringsdato**-feltet angir du en dato som er senere enn arbeidsdatoen.
8.  Angi **1** i feltet **Bilagsnr.**. Dette oppretter et dokument som du kan referere til senere for sporing.  
9. Velg **OK**-knappen for å kjøre kjørselen. Det vises en melding. Velg **OK**-knappen for å fortsette. Lukk vinduet **Prosjektoppgavelinjer**.  

    > [!NOTE]  
    >  Meldingen angir at advarsler er knyttet til VIA-beregningen. Du vil gå gjennom advarslene i neste prosedyre.  

10. Utvid hurtigfanen **VIA og føring** på **Prosjekt**-kortet for å vise de beregnede verdiene. Du kan også se **VIA-bokføringsdato** og eventuelle verdier som er bokført i finans.  

 Legg merke til at verdien for **Ført kostbeløp** er 215,60 i kolonnen **Til bokføring**. Dette gjenspeiler de totale kostnadene for de to varene i gruppen med prosjektoppgavene 1110 – 1130. Det tredje elementet ble satt til **Utelatt**, og er derfor ikke inkludert i VIA-beregningen.  

### <a name="to-review-wip-warnings"></a>Se gjennom VIA-advarsler  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **VIA-cockpit for prosjekt**, og velg deretter den relaterte koblingen.  
2.  Velg prosjektet **Klepp Datakontor A/S**, og velg deretter handlingen **Vis advarsler**.  
3.  Se gjennom advarselen som er knyttet til prosjektet, i vinduet **VIA-advarsler for prosjekt**.  

 Etter denne regnskapsperioden må Marie beregne VIA på nytt for å ta med ferdig arbeid hittil.  

### <a name="to-recalculate-wip"></a>Slik beregner du VIA på nytt:  

1.  På **Prosjekt**-kortet velger du handlingen **VIA-poster** for å vise VIA-beregningen.  

     Vinduet **VIA-poster for prosjekt** viser VIA-postene som sist ble beregnet i et prosjekt, selv om VIA ennå ikke er bokført i Finans.  

2.  Følg trinnene i fremgangsmåten som forklarer hvordan du beregner VIA, for å beregne VIA på nytt. Hver gang VIA beregnes, blir det opprettet en post i vinduet **VIA-poster for prosjekt**.  
3.  Lukk vinduet.  

> [!NOTE]  
>  Varer i arbeid og føring blir bare beregnet. De bokføres ikke i finans. Hvis du vil gjøre det, må du kjøre kjørselen **Bokfør VIA i Finans** når du har beregnet VIA og føring.

## <a name="posting-wip-to-general-ledger"></a>Bokføre VIA i Finans  
 Nå som Marie har beregnet VIA for dette prosjektet, kan hun bokføre VIA i Finans.  

### <a name="to-post-wip-to-general-ledger"></a>Slik bokfører du VIA i Finans  

1.  Merk prosjektet **Klepp Datakontor A/S** i oversikten **Prosjekter**.  
2.  Velg **VIA**-handlingen, og velg deretter **Bokfør VIA i Finans**-handlingen.  
3.  Velg **Klepp Datakontor A/S** i **Nr.** på hurtigfanen **Prosjekt** i vinduet **Bokfør VIA i Finans for prosjekt**. .  
4.  Angi **1** i feltet **Bilagsnr. for tilbakeføring** i hurtigfanen **Alternativer**.  
5.  Velg **OK**-knappen for å bokføre VIA til finans.  
6.  Velg **OK**-knappen for å lukke bekreftelsesvinduet.  

     Når du har fullført bokføringen, kan du vise bokføringsopplysningene i vinduet **VIA-finansposter**.  

7.  I **Prosjekter**-listen velger du **Klepp Datakontor A/s**-prosjektet, og velger deretter **VIA-finansposter**-handlingen.  

     I vinduet **VIA-finansposter** for prosjekt, kontrollerer du at VIA er bokført i Finans.  

8.  Lukk vinduet.  
9. Åpne **Prosjekt**-kortet for prosjektet **Klepp Datakontor A/S**.  
10. Legg merke til at **Ført finanskostbeløp** nå er fylt ut i kolonnen **Bokført** på hurtigfanen **VIA og føring**, noe som indikerer at VIA er bokført i finans.  
11. Velg **OK**-knappen for å lukke kortet.  

## <a name="reversing-a-wip-posting"></a>Tilbakeføre en VIA-bokføring  
 Marie fastslår at prosjektoppgavene som ble utelatt fra beregningen av VIA, skulle ha vært beregnet i VIA. Hun kan tilbakeføre feil bokføringer uten å måtte bokføre nye VIA-bokføringer.  

### <a name="to-reverse-a-wip-posting"></a>Slik tilbakefører du en VIA-bokføring:  

1.  Merk prosjektet **Klepp Datakontor A/S** i oversikten **Prosjekter**.  
2.  Velg **VIA**-handlingen, og velg deretter **Bokfør VIA i Finans**-handlingen.  
3.  Velg **Klepp Datakontor A/S** i **Nr.** på hurtigfanen **Prosjekt** i vinduet **Bokfør VIA i Finans for prosjekt**. .  
4.  Angi **1** i feltet **Bilagsnr. for tilbakeføring** i hurtigfanen **Alternativer**.  
5.  Angi den opprinnelige bokføringsdatoen i **Bokføringsdato for tilbakeføring**. Det bør være den samme datoen som du brukte til å beregne VIA første gang.  
6.  Merk av for **Bare tilbakefør**. Dermed tilbakeføres tidligere bokført VIA, men ny VIA bokføres i Finans.  
7.  Velg **OK**-knappen for å kjøre kjørselen, og velg deretter **OK**-knappen for å lukke bekreftelsesvinduet.  
8.  Åpne **Prosjekt**-kortet for **Klepp Datakontor A/S**.  
9. På hurtigfanen **VIA og føring** kontrollerer du at det ikke finnes noen bokførte VIA-poster.  
10. Lukk dette vinduet.  
11. Velg **Klepp**-prosjektet i **Prosjekter**-listen, velg **VIA**-handlingen, og velg deretter **VIA-finansposter**. Det er merket av for **Tilbakeført** på VIA-postene.  
12. Lukk dette vinduet.  
13. Åpne **Prosjektoppgavelinjer** for prosjektet, ta med delene av prosjektet som skal være i VIA-beregningen, og gjenberegn og bokfør deretter den nye verdien i Finans.  

    > [!NOTE]  
    >  Anta at Marie har beregnet og bokført VIA for et prosjekt med feil datoer. Når hun følger metoden som ble diskutert tidligere, kan hun tilbakeføre uriktige bokføringer, rette datoene og bokføre i Finans på nytt.  

## <a name="next-steps"></a>Neste trinn  
 Denne gjennomgangen har vist deg trinnene for å beregne VIA i [!INCLUDE[d365fin](includes/d365fin_md.md)]. På større prosjekter kan det være praktisk å overføre kost til en VIA-kontoen mens prosjektet fullføres. Denne gjennomgangen har vist deg hvordan du utelater oppgavelinjer fra en beregning. Det viser deg også når du vil måtte beregne på nytt. Til slutt viser denne gjennomgangen hvordan du bokfører VIA til finans. Et eksempel på hvordan du tilbakefører en VIA-bokføring til finans, er også inkludert.  

## <a name="see-also"></a>Se også  
 [Gjennomgang av forretningsprosesser](walkthrough-business-process-walkthroughs.md)  
 [Gjennomgang: prosjektstyring](walkthrough-managing-projects-with-jobs.md)   
 [Forstå VIA-metoder](projects-understanding-wip.md)   
 [Overvåke fremdrift og prestasjon](projects-how-monitor-progress-performance.md)  
 [Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

