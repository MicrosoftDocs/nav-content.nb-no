---
title: Bruke Dynamics NAV Content Pack for Power BI
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: ad9519b8ce9c244480308ccc99c05e78e4926b06
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---

# <a name="using-the-dynamics-nav-content-pack-for-power-bi"></a>Bruke Dynamics NAV Content Pack for Power BI
Få innsikt i Dynamics NAV-dataene på en enkel måte med Power BI og Dynamics NAV-innholdspakken. Power BI henter dataene, og deretter bygger du et forhåndskonfigurert instrumentbord og rapporter basert på dataene.  

Content Pack er forhåndskonfigurert til å arbeide med salgsdata og økonomiske data fra demonstrasjonsselskapet som du får når du registrerer deg for Dynamics NAV -forhåndsvisning.  

- Velg hvilken som helst visning på instrumentbordet for å hente frem en av sju underliggende rapportene.  
- Filtrere rapporten eller legg til felt som du vil overvåke.  
- Fest denne tilpassede visningen på instrumentbordet for å fortsette sporing.  
Instrumentbordet og underliggende rapporter oppdateres daglig. Du kan kontrollere tidsplanen for oppdatering og endre hyppigheten for datasettet.  

## <a name="accessing-dynamics-nav-in-power-bi"></a>Tilgang til Dynamics NAV i Power BI
Hvis du vil se Dynamics NAV-dataene i Power BI, må du ha følgende:  

- Tilgang til Dynamics NAV. Hvis du vil ha mer informasjon, kan du se [Dynamics NAV](http://go.microsoft.com/fwlink/?LinkID=759714).  
- Tilgang til Power BI. Hvis du vil ha mer informasjon , kan du se [Power BI](https://powerbi.microsoft.com).

På Power BI-nettstedet finner du mer informasjon om hvordan du [legger til Dynamics NAV Content Pack i Power BI](http://go.microsoft.com/fwlink/?LinkID=760850).  

Hvis du vil ha tilgang til Dynamics NAV Content Pack i Power BI, må du angi følgende informasjon i tilkoblingsvinduet:

| Felt       | Beskrivelse              |
|-------------|--------------------------|
|**Nettadresse for OData-feed**|Nettadressen til OData, slik at Power BI får tilgang til data fra firmaet, for eksempel https://mittfirma.com:7048/MS/OData/Company('CRONUS%20US').|
|**Godkjenningsmetode**|Velg **Grunnleggende**.|
|**Brukernavn**|E-postkontoen som du brukte til å registrere deg for Dynamics NAV, for eksempel *me@mybusiness.com*.|
|**Passord**|Dette er tilgangsnøkkelen for webtjenesten for brukerkontoen i Dynamics NAV.|

Dette betyr at du må ha to deler av informasjon fra Dynamics NAV: Nettadressen for OData og tilgangsnøkkelen for webtjenesten for din brukerkonto.  
**Hente nettadressen**  
Når du legger til Dynamics NAV i Power BI, må du angi en nettadresse slik at Power BI kan få tilgang til data fra firmaet. I tilkoblingsvinduet kalles nettadressen **Nettadresse for OData-feed**, og den må ha følgende format:

         https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
I dette eksemplet er *mittfirma* navnet på Dynamics NAV-tjenesten, og *CRONUS US* er navnet på demonstrasjonsselskapet der *%20* representerer mellomrommet i navnet.   
Hvis du vil hente nettadressen, søler du etter og åpner vinduet **Webtjeneste** i Dynamics NAV. Dette vinduet viser webtjenester som er tilgjengelige, og du kan kopiere koblingen fra feltet **Nettadresse for OData** for en av de standard OData-webtjenestene.  
**Hente tilgangsnøkkel for webtjeneste**  
Hvis du vil bruke data fra Dynamics NAV må du i Power BI angi brukernavnet ditt, som er e-postkontoen din, og et passord, i vinduet **Koble til Dynamics NAV**. Passordet er tilgangsnøkkelen for webtjenesten som er angitt for brukerkontoen i Dynamics NAV.  
hvis du vil hente en tilgangsnøkkel for webtjeneste i Dynamics NAV, søker du etter **Brukere**-vinduet og åpner deretter kortet for brukerkontoen din. I hurtigfanen **Webtjeneste – tilgang** kopierer du innholdet i feltet **Webtjeneste – tilgangsnøkkel**. Hvis feltet er tomt, går du til båndet og velger **Endre tilgangsnøkkel for webtjeneste**, velger feltet **Nøkkel utløper aldri** og velger deretter OK. Deretter kan du kopiere nøkkelen.  

## <a name="getting-data-from-dynamics-nav"></a>Hente data fra Dynamics NAV
Dynamics NAV-instrumentbordet viser de vanligste rapportene som du vil bruke til å spore din virksomhet. Dataene blir hentet fra Dynamics NAV-firmaet ved hjelp av webtjenester for å lese sanntidsdata. I Dynamics NAV viser vinduet **Webtjenester** webtjenester som er satt opp for deg, inkludert følgende som brukes av Content Pack i Power BI:  

- ItemSalesAndProfit  
- ItemSalesByCustomer  
- powerbifinance-setup  
- SalesDashboard  
- SalesOpportunities  
- SalesOrdersBySalesPerson  
- TopCustomerOverview  

**Merk**: Hvis du endrer navnet på noen av disse webtjenestene, vises ikke dataene vil ikke i Power BI.  
Hvis du vil legge til bruker andre data i Power BI, må du finne tabellene i Dynamics NAV, vise dem som webtjenester og deretter legge dem til i Content Pack. Dette er et avansert scenario, og vi anbefaler at du starter med data som allerede er tilgjengelige i Power BI.  

## <a name="troubleshooting"></a>Feilsøking
Power BI-instrumentbordet er avhengig av de publiserte webtjenestene som er nevnt ovenfor, og du vil se data fra demonstrasjonsselskapet eller ditt eget selskap hvis du importerer data fra din gjeldende økonomiløsning. Hvis noe går galt, vil denne delen imidlertid gir en løsning for de vanligste problemene.  

**"Parametervalidering mislyktes, må du kontrollere at alle parametrene er gyldige"**  
Hvis du ser denne feilen når du angir nettadressen for Dynamics NAV, må du kontrollere at følgende krav er oppfylt:  

- Nettadressen har nøyaktig dette mønsteret:

    https://mittfirma.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
- Slett all tekst etter firmanavnet i parentes  
- Kontroller at det ikke er en etterfølgende skråstrek på slutten av nettadressen.  
- Kontroller at det er en sikker tilkobling, som angis ved at nettadressen begynner med *https*.  


**"Påloggingen mislyktes"**  
Hvis du får en "påloggingen mislyktes"-feil når du logger på instrumentbordet ved hjelp av Dynamics NAV-legitimasjonen, kan dette skyldes ett av følgende problemer:

* Kontoen du bruker har ikke tillatelse til å lese Dynamics NAV-dataene fra kontoen din.

    Kontroller brukerkontoen i Dynamics NAV, og kontroller at du har brukt riktig tilgangsnøkkel for webtjeneste som passord, og prøv deretter på nytt.  
* Dynamics NAV-forekomsten som du prøver å koble til, har ikke et gyldig SSL-sertifikat. I dette tilfellet vil du se en mer detaljert feilmelding ("kan ikke opprette en klarert relasjon for SSL").

    **Merk**: Selvsignerte sertifikater støttes ikke.  


**"Oops"**  
Hvis du ser en "Oops"-feilmelding etter at du har fullført godkjenningsdialogboksen, forårsakes dette vanligvis av et problem med tilkoblingen til dataene for Content Pack.

* Kontroller at nettadressen følger mønsteret som ble angitt tidligere:

    https://mittfirma.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
* En vanlig feil er å angi den fullstendige nettadressen for en bestemt webtjeneste:

    https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')/powerbifinance-setup  
* Det kan også hende du har glemt å angi navnet på firmaet:

    https://mittfirma.projectmadeira.com:7048/MS/OData/  


## <a name="see-also"></a>Se også
[Velkommen til Dynamics NAV](across-get-started.md)  

