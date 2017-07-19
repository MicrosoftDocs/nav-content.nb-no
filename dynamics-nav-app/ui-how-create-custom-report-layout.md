---
title: Opprette et egendefinert rapportoppsett
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
ms.openlocfilehash: 90136439e09deb00a9aed9344fc5f89812caef3a
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-create-a-custom-report-layout"></a>Opprette et egendefinert rapportoppsett
En rapport har som standard et innebygd rapportoppsett, som kan være et RDLC-rapportoppsett, et innebygd Word-rapportoppsett eller i noen tilfeller begge typer. Du kan ikke endre innebygde oppsett. Du kan imidlertid opprette egendefinerte oppsett der du kan endre utseendet på rapporten når den vises, skrives ut eller lagres. Du kan opprette flere egendefinerte rapportoppsett for samme rapport og deretter bytte oppsettet som brukes av en rapport, etter behov.

Hvis du vil opprette et egendefinert oppsett, kan du lage en kopi av et eksisterende egendefinert oppsett eller legge til et nytt egendefinert oppsett, som i de fleste tilfeller er basert på et innebygd oppsett. Når du legger til et nytt egendefinert oppsett, kan du legge til en RDLC-rapportoppsettype, en Word-rapportoppsettype eller begge typer. Det nye egendefinerte oppsettet baseres automatisk på det innebygde oppsettet for rapporten hvis det er tilgjengelig. Hvis det ikke finnes noen innebygde oppsett for typen, opprettes et nytt, tomt oppsett, som du må endre og utforme fra grunnen av. Hvis du vil ha mer informasjon om RDLC- og Word-rapportoppsett, innebygde og egendefinerte oppsett og mer, kan du se [Håndtere rapportoppsett](ui-manage-report-layouts.md).  

## <a name="to-create-a-custom-layout"></a>Slik oppretter du et egendefinert oppsett
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Rapportoppsettsvalg** og velger deretter den relaterte koblingen.  
Vinduet **Rapportoppsettsvalg** viser alle rapportene som er tilgjengelige i selskapet som er angitt i feltet Selskap øverst i vinduet.
2. Angi selskapet du vil opprette rapportoppsettet i, i **Selskap**-feltet.
3. Velg raden for rapporten du vil bruke opprette oppsettet for, og velg deretter **Egendefinerte oppsett**.  
Vinduet **Egendefinerte rapportoppsett** vises og inneholder en oversikt over alle de egendefinerte oppsettene som er tilgjengelige for den valgte rapporten.
4. Hvis du vil opprette en kopi av et eksisterende egendefinert oppsett, velger du det eksisterende egendefinerte oppsettet fra listen, og deretter velger du **Kopier**.  
Kopien av det egendefinerte oppsettet vises i vinduet **Egendefinerte rapportoppsett** og inneholder ordene Kopi av i Beskrivelse-feltet.
5. Hvis du vil legge til et nytt egendefinert oppsett som er basert på et innebygd oppsett, gjør du følgende:  
    1. Velg **Ny**. Vinduet **Sett inn innebygd oppsett for en rapport** vises. Feltene **ID** og **Navn** fylles ut automatisk.
    2. Hvis du vil legge til en egendefinert Word-rapportoppsettype, merker du av for **Sett inn Word-oppsett**.
    3. Hvis du vil legge til en egendefinert RDLC-rapportoppsettype, merker du av for **Sett inn RDLC-oppsett**.
    4. Velg **OK**-knappen.  
    De nye egendefinerte oppsettene vises i vinduet **Egendefinerte rapportoppsett**. Hvis et nytt oppsett er basert på et innebygd oppsett, står det **Kopi av innebygd oppsett** i **Beskrivelse**-feltet. Hvis det ikke finnes noe innebygd oppsett for rapporten, står det **Nytt oppsett** i **Beskrivelse**-feltet, som angir at det egendefinerte oppsettet er tomt.
6. **Selskapsnavn**-feltet er som standard tomt, noe som betyr at det egendefinerte oppsettet er tilgjengelig for rapporten i alle selskaper. Hvis du vil gjøre det egendefinerte oppsettet bare tilgjengelig i et bestemt selskap, velger du **Rediger**, og deretter angir ønsket selskap i **Selskapsnavn**-feltet.

## <a name="see-also"></a>Se også
[Håndtere rapportoppsett](ui-manage-report-layouts.md)  
[Endre gjeldende oppsett som skal brukes i en rapport](ui-how-change-layout-currently-used-report.md)

