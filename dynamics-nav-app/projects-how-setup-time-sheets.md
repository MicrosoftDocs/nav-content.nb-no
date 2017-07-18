---
title: Definere timelister
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 6cbacce79ce185d6ed00ea8383259d1b28f9e11b
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-time-sheets"></a>Definere timelister
Timelister i Dynamics NAV håndterer tidsregistrering i ukentlige intervaller på sju dager. Du kan bruke dem til å spore tiden som brukes på prosjekter, og du kan bruke dem til å registrere enkel registrering av ressurstid. Før du kan bruke timelister, må du angi hvordan du vil at de skal settes opp og konfigureres.

Når du har definert hvordan organisasjonen vil bruke timelister, kan du angi om og hvordan timelister er godkjent. Avhengig av behovene i organisasjonen, kan du angi:

- En eller flere brukere som administrator for timeliste og godkjenning for alle timelister.
- En godkjenner av timelister for hver ressurs.

Når du har definert timelister, kan du opprette timelister for ressurser, tilordne dem til planleggingslinjer og bokføre timelistelinjer. Se [Bruke timelister](projects-how-use-time-sheets.md) for mer informasjon.

## <a name="to-set-up-general-information-for-time-sheets"></a>Slik definerer du generell informasjon for timelister  

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Ressursoppsett** og velger deretter den relaterte koblingen.  
2. Fyll ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
3. For feltet **Timeliste etter prosjektgodkjenning** velger du ett av følgende alternativer.

|Alternativ |Beskrivelse|
|---|---|
|**Aldri**|Brukeren i feltet **Bruker-ID for godkjenner av timeliste:** på ressurskortet godkjenner timelisten.|
|**Alltid**|Brukeren i feltet **Ansvarlig person** på prosjektkortet godkjenner timelisten.|
|**Bare maskin**´|Hvis timelisten for maskin er knyttet til et prosjekt, godkjenner brukeren i feltet **Ansvarlig person** på prosjektkortet, timelisten. Hvis timelisten for maskin er knyttet til en ressurs, godkjenner brukeren i feltet **Bruker-ID for godkjenner av timeliste:** på ressurskortet, timelisten.

## <a name="to-assign-a-time-sheet-administrator"></a>Slik tilordner du en timelisteadministrator  

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Brukeroppsett** og velger deretter den relaterte koblingen.  
2.  Legg til en ny bruker hvis brukerlisten ikke inkluderer personen som du vil skal være ansvarlig for timelisteregistrering. Hvis du vil ha mer informasjon, kontakt systemansvarlig.  
3. Velg en bruker som administrator for en timeliste, og merk deretter av for **Administrator for timeliste** .  

**Tips**: Det anbefales at du velger bare én bruker som administrator for timelisten i et selskap. I den følgende fremgangsmåten setter du opp en timelisteeier og -godkjenner, der godkjenneren av timelisten er tilordnet for hver ressurs.  

## <a name="to-assign-a-time-sheets-owner-and-approver"></a>Slik tilordner du en timelisteeier og -godkjenner  

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Ressurser** og velger deretter den relaterte koblingen.
2. Merk ressursen du vil definere muligheten til å bruke timelister for, og merk deretter av for **Bruk timeliste**.  
3. Angi ID-en for eieren av timelisten i feltet **Bruker-ID for eier av timeliste:**. Eieren kan angi tidsbruk på en timeliste og sende den til godkjenning. Når ressursen er en person, er denne personen vanligvis også eieren.  
4. Angi ID-en for godkjenneren av timelisten i feltet **Bruker-ID for godkjenner av timeliste**. Godkjenneren kan godkjenne, avvise eller åpne på nytt en timeliste.  

**Merk**: Du kan ikke endre ID-en for godkjenneren av timelisten hvis det finnes timelister som ennå ikke er behandlet og som har statusen **Sendt** eller **Åpen**.

## <a name="see-also"></a>Se også
[Konfigurere prosjektstyring](projects-setup-projects.md)  
[Administrere prosjekter](projects-manage-projects.md)  
[Finans](finance-setup.md)  
[Håndtere kjøp](purchasing-manage-purchasing.md)         
[Håndtere salg](sales-manage-sales.md)      
[Arbeide med Dynamics NAV](ui-work-product.md)  

