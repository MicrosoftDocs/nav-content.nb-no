---
title: Administrere prosjektbudsjetter
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
ms.openlocfilehash: c28e23c4ae0082265357a567ea82795b77ac8f1c
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-manage-job-budgets"></a>Administrere prosjektbudsjetter
Du kan opprette et budsjett for hvert prosjekt. Budsjettet brukes til å planlegge ressursene du tildeler til et prosjekt. Budsjettet kan enten være generelt med få poster, eller det kan inneholde mange poster som er oppdelt i aktivitetsnivåer. Deretter kan du sammenligne de budsjetterte beløpene med det faktiske forbruket slik det er registrert i prosjektkladden. Ved å overvåke forskjeller mellom faktisk bruk og budsjettert bruk kan du kontrollere et pågående prosjekt og forbedre kvaliteten på fremtidige prosjekter ved å redusere risikoen for å underestimere kostnader.

Følgende fremgangsmåte beskriver hvordan du kan beregne budsjetterte kostnader under planleggingen. Hvis du vil ha informasjon om registrering av budsjetterte sammenlignet med faktiske prosjektpriser og kostnader, kan du se [Registrere forbruk for prosjekter](projects-how-record-job-usage.md).  

## <a name="JobBudgetCosts"></a> Slik estimerer du budsjetterte kostnader for et prosjekt  
Når en kunde vil vite prisen på et prosjekt som faktureres basert på forbruk, må du fastsette de budsjetterte kostbeløpene for prosjektet. Du bruker vinduet **Prosjektoppgavelinjer** til å gjøre dette.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Prosjekter** og velger deretter den relaterte koblingen.  
2. Åpne et relevant prosjekt.
3. Merk en oppgavelinje for bokføring, og velg deretter handlingen **Prosjektplanleggingslinjer**.
4. Fyll ut feltene etter behov på en ny linje. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.   

Se følgende informasjon for feltet **Linjetype**.  

|Linjetype |Beskrivelse |
|----------|------------|
|**Både Budsjett og Fakturerbar**|Kost- og prisbeløpene som er angitt på planleggingslinjen, er budsjettert kost for den bestemte planleggingslinjen. Prisbeløpet vil bli fakturert.|
|**Budsjett**|Kunden belastes ikke for forbruk. Forbruk overføres ikke til en faktura, men brukes likevel i VIA-beregningen.|
|**Fakturerbar**|Kunden belastes for forbruk. Forbruk overføres til fakturaen basert på antallet som er angitt i feltet Ant. som skal overføres til faktura.|

**Merk**: Feltet **Planleggingsdato** for planleggingslinjen inneholder datoen da forbruk som er knyttet til planleggingslinjen, er forventet å fullføres. Det er også datoen da planleggingslinjen kan overføres til en salgsfaktura og bokføres.  

**Merk**: Når du fyller ut feltet **Antall**, blir all informasjon om totalpris og totalkostnad beregnet og fylt ut for den planleggingslinjen. Du kan redigere dem når som helst.

I vinduet **Prosjektkort** kan du nå se en oversikt over totalt budsjetterte kostnader, budsjettert pris, fakturerbar kostnad og fakturerbar pris for hver oppgave.

Hvis du vil ha informasjon om registrering av budsjetterte sammenlignet med faktiske prosjektpriser og kostnader, kan du se [Registrere forbruk for prosjekter](projects-how-record-job-usage.md).

## <a name="see-also"></a>Se også
[Administrere prosjekter](projects-manage-projects.md)  
[Finans](finance-setup.md)  
[Håndtere kjøp](purchasing-manage-purchasing.md)         
[Håndtere salg](sales-manage-sales.md)      
[Arbeide med Dynamics NAV](ui-work-product.md)  

