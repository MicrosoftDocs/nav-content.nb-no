---
title: "Feilsøke registrering for Self-Service"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 931c427518694cbd0003ea82735292a019b388d5
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="troubleshooting-self-service-sign-up"></a>Feilsøke registrering for Self-Service
Registrering for Dynamics NAV er enkelt og kan gjøres svært raskt. Du kan opprette en gratis konto selv om du er en eksisterende organisasjon. Denne artikkelen beskriver problemer som kan oppstå under registrering.

## <a name="what-email-address-can-i-use-with-dynamics-nav"></a>Hvilken e-postadresse kan jeg bruke med Dynamics NAV?
Dynamics NAV krever at du bruker et e-postadresse for arbeid eller skole for å registrere deg. Dynamics NAV støtter ikke e-postadressene levert av e-posttjenester for forbrukere eller telekommunikasjonsleverandører. Dette inkluderer outlook.com, hotmail.com, gmail.com og andre.

Hvis du prøver å registrere deg med en personlig e-postadresse, får du en melding om å bruke en e-postadresse for arbeid eller skole.

## <a name="troubleshooting"></a>Feilsøking
I mange tilfeller kan du registrere deg for Dynamics NAV ved å følge registreringsprosessen nedenfor. Det er imidlertid flere grunner til hvorfor du ikke kanskje ikke kan fullføre registrering for Self-Service. Tabellen nedenfor viser en oversikt over noen av de vanligste årsakene som du ikke kanskje kan fullføre registreringen og metoder for midlertidig løsning av disse problemene.

|Symptom/feilmelding                                                                             |Årsak og løsning|
|--------------------------------------------------------------------------------------------------|--------------------|
|For e-postadresser for Office 365 som ikke er registrert i USA, kan du få en melding som følgende, under registrering: <br>**Dette fungerte ikke. Vi støtter ikke landet eller området ennå.**<br> |Dynamics NAV støtter for øyeblikket bare USA-registrert e-postkontoer for Office 365.|
|Personlige e-postadresser, som nancy@gmail.com, støttes ikke. Du får en feilmelding som følgende, under registrering: <br>**Du har angitt en personlig e-postadresse: Skriv inn e-postadressen for arbeid, slik at vi kan lagre firmaets data på en sikker måte.**<br> eller <br> **Dette ser ut som en personlig e-postadresse. Skriv inn adressen til arbeid, slik at vi kan koble til andre i firmaet. Og ikke bekymre deg. Vi deler ikke adressen din med andre.** | Dynamics NAV støtter ikke e-postadressene levert av e-posttjenester for forbrukere eller telekommunikasjonsleverandører. Hvis du vil fullføre registreringen, kan du prøve på nytt med en e-postadresse som er tilordnet arbeid eller skole. Hvis du fremdeles ikke kan registrere deg og er villig til å fullføre et mer avansert oppsett, kan du registrere for et nytt prøveabonnement for Office 365 og bruke den e-postadressen til å registrere deg.
|.gov- eller .mil e-postadresser Du mottar en melding som følgende, under registrering: <br>**Dynamics NAV er ikke tilgjengelig: Dynamics NAV er ikke tilgjengelig for brukere med e-postadressene .gov eller .mil på dette tidspunktet. Bruk en annen e-postadresse for arbeid eller kom tilbake senere.** <br>eller <br>**Vi kan ikke fullføre registreringen din. Det ser ut som Dynamics NAV ikke er tilgjengelig for arbeid eller skole.**|Dynamics NAV støtter ikke .gov- eller .mil-adresser på dette tidspunktet.|
|Registrering for Self-service er ikke aktivert. Du får en feilmelding som følgende, under registrering: <br>**Vi kan ikke fullføre registreringen din. IT-avdelingen har deaktivert registrering for Dynamics NAV. Kontakt dem for å fullføre registreringen.** <br>eller <br> **Dette ser ut som en personlig e-postadresse. Skriv inn adressen til arbeid, slik at vi kan koble til andre i firmaet. Og ikke bekymre deg. Vi deler ikke adressen din med andre.**|Organisasjonens systemansvarlige har deaktivert registrering for Self-service for Dynamics NAV. Hvis du vil fullføre registreringen, kontakter du systemansvarlig og ber om å følge instruksjonene på siden nedenfor, slik at eksisterende brukere kan registrere seg for Dynamics NAV og nye brukere kan bli med i eksisterende leietaker. Du kan også oppleve dette problemet hvis du registrerte deg for Office 365 via en partner.|
|E-postadressen er ikke en Office 365-ID. Du får en feilmelding som følgende, under registrering: <br>**Vi finner deg ikke på contoso.com. Bruker du en annen ID på arbeid eller skole? Prøv å logge på med denne, og hvis det ikke fungerer, kan du kontakte IT-avdelingen.**|Organisasjonen din bruker ID-er til å logge på Office 365 og andre Microsoft-tjenester, som er forskjellig fra e-postadressen din. E-postadressen din kan for eksempel være Nancy.Smith@contoso.com, men ID-en er nancys@contoso.com. hvis du vil fullføre registreringen, kan du bruke ID-en som organisasjonen har tilordnet for å logge på Office 365 eller andre Microsoft-tjenester. Hvis du ikke vet hva dette er, kontakter du systemansvarlig. Hvis du fremdeles ikke kan registrere deg og er villig til å fullføre et mer avansert oppsett, kan du registrere for et nytt prøveabonnement for Office 365 og bruke den e-postadressen til å registrere deg.|


## <a name="see-also"></a>Se også
[Velkommen til Dynamics NAV](across-get-started.md)  
[Arbeide med Dynamics NAV](ui-work-product.md)




