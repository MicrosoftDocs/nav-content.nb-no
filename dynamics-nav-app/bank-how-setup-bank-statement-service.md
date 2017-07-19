---
title: Konfigurere bankfeedservicen Envestnet Yodlee
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 270568214afd2ca8af15f0fa7640337c77ec2f1e
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-the-envestnet-yodlee-bank-feeds-service"></a>Konfigurere bankfeedservicen Envestnet Yodlee
Du kan importere elektroniske bankkontoutdrag fra banken slik at du raskt kan fylle ut vinduet **Betalingsavstemmingskladd**. Dermed kan du utligne betalinger og avstemme bankkontoen. Hvis du vil ha mer informasjon, kan du se [Utligne betalinger automatisk og avstemme bankkonti](receivables-apply-payments-auto-reconcile-bank-accounts.md).

**Merk**: The Envestnet Yodlee Bank Feeds-tjenesten eller en annen leverandørs bankfeedtjeneste, er kanskje ikke tilgjengelig i systemet. Hvis du vil bruke en bankfeedtjeneste til å importere bankkontoutdrag, kontakter du Microsoft-partneren din.

Når du har aktivert bankfeedservicen, må du koble den aktuelle bankkontoen til nettbankkontoen som feeden vil komme fra. Du kobler bankkonti til nettbankbankkonti i følgende ulike scenarier:

- En bankkonto finnes ikke i Dynamics NAV for nettbankkontoen. Du kan derfor opprette bankkontoen ved å koble fra nettbankkontoen.
- Det finnes en bankkonto i Dynamics NAV som du vil koble til en nettbankkonto.
- Tilkoblingen for en koblet bankkonto må være fjernet fordi du vil slutte å bruke bankfeedservice for kontoen.
- Nettbankkontoer er endret, og du vil oppdatere informasjon om bankkonti i Dynamics NAV.

Når bankfeedservicen er aktivert, kan du angi en bankkonto til automatisk å importere nye bankkontoutdrag til vinduet **Betalingsavstemmingskladd** hver annen timer. Transaksjoner for betalinger som allerede er bokført som utlignet og/eller avstemt i vinduet **Betalingsavstemmingskladd** vil ikke bli importert. Hvis du vil ha mer informasjon, kan du se avsnittet “Aktivere automatisk import av bankkontoutdrag”.

**Merk**: Hvis du bruker det assisterte oppsettet Konfigurer selskap, vil noen av trinnene i fremgangsmåtene nedenfor utføres automatisk når du kommer til firmaoppsettet for bankkontoen. Hvis du vil ha mer informasjon, kan du se [Velkommen til Dynamics NAV](across-get-started.md).

## <a name="to-enable-the-bank-feed-service"></a>Aktivere bankfeedservicen
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Bankkonti** og velger deretter den relaterte koblingen.
2. Åpne bankkontoen som du vil bruke for bankfeedservicen.
3. I vinduet **Bankkonto**, i feltet **Importformat for bankkontoutdrag**, velger du YODLEEBANKFEED.  

Bankfeedservicen vil bli aktivert når du kobler en bankkonto til den relaterte nettbankkontoen. Se den neste fremgangsmåten.  

## <a name="to-create-a-new-linked-bank-account"></a>Opprette ny tilknyttet bankkonto
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Bankkonti** og velger deretter den relaterte koblingen.
2. Velg den relevante bankkontoen, og velg deretter **Opprett ny tilknyttet bankkonto**. Vinduet **Bankkontotilknytning** åpnes etter en liten stund.

    **Merk**: Dette vinduet viser den faktiske nettsiden for bankfeedservicen Envestnet Yodlee. Terminologi og funksjonene i vinduet samsvarer kanskje ikke med instruksjonene i dette emnet.  
3. I vinduet **Tilknytning til nettbankkonto**, i ruten **Bankkontotilknytning**, bruker du søkefunksjonen til å finne banken der du har en eller flere nettbankkontoer.
4. Velg banknavn. Ruten **Logg på** åpnes.
5. Skriv inn brukernavnet og passordet du bruker til å logge på nettbanken, og velg deretter **Neste**.  
6. Bankfeedservicen klargjør å koble den første nettbankkontoen i den angitte banken, til en ny bankkonto i Dynamics NAV.

    **Merk**: Hvis du har mer enn én nettbankkonto i banken, må du opprette flere bankkonti i Dynamics NAV for disse ekstra nettbankkontoene. Se trinn 8 til 10.

    Når prosessen er fullført, vises banknavnet på i ruten **Mine kontoer** i kategorien **Tilknyttet**. Tallet i parentes angir hvor mange nettbankkontoer som ble tilknyttet.
7. Velg **OK**-knappen.

    Hvis bare én nettbankkonto er tilknyttet, åpnes vinduet **Bankkort** for det en ny bankkonto, forhåndsutfylt med navnet på nettbankkontoen. I dette tilfellet er tilknytningen av bankkontoen fullført. Det eneste som gjenstår er å opprette en bankkonto. Hvis du vil ha mer informasjon, kan du se [Opprette bankkonti](bank-how-setup-bank-accounts.md).

    Hvis mer enn én nettbankkonto ble tilknyttet, åpnes vinduet **Bankkontotilknytning** som viser alle nettbankkontoene som ikke er knyttet til bankkontoene i Dynamics NAV ennå. I det tilfellet følger du det neste trinnet.  
8. I vinduet **Bankkontotilknytning** velger du linjen for en nettbankkonto, og deretter velger du handlingen **Tilknytt ny bankkonto**.

    Vinduet **Bankkort** åpnes for det en ny bankkonto, forhåndsutfylt med navnet på nettbankkontoen.

    Hvis det allerede finnes en bankkonto i Dynamics NAV som du vil tilknytte nettbankkontoen, følger du fremgangsmåten nedenfor.  
9. I vinduet **Bankkontotilknytning** velger du linjen for en nettbankkonto, og deretter velger du handlingen **Tilknytt eksisterende bankkonto**.
10. I vinduet **Bankkontooversikt** velger du bankkontoen du vil knytte til, og deretter velger du **OK**-knappen.

## <a name="to-link-a-bank-account-to-an-online-bank-account"></a>Knytte en bankkonto til en nettbankkonto
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Bankkonti** og velger deretter den relaterte koblingen.
2. Velg linjen for en bankkonto som ikke er tilknyttet en nettbankkonto, og velg deretter handlingen **Tilknytt nettbankkonto**. Vinduet **Tilknytning til nettbankkonto** åpnes med navnet til banken forhåndsutfylt i ruten **Bankkontotilknytning**.
3. Velg banknavn. Ruten **Logg på** åpnes.
4. Skriv inn brukernavnet og passordet du bruker til å logge på nettbanken, og velg deretter **Neste**.

    Bankfeedservicen klargjør å koble bankkontoen i Dynamics NAV til den relaterte nettbankkontoen.

    Når prosessen er fullført, vises banknavnet på i ruten **Mine kontoer** i kategorien **Tilknyttet**. Hvis banken har mer enn én bankkonto, tilknyttes bare bankkontoen du valgte i trinn 2.
5. Velg **OK**-knappen.

I vinduet **Bankkontooversikt** er det merket av for **Tilknyttet**.

## <a name="to-unlink-a-bank-account"></a>Fjerne tilknytning for en bankkonto
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Bankkonti** og velger deretter den relaterte koblingen.  
2. Velg linjen for en tilknyttet bankkonto som du vil fjerne tilknytningen for en relatert nettbankkonto, og velg deretter handlingen **Fjern tilknytning for nettbankkonto**.

**Merk**: Hvis du velger **Ja** i bekreftelsesdialogboksen, fjernes tilknytningen til nettbankkontoen og påloggingsdetaljene nullstilles. Hvis du vil tilknytte bankkontoen til nettbankkontoen på nytt, må du logge på banken. Hvis du vil ha mer informasjon, kan du se avsnittet “Knytte en bankkonto til en nettbankkonto“.

## <a name="to-update-bank-account-linking"></a>Oppdatere bankkontotilknytning
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Bankkonti** og velger deretter den relaterte koblingen.
2. Velg den relevante bankkontoen, og velg deretter handlingen **Oppdater bankkontotilknytning**.

Hvis det finnes problemer for noen av de tilknyttede bankkontoene i vinduet **Bankkontooversikt**, åpnes vinduet **Bankkontotilknytning** som viser hvilke bankkontoer som har problemer. Problemer kan løses best ved å fjern tilkoblingen til nettbankkontoen og opprette tilknytningen på nytt. Hvis du vil ha mer informasjon, kan du se avsnittet “Knytte en bankkonto til en nettbankkonto“.

## <a name="to-enable-automatic-import-of-bank-statements"></a>Aktivere automatisk import av bankkontoutdrag
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Bankkonti** og velger deretter den relaterte koblingen.
2. Velg linjen for en tilknyttet bankkonto, og velg deretter handlingen **Oppsett for automatisk bankkontoutdragsimport**.
3. I vinduet **Oppsett for automatisk bankkontoutdragsimport**, i feltet **Antall dager inkludert**, angir du hvor langt tilbake i tid nye banktransaksjonene skal hentes.

    **Merk**: Det anbefales at du setter denne verdien til 7 dager eller mer.
4. Merk av for **Aktivert**.  
Hver time fylles vinduet **Betalingsavstemmingskladd** med eventuelle nye betalinger som er gjort i nettbankkontoen.

**Merk**: Transaksjoner for betalinger som allerede er bokført som utlignet og/eller avstemt i vinduet **Betalingsavstemmingskladd** vil ikke bli importert.

## <a name="see-also"></a>Se også  
[Definere bankvesen](bank-setup-banking.md)  
[Håndtere bankkonti](bank-manage-bank-accounts.md)  
[Bruke betalinger automatisk og avstemme bankkonti](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
[Tilpasse Dynamics NAV ved hjelp av utvidelser](ui-extensions.md)

