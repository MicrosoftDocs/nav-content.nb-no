---
title: Beregne ordrebekreftelsesdatoer
description: "Ordrebekreftelsesfunksjonen er et verktøy for beregning av når en vare tidligst kan leveres. Den oppretter i tillegg forslagslinjer for datoene du godtar."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/10/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 5c2167397d95d04c937ddf1820e6e9edff906b2f
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-calculate-order-promising-dates"></a>Beregne ordrebekreftelsesdatoer
Et firma må være i stand til å informere kundene om ordreleveringsdatoer. Med vinduet **Ordrebekreftelseslinjer** kan du gjøre dette fra en salgsordrelinje.  

Basert på en vares kjente og forventede tilgjengelighetsdatoer beregner [!INCLUDE[d365fin](includes/d365fin_md.md)] forsendelses- og leveringsdato på et øyeblikk, som deretter kan loves kunden.  

Hvis du angir en ønsket leveringsdato på en ordrelinje, brukes denne datoen som utgangspunkt for følgende beregninger:  

- ønsket leveringsdato - leveringstid = planlagt forsendelsesdato  
- planlagt forsendelsesdato - utgående lagerhåndteringstid = forsendelsesdato  

Hvis varene er tilgjengelige for plukking på forsendelsesdatoen, kan salgsprosessen fortsette. Hvis ikke varene er tilgjengelige for plukking på forsendelsesdatoen, vises en advarsel om at det er tomt på lager.  

Hvis du ikke angir en ønsket leveringsdato på ordrelinjen, eller hvis ønsket leveringsdato ikke kan innfris, beregnes datoen som varene tidligst er tilgjengelige på. Denne datoen angis deretter i feltet **Forsendelsesdato** på linjen, og datoen du planlegger å sende og levere varene til kunden på beregnes også ved hjelp av følgende beregninger.  

- forsendelsesdato + utgående lagerhåndteringstid = forsendelsesdato  
- planlagt forsendelsesdato + leveringstid = planlagt leveringsdato  

## <a name="about-order-promising"></a>Om ordrebekreftelse
Med funksjonen for ordrebekreftelse kan du gi løfte om at en ordre skal leveres en bestemt dato. Datoen da en vare er tilgjengelig for ordre (ATP) eller varens første mulige forsendelsesdato (CTP) beregnes, og ordrelinjer opprettes for disse datoene som du godtar. Funksjonen beregner når en vare tidligst kan leveres. Den oppretter i tillegg forslagslinjer, i tilfelle varene først må kjøpes for datoene du godtar.

[!INCLUDE[d365fin](includes/d365fin_md.md)] bruker to grunnleggende begreper:  

- Tilgjengelig for ordre (ATP)  
- Første mulige forsendelsesdato (CTP)  

### <a name="available-to-promise"></a>Tilgjengelig for ordre (ATP)  
Tilgjengelig for ordre (ATP) beregner datoer basert på reservasjonssystemet. Den utfører en tilgjengelighetskontroll for de ureserverte antallene på lager i forhold til planlagt produksjon, kjøp, overføringer og ordrereturer. Basert på denne informasjonen beregner [!INCLUDE[d365fin](includes/d365fin_md.md)] automatisk leveringsdatoen for kundens ordre fordi varene er tilgjengelige, enten på lager eller i planlagte mottak.  

### <a name="capable-to-promise"></a>Første mulige forsendelsesdato (CTP)  
Første mulige forsendelsesdato (CTP) forutsetter et "Hva om"-scenario der varen ikke er på lager og ingen ordrer er planlagt. Basert på dette scenariet beregner [!INCLUDE[d365fin](includes/d365fin_md.md)] den tidligste datoen varen kan være tilgjengelig, hvis den skal produseres, kjøpes eller overføres.  


### <a name="calculations"></a>Beregninger  
Når [!INCLUDE[d365fin](includes/d365fin_md.md)] beregner kundens leveringsdato, utføres to oppgaver:  

- Beregner den tidligste leveringsdatoen når kunden ikke har bedt om en bestemt leveringsdato.  
- Kontrollerer om leveringsdatoen som kunden har bedt om, eller som du har lovet kunden, er realistisk.  

Hvis kunden ikke ber om en bestemt leveringsdato, brukes arbeidsdatoen som leveringsdato, og tilgjengelighet baseres deretter på denne datoen. Hvis varen er på lager, beregner [!INCLUDE[d365fin](includes/d365fin_md.md)] fremover i tid for å fastsette når ordren kan leveres. Dette kan gjøres med følgende formler:  

- Forsendelsesdato + Utgående lager + Planlagt forsendelse + Håndteringstid = Dato  
- Planlagt forsendelsesdato + Leveringstid = Planlagt leveringsdato  

[!INCLUDE[d365fin](includes/d365fin_md.md)] kontrollerer deretter om beregnet leveringsdato er realistisk ved å beregne bakover i tid, for å bestemme når varen må være tilgjengelig for å overholde datoen som ble lovet. Dette kan gjøres med følgende formler:  

- Planlagt forsendelsesdato - Leveringstid = Planlagt leveringsdato  
- Planlagt forsendelsesdato - Utgående lagerhåndteringstid = Forsendelsesdato  

Leveringsdatoen brukes til å utføre tilgjengelighetskontrollen. Hvis varen er tilgjengelig på denne datoen, bekrefter [!INCLUDE[d365fin](includes/d365fin_md.md)] at forespurt/lovet levering kan innfris ved å angi at planlagt leveringsdato skal være lik forespurt/lovet leveringsdato. Hvis varen ikke er tilgjengelig, returneres en tom dato, og ordrebehandleren kan deretter bruke CTP-funksjonalitet.  

Basert på nye datoer og klokkeslett beregnes alle relaterte datoer i henhold til formlene som er oppført tidligere i denne delen. CTP-beregningen tar lengre tid, men den gir en nøyaktig dato for når kunden kan forvente å få varen levert. Datoene som er beregnes fra CTP, vises i feltene **Planlagt lev.dato** og **Tidligste forsendelsesdato** i vinduet **Ordrebekreftelseslinjer**.  

Ordrebehandleren fullfører CTP-prosessen ved å godta datoene. Dette betyr at en planleggingslinje og en reservasjonspost opprettes for varen før de beregnede datoene for å sikre at ordren blir dekket.  

I tillegg til den eksterne ordrebekreftelsen som du kan utføre i vinduet **Ordrebekreftelseslinjer** , kan du også bekrefte interne eller eksterne leveringsdatoer for stykklistevarer. Hvis du vil ha mer informasjon, kan du se [Vise tilgjengeligheten av varer](inventory-how-availability-overview.md).

## <a name="to-set-up-order-promising"></a>Slik angir du ordrebekreftelser  
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Oppsett for ordrebekreftelse**, og velg deretter den relaterte koblingen.  
2. Angi et nummer og en tidsenhetskode i feltet **Iverksett (tid)**. Velg én av følgende koder.  

    |Kode|Beskrivelse|  
    |----------|-----------------|  
    |**d**|Kalenderdag|  
    |**a**|Uke|  
    |**m**|Måned|  
    |**k**|Kvartal|  
    |**å**|År|  

    "3u" betyr for eksempel at Iverksett (tid) er tre uker. Bruk "n" som prefiks til en av disse kodene for å angi nåværende periode. Hvis du for eksempel vil at Iverksett (tid) skal være nåværende måned, angir du **nm**.  
3. Angi en nummerserie i feltet **Ordrebekreftelsesnr.**. ved å velge en linje fra listen i vinduet **Nr. serie**.  
4. Angi en ordrebekreftelsesmal i feltet **Ordrebekreftelsesmal** ved å velge en linje fra oversikten i vinduet **Best.forslagsmal - oversikt**.  
5. Angi et bestillingsforslag i feltet **Ordrebekreftelsesskjema** ved å velge en linje fra oversikten i vinduet **Best.forslagsnavn**.

### <a name="to-enter-inbound-warehouse-handling-time-in-the-inventory-setup-window"></a>Slik angir du inngående lagerhåndteringstid i lageroppsettvinduet  
Hvis du vil at lagerhåndteringstid skal tas med i beregningen av ordrebekreftelse på bestillingslinjen, kan du definere den som standard for lageret og lokasjonen.    
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Lageroppsett**, og velg deretter den relaterte koblingen.  
2. På hurtigfanen **Generelt** i feltet **Inngående lagerhåndteringstid** angir du hvor mange dager som skal tas med i beregningen av ordrebekreftelsen.  

> [!NOTE]  
>  Hvis du har fylt ut feltet **Inngående lagerhåndteringstid** på **lokasjonskortet** for lokasjonen, brukes dette feltet som standard for inngående lagerhåndteringstid.  

### <a name="to-enter-inbound-warehouse-handling-time-on-location-cards"></a>Slik angir du inngående lagerhåndteringstid på lokasjonskort  
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Lokasjon**, og velg deretter den relaterte koblingen.  
2.  Åpne det aktuelle lokasjonskortet.  
3.  På hurtigfanen **Lager** i feltet **Inngående lagerhåndteringstid** angir du hvor mange dager som skal tas med i beregningen av ordrebekreftelsen.  

> [!NOTE]  
>  Hvis du lar feltet **Inngående lagerhåndteringstid** stå tomt, brukes verdien i **Lageroppsett**-vinduet i beregningen.

### <a name="to-enter-outbound-warehouse-handling-time-in-the-inventory-setup-window"></a>Slik angir du utgående lagerhåndteringstid i lageroppsettvinduet  
Hvis du vil definere en utgående lagerhåndteringstid slik at den tas med i beregningen av ordrebekreftelsen på salgslinjen, kan du definere dette som standard for lageret.

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Lageroppsett**, og velg deretter den relaterte koblingen.  
2. På hurtigfanen **Generelt** i feltet **Utgående lagerhåndteringstid** angir du hvor mange dager som skal tas med i beregningen av ordrebekreftelsen.  

> [!NOTE]  
>  Hvis du har fylt ut feltet **Utgående lagerhåndteringstid** på lokasjonskortet for lokasjonen, brukes dette feltet som standard for utgående lagerhåndteringstid.  

### <a name="to-enter-outbound-warehouse-handling-time-on-location-cards"></a>Slik angir du utgående lagerhåndteringstid på lokasjonskort  
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Lokasjoner**, og velg deretter den relaterte koblingen.  
2.  Åpne det aktuelle lokasjonskortet.  
3.  På hurtigfanen **Lager** i feltet **Utgående lagerhåndteringstid** angir du hvor mange dager som skal tas med i beregningen av ordrebekreftelsen.  

> [!NOTE]  
>  Hvis du lar feltet **Utgående lagerhåndteringstid** stå tomt, brukes verdien i **Lageroppsett**-vinduet i beregningen.

## <a name="to-make-an-item-critical"></a>Slik gjør du en vare kritisk  
Før en vare kan inkluderes i beregningen av ordrebekreftelsen, må den være merket som kritisk. Dette oppsettet sikrer at ikke-kritiske varer ikke fører til uaktuell beregning av ordrebekreftelser.   
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Varer**, og velg deretter den relaterte koblingen.  
2.  Åpne det aktuelle varekortet.  
3.  På hurtifganen **Planlegging** velger du **Kritisk**-feltet.  

## <a name="to-calculate-an-order-promising-date"></a>Slik beregner du en ordrebekreftelsesdato  
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Ordre**, og velg deretter den relaterte koblingen.  
2.  Åpne den aktuelle ordren, og velg ordrelinjene du vil at programmet skal beregne.  
3.  Velg handlingen **Ordrebekreftelse** og deretter **Ordrebekreftelseslinjer**.  
4.  Velg en linje, og velg deretter ett av følgende alternativer:  

    - Velg **Tilgjengelig for ordre (ATP)** hvis du vil beregne når varen tidligst vil være tilgjengelig med hensyn til beholdning, tidsplanlagte mottak og bruttobehov.  
    - Velg **Første mulige forsendelsesdato (CTP)** hvis du vet at varen er utsolgt fra lager og du vil beregne når varen tidligst vil være tilgjengelig når du utsteder nye etterfyllingsforslag.  
5.  Velg **Godta**-knappen for å godta den tidligste leveringsdatoen som er tilgjengelig.  

## <a name="see-also"></a>Se også  
[Salg](sales-manage-sales.md)  
[Beregne dato for kjøp](purchasing-date-calculation-for-purchases.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

