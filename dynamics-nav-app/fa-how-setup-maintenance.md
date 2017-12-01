---
title: Definere aktivavedlikehold
description: "For å administrere aktivareparasjoner og -service angir du generelle vedlikeholdsopplysninger, koder for typen arbeid og en bokføringskonto for kost."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: repair, service
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: cb437985793e7fa4330d5bd8301d2808b5deafcc
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-fixed-asset-maintenance"></a>Definere vedlikehold av aktiva
For å styre vedlikehold av aktiva, må du først definere noen generelle vedlikeholdsopplysninger, en bokføringskonto for vedlikeholdskostnader og vedlikeholdskoder for typer arbeid, for eksempel rutineservice eller reparasjon.

## <a name="to-set-up-general-maintenance-information"></a>Slik definerer du generelle vedlikeholdsopplysninger:
Hvis du definerer vedlikeholdsfeltene, kan du bokføre vedlikeholdsutgifter fra aktivakladden.

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Aktiva**, og velg deretter den relaterte koblingen.
2. Velg aktivaet du vil definere forsikringsdekning for, og velg deretter handlingen **Rediger**.
3. Fyll ut feltene på hurtigfanen **Vedlikehold** etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-maintenance-codes"></a>Slik definerer du vedlikeholdskoder
Når du bokfører vedlikeholdskostnader fra en finanskladd, fyller du ut feltet **Vedlikeholdskode** for å registrere hva slags vedlikehold som er utført, for eksempel rutineservice eller reparasjon.

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Vedlikehold**, og velg deretter den relaterte koblingen.
2. I **Vedlikehold**-vinduet definerer du koder for ulike typer vedlikeholdsarbeid.

## <a name="to-set-up-maintenance-expense-accounts"></a>Slik definerer du utgiftskonti for vedlikehold
Du må først angi et kontonummer i vinduet **Bokf.grupper - aktiva** for å kunne bokføre vedlikeholdskostnader.

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bokføringsgrupper - aktiva**, og velg deretter den relaterte koblingen.
2. Fyll ut feltet **Konto for vedlikeholdsutgifter** for hver enkelt bokføringsgruppe.

> [!NOTE]  
>   Hvis du vil at vedlikeholdskostnader skal fordeles på avdelinger eller prosjekter, må du definere en fordelingsnøkkel. Se [Definere generelle aktivafunksjoner](fa-how-setup-general.md) for mer informasjon.

## <a name="see-also"></a>Se også
[Definere aktiva](fa-setup.md)  
[Aktiva](fa-manage.md)  
[Finans](finance.md)  
[Velkommen til [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

