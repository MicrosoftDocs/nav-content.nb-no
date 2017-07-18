---
title: Definere aktivaforsikring
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 44bb5f20702a01d9fbbc025889ec2bc3191813be
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-fixed-asset-insurance"></a>Definere aktivaforsikring
Hvis du vil behandle forsikringsdekning for aktiva, må du først sette opp noen generelle forsikringsopplysninger og et forsikringskort per polise.

## <a name="to-set-up-general-insurance-information"></a>Slik definerer du generelle forsikringsopplysninger  
Hvis du vil bruke forsikringsfunksjoner i Dynamics NAV, må du angi noen generelle forsikringsopplysninger.  
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktivaoppsett** og velger deretter den relaterte koblingen.  
2. Fyll ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.  

## <a name="to-set-up-insurance-types"></a>Slik definerer du forsikringstyper  
Du kan gruppere forsikringspoliser i kategorier, for eksempel tyveriforsikring og brannforsikring. Forsikringstypene brukes på forsikringskortet.
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Forsikringstyper** og velger deretter den relaterte koblingen.  
2. Fyll ut feltene etter behov.

## <a name="to-set-up-insurance-cards"></a>Slik definerer du forsikringskort  
Du kan samle opplysninger om hver enkelt forsikringspolise på forsikringskortet.  
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Forsikring** og velger deretter den relaterte koblingen.  
2. Velg **Ny** for å opprette et nytt forsikringskort i **Forsikring**-vinduet.  
3. Fyll ut feltene etter behov.

## <a name="to-set-up-insurance-journal-templates"></a>Slik definerer du forsikringskladdemaler  
Dynamics NAV oppretter automatisk en forsikringskladdemal første gang du åpner **Forsikringskladd**-vinduet, men du kan definere flere kladdemaler. Hvis du vil ha mer informasjon, kan du se [Arbeide med finanskladder](ui-work-general-journals.md).  
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Forsikringskladdemaler** og velger deretter den relaterte koblingen.  
2. Fyll ut feltene etter behov.

## <a name="to-set-up-insurance-journal-batches"></a>Slik definerer du forsikringskladder  
Du kan definere kladder i en forsikringskladdemal. Verdiene i kladden brukes som standardverdier hvis ikke feltene på kladdelinjene er fylt ut. Hvis du vil ha mer informasjon, kan du se [Arbeide med finanskladder](ui-work-general-journals.md)  
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Forsikringskladdemaler** og velger deretter den relaterte koblingen.  
2. Velg en forsikringskladdemal, og velg deretter **Kladder**-handlingen.
3. I vinduet **Forsikringskladder** fyller du ut feltene etter behov.

**Merk**: Tall har en bestemt funksjon i kladdenavn. Hvis en kladdemal eller et kladdenavn inneholder et tall, øker tallet automatisk med én hver gang du bokfører en kladd. Hvis for eksempel HH1 er angitt i feltet **Navn**, endres kladdenavnet til HH2 etter at kladden HH1 er bokført.

## <a name="see-also"></a>Se også
[Definere aktiva](fa-setup.md)  
[Administrere aktiva](fa-manage.md)  
[Finans](finance-setup.md)  
[Velkommen til Dynamics NAV](across-get-started.md)

