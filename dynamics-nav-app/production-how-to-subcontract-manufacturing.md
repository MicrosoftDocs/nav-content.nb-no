---
title: Underleveranse av produksjon
description: "Når bestillingen er opprettet fra underleverandørforslaget, kan den bokføres."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: fa1d42f623ba3d13f60d49b502c15fcc3f48bde7
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-subcontract-manufacturing"></a>Underleveranse av produksjon
Underleveranse av valgte operasjoner til leverandør er vanlig i mange produksjonsselskaper. Underleveranse kan skje en sjelden gang eller være en vesentlig del av alle produksjonsprosesser.

Programmet har mange verktøy for håndtering av underleveransearbeid:  

- Arbeidssentre med tilordnet leverandør: Du kan bruke denne funksjonen til å definere et arbeidssenter som er tilknyttet en leverandør (underleverandør). Dette kalles et arbeidssenter for underleveranse. Du kan angi et arbeidssenter for underleveranse i en ruteoperasjon, slik at du enkelt kan behandle underleveranseaktiviteten. I tillegg kan operasjonskostbeløpet tildeles på rute- eller arbeidssenternivået.  
- Arbeidssenterkost basert på enheter eller tid: Du kan bruke denne funksjonen til å angi om kost som er knyttet til arbeidssenteret, er basert på produksjonstiden eller på en ensartet pris per enhet. Selv om underleverandører vanligvis bruker en ensartet pris per enhet som betaling for tjenester, kan programmet håndtere begge alternativene (produksjonstid og ensartet pris per enhet).  
- Underleveranseforslag: Du kan bruke denne funksjonen til å finne produksjonsordrene med materiale som er klare til å bli sendt til en underleverandør, og til å opprette bestillinger for underleveranseoperasjoner fra produksjonsordreruter automatisk. Deretter bokføres bestillingsgebyrene automatisk i produksjonsordren under bokføringen av bestillingen. Du kan bare få tilgang til og bruke produksjonsordrer med statusen frigitt fra et underleveranseforslag.  

## <a name="subcontract-work-centers"></a>Arbeidssentre for underleveranse  
Arbeidssentre for underleveranse defineres på samme måte som vanlige arbeidssentre med tilleggsinformasjon. De tilordnes ruter på samme måte som andre arbeidssentre.  

### <a name="subcontract-work-center-fields"></a>Felt i arbeidssentre for underleveranse  
Feltet **Underleverandørnr.** angir arbeidssenteret som et arbeidssenter for underleveranse. Du kan angi nummeret på en underleverandør som forsyner arbeidssenteret. Feltet kan brukes til å administrere eksterne arbeidssentre som arbeider på kontrakt.  

Hvis du avtaler underleveranser med leverandøren med en ulik sats for hver prosess, velger du feltet **Bestemt enhetskost**. Dermed kan du definere en kost på hver rutelinje og sparer tiden det tar å angi hver bestilling. Kosten på rutelinjen brukes i behandling i stedet for kosten i kostfeltene i arbeidssenteret. Når du velger feltet **Bestemt enhetskost**, beregnes kost for leverandøren i henhold til ruteoperasjonen.  

Hvis du avtaler underleveranser med én enkelt sats per leverandør, lar du feltet **Bestemt enhetskost** stå tomt. Kostbeløpene defineres ved å fylle ut feltene **Direkte enhetskost**, **Indirekte kost-%** og **Sats for indirekte kostnader**.  

### <a name="routings-that-use-subcontract-work-centers"></a>Ruter som bruker arbeidssentre for underleveranse  
Arbeidssentre for underleveranse kan brukes til operasjoner i ruter på samme måte som vanlige arbeidssentre.  

Du kan definere en rute som bruker et eksternt arbeidssenter, som et standard operasjonstrinn. Alternativt kan du endre ruten for en bestemt produksjonsordre for å inkludere en ekstern operasjon. Dette kan bli nødvendig i en nødssituasjon, for eksempel hvis en server ikke fungerer riktig, eller i en midlertidig periode med høyere etterspørsel, der arbeid som vanligvis gjøres internt, må sendes til en underleverandør.  

Hvis du vil ha mer informasjon, kan du se [Opprette ruter](production-how-to-create-routings.md).  

## <a name="subcontracting-worksheet"></a>Underleveranseforslag  
Når du har beregnet underleveranseforslaget, opprettes det aktuelle dokumentet, i dette tilfellet en bestilling.  

# <a name="how-to-calculate-subcontracting-worksheets-and-create-subcontract-purchase-orders"></a>Beregne underleveranseforslag og opprette underleverandørbestillinger
Vinduet **Underleveranseforslag** fungerer som **Planleggingsforslag** ved å beregne den nødvendige forsyningen, i dette tilfellet bestillinger, som du ser gjennom i forslaget og deretter oppretter med funksjonen **Utfør handlingsmelding**.  

> [!NOTE]  
>  Du kan bare få tilgang til og bruke produksjonsordrer med statusen **Frigitt** fra et underleveranseforslag.  

### <a name="to-calculate-the-subcontracting-worksheet"></a>Slik beregner du underleveranseforslaget  
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Underleveranseforslag**, og velg deretter den relaterte koblingen.  
2.  Hvis du vil beregne forslaget, velger du handlingen **Beregn underleveranser**.  
3.  I vinduet **Beregn underleveranser** angir du filtre for underleveranseoperasjonene, eller arbeidssentrene der de utføres, for å beregne bare de relevante produksjonsordrene.  
4.  Velg **OK**-knappen.  

    Gå gjennom linjene i vinduet **Underleveranseforslag**. Informasjonen i dette forslaget kommer fra produksjonsordren og produksjonsordrerutelinjene og sendes til bestillingen når bestillingsdokumentet opprettes. Som i de andre forslagene, kan du slette en rad fra dette forslaget uten at det påvirker den opprinnelige informasjonen. Informasjonen vises igjen neste gang du kjører funksjonen **Beregn underleveranser**.  

### <a name="to-create-the-subcontract-purchase-order"></a>Slik oppretter du underleverandørbestillingen  
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Underleveranseforslag**, og velg deretter den relaterte koblingen.  
2.  I fanebladet **Handlinger**, under **Prosess** velger du **Utfør handlingsmelding**.  
3.  Velg feltet **Skriv ut bestillinger** hvis du vil skrive ut bestillingen når den opprettes.  
4.  Velg **OK**.  

Hvis alle underleveranseoperasjoner sendes til samme leverandørlokasjon, opprettes bare én bestilling.  

Forslagslinjen som ble gjort om til en bestilling, slettes fra forslaget. Når en bestilling er opprettet vises den ikke på nytt i forslaget.  

## <a name="posting-subcontract-purchase-orders"></a>Bokføre underleverandørbestillinger  
Når underleverandørbestillingene er opprettet kan de bli bokført. Når bestillingen mottas bokføres en kapasitetspost i produksjonsordren, og når den faktureres, bokføres den direkte kostnaden i produksjonsordren.  

Det bokføres automatisk en ferdigmeldingskladdelinjepost for produksjonsordren når kjøpet er bokført som mottatt. Dette gjelder bare hvis underleveranseoperasjonen er den siste operasjonen på produksjonsordreruten.  

> [!CAUTION]  
>  Det kan være at det ikke er ønskelig å bokføre utdata for en pågående produksjonsordre automatisk når underleveransevarer mottas. Årsaker til dette kan være at det forventede avgangsantallet som er bokført, kan være forskjellig fra det faktiske antallet og at bokføringsdatoen for de automatiske utdataene er misvisende.  
>   
>  For å unngå at den forventede avgangen for en produksjonsordre bokføres når kjøp fra underleverandører mottas, må du passe på at underleveranseoperasjonen ikke er den siste. Du kan også sette inn en ny siste operasjon for endelig avgangsantall.

## <a name="to-post-a-subcontract-purchase-order"></a>Slik bokfører du en underleverandørbestilling  
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bestillinger**, og velg deretter den relaterte koblingen.  
2.  Åpne en bestilling som er opprettet fra underleveranseforslaget.  

    På bestillingslinjene ser du den samme informasjonen som far i forslaget. Feltene **Prod.ordrenr.**, **Prod.ordrelinjenr.**, **Operasjonsnr.**, og **Arbeidssenternr.** er fylt med informasjon fra kildeproduksjonsordren.  

3.  Velg handlingen **Bokfør**.  

Det bokføres automatisk en ferdigmeldingskladdelinjepost for produksjonsordren når kjøpet er bokført som mottatt. Dette gjelder bare hvis underleveranseoperasjonen er den siste operasjonen på produksjonsordreruten.  

> [!CAUTION]  
>  Det kan være at det ikke er ønskelig å bokføre utdata for en pågående produksjonsordre automatisk når underleveransevarer mottas. Årsaker til dette kan være at det forventede avgangsantallet som er bokført, kan være forskjellig fra det faktiske antallet og at bokføringsdatoen for de automatiske utdataene er misvisende.  
>   
>  For å unngå at den forventede avgangen for en produksjonsordre bokføres når kjøp fra underleverandører mottas, må du passe på at underleveranseoperasjonen ikke er den siste. Du kan også sette inn en ny siste operasjon for endelig avgangsantall.  

Direkte kost for bestillingen bokføres til bestillingen når bestillingen er bokført som fakturert.  

## <a name="see-also"></a>Se også  
[Produksjon](production-manage-manufacturing.md)    
[Definere produksjon](production-configure-production-processes.md)  
[Planlegging](production-planning.md)      
[Lager](inventory-manage-inventory.md)  
[Innkjøp](purchasing-manage-purchasing.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

