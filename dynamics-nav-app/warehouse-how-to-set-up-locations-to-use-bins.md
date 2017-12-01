---
title: Definere lokasjoner slik at de bruker hyller
description: "Hyller representerer den enkle lagerstrukturen og brukes til å komme med forslag om plasseringen av varer. Når du har opprettet hyllene, kan du definere det innholdet du vil plassere i hver hylle, svært spesifikt, eller hyllen kan fungere som en mobil hylle uten angitt innhold."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 95b36b6eed79da868c1e41905110788c90f24829
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-locations-to-use-bins"></a>Definere lokasjoner slik at de bruker hyller
Hyller representerer den enkle lagerstrukturen og brukes til å komme med forslag om plasseringen av varer. Når du har opprettet hyllene, kan du definere det innholdet du vil plassere i hver hylle, svært spesifikt, eller hyllen kan fungere som en mobil hylle uten angitt innhold.  

Når du skal bruke hyllen funksjonelt på en lokasjon, må du først aktivere funksjonaliteten på **Lokasjon**-kortet. Du utformer deretter vareflyten på lokasjonen ved å angi hyllekoder i oppsettsfeltene som representerer ulike flyter.  

> [!NOTE]  
>  Før du kan angi hyllekoder på lokasjonskortet, må hyllekodene være opprettet. Hvis du vil ha mer informasjon, kan du se [Opprette hyller](warehouse-how-to-create-individual-bins.md).  

## <a name="to-set-up-a-location-to-use-bins"></a>Sette opp en lokasjon til å bruke hyller  
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Lokasjoner**, og velg deretter den relaterte koblingen.  
2.  Velg lokajonen der du vil bruke hyller.  
3.  Velg handlingen **Rediger**.  
4.  På hurtigfanen **Lager** merker du av for **Hylle obligatorisk**.  
5.  Hvis du ikke bruker lagerstyring for lokasjonen, fyller du ut feltet **Standard hyllevalg** med metoden systemet skal bruke til å tilordne en standardhylle til en vare.  
6.  Åpne kortet for lokasjonen du vil konfigurere hyller for.
7.  På hurtigfanen **Hyller** velger du de hyllene du vil bruke som standard for mottak og leveringer og inngående, utgående og åpne produksjonshyller.  
8.  De hyllekodene du angir her, vil bli vist automatisk i hodene og på linjene i ulike lagerdokumenter. Standardhyllene definerer alle start- og sluttplasseringer for varene i lageret.  
9.  Hvis du bruker lagerstyring, velger du en hylle til lagerjusteringer. Hyllekoden i feltet **Hyllekode for justering** definerer den virtuelle hyllen som skal registrere avvik i beholdning når du registrerer enten observerte forskjeller som er registrert i lagerets varekladd, eller forskjeller som beregnes når du registrerer en lageropptelling.  
10. Fyll ut feltene i hurtigfane **Hylleprinsipp** hvis de er relevante for lageret. De viktigste feltene er **Hyllekapasitetsprinsipp**, **Tillat anbrekk** og **Plasseringsmal - kode**.  
11. På hurtigfanen **Lager** fyller du ut feltene **Utgående lagerhåndteringstid**, **Inngående lagerhåndteringstid** og **Hovedkalenderkode**. Se [Definere hovedkalendere](across-how-to-assign-base-calendars.md) for mer informasjon.

## <a name="filling-the-consumption-bin"></a>Fylle forbrukshyllen
Dette flytdiagrammet viser hvordan **Hyllekode**-feltet på produksjonsordrekomponentlinjer fylles ut i henhold til lokasjonsoppsettet.

![Flytskjema for hylle](media/binflow.png "BinFlow")  

## <a name="see-also"></a>Se også
[Lagerstyring](warehouse-manage-warehouse.md)  
[Lager](inventory-manage-inventory.md)  
[Definere lagerstyring](warehouse-setup-warehouse.md)     
[Monteringsstyring](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyring](design-details-warehouse-management.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

