---
title: "Bruke fordelingsnøkler i finanskladder"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: d239ab62c4be88ccc4a2ce2669dcc2c20a3c0126
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

#  <a name="how-to-use-allocation-keys-in-general-journals"></a>Bruke fordelingsnøkler i finanskladder
Du kan fordele en post i en finanskladd på flere forskjellige konti når du bokfører kladden. Fordelingen kan gjøres etter antall, prosent eller beløp.

## <a name="to-set-up-allocation-keys"></a>Definere fordelingsnøkler 
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Gjentakende finanskladd** og velger deretter den relaterte koblingen.
2. Velg feltet **Bunkenavn** for å åpne vinduet **Finanskladder**.
3. Du kan endre fordelinger på en eksisterende bunke i listen, eller du kan opprette en ny bunke med tildelinger.
  * Hvis du vil opprette en ny bunke, velger du handlingen **Ny** og går til neste trinn.
  * Hvis du vil endre fordelinger for en eksisterende kladd, velger du kladden og går til trinn 7.    
4. I feltet **Navn** skriver du inn et navn på kladden, for eksempel RENGJØRING. I feltet **Beskrivelse** angir du en beskrivelse som for eksempel Kladd for rengjøringsutgifter.
5. Når du er ferdig, lukker du vinduet. En ny, tom gjentakende kladd åpnes. 
6. Fyll ut feltene på linjen.
7. Velg handlingen **Fordelinger**. 
8. Legg til en linje for hver fordeling. Du må fylle ut enten feltet **Andel i pst.**, **Andel i antall** eller **Beløp**. Du må også fylle ut **Kontonummer** -feltet, og hvis du fordeler transaksjonen på globale dimensjoner, må du også fylle ut feltene for globale dimensjoner.
9. Hvis du angir en prosentsats på en linje, beregnes beløpet i feltet **Beløp** automatisk. Disse beløpene har motsatt fortegn av det totale beløpet i feltet **Beløp** i den gjentakende kladden.
10. Når du har angitt fordelingslinjene, velger du **OK** for å gå tilbake til vinduet **Gjentakende finanskladd**. Feltet **Fordelt beløp (USD)** fylles ut og samsvarer med **Beløp**-feltet.
11. Bokfør kladden.

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a>Endre en fordelingsnøkkel som allerede er definert
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Gjentakende finanskladd** og velger deretter den relaterte koblingen.
2. Velg kladden med fordelingen, i vinduet **Finansgjentak.kladd**.
3. Velg linjen med fordelingen, og velg deretter handlingen **Fordelinger**.
4. Endre de relevante feltene, og lukk vinduet.

## <a name="see-also"></a>Se også
[Arbeide med finanskladder](ui-work-general-journals.md)  
[Bokføre dokumenter og kladder](ui-post-documents-journals.md)




