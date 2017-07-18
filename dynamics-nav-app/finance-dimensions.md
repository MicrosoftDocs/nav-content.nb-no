---
title: Dimensjoner
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: a1b38e74717e87bea6efb46f8f4e5236b6ec4e64
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

#<a name="dimensions"></a>Dimensjoner
Dimensjoner er data du legger til i poster for å kategorisere dem for analyse. Du kan for eksempel ha dimensjoner som angir hvilket prosjekt eller hvilken avdeling en post kommer fra.
Deretter kan du bruke dimensjoner i stedet for å definere separate finanskonti for hver avdeling og hvert prosjekt. Dette gjør at du kan ha omfattende analyseinformasjon i dataene uten å måtte bruke en komplisert kontoplan.
Du kan definere et ubegrenset antall dimensjoner med et ubegrenset antall dimensjonsverdier.  

Du kan for eksempel definere en dimensjon som kalles *Avdeling*, og du bruker denne dimensjonen og dimensjonsverdien når du bokfører salgsdokumenter. Deretter kan du for eksempel senere få forretningsintelligensdata om hvilke varer er solgt av hvilke avdelinger.
Jo flere dimensjoner du definerer og bruker, jo mer detaljerte rapporter kan du basere dine forretningsavgjørelser på. En enkelt salgspost kan for eksempel inneholde flerdimensjonsinformasjon om hvilken konto varesalget er bokført på, hvor varen ble solgt, hvem som solgte den, og hva slags kunde som kjøpte den.  

## <a name="using-dimensions"></a>Bruke dimensjoner
I et dokument, for eksempel en ordre, kan du legge til dimensjonsinformasjon om én enkelt dokumentlinje og selve dokumentet. I vinduet **Ordre** kan du for eksempel angi dimensjonsverdier for de to første snarveisdimensjonene direkte i dokumenthodet, og du kan legge til mer dimensjonsinformasjon hvis du velger knappen **Dimensjoner**.  
Hvis du i stedet arbeider i en kladd, kan du også legge til dimensjonsinformasjon i en post på samme måte, forutsatt at du har opprettet snarveisdimensjoner som felt direkte i kladdelinjer.  
Du kan definere standarddimensjoner for konti eller kontotyper, slik at dimensjoner og dimensjonsverdier fylles ut automatisk.  

## <a name="dimension-sets"></a>Dimensjonssett
Et dimensjonssett er en unik kombinasjon av dimensjonsverdier. Det lagres som dimensjonssettposter i databasen. Hver dimensjonssettpost representerer én enkelt dimensjonsverdi. Dimensjonssettet identifiseres av en felles dimensjonssett-ID som tilordnes hver dimensjonssettpost som tilhører dimensjonssettet.  

Når du oppretter en ny kladdelinje, et nytt dokumenthode eller en ny dokumentlinje, kan du angi en kombinasjon av dimensjonsverdier. I stedet for at hver dimensjonsverdi lagres eksplisitt i databasen, tilordnes en dimensjonssett-ID til kladdelinjen, dokumenthodet eller dokumentlinjen for å angi dimensjonssettet.  

## <a name="see-also"></a>Se også
[Finans](finance-setup.md)  
[Definere dimensjoner](finance-setup-setup-dimensions.md)  

