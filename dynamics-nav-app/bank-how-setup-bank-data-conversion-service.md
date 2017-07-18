---
title: Konfigurere tjeneste for konvertering av bankdata
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 801e2abee52ec9804028a797e4f330b5e080549a
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-the-bank-data-conversion-service"></a>Konfigurere tjeneste for konvertering av bankdata
Du kan eksportere betalingslinjer fra vinduet **Betalingskladd** til en datastrøm som du deretter laster opp til banken for automatisk behandling, slik at du ikke trenger å foreta elektroniske betalinger individuelt. Hvis du vil ha mer informasjon, kan du se [Eksportere betalinger til en bankfil](payables-how-export-payments-bank-file.md).

En global tjenesteleverandør for å konvertere betalingsinformasjon til hvilket som helst dataformat banken krever, er koblet til og klar til å aktiveres i Dynamics NAV.

Du kan også bruke tjenesten for bankdatakonvertering til å konvertere en bankkontoutdragsfil du mottar fra banken, til en datastrøm du kan importere til Dynamics NAV, som et alternativ til bankdatafeedtjenesten Envestnet. Hvis du vil ha mer informasjon, kan du se [Utligne betalinger automatisk og avstemme bankkonti](receivables-apply-payments-auto-reconcile-bank-accounts.md).

**Merk**: Konverteringstjenesten for bankdata kan sette en grense for hvor mange linjer som kan eksporteres i én fil. Du får en feilmelding hvis grensen er overskredet. Det anbefales at bankkontoutdragsfiler ikke overstiger 1 000 linjer, siden behandlingstiden i konverteringstjenesten for bankdata kan øke betraktelig.

## <a name="to-sign-your-company-up-for-the-bank-data-conversion-service"></a>Slik registrerer du selskapet for tjenesten for bankdatakonvertering:
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Tjenesteoppsett for bankdatakonvertering** og velger deretter den relaterte koblingen.  
2. Vinduet **Tjenesteoppsett for bankdatakonvertering** åpnes med tre felt som er forhåndsutfylt med de aktuelle URL-adressene til leverandøren av konverteringstjenesten for bankdata.

    **Merk**: I CRONUS International Ltd. -demonstrasjonsdatabasen blir feltene Brukernavn og Passord forhåndsutfylt med påloggingsinformasjon for demonstrasjon som du erstatter med selskapets faktiske informasjon når du registrerer deg for konverteringstjenesten for bankdata.
3. I feltet **Nettadresse for registrering** velger du nettleserknappen for å åpne registreringssiden for tjenesteleverandøren.  
4. På registreringssiden for tjenesteleverandøren av bankdata, skriver du inn brukernavn og passord for firmaets tjenesteabonnement, og deretter fullfører du registreringsprosessen som beskrevet av tjenesteleverandøren.

    Selskapet er nå registrert for tjenesten for bankdatakonvertering. Fortsett med å skrive inn brukernavnet og passordet som du angav for tjenesten i de tilknyttede oppsettfeltene i Dynamics NAV.
5. I vinduet **Tjenesteoppsett for bankdatakonvertering**, i **Brukernavn**-feltet, angir du den samme verdien du angav som påloggingsnavn på tjenesteleverandørens side i trinn 4.
6. I **Passord**-feltet angir du den samme verdien du angav i **Passord**-feltet på tjenesteleverandørens side i trinn 4.

## <a name="to-encrypt-your-login-information"></a>Slik krypterer du påloggingsinformasjonen:
Det anbefales at du beskytter påloggingsinformasjonen du angir i vinduet **Tjenesteoppsett for bankdatakonvertering**. Du kan kryptere data på Dynamics NAV-serveren ved å generere nye eller importere eksisterende krypteringsnøkler du aktiverer på Dynamics NAV-serverforekomsten som kobler til databasen.

1. I vinduet **Tjenesteoppsett for bankdatakonvertering** velger du handlingen **Krypteringsadministrasjon**.
2. I vinduet **Administrasjon av datakryptering** aktiverer du kryptering av dataene.

##<a name="to-view-or-update-the-list-of-currently-supported-bank-data-formats"></a>Vise eller oppdatere listen over gjeldende bankdataformater som støttes
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Tjenesteoppsett for bankdatakonvertering** og velger deretter den relaterte koblingen.
2. Velg handlingen **Banknavn – datakonverteringsliste** i vinduet **Tjenesteoppsett for bankdatakonvertering** for å åpne oversikten over banknavn som representerer bankdataformater som støttes av konverteringstjenesten.
3. På siden **Banknavn – datakonverteringsliste** velger du handlingen **Oppdater banknavnliste**.

Listen over bankdataformater som støttes av tjenesten for bankdatakonvertering, er nå oppdatert. Dette er listen over banknavn, filtrert etter land/område, som du kan velge blant i feltet **Banknavn – datakonvertering** i vinduet **Bankkort**.

**Merk**: Oppdateringen av bankdataformater som støttes, oppstår også når du velger eller angir en verdi i feltet **Banknavn – datakonvertering** i bankkontoen.

Du har nå registrert deg for tjenesten for bankdatakonvertering. Fortsette med å gjenspeile informasjonen for hver bankkonto skal bruke tjenesten.

## <a name="to-set-up-bank-accounts-to-use-the-bank-data-conversion-service"></a>Slik oppretter du bankkonti som bruker tjenesten for bankdatakonvertering:
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Bankkonti** og velger deretter den relaterte koblingen.
2. Åpne kortet for en bankkonto som du vil eksportere eller importere bankfiler for, ved hjelp av tjenesten bankdatakonvertering.
3. I hurtigfanen **Overføring**, i feltet **Betalingseksportformat**, velger du **Tjeneste for bankdatakonvertering – kredittoverføring** for å definere betalingseksport.
4. I feltet **Banknavn – datakonvertering** angir eller velger du navnet på bankdataformatet som du registrerte deg for i trinn 4 i avsnittet “Registrere deg for konverteringstjenesten for bankdata”.
5. Gjenta trinn 1 til og med 4 for andre bankkonti som skal bruke konverteringstjenesten for bankdata.

## <a name="see-also"></a>Se også  
[Definere bankvesen](bank-setup-banking.md)  
[Håndtere bankkonti](bank-manage-bank-accounts.md)

