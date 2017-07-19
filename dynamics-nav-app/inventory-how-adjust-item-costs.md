---
title: Justere varekost
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 59db38c159dd2810656edc668ee431c6414b9d90
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-adjust-item-costs"></a>Justere varekost   
Kostnaden for en vare (lagerverdien) som du kjøper og senere selger, kan endres i løpet av levetiden, for eksempel fordi en fraktkostnader er lagt til innkjøpskostnaden etter at du har solgt varen. Hvis du alltid vil vite riktig lagerverdi, må varekostnader derfor justeres regelmessig.
Dette sikrer at salgs- og fortjenestestatistikk er oppdatert og at økonomiske KPI-er er riktige.

**Merk**: Varekostnader er justert bare av FIFO-lagermetoden. Dette betyr at enhetskosten for en vare er den faktiske verdien for et hvilket som helst mottak av varen, og at lageret er vurdering med antakelsen av at de første elementene som er plassert i lageret, selges først.

Funksjonen for kostnadsjustering behandler bare verdiposter som ennå ikke er justert. Hvis funksjonen støter på en situasjon der endrede inngående kost må videresendes til tilknyttede utgående poster, opprettes det nye justeringsoppføringer, som er basert på informasjonen i de opprinnelige verdipostene, men som inneholder justeringsbeløpet. Funksjonen for kostnadsjustering bruker bokføringsdatoen for den opprinnelige verdiposten i justeringsposten hvis denne datoen ikke er i en lukket lagerperiode. I så tilfelle bruker programmet startdatoen for den neste åpne lagerperioden. Hvis lagerperioder ikke brukes, styrer datoen i feltet **Bokf. tillatt fra** i vinduet **Finansoppsett** når justeringsposten bokføres.

**Merk**: Når varekostnader er justert, må lagerkost bokføres automatisk eller manuelt i finans. Hvis du vil ha mer informasjon, kan du se [Bokføre lagerkost i finans](inventory-how-post-inventory-cost-gl.md).

Du kan justere varekostnader på to måter:
 - Automatisk ved at systemet justerer eventuelle kostendringer hver gang du bokfører lagertransaksjoner.
 - Manuelt ved å kjøre kjørselen **Juster kostverdi - vareposter** for én eller flere varer når du vet at kostnadene er endret.  

## <a name="to-adjust-item-costs-automatically"></a>Justere varekost automatisk
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Lageroppsett** og velger deretter den relaterte koblingen.
2. I vinduet **Lageroppsett** i feltet **Automatisk kostjustering**, velger du én av følgende verdier:

|Alternativ |Virkemåte |
|-------|---------|
|Aldri|Kostnader justeres ikke ved bokføring|
|Dag|Kostnader justeres hvis bokføring skjer innen én dag etter arbeidsdatoen|
|Uke|Kostnader justeres hvis bokføring skjer innen én uke etter arbeidsdatoen|
|Måned|Kostnader justeres hvis bokføring skjer innen én måned etter arbeidsdatoen|
|Kvartal|Kostnader justeres hvis bokføring skjer innen ett kvartal etter arbeidsdatoen|
|År|Kostnader justeres hvis bokføring skjer innen ett år etter arbeidsdatoen|
|Alltid|Kostnader justeres alltid ved bokføring, uansett bokføringsdato|

## <a name="to-adjust-item-costs-manually"></a>Justere varekost manuelt
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Juster kostverdi - vareposter** og velger deretter den relaterte koblingen.
2. I vinduet **Juster kostverdi - vareposter** angir du hvilke varer du vil justere kostnader for og om de justerte kostnadene bokføres til økonomimodulen samtidig.

## <a name="see-also"></a>Se også
[Håndtere lager](inventory-manage-inventory.md)  
[Bokføre lagerkost i finans](inventory-how-post-inventory-cost-gl.md)  
[Håndtere salg](sales-manage-sales.md)  
[Håndtere kjøp](purchasing-manage-purchasing.md)

