---
title: Designdetaljer - Varesporingstilgjengelighet
description: "Vinduene **Varesporingslinjer** og **Varesporingssummering** inneholder dynamisk tilgjengelighetsinformasjon for serie- eller partinumre. Hensikten med dette er å gjøre utgående dokumenter, for eksempel ordrer, klarere for brukere ved å vise dem serienumrene eller antallet partinumre som for øyeblikket er tilordnet i andre åpne dokumenter. Dette reduserer usikkerhet som skyldes doble tildelinger og vekker tillit hos ordrebehandlere om at varesporingsnumrene og datoene de bekrefter på ikke-bokførte ordrer, kan oppfylles."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/26/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 4d106a10ab0f6a6c0e0eb63c6e6641f9ff358e9e
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-item-tracking-availability"></a>Designdetaljer: Varesporingstilgjengelighet
Vinduene **Varesporingslinjer** og **Varesporingssummering** inneholder dynamisk tilgjengelighetsinformasjon for serie- eller partinumre. Hensikten med dette er å gjøre utgående dokumenter, for eksempel ordrer, klarere for brukere ved å vise dem serienumrene eller antallet partinumre som for øyeblikket er tilordnet i andre åpne dokumenter. Dette reduserer usikkerhet som skyldes doble tildelinger og vekker tillit hos ordrebehandlere om at varesporingsnumrene og datoene de bekrefter på ikke-bokførte ordrer, kan oppfylles. Hvis du vil ha mer informasjon, kan du se [Designdetaljer: Vindu for varesporingslinjer](design-details-item-tracking-lines-window.md).  

 Når du åpner vinduet **Varesporingslinjer**, hentes tilgjengelighetsdata fra **Varepost**-tabellen og **Reservasjonspost**-tabellen uten noe datofilter. Når du velger **Serienr.**-feltet eller **Partinr.**-feltet, åpnes vinduet **Varesporingssummering** med et sammendrag av varesporingsinformasjonen i **Reservasjonspost**-tabellen. Sammendraget inneholder følgende informasjon om hvert serie- eller partinummer på varesporingslinjen:  

|Felt|Beskrivelse|  
|---------------------------------|---------------------------------------|  
|**Antall i alt**|Det totale antallet for serie- eller partinummeret som for øyeblikket er på lager.|  
|**Ønsket antall i alt**|Det totale antallet for serie- eller partinummeret som for øyeblikket er forespurt i alle dokumenter.|  
|**Gjeldende antall i kø**|Antallet som registreres i gjeldende forekomst av vinduet **Varesporingslinjer**, men som ikke er lagret i databasen ennå.|  
|**Totalt disp. antall**|Antallet for serie- eller partinummeret som brukeren kan be om.<br /><br /> Dette antallet blir beregnet fra andre felt i vinduet, slik:<br /><br /> totalt antall – (ønsket antall i alt + gjeldende antall i kø).|  

> [!NOTE]  
>  Du kan også vise informasjonen i den foregående tabellen ved å bruke funksjonen **Velg poster** i vinduet **Varesporingslinjer**.  

 For å bevare databaseytelsen hentes tilgjengelighetsdata bare én gang fra databasen når du åpner vinduet **Varesporingslinjer** og når du bruker funksjonen **Oppdater tilgjengelighet** i vinduet.  

## <a name="calculation-formula"></a>Beregningsformel  
 Tilgjengeligheten av et bestemt serie- eller partinummer beregnes på følgende måte, som beskrevet i den forrige tabellen.  

 totalt disponibelt antall = antallet på lager – (alle behov + antallet som ennå ikke er lagret i databasen)  

> [!IMPORTANT]  
>  Denne formelen innebærer at tilgjengelighetsberegningen for serie- eller partinumre bare tar hensyn til beholdning og ignorerer forventede mottak. Levering som ennå ikke er bokført på lager, påvirker derfor ikke varesporingstilgjengelighet, i motsetning til vanlig varedisposisjon der forventede mottak er inkludert.  

## <a name="see-also"></a>Se også  
 [Designdetaljer: Varesporing](design-details-item-tracking.md)

