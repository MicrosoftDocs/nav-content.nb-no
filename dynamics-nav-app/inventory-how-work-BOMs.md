---
title: "Arbeide med stykklister for å håndtere komponenter"
description: "Du oppretter en monteringsstykkliste eller produksjonsstykkliste for å spesifisere komponenter eller ressurser som kreves for å sette sammen varen som stykklisten representerer."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 09/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 9515ab4e5fc1003fd175c0946aeaceba33dac825
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-work-with-bills-of-material"></a>Arbeide med stykklister
Du bruker stykklister til å strukturere overordnede varer som må monteres eller produseres av ressurser eller produksjonsressurser fra komponenter. En monteringsstykkliste kan også brukes til å selge en overordnet vare som et sett som består av dens komponenter.

## <a name="assembly-boms-or-production-boms"></a>Monteringsstykklister eller produksjonsstykklister
Du bruker monteringsordrer for å produsere sluttvarer fra komponenter i en enkel prosess som kan utføres av én eller flere grunnleggende ressurser, som ikke er produksjonsressurser eller arbeidssentre, eller uten noen ressurser. En monteringsprosess kan for eksempel være å plukke to flasker vin og én kaffepose og deretter pakke dem som en gave.  

En monteringsstykkliste er hoveddataene som definerer hvilke komponentvarer som inngår i en montert sluttvare, og hvilke ressurser som brukes til å montere monteringselementet. Når du angir en monteringsvare og et antall i hodet i en ny monteringsordre, fylles monteringsordrelinjene automatisk ut i henhold til monteringsstykklisten, med én monteringsordrelinje per komponent eller ressurs. Hvis du vil ha mer informasjon, se [Monteringsstyring](assembly-assemble-items.md).

Monteringsstykklister beskrives i dette emnet.

Du bruker produksjonsordrer for å produsere sluttvarer fra komponenter i en kompleks prosess som krever en produksjonsrute og arbeidssentre eller produksjonsressurser, som representerer produksjonskapasitet. En produksjonsprosess kan for eksempel være å skjære stålplater i én operasjon, sveise dem sammen i neste operasjon og male sluttvaren i siste operasjon. Se også [Produksjon](production-manage-manufacturing.md) for mer informasjon.  

En produksjonsstykkliste er hoveddata som definerer en produksjonsvare og komponentene som inngå i den. For monteringsvarer må produksjonsstykklisten sertifiseres og tilordnes til produksjonsvaren før den kan brukes i en produksjonsordre. Når du angir produksjonsvaren på en produksjonsordrelinje, enten manuelt eller ved å fornye ordren, vil innholdet i produksjonsstykklisten gjøres til produksjonsordrekomponentene. Hvis du vil ha mer informasjon, kan du se [Opprette produksjonsstykklister](production-how-to-create-production-boms.md).  

Konseptet med ressurser i produksjon er mye mer avansert enn i monteringsstyring. Arbeidssentre og produksjonsressurser fungerer som ressurser, og produksjonstrinn representeres av operasjoner som er tilordnet til ressurser i produksjonsruter. Hvis du vil ha mer informasjon, kan du se [Opprette ruter](production-how-to-create-routings.md).

Både monteringsordrer og produksjonsordrer kan kobles direkte til salgsordrer. Du kan imidlertid bare bruke monteringsordrer til å tilpasse sluttvaren direkte for en kundeforespørsel med ordren.

## <a name="to-create-an-assembly-bom"></a>Slik oppretter du en monteringsstykkliste:
Hvis du vil definere en overordnet vare som består av andre varer, og potensielt av ressursene som kreves for å sette sammen den overordnede varen, må du opprette en monteringsstykkliste.  

Monteringsstykklister inneholder vanligvis varer, men kan også inneholde en eller flere ressurser som trengs for å sette monteringsvaren sammen.

Monteringsstykklister kan ha flere nivåer, noe som betyr at en komponent i monteringsstykklisten selv kan være en monteringsvare. I så fall skal **Monteringsstykkliste**-feltet på monteringsstykklistelinjen inneholde **Ja**.

Spesielle krav gjelder for varer i monteringsstykklister med hensyn til tilgjengelighet. Hvis du vil ha mer informasjon, kan du se delen «Vise tilgjengeligheten til en vare etter bruk i monteringsstykklister» i [Vise tilgjengeligheten av varer](inventory-how-availability-overview.md).

Oppretting av en monteringsstykkliste foregår i to trinn:
- Definere en ny vare
- Definere stykklistestrukturen for monteringsvaren.

1. Definer en ny vare. Hvis du vil ha mer informasjon, kan du se [Registrere nye varer](inventory-how-register-new-items.md).

    Fortsette med å registrere komponenter eller ressurser i monteringsstykklisten.  
2. I vinduet **Varekort** for en monteringsvare velger du **Montering** og velger deretter **Monteringsstykkliste**.
3. Fyll ut feltene etter behov i vinduet **Monteringsstykkliste**. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-view-the-components-of-an-assembly-item-indented-according-to-the-bom-structure"></a>Vise komponentene i en monteringsvare som er rykket inn i henhold til stykklistestrukturen
Fra vinduet **Monteringsstykkliste** kan du åpne et eget vindu som viser komponentene og ressurser som er rykket inn, i henhold til deres stykklisteposisjon under monteringsvaren.

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Varer**, og velg deretter den relaterte koblingen.
2. Åpne kortet for en monteringsvare. (Feltet **Monteringsstykkliste** i vinduet **Varer** inneholder **Ja**.)
3. I vinduet **Varekort** velger du **Montering** og velger deretter **Monteringsstykkliste**.
4. I vinduet **Monteringsstykkliste** velger du handlingen **Vis stykkliste**.

## <a name="to-replace-the-assembly-item-with-its-components-on-document-lines"></a>Slik erstatter du monteringsvaren med dens komponenter i dokumentlinjer
Du kan bruke en spesiell funksjon erstatte linjen for varen samlingen med nye linjer for komponentene fra en salgs- og kjøpsdokument som inneholder en vare i produksjonen. Denne funksjonen er nyttig for eksempel hvis du vil selge komponentene som et sett med samlingen varen.

**Forsiktigh**: Når du har brukt funksjonen **Utfold Stykkliste**, er det ikke enkelt å angre den. Du må slette ordrelinjene som representerer komponentene og deretter skrive inn en ordrelinje for monteringsvaren på nytt.

Følgende fremgangsmåte er basert på en faktura. De samme trinnene gjelder for andre salgsdokumenter og på alle kjøpsdokumenter.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Salgsfakturaer** og velger deretter den relaterte koblingen.
2. Åpne en salgsfaktura som inneholder en linje for en monteringsvare.
3. Velg linjen for monteringsvaren, og velg deretter linjehandlingen **Utfold stykkliste**.

Alle feltene på salgsfakturalinjen for monteringsvaren er tomme med unntak av for feltet **Vare** og **Beskrivelse**. Komplette salgsfakturalinjer settes inn for komponentene og mulige ressurser som utgjør monteringsvaren.

**Merk**: Funksjonen Utfold stykkliste finnes også i vinduet **Monteringsstykkliste**.

## <a name="to-calculate-the-standard-cost-of-an-assembly-item"></a>Slik beregner du standardkosten for en monteringsvare
Du beregner enhetskosten for en monteringsvare ved å opprullere enhetskosten for hver komponent og ressurs i varens monteringsstykkliste.

Du kan også beregne og oppdatere standardkost for én eller flere varer i vinduet **Standardkost - forslag**. Hvis du vil ha mer informasjon, kan du se [Oppdatere standardkost](finance-how-to-update-standard-costs.md).  

Enhetskosten for en monteringsstykkliste er alltid lik totalsummen for enhetskostnadene for komponentene, inkludert andre monteringsstykklister og ressurser.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Varer** og velger deretter den relaterte koblingen.
2. Åpne kortet for en monteringsvare. (Feltet **Monteringsstykkliste** i vinduet **Varer** inneholder **Ja**.)
3. I vinduet **Varekort** velger du **Montering** og velger deretter **Monteringsstykkliste**.
4. I vinduet **Monteringsstykkliste** velger du **Beregn standardkost**.
5. Velg ett av følgende alternativer, og velg deretter **OK**.

|Alternativ |Beskrivelse |
|-------|------------|
|**Øverste nivå**|Beregner monteringsvaren standardkostnad som den totale kostnaden for alle kjøpte eller monterte varer i monteringsstykklisten, uavhengig av eventuelle underliggende monteringsstykklister.|
|**Alle nivåer**|Beregner monteringsvarens standardkost som summen av: 1) det beregnede kostbeløpet for alle underliggende monteringsstykklister i monteringsstykklisten. 2) kostnadene for alle innkjøpte varer på monteringsstykklisten.|



Kostnadene for varer som utgjør monteringsstykklisten kopieres fra komponentvarekortene. Hver varekostnad multipliseres med antallet, og kostbeløpet vises i feltet **Enhetskost** på varekortet.

## <a name="see-also"></a>Se også
[Registrere nye varer](inventory-how-register-new-items.md)  
[Vise tilgjengeligheten av varer](inventory-how-availability-overview.md)     
[Lager](inventory-manage-inventory.md)  
[Arbeide med [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](ui-work-product.md)

