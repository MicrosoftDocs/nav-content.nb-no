---
title: Tilpasse sider i Dynamics Windows-klienten
description: "Lær hvordan du kan tilpasse brukergrensesnittet slik at det passer til din arbeidsmåte."
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: e22f3464c6a4dd917880ad0b903880fe5f57a37d
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="personalizing-your-workspace-in-the-dynamics-windows-client"></a>Tilpasse arbeidsområdet i Dynamics Windows-klienten
Du kan tilpasse arbeidsområdet slik at det passer til arbeidet og preferansene ved å endre sider slik at de bare viser informasjon du trenger, der du trenger den. Tilpasningsendringene som du utfører, påvirker bare hva du ser, ikke hva andre brukere ser. Du kan tilpasse mange deler av brukergrensesnittet, inkludert handlinger du vil ha med på båndet, plassering av felt i hurtigfaner eller faktabokser og menyelementer du vil ha med i navigasjonsruten.

> [!NOTE]  
> Du kan også tilpasse sider ved hjelp av [!INCLUDE[nav_web_md](includes/nav_web_md.md)]. Hvis du vil vite hvordan tilpasning fungerer mellom de to klientene, kan du se [Oversikt over tilpasning](ui-personalization-overview.md).

## <a name="how-to-personalize-your-workspace"></a>Slik tilpasser du arbeidsområdet
Du utfører det meste av tilpasningsarbeidet ved hjelp av **Tilpass**-funksjonen, som du får tilgang til fra praktisk talt alle typer sider ved å gjøre følgende:

1.  Åpne siden som du vil tilpasse.
2.  Øverst til venstre velger du **Program**-menyen ![Programmeny-knappen på menylinjen](media/applicationmenuicon.png "ApplicationMenuIcon"), velg **Tilpass**, og velg deretter ett av tilpasningsalternativene.

Det finnes også noen grunnleggende grensesnittendringer, for eksempel justere størrelsen på et vindu eller utvide bredden for kolonner, som du gjør direkte på siden, utenfor alternativet **Tilpass**.

## <a name="general-information"></a>Generell informasjon
Når du tilpasser brukergrensesnittet, er det lurt å være oppmerksom på følgende:

-   Du kan registrere flere tilpasninger på den samme siden basert på ulike tilgangspunkt til siden. Vinduet Ordrer kan for eksempel tilpasses slik at det ser annerledes ut når det åpnes fra vinduet Kundekort enn når det åpnes fra rollesenteret Ordrebehandler. Punktet der du går til siden som skal tilpasses, registreres i denne bestemte sidetilpasningen. Derfor kan det være flere tilpassede sideoppføringer i databasen, som du kan se i vinduet **Slett brukertilpasning**.

-   Programmet kan konfigureres til å vise og skjule brukergrensesnittelementer (for eksempel felt, hurtigfaner og faktabokser) basert på lisensen eller tillatelser. Du vil bare kunne se og tilpasse elementfelt som du har tillatelse til.

## <a name="customize-ribbons"></a>Tilpass bånd
Båndet gir deg tilgang til flere handlinger. Ved å tilpasse båndet kan du optimalisere det for dine arbeidsprosesser og preferanser. Hvis du for eksempel ofte bruker **Dimensjoner**-vinduet, kan du legge til **Dimensjoner**-handlingen i handlingsgruppen **Prosess**. Du kan også fjerne handlinger du aldri bruker, for å få bedre oversikt.  

Du kan utføre følgende oppgaver for å tilpasse bånd på sider:  

-   Legg til, gi nytt navn til eller fjern kategorier, grupper, handlinger og menyer.  
-   Endre rekkefølgen på handlinger.  
-   Gjenopprette båndet til standardinnstillingen.  

### <a name="to-customize-a-ribbon"></a>Slik tilpasser du et bånd
1. Åpne siden som du vil endre.
2. Øverst til venstre velger du ikonet for **Program**-menyen ![Programmeny-knappen på menylinjen](media/applicationmenuicon.png "ApplicationMenuIcon"), velger **Tilpass** og deretter **Tilpass båndet**.

Dialogboksen **Ordne handlinger i båndet** er inndelt i to ruter. Ruten **Tilgjengelige handlinger** viser alle handlingene som du kan velge å legge til på siden. Ruten **Vis handlinger i denne rekkefølgen** viser strukturen for alle handlingene som vises på siden for øyeblikket.

-   Elementer på rotnivå definerer kategoriene.

    -   Elementer på andre nivå definerer en gruppe i en kategori.

        -   Elementer på tredje nivå definerer en meny for handlinger i en gruppe

### <a name="add-a-group"></a>Legge til en gruppe
Velg kategorien som du vil ha gruppen under, og velg deretter **Opprett gruppe**. Du kan ikke legge til en gruppe under en meny.

### <a name="add-a-menu"></a>Legge til en meny
Velg gruppen som du vil ha menyen under, og velg deretter **Opprett meny**. Du kan bare legge til en meny i en gruppe eller en annen meny.

#### <a name="add-an-action"></a>Legge til en handling
Merk den i ruten **Tilgjengelige handlinger**, velg **Legg til** for å legge den til i ruten **Vis handlinger i denne rekkefølgen**, og bruk deretter knappene **Flytt opp** og **Flytt ned** til å plassere den der du vil ha den.

Du kan ikke legge til en handling i en kategori - bare i en gruppe eller en meny.

###  <a name="limitations-and-recommendations"></a>Begrensninger og anbefalinger
Vær oppmerksom på følgende begrensninger når du tilpasser båndet:  

-   Systemkategorier eller -grupper, for eksempel  **Hjem**    eller  **Ny**, kan ikke flyttes eller gis nytt navn. Plasseringen av noen grupper, for eksempel  **Nytt dokument**,  er fast.  
-   Handlinger eller grupper som har dynamisk synlighet, kan ikke legges til eller fjernes.
-   Du kan bare lage menyer i grupper, ikke i faneblad.  
-   Du kan ha en meny i en annen meny, men dette anbefales ikke.  
-   Hvis du ser uventet atferd med grupper og handlinger etter å ha tilpasset båndet, gjør du følgende:  

    1.  Tom, men ikke slett gruppen der problemet oppstår.  
    2.  Lukk dialogboksen ved hjelp av **OK**-knappen.  
    3.  Åpne dialogboksen på nytt og legg handlingene til i gruppen på nytt.  

> [!IMPORTANT]  
>  Alle tilpassinger som endrer båndet, kan påvirke veiledning i Hjelp for [!INCLUDE[navnow_md](includes/navnow_md.md)], fordi navigasjonstrinnene i hjelpen kan referere til et annet båndoppsett.

## <a name="customize-fasttabs"></a>Tilpasse hurtigfaner
Hurtigfaner bidrar til å organisere informasjon om sider i enkle, håndterbare grupper. Du kan tilpasse hurtigfanene på sider slik at de støtter arbeidsflyten. Du vil for eksempel kanskje vise færre hurtigfaner eller skjule bestemte felt på hurtigfaner. Du kan også fremheve de viktigste feltene som skal inkluderes i hurtigfaneoverskriftene når hurtigfanene er skjult.  

### <a name="to-customize-a-fasttab"></a>Slik tilpasser du en hurtigfane  

1.  Åpne siden som du vil endre.
2.  Velg ikonet for **Program**-menyen ![Programmeny-knappen på menylinjen](media/applicationmenuicon.png "ApplicationMenuIcon"), velg **Tilpass** og deretter **Tilpass denne siden**.  
3.  I dialogboksen **Tilpass <Page Name>** velger du **Hurtigfaner**.  

### <a name="add-move-or-remove-fasttabs"></a>Legge til, flytte eller fjerne hurtigfaner
Boksen **Vis hurtigfaner i denne rekkefølgen** inneholder hurtigfanene som finnes på siden for øyeblikket, og rekkefølgen de vises i. Bruk knappene **Legg til**, **Fjern** og **Flytt opp** og **Flytt ned** til å utføre endringer.

### <a name="show-and-hide-fields-on-fasttabs"></a>Vise og skjule felt i hurtigfaner
I boksen **Vis hurtigfaner i denne rekkefølgen** velger du hurtigfanen du vil endre, og deretter velger du **Tilpass hurtigfane**. Bruk knappene til å tilpasse feltene som du vil vise, og rekkefølgen på siden.

Angi **Viktighet** på følgende måte:
-   Hvis du vil vise feltet i hurtigfaneoverskriften når hurtigfanen er skjult, må du angi dette som **Forfremmet**.
- Hvis du vil at feltet skal skjules med mindre brukeren velger handlingen **Vis flere felt** i hurtigfanen, angir du dette som **Tillegg**.
-   **Standard** er standard eller vanlig innstilling.

### <a name="set-up-field-for-quick-entry"></a>Definere felt for hurtigoppføring
Merk av for **Hurtigoppføring** for å legge til feltet i listen over hurtigoppføringsfelt. Når du arbeider på siden og trykker ENTER i et felt, hopper pekeren til neste felt som er angitt som et hurtigoppføringsfelt.

## <a name="customize-factboxes"></a>Tilpasse faktabokser
Du bruker Faktaboksene til å vise informasjon om posten du har valgt i oversikten eller åpnet på en oppgaveside. Du kan velge hvilke faktabokser som skal vises i faktaboksruten. Du kan også tilpasse faktaboksene slik at de bare viser feltene du har bruk for.  

### <a name="to-show-or-hide-the-factbox-pane"></a>Slik viser eller skjuler du faktaboksruten
Faktabokser befinner seg i en faktaboksrute, som du kan velge å vise eller skjule på sidebasis. Dette gjør det mulig for deg å enkelt skjule flere faktabokser uten å måtte fjerne dem enkeltvis.

1.  Åpne siden som du vil endre.
2.  Velg ikonet for **Program**-menyen ![Programmeny-knappen på menylinjen](media/applicationmenuicon.png "ApplicationMenuIcon"), velg **Tilpass** og deretter **Faktabokser**. En hake angir at faktaboksruten vises.  

### <a name="to-customize-the-factbox-pane"></a>Slik tilpasser du faktaboksruten  
1.  Åpne siden som du vil endre.
2.  Velg ikonet for **Program**-menyen ![Programmeny-knappen på menylinjen](media/applicationmenuicon.png "ApplicationMenuIcon"), velg **Tilpass** og deretter **Velg faktabokser**.  

### <a name="add-a-factbox"></a>Legge til en faktaboks  

Velge faktaboksen du vil legge til i faktaboksruten, i boksen **Tilgjengelige faktabokser**, og deretter velger du **Legg til**-knappen.  

### <a name="remove-a-factbox"></a>Fjerne en faktaboks  

I boksen **Vis faktabokser i denne rekkefølgen** velger du faktaboksene og deretter **Fjern**-knappen.   

### <a name="change-the-order-of-the-factboxes"></a>Endre faktaboksenes rekkefølge  

I boksen **Vis faktabokser i denne rekkefølgen** velger du faktaboksen som du vil fjerne, og deretter velger du knappene **Flytt opp** eller **Flytt ned** til faktaboksen er plassert der du vil ha den.  

### <a name="change-the-fields-in-a-factbox"></a>Endre feltene i en faktaboks  

1.  I boksen **Vis faktabokser i denne rekkefølgen** velger du faktaboksen og deretter **Tilpass del**.  

2.   Boksen **Tilgjengelige felt** viser alle feltene du kan velge mellom. Boksen **Viste felt** viser alle feltene som vises i faktaboksen for øyeblikket. Bruk knappene for å legge til, fjerne og flytte feltene.   


## <a name="customize-columns-in-a-list-or-on-document-lines"></a>Tilpasse kolonner i en liste eller på dokumentlinjer
Du kan få en bedre oversikt over informasjonen du trenger, hvis du tilpasser listesider og kortsider ved å legge til eller fjerne kolonner i rutenettene, endre rekkefølge for kolonner og legge til en fryst rute.  

### <a name="to-add-remove-and-arrange-columns"></a>Slik legger du til, fjerner og organiserer kolonner  

1.  Du kan legge til, fjerne eller endre rekkefølge for kolonner på to måter:

    -   Velg ikonet for **Program**-menyen ![Programmeny-knappen på menylinjen](media/applicationmenuicon.png "ApplicationMenuIcon"), velg **Tilpass** og deretter **Velg kolonner**.
    -   Høyrevelg en kolonneoverskrift, og velg deretter **Velg kolonner**.

2.  I dialogboksen **Velg hvilke kolonner som skal vises i oversikten** inneholder ruten **Tilgjengelige kolonner** kolonner som er skjult. Ruten **Vis kolonner i denne rekkefølgen** inneholder kolonner som vises. Bruk knappene **Legg til** og **Fjern** til å flytte kolonner fra ett felt til et annet. Bruk knappene **Flytt opp** og **Flytt ned** til å plassere kolonnene.

>[!TIP]
>Merk av for **Hurtigoppføring** for å legge til feltet i listen over hurtigoppføringsfelt. Når du arbeider på siden og trykker ENTER i et felt, hopper pekeren til neste felt som er angitt som et hurtigoppføringsfelt.

### <a name="to-set-the-freeze-pane"></a>Slik angir du den fryste ruten
En liste kan ha mange kolonner, noe som kan fremtvinge at du må rulle vannrett for å vise alle kolonnene. Det kan være kolonner som du alltid vil vise også når du ruller. Dette kan du gjøre ved å legge til en loddrett fryst rute for å hindre at visse kolonner ruller. Dette gjør det mulig å sikre at bare mindre viktige kolonner flyttes når du ruller.

Hvis du vil angi den fryste ruten, velger du kolonnen som den fryste ruten skal starte etter, og velg deretter **Legg til Frys rute**.

## <a name="customizing-the-navigation-pane"></a>Tilpasse navigasjonsruten
Navigasjonsruten viser en meny med koblinger til ulike oversiktssider. Koblingene er gruppert under knapper på rotnivå.

### <a name="to-customize-the-navigation-pane"></a>Slik tilpasser du navigasjonsruten  

Velg ikonet for **Program**-menyen ![Programmeny-knappen på menylinjen](media/applicationmenuicon.png "ApplicationMenuIcon"), velg **Tilpass** og deretter **Tilpass navigasjonsrute**.  

### <a name="rename-or-rearrange-buttons-in-the-navigation-pane"></a>Gi nytt navn til eller omorganisere knapper i navigasjonsruten  
I dialogboksen **Tilpass navigasjonsrute** i ruten til venstre velger du knappen du vil flytte, gi nytt navn til eller fjerne, og deretter velger du den aktuelle knappen midt i vinduet.

Du kan ikke flytte, gi nytt navn til eller fjerne **Hjem**-knappen. **Avdelinger**-knappen kan fjernes fra navigasjonsruten, men ikke gis nytt navn eller flyttes.

### <a name="add-a-new-menu-button"></a>Legge til en ny menyknapp
Du kan opprette en ny knapp på rotnivå og deretter legge til en meny med koblinger under knappen for å åpne forskjellige sider.

1. Velg **Ny** i dialogboksen **Tilpass navigasjonsrute**, og skriv deretter inn et navn i **Navn**-feltet.
2.  Velg **OK**.

Du kan legge til koblinger i knappen.  

### <a name="add-a-link-to-a-button"></a>Legge til en kobling i en knapp   
Hvis du har tillatelse til å vise en oversikt, for eksempel ordreoversikten, kan du legge til en kobling til oversikten fra en knapp i navigasjonsruten.  

1.  Velg menyen der du vil legge til koblingen, i feltet **Navigasjonsruteknapper** i dialogboksen **Tilpass navigasjonsrute**.  

2.  Velg **Legg til**-knappen.  

3.  Bla til koblingen du vil legge til, og velg deretter **OK**-knappen.  
> [!TIP]
> Hvis du finner en kobling på **Avdelinger**-sidene, kan du også legge den til i navigasjonsruten. Hvis du vil ha mer informasjon, se delen Legge til en kobling fra avdelingene til rollesenteret.  

### <a name="move-or-copy-a-link-from-one-button-to-another"></a>Flytte eller kopiere en kobling fra én knapp til en annen  

1.  Velg menyen der koblingen vises for øyeblikket, i feltet **Navigasjonsruteknapper** i dialogboksen **Tilpass navigasjonsrute**.  

2.  I ruten **Oversikter** velger du koblingen du vil flytte, og deretter velger du **Flytt til** eller **Kopier til**  

3.  Velg navigasjonsknappen du vil legge til koblingen i, og klikk deretter **OK**-knappen.  

### <a name="rearrange-the-order-of-a-links-under-a-button"></a>Endre rekkefølgen for koblinger under en knapp  

1.  I **Oversikter**-ruten velger du koblingen du vil flytte.  

2.  Plasser koblingen ved hjelp av knappene **Flytt opp** og **Flytt ned**.

## <a name="adding-department-links-to-the-role-center"></a>Legge til avdelingskoblinger i rollesenteret
Noen ganger kan det hende at du på en **Avdelinger**-side finner en kobling som du vil legge til i rollesenteret ditt for enkel tilgang. Hvor du kan plassere koblingen i rollesenteret avhenger av kategorien for koblingen på **Avdelinger**-siden.

I tabellen nedenfor finner du en oversikt over hvilke typer koblinger som finnes i hver kategori på **Avdelinger**-sidene, og hvor du kan legge dem til i rollesenteret.  

|**Kategori**|**Viser**|**Legg til kobling i**|  
|------------------|------------------|---------------------|  
|Oversikter|Oversiktssider|**Hjem**-knappen i navigasjonsruten|  
|Oppgaver|Oppgavesider, kjørsler, forslag, kladder|Kategorien **Handlinger** i båndet|  
|Rapporter og analyse|Rapporter, kjørsler, matrisevinduer|Kategorien **Rapporter** i båndet|  
|Dokumenter|Dokumenter, for eksempel fakturaer og purringer|**Rapporter** i båndet|  
|Arkiv/historikk|Bokførte/ferdige bilag, registre|**Hjem**-knappen i navigasjonsruten|  
|Administrasjon|Oppsettvinduer|Kategorien **Handlinger** i båndet|  

### <a name="to-copy-department-links-to-your-role-center"></a>Slik kopierer du avdelingskoblinger til rollesenteret  

1.  Åpne **Avdelinger**-siden.  

2.  Høyrevelg koblingen, og velg deretter følgende (bare ett av disse alternativene vil være tilgjengelig).  

    |**Velg**|**Hvis du vil legge til koblingen i**|  
    |----------------|----------------------------|  
    |**Legg til i navigasjonsruten**|**Hjem**-knappen i navigasjonsruten i rollesenteret.|  
    |**Legg til i handlinger på rollesenterbånd**|Menyen **Handlinger** på båndet i rollesenteret|  
    |**Legg til i rapporter på rollesenterbånd**|**Rapporter**-menyen på båndet i rollesenteret.|  

3.  Bekreft meldingen som vises.  

 Den nye koblingen vises nå i menyen der du la den til. Det kan imidlertid være aktuelt å flytte koblingen til en annen posisjon på menyen. Hvis du for eksempel har lagt til en kobling i navigasjonsruten, vises den i **Hjem**-menyen, men du kan flytte den til en annen meny i navigasjonsruten. Se delen Tilpasse navigasjonsruten for mer informasjon.

## <a name="adding-charts-to-role-centers-and-list-pages"></a>Legge til diagrammer i rollesentre og på oversiktssider
Når du har kompleks informasjon, kan du ha behov for å se en visuell fremstilling av dataene for å avdekke tendenser og ta beslutninger. Du vil kanskje for eksempel overvåke saldiene per bankkonto for firmaet ditt i et diagram. Du bruker grafikkruten til å visuelt vise data fra en oversikt på følgende sidetyper:  

-   I rollesenteret, der du kan velge blant forhåndsdefinerte generiske diagrammer.  

-   På en oversiktsside, der du kan velge å vise en liste som et diagram.  

### <a name="to-add-a-generic-chart-to-your-role-center"></a>Slik legger du til et generisk diagram i rollesenteret:  

1.  I rollesenteret velger du ikonet for **Program**-menyen ![Programmeny-knappen på menylinjen](media/applicationmenuicon.png "ApplicationMenuIcon"), velg **Tilpass** og deretter **Tilpass denne siden**.  

2.  I **Tilgjengelige deler**-feltet i vinduet **Tilpass rollesenteret** velger du **Diagramdel**, og deretter velger du **Legg til**.  

3.  Bruk knappene **Flytt opp**, **Flytt ned**, **Flytt til venstre** og **Flytt til høyre** til å plassere diagramdelen på rollesenteret.  

4.  Velg diagramdelen og **Tilpass del**.  

5.  I **Tilpass diagram**-vinduet velger du det forhåndsdefinerte diagrammet du vil vise, og velger deretter **OK**-knappen.  

### <a name="to-view-a-list-as-a-chart"></a>Slik viser du en liste som et diagram:  

1.  Velg handlingen **Vis som diagram** på oversiktssiden.  

2.  Velg et mål og en dimensjon for å opprette et egendefinert diagram. Hvis du vil ha mer informasjon, kan du velge en sekundær dimensjon. Du kan for eksempel lage et enkelt stolpediagram ved å velge en dimensjon på x-aksen og deretter velge dimensjonen **Dimensjonsantall** på y-aksen.  

> [!NOTE]  
>  Som standard er grafikkruten skjult fordi den kan redusere programmets ytelse. Du bør bare vise diagrammet når du trenger informasjonen.  

## <a name="handling-external-files-and-automation-objects"></a>Håndtere eksterne filer og automatiseringsobjekter
Når [!INCLUDE[navnow_md](includes/navnow_md.md)] mottar en ekstern fil, vises en dialogboks. I tillegg til å velge hva du skal gjøre med filen kan du bestemme hvordan du vil behandle filtypen neste gang den blir mottatt.  

Når [!INCLUDE[navnow_md](includes/navnow_md.md)] må kjøre et automatiseringsobjekt, vises en dialogboks. Du kan bestemme om denne objekttypen alltid eller aldri skal kunne kjøre.  

### <a name="to-specify-how-to-handle-external-files"></a>Slik angir du hvordan eksterne filer skal behandles:  

1.  Når dialogboksen vises, fjerner du merket for **Be alltid om bekreftelse før denne typen filer åpnes.** hvis du vil at [!INCLUDE[navnow_md](includes/navnow_md.md)] skal huske hvilket alternativ du velger i trinn 2. Neste gang denne typen fil må håndteres, vises ikke dialogboksen, og filen vil bli behandlet som angitt i trinn 2.  

     Du kan også merke av for **Be alltid om bekreftelse før denne typen filer åpnes**, slik at det alltid vises en dialogboks denne filtypen blir mottatt.  

2.  Velg **Åpne**, **Lagre** eller **Avbryt**. Filen behandles i henhold til valget ditt.  

### <a name="to-specify-how-to-handle-automation-objects"></a>Slik angir du hvordan automatiseringsobjekter skal behandles:  

Når dialogboksen vises, merker du av for **Tillat alltid** hvis du vil at [!INCLUDE[navnow_md](includes/navnow_md.md)] alltid skal kjøre denne typen automatiseringsobjekt. Neste gang denne typen automatiseringsobjekt må kjøre, vises ikke dialogboksen og automatiseringsobjektet kjøres direkte.  

Du kan eventuelt merke av for **Tillat aldri**. Neste gang denne typen automatiseringsobjekt må kjøre, vises ikke dialogboksen og automatiseringsobjektet kjøres ikke.  

## <a name="CancelPersonalization"></a>Annullere tilpasning
Annullere tilpasning kan deles inn i to kategorier:

-   Annullere endringer du gjorde ved hjelp av **Tilpass**-funksjonen.
-   Annullere grunnleggende grensesnittendringer.

### <a name="cancel-customization"></a>Annullere tilpasning
Hvis du vil avbryte alle tilpassinger i brukergrensesnitt som du har gjort for en side under gjeldende brukerpålogging, eller siden du sist avbrøt tilpassinger i brukergrensesnittet, kan du bruke vinduet **Slett brukertilpasning**. Sideoppsettet du sletter tilpasningen for, tilbakestilles deretter til standardkonfigurasjonen for profilen.  

Hvis du vil avbryte tilpassingen i brukergrensesnittet som du har gjort i et bestemt område i brukergrensesnittet på en side, for eksempel båndet, kan du bruke **Gjenopprett standarder** i vinduet **Tilpass**. Oppsettet for det bestemte grensesnittområdet på denne siden tilbakestilles til standardkonfigurasjonen for profilen.  

#### <a name="to-cancel-all-ui-customization-that-you-have-made-to-a-page"></a>Slik annullerer du alle grensesnittilpasninger du har gjort på en side:  

1.  Skriv inn **Slett brukertilpasning** i **Søk**-boksen, og velg deretter den tilknyttede koblingen.  

2.  Velg siden du vil annullere grensesnittilpasningen for, og velg deretter **Slett** under **Vis** i fanebladet **Hjem**.  

> [!NOTE]  
>  Alle tilpassinger i brukergrensesnittet på siden som du har gjort under gjeldende brukerpålogging eller siden du sist brukte knappen **Slett brukertilpasning**, blir avbrutt. Sideoppsettet tilbakestilles til standardkonfigurasjonen for profilen din, som ble konfigurert av systemansvarlig eller installert med [!INCLUDE[navnow](includes/navnow_md.md)].  

#### <a name="to-cancel-ui-customization-that-you-have-made-to-a-ui-area-on-a-page"></a>Slik annullerer du grensesnittilpasning du har gjort i et grensesnittområde på en side:  

1.  Fra siden der du har tilpasset et grensesnittområde, for eksempel båndet, velger du ikonet for **Program**-menyen ![Programmeny-knappen på menylinjen](media/applicationmenuicon.png "ApplicationMenuIcon"), velger **Tilpass**, og deretter velger du **Tilpass <UI area>**.  

2.  Nederst i vinduet **Tilpass** velger du **Gjenopprett standarder**.  

> [!NOTE]  
>  Alle tilpassinger av brukergrensesnittområdet som du har gjort for siden under gjeldende brukerpålogging eller siden du sist brukte knappen **Gjenopprett standarder**, blir avbrutt. Sideoppsettet i grensesnittområdet på siden tilbakestilles til standardkonfigurasjonen for profilen din, som ble konfigurert av systemansvarlig eller installert med [!INCLUDE[navnow](includes/navnow_md.md)].

### <a name="cancel-basic-ui-changes"></a>Annullere grunnleggende grensesnittendringer
Du annullerer grunnleggende grensesnittendringer ved å åpne vinduet **Tilbakestill brukerdefinerte innstillinger** fra rollesenteret.  

Grunnleggende grensesnittendringer omfatter ting som:
 -  Endre størrelsen på og plasseringen av alle vinduer.
 -  Endre kolonnebredden
 -  Endre høyden på kolonneoverskrifter.
 -  Sortere etter kolonner i en liste.
 -  Vise lister som diagram.
 -  Angi hvordan eksterne filer og automatiseringsobjekter skal behandles.  

#### <a name="to-cancel-basic-ui-changes"></a>Slik annullerer du grunnleggende grensesnittendringer

1.  Gå til rollesenteret.  

     På **Program**-menyen ![Programmeny-knappen på menylinjen](media/applicationmenuicon.png "ApplicationMenuIcon") velger du **Tilpass** og deretter **Tilbakestill brukerdefinerte innstillinger**.  

2.  Velg **Tilbakestill innstillinger i brukergrensesnittet**. Du kan eventuelt velge knappen **Tilbakestill alle** for å avbryte beslutninger for behandling av filer og automatiseringsobjekter.  

 Alle grunnleggende endringer i brukergrensesnittet for [!INCLUDE[navnow_md](includes/navnow_md.md)], som du har utført under gjeldende brukerpålogging eller siden du sist valgte knappen **Tilbakestill innstillinger i brukergrensesnittet**, blir avbrutt. Brukergrensesnittet tilbakestilles til standardkonfigurasjonen for profilen.  

#### <a name="to-cancel-your-decision-for-running-or-saving-external-files"></a>Slik annullerer du beslutningen om kjøring og lagring av eksterne filer:  

1.  Gå til rollesenteret.  

     På **Program**-menyen ![Programmeny-knappen på menylinjen](media/applicationmenuicon.png "ApplicationMenuIcon") velger du **Tilpass** og deretter **Tilbakestill brukerdefinerte innstillinger**.  

2.  Velg **Tilbakestill filbehandlingsbeslutning**. Du kan eventuelt velge knappen **Tilbakestill alle** for å avbryte visningsendringer og beslutninger for behandling av filer og automatiseringsobjekter.  

 Alle avgjørelser for standardbehandling av filtypene, som du har gjort under gjeldende brukerpålogging eller siden du sist valgte knappen **Tilgang til klientfil**, blir avbrutt og tilbakestilt til standardkonfigurasjonen for profilen. Neste gang [!INCLUDE[navnow_md](includes/navnow_md.md)] mottar en ekstern fil av en hvilken som helst type, vises en dialogboks med alternativene **Lagre**, **Kjør** og **Avbryt**.  

### <a name="to-cancel-your-decision-for-handling-automation-objects"></a>Slik annullerer du beslutningen om håndtering av automatiseringsobjekter:  

1.  Gå til rollesenteret.  

     På **Program**-menyen ![Programmeny-knappen på menylinjen](media/applicationmenuicon.png "ApplicationMenuIcon") velger du **Tilpass** og deretter **Tilbakestill brukerdefinerte innstillinger**.  

2.  Velg **Opphev beslutninger om automatisering**. Du kan eventuelt velge knappen **Tilbakestill alle** for å avbryte visningsendringer og beslutninger for kjøring og lagring av eksterne filer.  

 Alle avgjørelser om hvordan du kjører automatiseringsobjekter, som du har utført under gjeldende brukerpålogging eller siden du sist valgte knappen **Tilbakestill avgjørelser om automatisering**, blir avbrutt. Virkemåten til filhåndteringen tilbakestilles til standardkonfigurasjonen for profilen. Neste gang [!INCLUDE[navnow_md](includes/navnow_md.md)] må kjøre et automatiseringsobjekt av en hvilken som helst type, vises en dialogboks med alternativene **Tillat alltid** og **Tillat aldri**.    

<!--Use the following table to get more information about customizing the different elements of the UI.

| To | See |
| --- | --- |
| Change which actions to show on the ribbon and how the actions are grouped. |[How to: Customize FastTabs](purchasing-how-record-purchases.md) |
|Change which FastTabs to show and which fields to include on the FastTabs.|[How to: Request Quotes](purchasing-how-request-quotes.md)|
|Add, remove, or arrange columns in a list or document-lines that represent fields in the underlying tables. |[ How to: Add or Remove Columns in a List or on Document Lines](purchasing-how-purchase-products-sale.md) |
| Rename or rearrange buttons, create a new menu button, add a link to a menu, or rearrange the order of a menu. |[ How to: Customize the Navigation Pane](purchasing-how-correct-cancel-unpaid-purchase-invoices.md) |
| Add a link from a department page to your Role Center. |[How to: Process Purchase Returns or Cancellations](purchasing-how-register-new-vendors.md) |
|Add a chart to your Role Center or to a list page.|[How to: Combine Receipts on a Single Invoice](purchasing-how-to-combine-receipts.md)|
| Unod personalization that you have made to your user interface, either for a specific area on a page, such as a ribbon, or for the whole page.|[How to: Cancel Personalization](ui-customization-cancel.md)|
-->


## <a name="see-also"></a>Se også
[Tilpasse arbeidsområdet i Dynamics webklienten](ui-personalization-user.md)  
[Oversikt over tilpasning](ui-personalization-overview.md)  

