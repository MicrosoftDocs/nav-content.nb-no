---
title: "Angi fargede indikatorer for å tilpasse visuelle signaler om aktiviteten for et bunke-ikon"
description: "Definere en farget indikator på en bunkeflis for å gi et tilpasset visuelt signal for aktiviteten for bunke-ikonet."
documentationcenter: 
author: SusanneWindfeldPedersen
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: personalize, customize
ms.date: 03/29/2017
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 6a2b7deb2f256e3b6bf52f1b0a66fe47d049c452
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-a-colored-indicator-on-cues"></a>Definere en farget indikator for bunke-ikoner
Du kan definere bunke-ikoner som vises på **Hjem**-siden med en indikator som endrer farge basert på dataverdiene i bunke-ikonene.

Indikatoren vises som en farget linje langs øverste kant av bunkeflisen. Den gir et visuelt signal om statusen for aktiviteten for bunke-ikonet, som kan angi fordelaktige eller ufordelaktige tilstander som ber brukeren om å gjøre noe. Hvis det for eksempel vises pågående salgsfakturaer på et bunke-ikon, kan du angi at indikatoren skal være grønn (fordelaktig) når antall pågående salgsfakturaer er under 10, og at den skal være rød (ufordelaktig) når det totale antallet er over 20.

Du bruker vinduet **Oppsett for bunke-ikon** til å definere indikatorer for alle bunke-ikonene som er tilgjengelige i selskapsdatabasen.

Hvis du vil definere indikatoren, kan du angi opptil to terskelverdier som definerer tre områder med dataverdier (lav, middels og høy) som du kan bruke en annen farge (eller stil) med.

## <a name="to-set-up-colored-indicators-on-cues"></a>Slik definerer du fargede indikatorer for bunke-ikoner
1. Under **Aktiviteter** på **Hjem**-siden, velger du **Definer bunke-ikoner**.  
   Vinduet **Oppsett for bunke-ikon** vises. Vinduet viser indikatorer som er definert for bunke-ikoner.
2. Hvis du vil endre en indikator, redigerer du feltene og endrer for eksempel verdier for forskjellige terskler.  

Tabellen nedenfor viser fargene som tilsvarer alternativene i feltene **Stil for nedre område**, **Stil for midterste område** og **Stil for øvre område**.

| Alternativ | Farge |
| --- | --- |
| **Ingen** |Ingen farge (samme farge som bunken)|
| **Fordelaktig** |Grønn |
| **Ufordelaktig** |Rød |
| **Tvetydig** |Gul |
| **Underordnet** |Grå |

## <a name="see-also"></a>Se også
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

