---
title: Endre gjeldende oppsett som skal brukes i en rapport
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
ms.openlocfilehash: f1411704a7b2a0565d4b23d91e04e271af07659e
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-change-which-layout-is-currently-used-on-a-report"></a>Endre gjeldende oppsett som skal brukes i en rapport
En rapport kan defineres med flere rapportoppsett, som du deretter kan bytte mellom etter behov.

Avhengig av oppsettene som er tilgjengelige for en rapport, kan du velge om du vil bruke et innebygd RDLC-rapportoppsett, et innebygd Word-rapportoppsett eller et egendefinert oppsett. Hvis du vil ha mer informasjon om RDLC- og Word-rapportoppsett, innebygde og egendefinerte oppsett og mer, kan du se [Håndtere rapportoppsett](ui-manage-report-layouts.md).

## <a name="to-change-the-layout-that-is-used-on-a-report"></a>Slik endrer du oppsettet som brukes i en rapport
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Rapportoppsettsvalg** og velger deretter den relaterte koblingen.  
Vinduet **Rapportoppsettsvalg** viser alle rapportene som er tilgjengelige for selskapet som er angitt i feltet Selskap øverst i vinduet. Feltet Valgt oppsett angir oppsettet som brukes i rapporten for øyeblikket.
2. Angi selskapet som inkluderer rapporten, i **Selskap**-feltet øverst i vinduet.
3. Hvis du vil endre oppsettet som brukes av en rapport, angir du ett av følgende alternativer for feltet **Valgt oppsett** i raden for rapporten i listen:
    - RDLC (innebygd): Bruker det innebygde RDLC-rapportoppsettet i rapporten.
    - Word (innebygd): Bruker det innebygde Word-rapportoppsettet i rapporten.
    - Egendefinert: Bruker et egendefinert oppsett i rapporten.  
    Du kan se hvilke egendefinerte oppsett som er tilgjengelige for rapporten, i faktaboksen Rapportoppsettsdel. Hvis det ikke finnes noen egendefinerte oppsett for rapporten, må du først opprette et. Hvis du velger dette alternativet, går du til neste fremgangsmåte for å angi det egendefinerte oppsettet du vil bruke.
**Merk**: Hvis du velger **RDLC (innebygd)** eller **Word (innebygd)** og får en feilmelding om at rapporten ikke har et oppsett for den angitte typen, må du velge et annet oppsettalternativ eller opprette et egendefinert rapportoppsett av typen du vil bruke.

Hvis du valgte et innebygd RDLC- eller Word-rapportoppsett, kreves ingen ytterligere handling, og oppsettet brukes neste gang rapporten kjøres.

## <a name="to-specify-a-custom-layout-on-a-report"></a>Angi et egendefinert oppsett i en rapport
1. Du angir hvilket egendefinert oppsett som skal brukes i rapporten, fra vinduet **Egendefinerte rapportoppsett**. Hvis vinduet **Egendefinerte rapportoppsett** ikke er åpent, velger du oppslagsknappen i feltet **Beskrivelse av rapportoppsett**.
2. Merk raden for egendefinert oppsett du vil bruke, i vinduet **Egendefinerte rapportoppsett**, og velg deretter **OK**-knappen.

Du går tilbake vinduet **Egendefinerte rapportoppsett**. Navnet på det valgte egendefinerte oppsettet vises i feltet **Beskrivelse av egendefinert oppsett**. Det egendefinerte oppsettet brukes neste gang du kjører rapporten.

## <a name="see-also"></a>Se også
[Håndtere rapportoppsett](ui-manage-report-layouts.md)

