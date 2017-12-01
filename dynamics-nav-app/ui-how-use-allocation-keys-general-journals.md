---
title: "Bruke fordelingsnøkler i finanskladder "
description: "Lær hvordan du kan bruke fordelingsnøkler i kladder."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cost accounting
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3d3944d5f7e9bfe5390fd63b2ae1d05f62efab49
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-use-allocation-keys-in-general-journals"></a>Bruke fordelingsnøkler i finanskladder
Du kan fordele en post i en finanskladd på flere forskjellige konti når du bokfører kladden. Fordelingen kan gjøres etter antall, prosent eller beløp.

## <a name="to-set-up-allocation-keys"></a>Definere fordelingsnøkler
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Gjentakende finanskladd**, og velg deretter den relaterte koblingen.
2. Velg feltet **Bunkenavn** for å åpne vinduet **Finanskladder**.
3. Du kan endre fordelinger på en eksisterende bunke i listen, eller du kan opprette en ny bunke med tildelinger.
   * Hvis du vil opprette en ny bunke, velger du handlingen **Ny** og går til neste trinn.
   * Hvis du vil endre fordelinger for en eksisterende kladd, velger du kladden og går til trinn 7.    
4. I feltet **Navn** skriver du inn et navn på kladden, for eksempel RENGJØRING. I feltet **Beskrivelse** angir du en beskrivelse som for eksempel Kladd for rengjøringsutgifter.
5. Når du er ferdig, lukker du vinduet. En ny, tom gjentakende kladd åpnes.
6. Fyll ut feltene på linjen.
7. Velg handlingen **Fordelinger**.
8. Legg til en linje for hver fordeling. Du må fylle ut enten feltet **Andel i pst.**, **Andel i antall** eller **Beløp**. Du må også fylle ut feltet **Kontonr.** og, hvis du fordeler transaksjonen på globale dimensjoner, feltene for globale dimensjoner.
9. Hvis du angir en prosentsats på en linje, beregnes beløpet i feltet **Beløp** automatisk. Disse beløpene har motsatt fortegn av det totale beløpet i feltet **Beløp** i den gjentakende kladden.
10. Når du har angitt fordelingslinjene, velger du **OK** for å gå tilbake til vinduet **Gjentakende finanskladd**. Feltet **Fordelt beløp (USD)** fylles ut og samsvarer med **Beløp**-feltet.
11. Bokfør kladden.

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a>Endre en fordelingsnøkkel som allerede er definert
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Gjentakende finanskladd**, og velg deretter den relaterte koblingen.
2. Velg kladden med fordelingen, i vinduet **Finansgjentak.kladd**.
3. Velg linjen med fordelingen, og velg deretter handlingen **Fordelinger**.
4. Endre de relevante feltene, og velg deretter **OK**.

## <a name="see-also"></a>Se også
[Arbeide med finanskladder](ui-work-general-journals.md)  
[Bokføre dokumenter og kladder](ui-post-documents-journals.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

