---
title: Registrere Dynamics NAV i Azure-administrasjonsportalen
author: edupont04
manager: edupont
ms.author: edupont
ms.custom: na
ms.date: 11/15/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 225773f7f686dd6e9a79f759d520d66f7e7b9d0a
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---
# <a name="how-to-register-dynamics-nav-in-the-azure-management-portal"></a>Registrere Dynamics NAV i Azure-administrasjonsportalen
Hvis du vil bruke tjenester som er basert på Microsoft Azure, må du registrere Dynamics NAV i Azure-administrasjonsportalen. Utvidelsen [Salgs- og lagerprognose](ui-extensions-sales-forecast.md) krever for eksempel at du angir en API-nøkkel og API-URI, og andre tjenester krever lignende informasjon. Så hvor du finner denne informasjonen?

Du kan bruke veiledningen **Konfigurer Azure-administrasjonsportalen** for å registrere Dynamics NAV i Azure-administrasjonsportalen og trekke ut informasjonen du trenger for å bruke tjenester, som utvidelsen Salgs- og lagerprognose, Power BI, Office 365 og så videre. Du trenger bare registrere deg i Azure-administrasjonsportalen én gang, og du må være administrator eller superbruker i Dynamics NAV.

Poenget med registreringen er at Dynamics NAV og tjenesten som du vil koble til, må du ha kjenne til Azure AD-detaljene (Azure Active Directory) om hverandre.

## <a name="to-register-dynamics-nav-in-the-azure-management-portal"></a>Slik registrerer du Dynamics NAV i Azure-administrasjonsportalen
1. Logg på Azure-administrasjonsportalen på [https://portal.azure.com](https://portal.azure.com).
    Hvis du ikke er kjent med Azure-administrasjonsportalen, finner du veiledning i [Azure-dokumentasjonsbiblioteket](https://azure.microsoft.com/en-us/documentation/articles).
2. I den venstre navigasjonsruten velger du **Flere tjenester**, og deretter velger du **Appregistreringer**.
3. I den øverste menyen velger du **Legg til**, og deretter fyller du ut feltene i **Opprett rute** med følgende informasjon:
    - **Navn**: Angi et navn for Dynamics NAV-løsning, for eksempel *Dynamics NAV*.
    - **Programtypen**: Velg **Nettapp*/API**.
    - **URL-adresse for pålogging**: Skriv inn URL-adressen for Dynamics NAV-nettleserklienten, for eksempel *https://MinServer:8080/DynamicsNAV/WebClient/OAuthLanding.htm*.
        OAuthLanding.htm-fil er en fil som hjelper deg med å administrere utveksling av data mellom Dynamics NAV og andre tjenester via Azure AD.
4. Velg **Opprett**-knappen.
    Dette legger Dynamics NAV til i **Appregistrering**-ruten, så du kan nå legge til innstillinger i den.
5. I **Appregistrering**-listen velger du den nye appen. Hvis dette ikke åpner **Innstillinger**-ruten, vil du se en handling for å åpne **Innstillinger**.
6. I **Innstillinger**-ruten i delen **API-tilgang**, velger du **Nøkler**.
7. I **Nøkler**-ruten angir du en beskrivelse og når du vil la nøkkelen utløpe, og velg deretter **Lagre**.
8. Kopiere den genererte nøkkelen til en midlertidig plassering. Du trenger den i neste prosedyre.
9. I delen **API-tilgang** velger du **Nødvendige tillatelser**.
    - Legg til delegerte tillatelser for å vise alle rapporter til Power BI-tjenesten
    - Legg til delegerte tillatelser for å logge på og lese brukerprofilen til Windows Azure Active Directory
    - Gjenta for andre tjenester du vil gi tilgang til din forekomst av Dynamics NAV
10. Lukk **Innstillinger**-ruten, og deretter, i **Grunnleggende**-ruten, kopierer du verdien for **applikasjons-ID** til en midlertidig plassering.

Du har nå registrert Dynamics NAV i Azure-administrasjonsportalen, du har gitt tilgang til relevante tjenester, og du har trukket ut informasjonen du trenger i Dynamics NAV.  

## <a name="to-add-the-information-to-dynamics-nav"></a>Slik legger du til informasjonen i Dynamics NAV
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Veiviser for installasjon av Azure AD-app** og velger deretter den relaterte koblingen.
2. Velg **Neste** i veiviseren.
3. I **Klient-ID**-feltet angir du hvilket innhold du kopierte fra **applikasjons-ID**-feltet tidligere.
4. I **Hemmelig nøkkel**-feltet angir du hvilket innhold du kopierte fra **Nøkler**-ruten tidligere.
5. Velg **Neste**. Hvis du ikke ser en feilmelding, er du nå ferdig.

Dynamics NAV er registrert og klar til å koble til tjenester som Cortana Intelligence og Power BI.

## <a name="see-also"></a>Se også
[Salgs- og lagerprognose](ui-extensions-sales-forecast.md)  
[Konfigurere Dynamics NAV](setup.md)  

