---
title: Arbeide med vareattributter
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
ms.openlocfilehash: eaf539f1d4d00c2cd5679f39f29a3428e33ee1fd
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-item-attributes"></a>Arbeide med vareattributter
Når en kunde sender en forespørsel om en vare, enten i korrespondanse eller i en integrert nettbutikk, kan kunden spørre om eller søke etter i henhold til egenskaper, for eksempel høyde og modellår. Hvis du vil levere denne kundeservicen, kan du tilordne varen attributtverdier av forskjellige typer, som deretter kan brukes ved søk etter varer.

Du kan også tilordne vareattributter til varekategorier, som deretter brukes på varene som bruker varekategoriene. Hvis du vil ha mer informasjon, kan du se [Kategorisere varer](inventory-how-categorize-items.md).

## <a name="to-create-item-attributes"></a>Slik oppretter du vareattributter:
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Vareattributter** og velger deretter den relaterte koblingen.
2. I vinduet **Vareattributter** velger du handlingen **Ny**.
3. Fyll ut feltene etter behov i vinduet **Vareattributt**. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.

**Merk**: Hvis du velger **Alternativ** i **Type**-feltet, kan du deretter velge handlingen **Verdier for vareattributt** for å opprette verdier for vareattributtet. Hvis du vil ha mer informasjon, kan du se avsnittet "Slik oppretter du verdier for vareattributter av typen Alternativ".  

## <a name="to-create-values-for-item-attributes-of-type-option"></a>Slik oppretter du verdier for vareattributter av typen Alternativ:
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Vareattributter** og velger deretter den relaterte koblingen.
2. I vinduet **Vareattributter** velger du et vareattributt av typen Alternativ som du vil opprette verdier for, og deretter velger du handlingen **Verdier for vareattributt**.
3. Fyll ut feltene etter behov i vinduet **Verdier for vareattributt**. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.

## <a name="to-assign-item-attributes-to-items"></a>Slik tilordner du vareattributter til varer:
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Varer** og velger deretter den relaterte koblingen.
2. I vinduet **Varer** velger du vareattributtet du vil tilordne vareattributter til, og deretter velger du handlingen **Attributter**.
3. I vinduet **Verdier for vareattributt** velger du handlingen **Ny**.
4. I **Attributt**-feltet velger du AssistEdit-knappen og velger et eksisterende vareattributt. Du kan også velge **Ny**-handlingen for å opprette et nytt vareattributt først, som forklart under "Slik oppretter du vareattributter".
5. I **Verdi**-feltet angir du vareattributtverdien, for eksempel "2010" for attributtet Modellår.
6. For vareattributter av typen Alternativ velger du AssistEdit-knappen i **Verdi**-feltet og velger en verdi for vareattributtet. Du kan også velge **Ny**-handlingen for å opprette en ny vareattributtverdi først, som forklart under "Slik oppretter du verdier for vareattributter av typen Alternativ".
7. Gjenta trinn 4 til 6 for alle vareattributter du vil tilordne varen.

## <a name="to-assign-item-attributes-to-item-categories"></a>Slik tilordner du vareattributter til varekategorier:
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Varekategorier** og velger deretter den relaterte koblingen.
2. I vinduet **Varekategorier** velger du varekategorien du vil tilordne vareattributter til, og deretter velger du handlingen **Rediger**.
3. I **Varekategorikort**-vinduet på **Attributter**-hurtigfanen velger du handlingen **Ny**.
4. I **Attributt**-feltet velger du AssistEdit-knappen og velger et eksisterende vareattributt. Du kan også velge **Ny**-handlingen for å opprette et nytt vareattributt først, som forklart under "Slik oppretter du et vareattributt".
5. I **Standardverdi**-feltet velger du AssistEdit-knappen og velger en verdi for vareattributtet.
6. Gjenta trinn 4 og 5 for alle vareattributter du vil tilordne varekategorien.

**Merk**: Vareattributter for overordnede varekategorier arves til underordnede varekategorier. Dette angis av **Arvet fra**-feltet på **Attributter**-hurtigfanen. Hvis du vil ha mer informasjon, kan du se [Kategorisere varer](inventory-how-categorize-items.md).

## <a name="to-filter-by-item-attributes"></a>Slik filtrerer du etter vareattributter:
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Varer** og velger deretter den relaterte koblingen.
2. I vinduet **Varer** velger du handlingen **Filtrer etter attributter**.
3. I vinduet **Filtrer varer etter attributt** velger du AssistEdit-knappen i **Attributt**-feltet og et vareattributt.
4. I **Verdi**-feltet velger du AssistEdit-knappen og velger en eksisterende attributtverdi å filtrere varer etter.

    **Merk**: Du kan bare velge verdier direkte for vareattributter som har faste verdier, for eksempel farge. For vareattributter med variable verdier, for eksempel bredde, må du angi verdien for vareattributtet ved først å velge en betingelse. Se trinn 5.
5. I **Verdi**-feltet for et variabelt vareattributt velger du AssistEdit-knappen.
6. I **Betingelse**-feltet i vinduet **Angi filterverdi** velger du rullegardinpilen og velger en betingelse.
7. I **Verdi**-feltet angir du en attributtverdi å filtrere varer etter.

    **Eksempel**: Hvis du vil filtrere på varer der materialbeskrivelsen begynner med "blå", fyller du ut feltene som følger: **Attributt**-feltet: Materialbeskrivelse, **Betingelse**-feltet: Begynner med, **Verdi**-felt: blå.
8. Velg **OK**-knappen.   

Varene i vinduet **Varer** er filtrert etter de angitte verdiene for vareattributt.

## <a name="see-also"></a>Se også
[Kategorisere vare](inventory-how-categorize-items.md)    
[Registrere en nye produkter](inventory-how-register-new-products.md)  
[Håndtere lager](inventory-manage-inventory.md)  
[Arbeide med Dynamics NAV](ui-work-product.md)

