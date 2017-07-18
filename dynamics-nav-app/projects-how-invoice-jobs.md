---
title: Fakturere prosjekter
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
ms.openlocfilehash: c0dcce83dfba30af38f33a6bf814b15862d5fc19
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-invoice-jobs"></a>Fakturere prosjekter
I løpet av prosjektet kan det akkumuleres prosjektkostnader fra ressursforbruk, materiale og prosjektrelaterte kjøp. Under fremdriften til prosjektet blir disse transaksjonene bokført til prosjektkladden. Det er viktig at alle kostnader blir registrert i prosjektkladden før du fakturerer kunden.

Du kan fakturere hele prosjektet fra vinduet **Prosjektoppgavelinjer** eller bare fakturere utvalgte fakturerbare linjer fra vinduet **Planleggingslinjer**. Fakturering kan utføres etter at prosjektet er fullført, eller ved bestemte intervaller under fremdriften til prosjektet, basert på en faktureringsplan.

**Merk**: Hvis du velger **Fakturerbar** i feltet **Prosjektlinjetype** i kjøpsdokumentene for prosjektrelaterte kjøp, opprettes deretter prosjektplanleggingslinjer som er klare til fakturering til kunden. Hvis du vil ha mer informasjon, se [Administrere prosjektforsyninger](projects-how-manage-project-supplies.md).

## <a name="to-create-and-post-a-job-sales-invoice"></a>Slik oppretter og bokfører du en salgsfaktura for prosjekt  
Du kan opprette en faktura for et prosjekt eller for én eller flere prosjektoppgaver for en kunde enten når arbeidet som skal faktureres, er fullført, eller når faktureringsdatoen som er basert på et faktureringsestimat, er nådd.

Fra vinduet **Prosjekter** kan du fakturere en kunde ved å velge prosjektet, og deretter velge handlingen **Opprett salgsfaktura for prosjekt**. Følgende fremgangsmåte viser hvordan du bruker en satsvis jobb til å fakturere flere prosjekter.  

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Opprett salgsfaktura for prosjekt** og velger deretter den relaterte koblingen.  
2. Fyll ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
3. Angi filtre hvis du vil begrense prosjektene som kjørselen skal behandle.
3. Velg **OK**-knappen for å opprette fakturaene.  

## <a name="to-create-multiple-job-sales-invoices-from-job-planning-lines"></a>Slik oppretter du flere prosjektsalgsfakturaer fra prosjektplanleggingslinjer  
Du kan opprette en faktura fra en prosjektplanleggingslinje og samtidig angi antallet for varen, ressursen eller finanskontoen som du vil fakturere.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Prosjekter** og velger deretter den relaterte koblingen.
2. Åpne et relevant prosjekt.
3. Velg en prosjektoppgave der feltet **Prosjektoppgavetype** inneholder **Bokføring**, og velg deretter handlingen **Prosjektplanleggingslinjer**.  
4. På en prosjektplanleggingslinjer, i feltet **Ant. som skal overføres til faktura** angir du antallet av varen, ressursen, finanskontotypen du vil fakturere.  
5. Velg handlingen **Opprett salgsfaktura**.
6. I vinduet **Opprett salgsfaktura for prosjekt** skriver du inn bokføringsdatoen og om du vil opprette en ny faktura eller føye til denne fakturaen til en eksisterende.
7. Velg **OK**-knappen.

    Du kan se antallet i feltet **Ant. overført til faktura** på prosjektplanleggingslinjen.

8. I vinduet **Prosjektplanleggingslinjer** velger du handlingen **Salgsfakturaer/kreditnotaer**.

    Vinduet **Salgsfaktura** åpnes og viser antallet du har overført til fakturaen.  
9. Gjør flere endringer, og velg deretter handlingen **Bokfør**.

**Merk**: Fremgangsmåten ovenfor er identisk for å opprette, gå gjennom og bokføre en prosjektrelatert salgskreditnota.

## <a name="to-calculate-and-post-job-completion-entries"></a>Slik beregner og bokfører du prosjektferdiggjørelsesposter  
Når du har fullført alle aktiviteter for et prosjekt, inkludert bokføring og fakturering, må du oppdatere prosjektet for å sette **Status** til **Ferdig**. Deretter må du reversere alle VIA-er som er bokført i finans.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Prosjekter** og velger deretter den relaterte koblingen.  
2. Merk et åpent prosjekt, og velg handlingen **Rediger**.
3. I feltet **Status** velger du **Fullført**.
4. Følg hjelpetrinnene for å beregne og bokføre VIA. Alternativt følger du trinn 5 og 6 hvis du vil gjøre dette manuelt.  
5. Velg handlingen **Beregn VIA**.
6. I vinduet **Beregn VIA for prosjekt** fyller du ut feltene etter behov.  

     VIA-postene for prosjekt du oppretter ved å kjøre kjørselen, vil ha en avmerking i **Prosjekt ferdig**-boksen for å angi at de er ferdiggjørelsesposter.  

7. Velg handlingen **Bokfør VIA i Finans for prosjekt**.
8. Fyll ut feltene etter behov i vinduet **Bokfør VIA i Finans for prosjekt**.  

     VIA-finanspostene for prosjekt som du oppretter ved å kjøre kjørselen, vil ha en avmerking i **Prosjekt ferdig**-boksen for å angi at de er ferdiggjørelsesposter.

## <a name="see-also"></a>Se også
[Administrere prosjekter](projects-manage-projects.md)  
[Finans](finance-setup.md)  
[Håndtere kjøp](purchasing-manage-purchasing.md)         
[Håndtere salg](sales-manage-sales.md)      
[Arbeide med Dynamics NAV](ui-work-product.md)  

