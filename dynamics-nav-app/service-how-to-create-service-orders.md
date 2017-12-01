---
title: Opprette serviceordrer
description: "Du kan bruke vinduet **Serviceordre** til å opprette dokumenter der du angir opplysninger om en service, for eksempel reparasjon og vedlikehold, på servicevarer etter forespørsel fra kunde."
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: aa0578c7311fcd997653c6dc6d31325abd1d367c
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-create-service-orders"></a>Opprette serviceordrer
Du kan bruke vinduet **Serviceordre** til å opprette dokumenter der du angir opplysninger om en service, for eksempel reparasjon og vedlikehold, på servicevarer etter forespørsel fra kunde.  
  
Når du oppretter en serviceordre, trenger du bare å fylle ut noen få felt. Noen av feltene er valgfrie, og mange fylles ut automatisk når du fyller ut tilknyttede felt.  
  
## <a name="to-create-a-service-order"></a>Slik oppretter du en serviceordre    
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Serviceordrer**, og velg deretter den relaterte koblingen.  
2. Opprett en ny serviceordre.  
3. I **Nr.** -feltet angir du et nummer på serviceordren.  
  
     Hvis du har definert en nummerserie for serviceordre i vinduet **Serviceoppsett**, kan du eventuelt trykke Enter for å velge det neste tilgjengelige serviceordrenummeret.  
  
4. I feltet **Kundenr.** -feltet velger du den aktuelle kunden fra listen. De kunderelevante feltene fylles ut med informasjon fra **Kunde**-tabellen.  
  
5. Avhengig av innstillingene på hurtigfanen **Obligatoriske felt** i vinduet **Serviceoppsett** kan det hende du må fylle ut feltet **Serviceordretype** og **Selgerkode**.  
6. Fyll eventuelt ut de gjenværende feltene.  
7. Registrere servicevarelinjene.  

## <a name="to-create-a-service-order-from-a-contract"></a>Slik oppretter du en serviceordre fra en kontrakt  
Du kan automatisk opprette serviceordrer for vedlikehold av servicevarer basert på servicekontrakter.  
  
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Opprett kontraktserviceordrer**, og velg deretter den relaterte koblingen.  
2. På hurtigfanen **Servicekontrakthode** angir du hvilke filtre du vil bruke.  
3. På til hurtigfanen **Alternativer**, fyller du ut feltene **Startdato** og **Sluttdato** med startdato og sluttdato for perioden som du vil opprette kontraktserviceordrer for. Kjørselen oppretter serviceordrer som omfatter servicevarer i servicekontrakter med de neste planlagte servicedatoene innenfor denne perioden.  
  
    > [!NOTE]  
    >  Det finnes en begrensning på antall dager du kan bruke som datointervall hver gang du bruker denne kjørselen. Du angir denne begrensningen i feltet **Kontraktserv.ordre - maks. dager** i vinduet **Serviceoppsett**.  
  
4. I feltet **Handling** velger du **Opprett serviceordre**.  

## <a name="to-convert-a-service-quote-to-a-service-order"></a>Slik konverterer du et servicetilbud til en serviceordre
Når en kunde har godkjent et servicetilbud, konverterer du det til en serviceordre. Tilbudet slettes, og en ny serviceordre defineres med den samme beskrivelsen som servicetilbudet. Responsdatoen og -tiden beregnes på nytt for serviceordren, og statusen settes til **I kø**. Reparasjonsstatusen til servicevarene i ordren endres til **Første**.  
  
[!INCLUDE[d365fin](includes/d365fin_md.md)] søker etter fordelingsposter for alle servicevarene i servicetilbudet med statusen **Aktiv**. Hvis programmet finner slike tildelingsposter, oppdateres tildelingsstatusen til **Ny tildeling nødvendig**. Når du tildeler servicevarene på nytt i serviceordren, oppdateres statusen for tildelingspostene som er registrert for tilbudet, til **Ferdig.**   

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Servicekontrakttilbud**, og velg deretter den relaterte koblingen.  
2. Velg servicetilbudet du vil konvertere til en serviceordre.  
3. Velg handlingen **Lag ordre**.  

## <a name="to-check-item-availability-for-one-or-more-orders"></a>Kontrollere varedisposisjon for én eller flere ordrer  
Du kan kontrollere om en vare du trenger for å innfri en ordre, er på lager. Hvis den ikke er det, kan du finne ut når den skal være på lager. Hvis en vare kan reserveres, kan du i tillegg reservere den for å sikre at den er tilgjengelig for bruk. Du kan kontrollere tilgjengeligheten for en bestemt ordre eller for alle ordrer.  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Servicefordeling**, og velg deretter den relaterte koblingen.  
2. Gjør ett av følgende:  
  
    * For én bestemt ordre velger du ordren og deretter handlingen **Behovsoversikt**.  
    * For alle ordrer velger du **Vis dokument**. **Serviceordre**-vinduet åpnes.  
  
3. Vis varegrupperingen og informasjon om tilgjengeligheten av varen på siden **Behovsoversikt**. Du kan for eksempel se hvor mange varer som er på lager. Du kan også se om og når en vare blir tilgjengelig hvis den er i restordre, det vil si at kildetypen er Kjøp, eller om den er reservert. 

## <a name="to-reserve-an-item-for-a-service-order"></a>Reservere en vare for en serviceordre
Hvis du vil være sikker på at en vare er tilgjengelig for en serviceordre, kan du reservere varen. 

1. Skriv inn **Serviceordrer** i **Søk**-boksen, og velg deretter den relaterte koblingen.  
2. Velg serviceordren, og velg deretter **Rediger**.  
3. Velg **Handlinger**, **Ordre** og deretter **Servicelinjer**.  
4. På siden **Servicelinjer** velger du varen vil reservere, og deretter velger du handlingen **Reserver**.  
5. På siden **Reservasjon** velger du **Reserver fra gjeldende linje**. 

## <a name="to-insert-lines-based-on-standard-service-codes"></a>Sette inn linjer basert på standard servicekoder  
Hvis du har definert standard servicekoder og knyttet dem til servicevaregrupper, kan du sette inn standardlinjene som er koblet til standard servicekoder, i servicedokumenter. Hvis du vil ha mer informasjon, kan du se [Definere standard servicekoder](service-how-setup-service-coding.md).   

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Serviceordrer**, og velg deretter den relaterte koblingen.  
2. Opprett en ny serviceordre.  
3. Fyll ut feltene etter behov.  
4. Legg inn nødvendig informasjon på servicevarelinjene.  
5. Velg linjen med servicevaren som du vil opprette servicelinjer for, og velg deretter **Hent standard servicekoder**. Vinduet **Standard servicevaregruppekoder** åpnes med standardkodene for servicevaregruppen som er angitt i linjen.  
6. Velg ønsket kode, og klikk på **OK**-knappen for å registrere standard servicelinjer.  
  
> [!NOTE]  
>  Hvis feltet **Servicevaregruppekode** i servicevarelinjen i dokumentet er tomt, betyr dette at servicevaren ikke tilhører noen servicevaregruppe. I dette tilfellet inneholder vinduet **Standard servicevaregruppekoder** en liste over alle standard servicekoder. Du må velge i listen hvis du vil sette inn standard servicelinjer i dokumentet. Du kan også velge i listen over standard servicekoder som er knyttet til en bestemt servicevaregruppe. Hvis du vil vise listen, velger du den aktuelle koden i feltet **Servicevaregruppekode** i vinduet **Standard servicevaregruppekoder**.  

## <a name="to-register-internal-or-public-comments"></a>Registrere interne eller offentlige merknader
Du kan legge til merknader som skrives ut på en serviceordre og servicetilbud for å angi tilleggsinformasjon. Du kan legge til opptil 80 tegn, medregnet mellomrom. Hvis du har behov for å skrive inn mer tekst, velger du en ny linje. Hvis du vil registrere en kommentar, velger du en linje og deretter handlingen **Merknader**.  

## <a name="to-delete-invoiced-service-orders"></a>Slik sletter du fakturerte serviceordrer  
Ordrer slettes vanligvis automatisk etter at de er fullstendig fakturert. Når en faktura bokføres, opprettes en tilhørende post i vinduet **Bokførte servicefakturaer**. Det bokførte dokumentet kan vises på siden **Bokført servicefaktura**.  
  
Serviceordrer slettes ikke automatisk hvis det totale antallet i ordren ikke er bokført fra selve serviceordren, men fra **Servicefaktura**-vinduet. Da må du kanskje slette fakturerte ordrer som ikke er slettet. Du kan gjøre dette ved hjelp av kjørselen **Slett fakturerte serviceordrer**.  

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Slett fakturerte serviceordrer**, og velg deretter den relaterte koblingen. Forespørselsvinduet for kjørselen **Slett fakturerte serviceordrer** åpnes.  
2. Du kan velge ordrene som skal slettes ved å definere filtre i **Nr.**-, **Kundenr.**- og **Fakturatil-kundenr.**- -feltene.  
3. Velg **OK**.  


## <a name="see-also"></a>Se også  
[Servicebokføring](service-service-posting.md)  
[Bokføre en serviceordre](service-how-to-post-service-orders.md)  
[Konfigurere servicehåndtering](service-setup-service.md)  
[Arbeide med serviceoppgaver](service-how-to-work-on-service-tasks.md)  
[Tildele ressurser](service-how-to-allocate-resources.md)  

