---
title: Slik tilordner du serie- og partinumre til varer for varesporing
description: "Du kan legge til serie- og partinumre i ethvert utgående eller inngående dokument, og tilhørende bokførte varesporingsposter vises i de relaterte varepostene."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/22/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: fa6677e2f856fd22ff56139332aa307919b0ab96
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-work-with-serial-and-lot-numbers"></a>Arbeide med serie- og partinumre
Du kan tilordne serie- og partinumre i ethvert utgående eller inngående dokument, og tilhørende bokførte varesporingsposter vises i de relaterte varepostene. Du utfører arbeidet i **Varesporingslinjer**-vinduet.

Matrisen over antallsfelt øverst i vinduet **Varesporingslinjer** gir en oversikt over antallene og summene til varesporingsnumrene som defineres på linjene. Antallene må samsvare med dem som finnes i dokumentlinjen, som er indikert med en 0 i **Udefinert**-feltene.

Av hensyn til ytelsen samler programmet tilgjengelighetsinformasjonen i vinduet **Varesporingslinjer** bare én gang når du åpner vinduet. Dette betyr at programmet ikke oppdaterer tilgjengelighetsinformasjonen mens du har vinduet åpent, selv om det forekommer endringer på lageret eller i andre dokumenter i løpet av denne tiden.

Varer med serie- eller partinumre kan spores både bakover og fremover i forsyningskjeden. Dette er nyttig for generell kvalitetskontroll og tilbakekalling av proukter. Hvis du vil ha mer informasjon, kan du se [Spore varesporede varer](inventory-how-to-trace-item-tracked-items.md).

## <a name="about-picking-serial-or-lot-numbers-in-the-warehouse"></a>Om plukking av serie- eller partinumre i Lager
Utgående håndtering av serie-/partinumre er en oppgave som utføres under mange ulike lagerprosesser.  

I enkelte prosesser har ikke lagervarene serie- eller partinumre, og lagermedarbeideren må tilordne nye under utgående håndtering, vanligvis fra en forhåndsdefinert nummerserie.

I enkle prosesser har lagervarene allerede serie- eller partinumre, for eksempel tilordnet under plasseringen, og disse numrene overføres automatisk gjennom alle utgående lageraktiviteter uten medvirkning fra lagermedarbeiderne.

Bestemte serie- eller partinumre er definert i kildedokumentet, for eksempel en ordre, som lagermedarbeideren må respektere under utgående lagerhåndtering i spesielle situasjoner for serie - eller partinummererte varer. Dette kan skyldes at kunden har bedt om et bestemt parti under bestillingsprosessen. Når lagerplukk- eller plukkdokumentet opprettes fra et utgående kildedokument der serie- eller partinumre allerede er definert, vil alle felt i vinduet **Varesporingslinjer** låses for skriving under lagerplukkingen, bortsett fra feltet **Ant. som skal håndt**. I så fall angir lagerplukklinjene varesporingsnumrene på individuelle hentings- og plasseringslinjer. Antallet er allerede delt inn i unike serie- eller partinummerkombinasjoner, fordi ordren spesifiserer varesporingsnumrene som skal leveres.  

## <a name="item-tracking-availability"></a>Varesporingstilgjengelighet
Når du arbeider med serie- og partinumre, beregner [!INCLUDE[d365fin](includes/d365fin_md.md)] tilgjengelighetsinformasjon for parti- og serienumre og viser den i de ulike varesporingsvinduene. Dette viser hvor mye av et parti- eller serienummer som for tiden brukes på andre dokumenter. Dette reduserer antall feil og usikkerhet forårsaket av doble tildelinger.

I vinduet **Varesporingslinjer** vises et advarselsikon i feltet **Tilgjengelighet, Partinr.** eller **Tilgjengelighet, Serienr.** hvis noe av eller hele antallet du har valgt allerede brukes i andre dokumenter, eller hvis parti- eller serienummeret ikke er tilgjengelig.

I vinduet **Partinr. / Serienr.oversikt**, vinduet **Partinr. / Tilgjengelighet for serienummer** og vinduet **Varesporing - velg poster** vises informasjon om hvor stort antall av en vare som brukes. Dette inkluderer følgende informasjon.

|Felt|Beskrivelse|
|-----|-----------|  
|**Antall i alt**|Totalt antall varer på lager|
|**Ønsket antall i alt**|Totalt antall varer som det er ønske om å bruke i dette eller andre dokumenter|
|**Gjeldende antall i kø**|Antall ønskede varer som vil bli brukt i det gjeldende dokumentet, men som ennå ikke er bundet i databasen|
|**Gjeldende ønsket antall**|Antallet ønskede varer som vil bli brukt i det gjeldende dokumentet|
|**Totalt disp. antall**|Totalt antall varer på lager minus antallet av varen som det er ønske om å bruke i dette og andre dokumenter (ønsket antall i alt), og minus antallet som det er ønske om å bruke, men som ennå ikke er bundet i dette dokumentet (gjeldende antall i kø)|

Hvis du arbeider i vinduet **Varesporingslinjer** i en lang periode, eller hvis det skjer mye med varen du arbeider med, kan du velge handlingen **Oppdater tilgjengelighet**. I tillegg kontrolleres tilgjengeligheten av varen automatisk på nytt når du lukker vinduet, for å bekrefte at det ikke finnes noen tilgjengelighetsproblemer.

## <a name="to-set-up-item-tracking-codes"></a>Slik definerer du en varesporingskode
En varesporingskode viser hvordan et selskap bruker serie- og partinumre til å holde styr på varer på forskjellige steder i lageret.  

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Varesporingskoder**, og velg deretter den relaterte koblingen.  
2. Velg handlingen **Ny**.
3. Fyll ut feltene etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
4. I hurtigfanene **Serienr.** og **Partinr.** definerer du hvordan varesporing etter henholdsvis serie- eller partinumre skal foregå.  

### <a name="to-set-up-expiration-rules-for-serial-or-lot-numbers"></a>Slik setter du opp utløpsregler for serie-/partinumre  
Du ønsker kanskje å opprette bestemte utløpsdatoer og -regler for enkelte varer i varesporingskoden. Denne funksjonaliteten gjør at du kan holde orden på når serie- og partinumrene utløper.

1. Velg en eksisterende varesporingskode, og velg deretter **Rediger**-handlingen.  
2.  På hurtigfanen **Diverse** merker du følgende avmerkingsbokser.  

    |Felt|Beskrivelse|  
    |---------------------------------|---------------------------------------|  
    |**Bruk ikke etter utløpsdato**|Angir at en utløpsdato av varesporingsnummeret ved inngang til lageret, og denne utløpsdatoen må det tas hensyn til ved utgang fra lageret.|  
    |**Manuelt ang. utløpsdato obl.**|Angir at du må angi manuelt en utløpsdato på varesporingslinjen.|  

### <a name="to-set-up-warranties-for-serial-or-lot-numbers"></a>Slik setter du opp garantier for serie-/partinumre  
Du ønsker kanskje å opprette bestemte garantier for enkelte varer i varesporingskoden. Denne funksjonen gjør det mulig å holde oversikt over når garantiene for bestemte serie- eller partinumre i lageret utløper.        
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Varesporingskoder**, og velg deretter den relaterte koblingen.  

1. Velg en eksisterende varesporingskode, og velg deretter **Rediger**-handlingen.  
2.  På hurtigfanen **Div.** fyller du ut feltet **Garantidatoformel** og velger avmerkingsboksen som følger.  

    |Felt|Beskrivelse|  
    |---------------------------------|---------------------------------------|  
    |**Garantidatoformel**|Angir den siste garantidagen for varen.|  
    |**Manuelt angitt garantidato obl.**|Angir at du må angi en garantidato på varesporingslinjen manuelt.|  

## <a name="to-record-serial-or-lot-number-information"></a>Slik registrerer du opplysninger om serie-/partinumre  
Hvis du trenger å knytte spesielle opplysninger til et spesielt varesporingsnummer, for eksempel av kvalitetshensyn, kan du gjøre dette på kortet med serie- eller partinummeropplysninger.

1. Åpne et dokument som har serie- eller partinumre tilordnet.
2. Åpne vinduet **Varesporingslinjer** for dokumentet.
3. Velg for eksempel handlingen **Informasjonskort for serienr.**  

    **Serienr.**- og **Partinr.**-feltet blir forhåndsutfylt fra varesporingslinjen.  
4. Skriv inn litt informasjon i **Beskrivelse**-feltet, for eksempel om tilstanden til varen.  
5. Velg **Kommentar** for å opprette en egen kommentarpost.  
6. Merk av for **Sperret** for å utelate serie- eller partinummeret fra alle transaksjoner.  

## <a name="to-modify-existing-serial-or-lot-number-information"></a>Slik endrer du eksisterende informasjon om serie- eller partinumre  
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Varer**, og velg deretter den relaterte koblingen.  
2. Velg en vare som har en varesporingskode, og som har informasjon om serie- eller partinumre.
3. Fra **Varekort**-vinduet velger du **Poster** og deretter **Poster**.
4. Velg feltet **Partinr.** eller **Serienr.** Hvis det finnes informasjon for dette varesporingsnummeret, åpnes vinduet **Informasjonsoversikt for partinummer** eller **Informasjonsoversikt for serienummer**.  
5. Velg et kort, og velg deretter **Informasjonskort for partinr. eller Informasjonskort for serienr.**  
6. Endre teksten for kort beskrivelse, merknadsposten eller **Sperret**-feltet.  

Du kan ikke endre serie- eller partinumre eller antall. Du må reklassifisere den aktuelle vareposten for å gjøre dette. Hvis du vil ha mer informasjon om dette, kan du se "Slik reklassifiserer du parti- eller serienumre".

## <a name="to-assign-serial-or-lot-numbers-during-an-inbound-transaction"></a>Slik tilordner du serie- eller partinumre ved en inngående transaksjon  
For selskaper som vil holde styr på varene allerede fra begynnelsen, er bestillingen ofte det sentrale dokumentet. I dette tilfellet er ofte bestillingsordren det sentrale dokumentet, men varesporing kan imidlertid håndteres fra et hvilket som helst inngående dokument, og bokførte poster kan vises i de tilhørende varepostene.  

Det er oppsettet av vinduet **Kort for varesporingskode** som angir hvordan selskapet håndterer varesporingsnumre.  

> [!NOTE]  
>  Hvis du vil bruke varesporingsnumre i lageraktiviteter, må oppsettsfeltene **Lagerparti - sporing** og **Lagers.nr. - sporing** være valgt, siden de definerer de spesielle prinsippene i håndtering av serie- og partinumre i lageraktiviteter.  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bestillinger**, og velg deretter den relaterte koblingen.  
2.  Velg den aktuelle dokumentlinjen. På hurtigfanen **Linjer** velger du **Linje** og deretter **Varesporingslinjer**.  

    Du kan tilordne serie- eller partinumre på følgende måter:  

    -   Automatisk, ved å velge **Tilordne serienr.** eller **Tilordne partinr.** for å tilordne serie-/partinumre fra forhåndsdefinerte nummerserier.  
    -   Automatisk, ved å velge **Opprett egendefinert s.nr.** hvis du vil at programmet skal tilordne serie-/partinumre basert på nummerserier som er definert spesielt for de mottatte varene.  
    -   Manuelt, ved å angi serie- eller partinumre direkte, for eksempel leverandørens numre.  
    -   Manuelt ved å tilordne hver vareenhet et bestemt nummer.  

3. Hvis du vil tilordne automatisk, velger du **Opprett egendefinert s.nr.**  
4. I feltet **Egendef. serienr.** angir du startnummeret på en beskrivende serienummerserie, for eksempel **S/N-Lev0001**.  
5. I feltet **Økning** angir du 1 for å angi at hvert nye nummer skal økes med én.  

    Feltet **Ant. som skal oppr.** inneholder linjeantallet som standard, men du kan endre det.  

6. Merk av for **Opprett nytt partinr.** hvis du vil samle de nye serienumrene i et parti.  
7. Velg **OK**.  

Et partinummer med individuelle serienumre opprettes i henhold til vareantallet på dokumentlinjen, og begynner med **S/N-Vend0001**.  

Matrisen over antallsfelt i hodet gir en dynamisk oversikt over antallene og summene til varesporingsnumrene du definerer i vinduet. Antallene må samsvare med dem som finnes i dokumentlinjen, som er markert med en 0 i **Udefinert**-feltene.  

Når dokumentet bokføres, overføres varesporingspostene til de tilhørende varepostene.

## <a name="to-assign-a-serial-or-lot-number-during-an-outbound-transaction"></a>Slik tilordner du et serie-/partinummer ved en utgående transaksjon  
Det finnes to måter å legge til serie- og partinumre i utgående transaksjoner:  

-   Velge mellom eksisterende serie- eller partinumre. Dette er aktuelt når det allerede er tilordnet varesporingsnumre ved en inngående transaksjon. Hvis du vil ha mer informasjon, kan du se "Slik velger du fra eksisterende serienumre og partinumre".
-   Tilordne nye serie- eller partinumre ved utgående transaksjoner. Dette gjelder når varesporingsnumrene ikke tilordnes varer før de er solgt og klar for levering.  

De ulike reglene for varesporingsnumre konfigureres i vinduet **Kort for varesporingskode**.  

> [!NOTE]  
>  Hvis du vil tilordne varesporingsnumre i lageraktiviteter, må det være merket av for **Lagers.nr. - sporing** og **Lagerparti - sporing** på kortet for varesporingskode for varen.    

1. Velg den aktuelle dokumentlinjen. På hurtigfanen **Linjer** velger du **Ordre** og deretter **Varesporingslinjer**.  

    Du kan tilordne varesporingsnumre på følgende måter:  
    -   Automatisk fra forhåndsdefinerte nummerserier: Velg **Tilordne serienr.** eller **Tilordne partinr.**  
    -   Automatisk, basert på parametere som du har definert spesielt for utgående vare: Velg **Opprett egendefinert s.nr.**  
    -   Manuelt, ved å angi serie- eller partinumre uten å bruke en nummerserie.  

2.  For denne fremgangsmåten tilordner du et serienummer automatisk ved å velge **Tilordne serienr.**  

    Feltet **Ant. som skal oppr.** inneholder linjeantallet som standard, men du kan endre det.  
3.  Velg feltet **Opprett nytt partinr.** hvis du vil samle de nye serienumrene i et parti.  
4.  Velg **OK**-knappen for å opprette et partinummer og nye serienumre i henhold til vareantallet på den aktuelle dokumentlinjen.  

Matrisen over antallsfelt øverst gir en dynamisk oversikt over antallene og summene til de varesporingsnumrene som du definerer i vinduet. Antallene må korrespondere med de som finnes i dokumentlinjen, som er markert med en **0** i **Udefinert**-feltene.  

Når dokumentet bokføres, overføres varesporingspostene til de tilhørende varepostene.  

## <a name="to-select-from-existing-serial-or-lot-numbers"></a>Slik velger du mellom eksisterende serie-/partinumre  
Når du arbeider med varer som krever varesporing, og du oppretter utgående transaksjoner, der varer går ut av lageret, må du vanligvis velge parti- eller serienumrene fra de som allerede finnes på lageret.  

 Det er oppsettet av tabellen **Varesporingskode** som angir hvordan selskapet håndterer varesporingsnumre.  

> [!NOTE]  
>  For at du skal kunne håndtere varesporingsnumre i lageraktiviteter, må varen opprettes med Sporing etter serienummer elle partinummer fordi dette fastsetter de spesielle prinsippene som styrer serie- og partinumrene på lageret.

1.  Merk linjen du vil velge serie- eller partinumre for, i et utgående dokument.  
2.  På hurtigfanen **Linjer** velger du **Handlinger**, velger **Linje** eller **Vare** og velger deretter **Varesporingslinjer**.  
3.  I vinduet **Varesporingslinjer** har du tre alternativer for å angi parti- eller serienummer:  

    -   Velg feltet **Partinr.** eller **Serienr.**, og velg et nummer i vinduet **Varesporingssummering**.  
    -   Velg handlingen **Velg poster**. **Velg poster**-vinduet inneholder alle parti- eller serienumre sammen med tilgjengelighetsinformasjon.

4. I **Valgt antall**-feltet angir du antallet for hvert parti- eller serienummer du vil bruke.   
5. Velg **OK**-knappen. Den valgte varesporingsinformasjonen overføres til vinduet **Varesporingslinjer**.  
6. Skriv eller skann inn varesporingsnummeret.

Matrisen over antallsfelt i hodet gir en dynamisk oversikt over antall og summer til de varesporingsnumrene som du definerer i vinduet. Antallene må korrespondere med de som finnes i dokumentlinjen, som er markert med en **0** i **Udefinert**-feltene.  

 Når du bokfører dokumentlinjen, overføres varesporingsinformasjonen til de tilhørende varepostene.

## <a name="to-handle-serial-and-lot-numbers-on-transfer-orders"></a>Slik håndterer du serie- og partinumre på overføringsordrer  
Framgangsmåten for håndteringen av serie- og partinumre som overføres mellom ulike lokasjoner, er omtrent den samme som for kjøp og salg av varer.  

Imidlertid er overføringsordren unik på den måten at både levering og mottak gjøres fra samme overføringslinje og derfor bruker samme forekomst av vinduet **Varesporingslinjer**. Dette betyr at varesporingsnumrene som leveres fra en lokasjon, må mottas uendret på den andre lokasjonen.  

 Det er oppsettet av tabellen  **Varesporingskode** som angir hvordan selskapet håndterer varesporingsnumre.    
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Overføringsordrer**, og velg deretter den relaterte koblingen.  
2.  Åpne overføringsordren du vil behandle. På hurtigfanen **Linjer** velger du **Linje**, velger **Varesporingslinjer** og velger deretter **Levering**.  
3.  I vinduet **Varesporingslinjer** tilordner eller velger du serie- eller partinumre som for en hvilken som helst annen utgående varetransaksjon.  

    Når du håndterer serie- og partinumre for overføringsvarer, er varene oftest allerede tilordnet numre. Derfor er det mest vanlig å velge mellom serie- eller partinumre som allerede er opprettet.  

4.  Bokfør overføringsordren, først levering og deretter mottak, slik at varene overføres med riktige varesporingsposter.  

Under overføringen er vinduet **Varesporingslinjer** skrivebeskyttet.  

## <a name="to-handle-serial-and-lot-numbers-when-getting-receipt-lines-from-a-purchase-invoice"></a>Slik håndterer du serie- og partinumre ved henting av mottakslinjer fra en kjøpsfaktura  
Når du bruker funksjonalitet for å hente bokførte mottaks- eller leveringslinjer fra relaterte fakturaer eller kreditnotaer, overføres alle varesporingslinjer i lagerdokumentene automatisk, men de blir behandlet på en spesiell måte.

Funksjonen støtter følgende inngående prosesser:  
-   **Hent mottakslinjer** - fra en kjøpsfaktura.  
-   **Hent returforsendelseslinjer** - fra en kjøpskreditnota.  

Funksjonen støtter følgende utgående prosesser:  
-   **Hent følgeseddellinje** - fra en salgsfaktura eller samlede følgesedler.  
-   **Hent returseddellinjer** - fra en salgskreditnota.  

I disse tilfellene kopieres de eksisterende varesporingslinjene automatisk til fakturaen eller kreditnotaen, men vinduet **Varesporingslinjer** tillater ikke endringer i serie- eller partinumre. Det er bare antallene som kan endres.  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Kjøpsfakturaer**, og velg deretter den relaterte koblingen.  
2.  Åpne en kjøpsfaktura for varene som er kjøp med serie- eller partinumre.  
3.  Velg **Hent mottakslinjer** på hurtigfanen **Linjer** fra en kjøpsfakturalinje.  
4.  Velg mottakslinjer som har varesporingslinjer, i vinduet **Hent mottakslinjer**, og klikk deretter **OK**.  

    Kildedokumentet kopieres til kjøpsfakturaen som en ny linje, og varesporingslinjene i dokumentet kopieres til det underliggende vinduet **Varesporingslinjer**.  

5.  Velg den overførte mottakslinjen i kjøpsfakturaen.  
6.  På hurtigfanen **Linjer** velger du **Linje** og deretter **Varesporingslinjer** for å se de overførte varesporingslinjene.  

Innholdet i feltene **Serienr.** og **Partinr.** kan ikke redigeres. Du kan imidlertid slette hele linjer eller endre antallene slik at de samsvarer med endringer gjort på kildelinjen.  

## <a name="to-reclassify-serial-or-lot-numbers"></a>Slik reklassifiserer du serie- eller partinumre  
Å reklassifisere varesporing for en vare betyr å endre et parti- eller serienummer til et nytt parti- eller serienummer eller endre utløpsdatoen til en ny utløpsdato. Hvis du arbeider med partier, kan du også slå sammen flere partier til ett. Du utfører disse oppgavene ved å bruke varereklassifiseringskladden.

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Vareoverføringskladd**, og velg deretter den relaterte koblingen.  
2.  Fyll ut linjen med de aktuelle opplysningene. Hvis du vil ha mer informasjon, se [Telle, justere og reklassifisere lagerbeholdning](inventory-how-count-adjust-reclassify.md).
3.  Velg **Varesporingslinjer**.  
4.  I feltet **Serienr.** eller **Partinr.** velger du gjeldende serie- eller partinummer.  
5.  Hvis du vil angi et nytt varesporingsnummer, angir du det i feltet **Nytt serienr.** eller **Nytt partinr.**. Hvis du vil, kan du slå sammen ett eller flere partier til ett nytt eller eksisterende parti.  

    > [!NOTE]  
    >  Vær oppmerksom på at når du reklassifiserer utløpsdatoer, blir varer med de tidligste utløpsdatoene for utgående transaksjoner foreslått først. Hvis du vil ha mer informasjon, kan du se [Plukking etter FEFO](warehouse-picking-by-fefo.md).  

5.  Hvis du vil angi en ny utløpsdato for serie- eller partinummeret, angir du det i feltet **Ny utløpsdato**.  

    > [!IMPORTANT]  
    >  Hvis du reklassifiserer et parti til det samme partinummeret, men med en annen utløpsdato, må du reklassifisere hele partiet og bruke én linje i vareoverføringskladden. Hvis du reklassifiserer flere enn ett parti til et nytt partinummer, som betyr at du slår sammen flere enn ett parti i ett nytt parti, må du angi samme utløpsdato for alle partiene. Hvis du reklassifiserer ett eksisterende parti til et annet eksisterende parti med en annen utløpsdato, må du bruke utløpsdatoen fra det andre partiet. Hvis du lar feltet **Ny utløpsdato** stå tomt, reklassifiseres parti- eller serienummeret med en tom utløpsdato.  

6.  Hvis du har eksisterende informasjon for det gamle serie- eller partinummeret, kan du kopiere den til det nye serie- eller partinummeret.  

    1.  I vinduet **Varesporingslinjer** velger du **Ny informasjon om serienummer** eller **Ny informasjon om partinummer**.  
    2.  Hvis du vil kopiere informasjon fra det gamle parti- eller serienummeret, velger du **Kopier informasjon**.  
    3.  Velg parti- eller serienummeret som du vil kopiere fra, i vinduet for informasjonsoversikt, og velg **OK**-knappen.  

7.  Hvis du vil endre den eksisterende informasjonen for parti- eller serienummeret, kan du registrere parti- eller serienummerinformasjon.  
8.  Bokfør kladden for å knytte de nye varesporingsnumrene eller utløpsdatoene til den tilhørende vareposten

## <a name="see-also"></a>Se også
[Spore varesporede varer](inventory-how-to-trace-item-tracked-items.md)   
[Lager](inventory-manage-inventory.md)  
[Designdetaljer: Varesporing](design-details-item-tracking.md)
[Designdetaljer: Varesporing og reservasjoner](design-details-item-tracking-and-reservations.md)  
[Reservere varer](inventory-how-to-reserve-items.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

