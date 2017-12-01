---
title: Aktivere plukking etter FEFO
description: "FEFO (først utløpt, først ut) er en sorteringsmetode som sikrer at de eldste elementene, det vil si de med de tidligste utløpsdato, plukkes først."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d3977cd235293d685490464e51aec16a95d01e9d
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-enable-picking-items-by-fefo"></a>Aktivere plukking av varer etter FEFO
FEFO (først utløpt, først ut) er en sorteringsmetode som sikrer at de eldste elementene, det vil si de med de tidligste utløpsdato, plukkes først.  

 Denne funksjonaliteten fungerer bare når følgende kriterier er oppfylt:  

-   Varen må ha et serie-/partinummer.  
-   På varens varesporingskodeoppsett må feltet **Lagerporing basert på s.nr.** eller feltet **Lagersporing basert på parti** velges.  
-   Varen må bokføres til lager med en utløpsdato.  
-   Det må merkes av for **Plukk nødv.** på lokasjonskortet.  
-   Det må merkes av for **Plukk i henhold til FEFO** på lokasjonskortet.  
-   Det må merkes av for **Hylle obligatorisk** på lokasjonskortet.  

 Når alle kriteriene er oppfylt, sorteres serie-/partinummererte varer som skal plukkes, med de eldste først i alle plukk og flyttinger, unntatt for varer som bruker SN-spesifikk eller partispesifikk sporing.  

> [!NOTE]  
>  Hvis enkelte serie-/partinummererte varer bruker spesifikk sporing, har disse førsteprioritet, og under disse vises de gjenstående, ikke-spesifikke serie-/partinumrene i henhold til FEFO.  

 Hvis to serie-/partinummererte varer har samme utløpsdato, velges varen med lavest serie- eller partinummer. Hvis serie- eller partinumrene er like, velges varen som ble registrert først.  

> [!NOTE]  
>  -   Når du plukker serie-/partinummererte varer i lokasjoner definert for lagerstyring, blir bare antall i hyller av typen *Plukk* plukket i henhold til FEFO.  
> -   Når du skal aktivere flyttinger i henhold til FEFO, må du la **Fra hylle**-feltet stå tomt i vinduet **Lagerflytting** eller **Flytteforslag**.  
> -   Hvis feltet **Bruk ikke etter utløpsdato** er valgt, inkluderes bare varer som ikke er utløpt, i plukkingen. Dette gjelder selv om du ikke bruker plukk i henhold til FEFO.  

## <a name="see-also"></a>Se også  
[Plukke varer](warehouse-pick-items.md)   
[Plukke varer for lagerlevering](warehouse-how-to-pick-items-for-warehouse-shipment.md)   
[Plukke varer med lagerplukk](warehouse-how-to-pick-items-with-inventory-picks.md)   
[Designdetaljer: Lagerstyring](design-details-warehouse-management.md)  
[Lager](inventory-manage-inventory.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

