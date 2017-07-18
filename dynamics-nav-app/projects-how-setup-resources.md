---
title: Definere ressurser
author: SorenGP
ms.custom: na
ms.date: 12/14/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 72f5304e6a69a736c9df2cbb9ca64c5f3c5261a2
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-resources"></a>Definere ressurser
For å behandle ressursaktiviteter på riktig måte må du definere ressursene og de relaterte kostnadene og prisene. De prosjektrelaterte prisene, rabattene og kostfaktorreglene er definert på prosjektkortet. Du kan angi kostnadene og prisene for individuelle ressurser, ressursgrupper eller alle tilgjengelige ressurser for firmaet.

Når ressurser brukes eller selges i et prosjekt, hentes de tilknyttede prisene og kostnadene fra informasjonen du definerer.

Du angir standardbeløpet per time når ressursen opprettes. Hvis du for eksempel bruker en bestemt maskin i fem timer på et prosjekt, beregnes prosjektet basert på beløpet per time.

## <a name="to-set-up-a-resource"></a>Slik konfigurerer du en ressurs
Opprette et kort for hver ressurs du vil bruke i prosjekter.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Ressurser** og velger deretter den relaterte koblingen.
2. Velg handlingen **Ny**.
3. Fyll ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.  

## <a name="to-set-up-a-resource-group"></a>Slik definerer du en ressursgruppe
Du kan kombinere flere ressurser i én ressursgruppe. Alle kapasiteter og budsjetter for ressursgrupper akkumuleres fra de enkelte ressursene. Det er også mulig å angi kapasiteter for ressursgrupper, enten uavhengig av akkumulerte verdier eller i tillegg til disse.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Ressursgrupper** og velger deretter den relaterte koblingen.
2. Velg handlingen **Ny**.
3. Fyll ut feltene etter behov.

## <a name="to-set-capacity-for-a-resource"></a>Angi kapasiteten til en ressurs 
Hvis du vil beregne hvor mye tid en ressurs kan bruke på prosjekter, må deres kapasitet først defineres som tilgjengelig tid per periode i arbeidskalenderen. Dette oppsettet brukes når du fyller ut prosjetplanleggingslinjer som inneholder ressursen. Hvis du vil ha mer informasjon, kan du se [Opprette prosjekter](projects-how-create-jobs.md).

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Ressurser** og velger deretter den relaterte koblingen.
2. Åpne det aktuelle ressurskortet, og velg deretter handlingen **Ressurskapasitet**.
3. I vinduet **Ressurskapasitet** i **Vis etter**-feltet, angir du lengden på perioden, for eksempel **Dag**, som vises i kolonner i hurtigfanen **Matrise for ressurskapasitet**.
4. For hver ressurs på en linje angir du for hver periode i kolonnene antall timer som ressursen er tilgjengelig.
5. Hvis du vil angi detaljer om ressursens ukentlige kapasitet innenfor en start- og sluttdato, kan du også velge handlingen **Angi kapasitet**.
6. I vinduet **Innstillinger for ressurskapasitet** fyller du ut feltene på en linje etter behov.
7. Velg handlingen **Oppdater kapasitet**. Vinduet **Ressurskapasitet** oppdateres med den angitte kapasiteten.
8. Lukk vinduet.

## <a name="to-set-up-alternate-resource-costs"></a>Slik definerer du alternative ressurskostpriser
I tillegg til kostprisen som er angitt på ressurskortet, kan du definere alternative kostpriser for hver ressurs. Hvis du for eksempel betaler ansatte en høyere timesats for overtid, kan du definere en ressurskostpris for overtidssatsen. Den alternative kostprisen du definerer for ressursen, overstyrer kostprisen på ressurskortet når du bruker ressursen i ressurskladden.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Ressurser** og velger deretter den relaterte koblingen.  
2. Velg ressursen som du vil definere ett eller flere alternative kostpriser for, og velg deretter handlingen **Kostpriser**.  
3. I vinduet **Ressurskostpriser** fyller du ut feltene på en linje etter behov.  
4. Gjenta trinn 3 for hvert alternativ ressurskostpris du vil definere.

**Merk**. Hvis du vil definere ressurskostpriser som skal gjelde for alle ressurser og ressursgrupper, åpner du vinduet **Ressurskostpriser** og fyller ut feltene.

## <a name="to-set-up-alternate-resource-prices"></a>Slik definerer du alternative ressurspriser  
I tillegg til prisen som er angitt på ressurskortet, kan du definere alternative priser for hver ressurs. Disse alternative prisene kan være betinget. De kan være avhengig av at ressursen brukes med et bestemt prosjekt eller arbeidstype.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Ressurser** og velger deretter den relaterte koblingen.
2. Velg ressursen som du vil definere ett eller flere alternative priser for, og velg deretter handlingen **Priser**.
3. I vinduet **Ressurspriser** fyller du ut feltene på en linje etter behov.
4. Gjenta trinn 3 for hvert alternativ ressurspris du vil definere.

## <a name="see-also"></a>Se også
[Konfigurere prosjektstyring](projects-setup-projects.md)  
[Administrere prosjekter](projects-manage-projects.md)  
[Finans](finance-setup.md)  
[Håndtere kjøp](purchasing-manage-purchasing.md)         
[Håndtere salg](sales-manage-sales.md)      
[Arbeide med Dynamics NAV](ui-work-product.md)  

