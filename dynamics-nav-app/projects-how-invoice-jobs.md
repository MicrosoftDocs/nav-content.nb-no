---
title: "Opprette en salgsfaktura for prosjekt for å fakturere et prosjekt"
description: Beskriver hvordan du kan fakturere kunder for prosjektutgifter etter hvert som et prosjekt skrider frem.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project invoice
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 74b9209216f6e62dfc9519b288adca785cdb8100
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-invoice-jobs"></a>Fakturere prosjekter
I løpet av prosjektet kan det akkumuleres prosjektkostnader fra ressursforbruk, materiale og prosjektrelaterte kjøp. Under fremdriften til prosjektet blir disse transaksjonene bokført til prosjektkladden. Det er viktig at alle kostnader blir registrert i prosjektkladden før du fakturerer kunden.

Du kan fakturere hele prosjektet fra vinduet **Prosjektoppgavelinjer** eller bare fakturere utvalgte fakturerbare linjer fra vinduet **Planleggingslinjer**. Fakturering kan utføres etter at prosjektet er fullført, eller ved bestemte intervaller under fremdriften til prosjektet, basert på en faktureringsplan.

> [!NOTE]  
>   Hvis du velger **Fakturerbar** i feltet **Prosjektlinjetype** i kjøpsdokumentene for prosjektrelaterte kjøp, opprettes prosjektplanleggingslinjer som er klare til å bli fakturert til kunden. Hvis du vil ha mer informasjon, kan du se [Administrere prosjektforsyninger](projects-how-manage-project-supplies.md).

## <a name="to-create-and-post-a-job-sales-invoice"></a>Slik oppretter og bokfører du en salgsfaktura for prosjekt
Du kan opprette en faktura for et prosjekt eller for én eller flere prosjektoppgaver for en kunde enten når arbeidet som skal faktureres, er fullført, eller når faktureringsdatoen som er basert på et faktureringsestimat, er nådd.

Fra vinduet **Prosjekter** kan du fakturere en kunde ved å velge prosjektet, og deretter velge handlingen **Opprett salgsfaktura for prosjekt**. Følgende fremgangsmåte viser hvordan du bruker en satsvis jobb til å fakturere flere prosjekter.  

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Opprett salgsfaktura for prosjekt**, og velg deretter den relaterte koblingen.  
2. Fyll ut feltene etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Angi filtre hvis du vil begrense prosjektene som kjørselen skal behandle.
4. Velg **OK** for å opprette fakturaene.  

## <a name="to-create-multiple-job-sales-invoices-from-job-planning-lines"></a>Slik oppretter du flere prosjektsalgsfakturaer fra prosjektplanleggingslinjer
Du kan opprette en faktura fra en prosjektplanleggingslinje og samtidig angi antallet for varen, ressursen eller finanskontoen som du vil fakturere.

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Prosjekter**, og velg deretter den relaterte koblingen.
2. Åpne et relevant prosjekt.
3. Velg en prosjektoppgave der feltet **Prosjektoppgavetype** inneholder **Bokføring**, og velg deretter handlingen **Prosjektplanleggingslinjer**.  
4. På en prosjektplanleggingslinjer, i feltet **Ant. som skal overføres til faktura** angir du antallet av varen, ressursen, finanskontotypen du vil fakturere.  
5. Velg handlingen **Opprett salgsfaktura**.
6. I vinduet **Opprett salgsfaktura for prosjekt** skriver du inn bokføringsdatoen og om du vil opprette en ny faktura eller føye til denne fakturaen til en eksisterende.
7. Velg **OK**.  

    Du kan se antallet i feltet **Ant. overført til faktura** på prosjektplanleggingslinjen.
8. I vinduet **Prosjektplanleggingslinjer** velger du handlingen **Salgsfakturaer/kreditnotaer**.

    Vinduet **Salgsfaktura** åpnes og viser antallet du har overført til fakturaen.  
9. Gjør flere endringer, og velg deretter handlingen **Bokfør**.

> [!NOTE]  
>   Fremgangsmåten ovenfor er identisk for å opprette, gå gjennom og bokføre en prosjektrelatert salgskreditnota.

## <a name="to-calculate-and-post-job-completion-entries"></a>Slik beregner og bokfører du prosjektferdiggjørelsesposter
Når du har fullført alle aktiviteter for et prosjekt, inkludert bokføring og fakturering, må du oppdatere prosjektet for å sette **Status** til **Ferdig**. Deretter må du reversere alle VIA-er som er bokført i finans.

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Prosjekter**, og velg deretter den relaterte koblingen.  
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
[Finans](finance.md)  
[Innkjøp](purchasing-manage-purchasing.md)         
[Salg](sales-manage-sales.md)      
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

