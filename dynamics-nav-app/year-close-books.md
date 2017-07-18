---
title: "Lukk bøker"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: ad75bfd18936df07e0fe9dcc5ed6bb94360ea965
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---
# <a name="close-books"></a>Lukk bøker
Når du har kontrollert at alle kontiene er oppdatert og har fordelt kost og inntekt, kan du lukke tablåene for et regnskapsår eller en periode.

Du trenger ikke å avslutte et år, men hvis du gjør det, blir det enklere å arbeide i systemet, ettersom du kan dra nytte av de gode filtreringsalternativene. Du trenger heller ikke å bekymre deg om å miste detaljer i transaksjoner når du avslutter, ettersom alle detaljer beholdes, selv etter at du har avsluttet året.

## <a name="closing-book-process"></a>Prosess for avslutning av tablå
Prosessen for å avslutte tablået omfatter disse hovedoppgaver:

1. Avslutte regnskapsperioden.

    Et regnskapsår er definert som én eller flere åpne perioder, som definert på siden **Regnskapsperioder**. Et vanlig regnskapsår består av 12 perioder på én måned hver, men du kan også velge en annen metode for å definere et år.

    Hvis du vil ha mer informasjon, kan du se [Avslutte regnskapsperioder](year-close-account-periods.md).

2. Registrere etterposter.

    Når du lukker et regnskapsår, må du angi flere administrative transaksjoner (for eksempel forhåndsbetalte og påløpte varer). Disse transaksjonene kalles justeringsposter. Det finnes ingen spesielle regler for bokføring av disse postene, og de (som andre poster) har en avmerking i **Etterpost**-feltet hvis de ble bokført på en dato i et lukket regnskapsår. Selv om et regnskapsår er avsluttet, kan du bokføre finansposter i det.

3. Overføre saldi fra resultatregnskapskontiene til balansen.

    Når et regnskapsår er lukket og alle etterposter er bokført, må resultatregnskapskontiene lukkes og nettoinntekten for året overføres til en konto under eiernes egenkapital i balansen. Bruk kjørselen Lukk resultatregnskapet til dette formålet. Kjørselen behandler alle finanskonti av typen Resultatregnskap og oppretter poster som tilbakefører saldiene. Disse postene er plassert i en kladd de kan bokføres fra. Kjørselen bokfører dem ikke automatisk, med unntak av når en tilleggsrapporteringsvaluta brukes. Når en tilleggsrapporteringsvaluta brukes, bokfører kjørselen direkte mot Finans.

    Hvis du vil ha mer informasjon,kan du se [Avslutte resultatregnskap](year-close-income-statement.md).
4. Bokføring av avslutningsposten for årsslutt sammen med motregning av poster på egenkapitalkontoen.

    Når kjørselen Avslutt resultatregnskapet er fullført, kan du bokføre poster som er generert av jobben. Hvis du ikke har angitt en konto for fri egenkapital i kjørselen, angir du en linje med en balansepost som bokfører nettoinntekten til riktig finanskonto under eiernes egenkapital i balansen. Til slutt bokfører du kladden.

    Hvis du vil ha mer informasjon, kan du se [Bokføre avslutningspost for årets slutt](year-how-post-year-end-close-entry.md).

## <a name="what-happens-when-you-close"></a>Dette skjer når du avslutter
Når du avslutter ved utgangen av året, flyttes egenkapitalen fra beregnet egenkapital til kontoen for fri egenkapital. Regnskapsåret merkes også som avsluttet, og alle etterfølgende poster for det avsluttede året merkes som etterposter.

Deretter genereres det en avslutningspost, men den bokføres ikke automatisk. Du får muligheten til å lage en eller flere motregningsposter for egenkapitalkontoen , som gjør at du kan fastsette hvordan du tildeler avslutningsposten. Hvis selskapet for eksempel har flere divisjoner, kan du generere en enkelt avslutningspost for alle divisjonene, og deretter kan du lage en motregningspost for egenkapitalkontoen til hver enkelt divisjon.

Du kan bokføre i et tidligere regnskapsår, selv etter at resultatkontoene er avsluttet, hvis du kjører kjørselen Lukk resultatregnskapet på nytt etterpå.

## <a name="see-also"></a>Se også
[Åpne et nytt regnskapsår](finance-setup-how-open-new-fiscal-year.md)

