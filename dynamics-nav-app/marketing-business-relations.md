---
title: Definere forretningsforbindelser for kontaktselskaper
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 20abe2f08fc726a008719f94389579d02ecbd275
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---
# <a name="set-up-business-relations-on-contact-companies"></a>Definere forretningsforbindelser for kontaktselskaper
Du kan bruke forretningsforbindelser blir brukt til å angi hvilket forretningsforhold du har til kontaktene, for eksempel prospekter, banker, konsulenter, serviceleverandører og så videre.

Bruk av forretningsforbindelser på kontakter er en totrinnsprosess. Først må definere du koden for forretningsforbindelsen. Du trenger bare utføre dette trinnet én gang for hver forretningsforbindelse. Når du har en kode for forretningsforbindelse, kan du begynne å tilordne koden til kontaktselskaper.

**Merk**: Hvis du vil synkronisere kontaktene med leverandører, kunder eller bankkonti i andre deler av applikasjonen, bør du definere en forretningsforbindelse for disse.

## <a name="define-a-business-relation-code"></a>Definere en kode for forretningsforbindelse
Koden for forretningsforbindelsen definerer en kategori eller type for forretningsforbindelsen, for eksempel BANK eller JURIDISK. Du kan ha flere forretningsforbindelseskoder. Hvis du vil definere forretningsforbindelsen, bruker du vinduet **Forretningsforbindelser**.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Forretningsforbindelser** og velger deretter den relaterte koblingen.
2. Velg handlingen **Ny**, og fyll ut en kode og en beskrivelse. Koden kan bestå av opptil 11 tegn, og kan inneholde en kombinasjon av tall og bokstaver.

## <a name="assign-business-relations-to-a-contact"></a>Tilordne forretningsforbindelser til en kontakt
Du kan ikke tilordne forretningsforbindelser til en kontaktperson, bare selskaper.

1. Åpne kontakten.
2. Velg handlingen **Selskap**, og deretter handlingen **Forretningsforbindelser**.

    Vinduet **Kontaktens forretn.forbind.** åpnes.
3. Velg forretningsforbindelsen du vil tilordne, i feltet **Forretn.forbindelseskode**.

Gjenta disse trinnene hvis du vil tilordne flere forretningsforbindelser. Du kan også tilordne forretningsforbindelser fra kontaktlisten ved å følge samme fremgangsmåte.

Antall forretningsforbindelser du har tilordnet kontakten, vises i feltet **Ant. forretningsforbindelser** i inndelingen **Segmentering** i vinduet **Kontakt**.

Når du har tilordnet forretningsforbindelser til kontaktene, kan du bruke disse opplysningene til å velge kontakter for segmentene. Hvis du vil ha mer informasjon, kan du se [Legge til kontakter i segmenter](marketing-add-contact-segment.md).

##<a name="see-also"></a>Se også
[Opprette kontaktselskaper](marketing-create-contact-companies.md)

