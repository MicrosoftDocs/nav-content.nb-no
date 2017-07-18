---
title: Bruke ressurser for prosjekter
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
ms.openlocfilehash: cced4bca42b74c2664fd18770f1616c57286e1c3
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-use-resources-for-jobs"></a>Bruke ressurser for prosjekter
Du registrerer ressursforbruket i prosjektkladden for å holde oversikt over kostnader, priser og arbeidstypene som er knyttet til prosjekter. Hvis du vil ha mer informasjon, kan du se [Registrere forbruk for prosjekter](projects-how-record-job-usage.md).

Du kan også bokføre ressursforbruket i en ressurskladd. Poster som er bokført i en ressurskladd, har ingen innvirkning på Finans.

## <a name="to-assign-resources-to-jobs"></a>Slik tilordner du ressurser til prosjekter
Du kan tilordne ressurser til prosjekter ved å opprette prosjektplanleggingslinjer for prosjektet. Hvis du vil ha mer informasjon, kan du se [Opprette prosjekter](projects-how-create-jobs.md).

## <a name="to-record-resource-usage-for-a-job"></a>Slik registrerer du ressursforbruk for et prosjekt

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Prosjektkladder** og velger deretter den relaterte koblingen.
2. Åpne en relevant prosjektkladd, og fyll deretter ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
3. Når kladden er fullført, kan du velge handlingen **Bokfør**.

## <a name="to-adjust-resource-prices"></a>Slik justerer du ressurspriser  
Hvis du vil endre kost- eller salgspriser for en rekke ressurser, kan du bruke en kjørsel.  

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Juster ressurskost/priser** og velger deretter den relaterte koblingen.
2. Fyll ut feltene på en linje etter behov, og klikk deretter **OK**.

**Merk**: Denne kjørselen verken oppretter eller endrer alternative kostnader eller priser for ressurser. Den endrer bare innholdet i feltet på ressurskortet for **Juster felt**-feltet som du valgte i kjørselen. Justeringen vil tre i kraft umiddelbart for ressurser, så kontroller justeringsfaktorene før du kjører den satsvise jobben.

## <a name="to-get-resource-price-change-suggestions-based-on-existing-alternate-prices"></a>Slik får du forslag til ressursprisendringer på bakgrunn av eksisterende alternative priser  
Hvis du allerede har definert alternative ressurspriser for noen ressurser, kan du bruke en kjørsel til å definere flere alternative ressurspriser.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Ressursprisendringer** og velger deretter den relaterte koblingen.
2. Velg handlingen **Foreslå ress.prisendr. (pris)** og fyll deretter ut feltene etter behov.
3. Velg **OK**-knappen.  
4. Når kjørselen er ferdig, viser vinduet **Ressursprisendringer** resultatene av kjørselen.

## <a name="to-get-resource-price-change-suggestions-based-on-standard-prices"></a>Slik får du forslag til ressursprisendringer på bakgrunn av standardpriser  
Hvis du vil definere flere alternative ressurspriser på bakgrunn av standardprisene på ressurskortene, kan du bruke en kjørsel.  

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Ressursprisendringer** og velger deretter den relaterte koblingen.
2. Velg handlingen **Foreslå ress.prisendr. (ress.)** og fyll deretter ut feltene etter behov.  
3. Velg **OK**-knappen.  
4. Når kjørselen er ferdig, åpner du vinduet **Ressursprisendringer** for å se resultatene av kjørselen.

## <a name="to-get-resource-price-change-suggestions-based-on-alternate-prices"></a>Slik får du forslag til ressursprisendringer på bakgrunn av alternative priser  
Hvis du allerede har definert alternative ressurspriser for noen ressurser, kan du bruke en kjørsel til å definere flere alternative ressurspriser.

1. Skriv inn **Foreslå ress.prisendr. (pris)** i **Søk**-boksen, og velg deretter den relaterte koblingen.  
2. Fyll ut feltene etter behov.
3. Velg **OK**-knappen.  
4. Når kjørselen er ferdig, åpner du vinduet **Ressursprisendringer** for å se resultatene av kjørselen.

## <a name="see-also"></a>Se også
[Administrere prosjekter](projects-manage-projects.md)  
[Finans](finance-setup.md)  
[Håndtere kjøp](purchasing-manage-purchasing.md)         
[Håndtere salg](sales-manage-sales.md)     
[Arbeide med Dynamics NAV](ui-work-product.md)  

