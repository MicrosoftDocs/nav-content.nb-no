---
title: Opprette arbeidsflyter
description: "Du kan opprette arbeidsflyter som kobler forretningsprosessoppgaver som utføres av forskjellige brukere. Systemoppgaver, for eksempel automatisk bokføring, kan tas med som trinn i arbeidsflyter, før eller etterfulgt av brukeroppgaver. Å be om og gi godkjenning til å opprette nye oppføringer er typiske arbeidsflyttrinn."
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: fcf0a0c9ffc12de6fe21adb2a0906f241374aa2c
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-workflows"></a>Opprette arbeidsflyter
Du kan opprette arbeidsflyter som kobler forretningsprosessoppgaver som utføres av forskjellige brukere. Systemoppgaver, for eksempel automatisk bokføring, kan tas med som trinn i arbeidsflyter, før eller etterfulgt av brukeroppgaver. Å be om og gi godkjenning til å opprette nye oppføringer er typiske arbeidsflyttrinn.  

I **Arbeidsflyt**-vinduet oppretter du en arbeidsflyt ved å føre opp de involverte trinnene på linjene. Hvert trinn består av en arbeidsflythendelse endret av hendelsesbetingelsene og et arbeidsflytsvar med svaralternativer. Du definerer arbeidsflyttrinn ved å fylle ut felt på arbeidsflytlinjer fra faste lister over verdier for hendelse og svar som representerer scenarier som støttes av programkoden.  

Når du oppretter arbeidsflyter, kan du kopiere trinnene fra eksisterende arbeidsflyter eller arbeidsflytmaler. Arbeidsflytmaler representerer ikke-redigerbare arbeidsflyter som finnes i den generelle versjonen av [!INCLUDE[d365fin](includes/d365fin_md.md)]. Koden for arbeidsflytmaler som er lagt inn av Microsoft, har prefikset "MS-", som i "MS PIW". Hvis du vil ha mer informasjon, kan du se [Opprette arbeidsflyter fra arbeidsflytmaler](across-how-to-create-workflows-from-workflow-templates.md).  

Hvis forretningsscenarioet krever arbeidsflythendelser eller svar som ikke støttes, må en Microsoft-partner implementere dem ved å tilpasse programkoden.  
  
> [!NOTE]  
>  Alle varsler om arbeidsflyttrinn sendes via en jobbkø. Kontroller at jobbkøen i installasjonen er definert til å håndtere arbeidsflytvarsler, og at det er merket av for **Start automatisk fra NAS**. Hvis du vil ha mer informasjon, kan du se [Bruke jobbkøer til å planlegge oppgaver](admin-job-queues-schedule-tasks.md).  

## <a name="to-create-a-workflow"></a>Slik oppretter du en arbeidsflyt:  
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Arbeidsflyter**, og velg deretter den relaterte koblingen.  
2. Velg handlingen **Ny**. Vinduet **Arbeidsflyt** åpnes.  
3. I **Kode**-feltet angir du maksimalt 20 tegn for å identifisere arbeidsflyten.  
4. For å opprette en arbeidsflyt fra en arbeidsflytmal, velg **Opprett arbeidsflyt fra mal** i **Arbeidsflyter**-vinduet. Hvis du vil ha mer informasjon, kan du se [Opprette arbeidsflyter fra arbeidsflytmaler](across-how-to-create-workflows-from-workflow-templates.md).  
5. I **Beskrivelse**-feltet beskriver du arbeidsflyten.  
6. I feltet **Kategori**, angi hvilken kategori arbeidsflyten tilhører.  
7. I **Når hendelse**-feltet angir du hendelsen som må inntreffe for å starte arbeidsflyttrinnet.  

    Når du velger feltet, åpnes vinduet **Arbeidsflythendelser**, der du kan velge fra alle arbeidsflythendelser som finnes.  
8. I feltet **Betingelse** angir du én eller flere betingelser som må oppfylles før hendelsen i feltet **Når hendelse** kan forekomme.  

    Når du velger feltet, åpnes vinduet **Hendelsesbetingelser** der du velger fra en liste over filterfelt som er aktuelle som betingelser for den aktuelle hendelsen. Du kan legge til nye filterfelt som du vil bruke som vilkår for hendelsen. Du kan angi filtre for hendelsesbetingelse på samme måte som du angir filtre på rapportforespørselssider.  

    Hvis arbeidsflythendelsen er en endring av et bestemt felt i en post, åpnes **Hendelsesvilkår**-vinduet med alternativer for å velge feltet og typen endring.  

    1.  For å angi en feltendring for hendelsen, velger du feltet som endres i **Hendelsesvilkår**-vinduet i **Felt**-feltet.  
    2.  I **Operator**-feltet velger du enten **Redusert**, **Økt** eller **Endret**.  
9. I feltet **Så svar** angir du svaret som skal følge når arbeidsflythendelsen inntreffer.  

     Når du velger feltet, åpnes vinduet **Arbeidsflytsvar**, der du kan velge fra alle arbeidsflytsvar som finnes, og angi svaralternativer for det valgte svaret.  
10. På hurtigfanen **Alternativer for det valgte svaret** angir du alternativer for arbeidsflytsvaret ved å velge verdier i ulike felt som vises, på følgende måte:  

    1.  Hvis du vil angi alternativer for et arbeidsflytsvar som involverer sending av en melding, fyller du ut feltene som beskrevet i følgende tabell.  

        |Felt|Beskrivelse|  
        |----------------------------------|---------------------------------------|  
        |**Bruker-ID for mottaker**|Angi brukeren som meldingen må sendes til. Obs!  Dette alternativet er bare tilgjengelig for arbeidsflytsvar med en plassholder for en bestemt bruker. For arbeidsflytsvar uten plassholdere for brukere er varslingsmottakeren vanligvis definert av brukeroppsettet for godkjenning.|  
        |**Kobling til målside**|Angi en annen side i [!INCLUDE[d365fin](includes/d365fin_md.md)] som koblingen i meldingen åpner i stedet for standardsiden.|  
        |**Egendefinert kobling**|Angi URL-adressen til en kobling som legges til i meldingen i tillegg til koblingen til en side i [!INCLUDE[d365fin](includes/d365fin_md.md)].|  
    2.  Hvis du vil angi alternativer for et arbeidsflytsvar som involverer oppretting av en godkjenningsforespørsel, fyller du ut feltene som beskrevet i følgende tabell.  

        |Felt|Beskrivelse|  
        |----------------------------------|---------------------------------------|  
        |**Forfallsdatoformel**|Angi hvor mange dager som gjenstår før godkjenningsforespørselen må løses fra datoen da den ble sendt.|  
        |**Deleger etter**|Angi om og når en forespørsel om godkjenning skal delegeres automatisk til relevant stedfortreder. Du kan velge å automatisk delegere en, to, eller fem dager etter datoen da godkjenningen ble forespurt.|  
        |**Godkjennertype**|Angi hvem godkjenneren er, i henhold til oppsettet for godkjenningsbrukere og arbeidsflytbrukere.<br /><br /> Følgende alternativer finnes:<br /><br /> -   **Selger/innkjøper** angir at brukeren som er definert i feltet **Selger/innkjøper - kode** i vinduet **Brukeroppsett for godkjenning**, bestemmer godkjenneren. Godkjenningsforespørselsposter blir deretter opprettet i henhold til verdien i feltet **Godkjennergrensetype**.<br />     Hvis du vil ha mer informasjon, kan du se [Konfigurere godkjenningsbrukere](across-how-to-set-up-workflow-users.md).|  
        |**Vis bekreftelsesmelding**|Angi om en bekreftelsesmelding skal vises til brukere når de ber godkjenning.|  
        |**Godkjennergrensetype**|Angi hvordan godkjenneres godkjenningsgrenser påvirker når godkjenningsforespørselsposter opprettes for dem. En kvalifisert godkjenner er en godkjenner med en godkjenningsgrense som er høyere enn verdien på forespørselen.<br /><br /> Følgende alternativer finnes:<br /><br /> 1.  **Godkjennerkjede** angir at godkjenningsforespørselsposter er opprettet for alle bestillerens godkjennere opptil og inkludert den første kvalifiserte godkjenneren.<br />2.  **Direkte godkjenner** angir at en godkjenningsforespørselspost bare opprettes for anmoderens umiddelbare godkjenner, uavhengig av godkjennerens godkjenningsgrense.<br />3.  **Første kvalifiserte godkjenner** angir at en godkjenningsforespørselspost bare opprettes for anmoderens første kvalifiserte godkjenner.<br />|  
    3.  Hvis du vil angi alternativer for et arbeidsflytsvar som involverer oppretting av kladdelinjer, fyller du ut feltene som beskrevet i følgende tabell.  

        |Felt|Beskrivelse|  
        |----------------------------------|---------------------------------------|  
        |**Finanskladdemalnavn**|Angi navnet på finanskladdemalen som de angitte kladdelinjene er opprettet i.|  
        |**Finanskladdenavn**|Angi navnet på finanskladden som de angitte kladdelinjene er opprettet i.|  

11. Velg knappene **Øk innrykk** og **Reduser innrykk** for å rykke inn hendelsesnavnet i **Når**-feltet for å definere plasseringen av trinnet i arbeidsflyten.  
    1.  Angi at trinnet er det neste i arbeidsflytrekkefølgen ved å rykke inn hendelsesnavnet under hendelsesnavnet i det forrige trinnet.  
    2.  Angi at trinnet er ett av flere alternative trinn som kan starte avhengig av tilstanden, ved å plassere hendelsesnavnet ved samme innrykk som de andre alternative trinnene. Ordne slike valgfrie trinn etter prioritet ved å plassere det viktigste trinnet først.  

    > [!NOTE]  
    >  Du kan bare endre innrykket for et trinn som ikke har et senere trinn.  

12. Gjenta trinn 7 til 11 for å legge til flere arbeidsflyttrinn, enten før eller etter trinnet du nettopp opprettet.  
13. Merk av for **Aktivert** for å angi at arbeidsflyten starter så snart hendelsen på det første trinnet av typen **Innpunkt** inntreffer. Hvis du vil ha mer informasjon, kan du se [Bruke arbeidsflyter](across-use-workflows.md).  

> [!NOTE]  
>  Ikke aktiver en arbeidsflyt før du er sikker på at arbeidsflyten er fullført og at de involverte arbeidsflyttrinnene kan starte.  

> [!TIP]  
>  Hvis du vil se relasjoner mellom tabeller som er brukt i arbeidsflyter, kan du velge ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport") og deretter angi **Arbeidsflyt – tabellrelasjoner**.  

## <a name="see-also"></a>Se også  
[Opprette arbeidsflyter fra arbeidsflytmaler](across-how-to-create-workflows-from-workflow-templates.md)   
[Konfigurere godkjenningsbrukere](across-how-to-set-up-approval-users.md)   
[Konfigurere arbeidsflytvarsler](across-setting-up-workflow-notifications.md)   
[Vise arkiverte forekomster av arbeidsflyttrinn](across-how-to-view-archived-workflow-step-instances.md)   
[Slette arbeidsflyter](across-how-to-delete-workflows.md)   
[Gjennomgang: Definere og bruke en arbeidsflyt for kjøpsgodkjenning](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)   
[Konfigurere arbeidsflyter](across-set-up-workflows.md)   
[Bruke arbeidsflyter](across-use-workflows.md)   
[Arbeidsflyt](across-workflow.md)      


