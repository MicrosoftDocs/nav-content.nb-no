---
title: "Håndtere rapportoppsett"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 57cd575c1f72841dae162b077d1f676720ee24e7
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---
    
# <a name="manage-report-layouts"></a>Håndtere rapportoppsett
Et rapportoppsett styrer innholdet og formatet for rapporten, blant annet hvilke datafelt i et rapportdatasett som skal vises i rapporten, hvordan de er ordnet, samt tekststil, bilder og mer. Fra Dynamics NAV-klienter kan du endre oppsettet som skal brukes i en rapport, opprette nytt oppsett eller endre eksisterende oppsett. 

Et rapportoppsett brukes især til å konfigurere følgende:

- Etikett- og datafeltene som skal tas med fra datasettet for Dynamics NAV-rapporten.
- Tekstformatet, for eksempel skrifttype, størrelse og farge.
- Selskapets logo og plasseringen.
- Generelle sideinnstillinger, for eksempel marger og bakgrunnsbilder. 

En Dynamics NAV-rapport kan defineres med flere rapportoppsett, som du kan bytte mellom etter behov. Du kan bruke ett av de innebygde rapportoppsettene, eller du kan opprette egendefinerte rapportoppsett og tilordne dem til rapportene etter behov.

Det finnes to typer rapportoppsett som du kan bruke i rapporter: Word og RDLC.

## <a name="word-report-layout-overview"></a>Oversikt over rapportoppsett for Word
Et Word-rapportoppsett er basert på et Word-dokument (DOCX-filtypen). Rapportoppsett for Word lar deg utforme rapportoppsett ved hjelp av Microsoft Word 2013 eller nyere. Et rapportoppsettet for Word bestemmer rapportens innhold – kontrollere hvordan innholdselementer ordnes og hvordan de ser ut. I et Word-rapportoppsettdokument brukes vanligvis tabeller til å ordne innhold, der cellene kan inneholde datafelt, tekst eller bilder.

## <a name="rdlc-layout-overview"></a>Oversikt over RDLC-oppsett
RDLC-oppsett er basert på oppsett for rapportdefinisjon for klient (filtypen RDLC eller RDL). Disse oppsettene er opprettet og endret ved hjelp av SQL Server Report Builder. Konseptet for utforming for RDLC ligner på Word-oppsett, der oppsettet definerer det generelle formatet for rapporten og bestemmer feltene fra datasettet som skal inkluderes. Å utforme RDLC-oppsett er en mer avansert oppgave enn å utforme Word-oppsett.

## <a name="built-in-and-custom-report-layouts"></a>Innebygde og egendefinerte rapportoppsett
Dynamics NAV inneholder flere innebygde oppsett. Innebygde oppsett er forhåndsdefinerte oppsett som er utformet for bestemte rapporter. Dynamics NAV-rapporter har en innebygget utforming som et RDLC-rapportoppsett, Word-rapportoppsett, eller i noen tilfeller begge. Du kan ikke endre innebygde rapportoppsett fra Dynamics NAV, men du bruker dem som et utgangspunkt for å lage egendefinerte rapportoppsett. 

Egendefinerte oppsett er rapportoppsett du utformer for å endre utseendet på en rapport. Vanligvis oppretter du et egendefinert oppsett basert på et innebygd oppsett, men du kan opprette dem fra grunnen av eller fra en kopi av et eksisterende egendefinert oppsett. Egendefinerte oppsett gjør at du kan ha flere oppsett for samme rapport som du kan bytte mellom etter behov. Du kan for eksempel ha ulike oppsett for hvert selskap i Dynamics NAV, eller du kan ha ulike oppsett for samme selskap for bestemte anledninger eller hendelser, for eksempel en kampanje eller julehøytiden.

## <a name="deciding-whether-to-use-a-word-or-rdlc-report-layout"></a>Avgjøre om du skal bruke et Word- eller RDLC-rapportoppsett 
Et rapportoppsett kan være basert på et Word-dokument eller en RDLC-fil. Når du skal velge mellom et Word-rapportoppsett og et RDLC-rapportoppsett, avhenger valget av hvordan du vil at den genererte rapporten skal se ut, og hvor god kjennskap du har til Word og SQL Server Report Builder. 

Generelle utformingskonsepter for Word og RDLC oppsett er svært like. Hver type har imidlertid visse utformingsfunksjoner som påvirker hvordan den genererte rapporten vises i Dynamics NAV. Dette betyr at Word-rapportoppsettet og RDLC-rapportoppsettet kan gi ulike utseender i samme rapport.

Prosessen for å definere Word-rapportoppsett og RDLC-rapportoppsett i rapporter er den samme. Den viktigste forskjellen er måten du endrer oppsett på. Word-rapportoppsettene er vanligvis enklere å opprette og endre enn RDLC-rapportoppsett, fordi du kan bruke Word. RDLC-rapportoppsett endres ved hjelp av SQL Server Report Builder, der målgruppen er mer erfarne brukere.

Hvis du vil ha informasjon om hvordan du endrer hvilket oppsett du vil bruke, kan du se [Endre gjeldende oppsett som skal brukes i en rapport](ui-how-change-layout-currently-used-report.md)

## <a name="see-also"></a>Se også
[Arbeide med Dynamics NAV](ui-work-product.md)  
[Opprette et egendefinert rapportoppsett](ui-how-create-custom-report-layout.md)  
[Sende dokumenter i e-post](ui-how-send-documents-email.md)

