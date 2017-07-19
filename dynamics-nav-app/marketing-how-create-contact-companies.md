---
title: Opprette kontaktselskaper
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: a16e1748472805137d6b9a6d792e93470333f6ff
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---
# <a name="create-contact-companies"></a>Opprette kontaktselskaper
Du kan opprette en kontakt for hvert nytt selskap du utfører en samhandling med, for eksempel kunder, leverandører, prospektive kunder, banker, advokatfirmaer, konsulenter og så videre.

Det er to måter å opprette en kontakt på: fra grunnen av eller fra en eksisterende kunde, leverandør eller bankkonto.

Før du oppretter en kontakt, bør du kontrollere innstillingene i vinduet **Markedsføringsoppsett**. Hvis du vil ha mer informasjon, kan du se [Konfigurere markedsføring og kontaktbehandling](marketing-setup-marketing.md).

## <a name="create-a-company-contact-from-scratch"></a>Opprette en selskapskontakt fra bunnen av
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kontakter** og velger deretter den relaterte koblingen.
2. Velg handlingen **Ny**.
3. Angi et nummer på kontakten i feltet **Nr.**.

  Hvis du har definert en nummerserie for kontakter i vinduet **Markedsføringsoppsett**, kan du eventuelt trykke Enter-tasten for å velge det neste tilgjengelige kontaktnummeret.
4. Sett **Type** til **Selskap**.
5. Fyll ut de andre feltene etter behov:

## <a name="create-a-company-contact-from-a-customer-vendor-or-bank-account"></a>Opprette en selskapskontakt fra en kunde, leverandør eller bankkonto
Hvis du allerede har definert en rekke kunder, leverandører og bankkonti, kan du opprette kontakter på grunnlag av de eksisterende dataene. Når du oppretter en kontakt på denne måten, synkroniseres kontaktinformasjonen med informasjon om kunden, leverandøren eller bankkontoen.

**Merk**: Før du kan opprette kontaktselskaper på denne måten, må du angi en forretningsforbindelseskode for kunder, leverandører og bankkonti, i vinduet **Markedsføringsoppsett**. Hvis du vil opprette kontakter fra en bankkonto, må du også angi nummerserie for bankkonti i vinduet **Finansoppsett**.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir ett av følgende, avhengig av hvor du vil opprette kontakter fra, og velger deretter den relaterte koblingen.
  * **Opprett kontakter fra kunder**
  * **Opprett kontakter fra leverandører**
  * **Opprett kontakter fra bankkonti**
2. Hvis du bare vil opprette kontakter fra bestemte kunder, leverandører eller bankkonti, definerer du filtre i inndelingen **Kunde**, **Leverandør** eller **Bankkonto** i vinduet for kjørselen som åpnes.
3. Velg **OK**-knappen for å starte oppretting av kontrakter.

  De neste kontaktnumrene i nummerserien tilordnes de nye kontaktene. Forretningsforbindelsen for leverandører som er angitt i vinduet **Markedsføringsoppsett**, tilordnes til nyopprettede kontakter.

**Tips**: Du kan også opprette en kunde, leverandør eller bankkonto fra en kontakt. Hvis du vil ha mer informasjon, kan du se [Opprette en kunde, leverandør eller bankkonto fra en kontakt](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).
##<a name="see-also"></a>Se også
[Synkronisere kontakter med kunder, leverandører og bankkonti](marketing-synchronize-contacts-customers-vendors-bank-accounts.md)  
[Tilordne forretningsforbindelser til en kontakt](marketing-business-relations.md#assign-business-relations-to-a-contact)  
[Tilordne bransjegrupper til en kontakt](marketing-industry-groups.md#assign-industry-groups-to-a-contact)  
[Tiordne postgrupper til en kontakt](marketing-mailing-groups.md#assign-mailing-groups-to-a-contact)  
[Opprette kontaktpersoner](marketing-create-contact-persons.md)  

