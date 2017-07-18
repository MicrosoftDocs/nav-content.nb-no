---
title: Arbeide med GIFI-koder i Canada
author: SorenGP
ms.custom: na
ms.date: 09/21/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 695bca0a6836c47610210b759ae48af27484761f
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

#<a name="how-to-work-with-gifi-codes-in-canada"></a>Arbeide med GIFI-koder i Canada
Økonomiske informasjonen kan inkludere finanskontoer, rapporter, resultatregnskap, balanse og kontoutdrag for fri egenkapital. Økonomisk informasjon klassifiseres ved hjelp av koder. Bruken av koder lar myndighetene behandle informasjon, klargjøre for elektronisk lagring og validere mva-informasjon elektronisk. Bruken av koder bidrar også til at statistiske organisasjoner kan arbeide mer effektivt. Økonomiske opplysninger er for eksempel lettere tilgjengelig. Hvis du vil ha mer informasjon, kan du se [nettstedet for CRA](http://www.cra-arc.gc.ca/).

CRA bruker GIFI-koder (General Index of Financial Information) til å innhente, validere og behandle elektronisk økonomiske opplysninger og mva-informasjon. Anbefalt fremgangsmåte er å tilordne GIFI-koder bare til bokføringskonti, slik at alle summeringer gjøres av din programvare for mva-klargjøring.

Når en konto tilknyttes en GIFI-kode, rapporteres den til skattemyndighetene under denne koden. Flere konti kan alle ha samme GIFI-kode, men hver konto kan ha bare én GIFI-kode.

Du kan eksportere saldoinformasjon etter GIFI-kode og lagre den eksporterte filen i Excel, noe som er nyttig for overføring av informasjon til din programvare for mva-klargjøring.

## <a name="to-set-up-gifi-codes"></a>Definere GIFI-koder
I Dynamics NAV må du definere GIFI-koder for finanskontoer, rapporter, balanse, resultatregnskap og utdrag for fri egenkapital.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **GIFI-koder** og velger deretter den relaterte koblingen.
2. I vinduet **GIFI-koder** velger du handlingen **Ny**.
3. Definer GIFI-koder ved å fylle ut feltene. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.

## <a name="to-associate-gifi-codes-with-gl-accounts"></a>Knytte GIFI-koder til finanskonti
Hvis du vil rapportere økonomiske opplysninger, må hver GIFI-kode være tilknyttet de aktuelle kontoene i kontoplanen.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kontoplan** og velger deretter den relaterte koblingen.
2. Velg en relevant finanskonto, og velg deretter handlingen **Rediger**.
3. I hurtigfanen **Kostregnskap**, i **GIFI-kode**-feltet , velger du en passende GIFI-kode.

## <a name="to-view-account-balances-using-the-gifi-code-report"></a>Vise kontosaldoer ved hjelp av GIFI-koderapporten
Du kan se gjennom kontosaldoene etter GIFI-kode ved hjelp av rapporten **Kontosaldoer etter GIFI-koder**.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kontosaldoer etter GIFI-kode** og velger deretter den relaterte koblingen.
2. Angi hva du vil inkludere i rapporten ved å fylle ut feltene. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
3. Velg knappen **Skriv ut** eller **Forhåndsvisning**.

## <a name="to-export-balance-information-using-gifi-codes"></a>Eksportere saldoinformasjon ved hjelp av GIFI-koder
Du kan eksportere saldoinformasjon ved hjelp av GIFI-koder, og lagre den eksporterte filen i Excel. Du kan endre, lagre eller slette filen. Du kan bruke filen til å overføre informasjon til din programvare for mva-klargjøring.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Eksporter GIFI-informasjon til Excel** og velger deretter den relaterte koblingen.
2. Angi hva du vil eksportere til Excel ved å fylle ut feltene. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
3. Velg **OK**-knappen.

**Merk:** Excel-filen har følgende egenskaper:

* Saldoen er avrundet til nærmeste prosent, men celleverdien beholder den samme prosenten som den gjør i Finans.

* Negative tall representeres som positive tall i hakeparenteser. -123 er derfor representert som (123).

## <a name="see-also"></a>Se også
[Finans](finance-setup.md)   
[Definere kjerneprosesser for økonomi](finance-setup-setup-finance-setup.md)

