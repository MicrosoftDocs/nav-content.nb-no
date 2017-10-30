---
title: Spore varesporede varer
description: "Du kan vise hvor en varesporet vare er brukt, inkludert hvordan og når den ble mottatt eller produsert, overført, solgt, forbrukt eller returnert. Du kan også finne alle gjeldende forekomster av et bestemt serie- eller partinummer i databasen. Dette gjør du ved hjelp av funksjonene Varesporing og Naviger."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 6d25a7b60f8b1b37ef9de34d5ffc098a89828ea8
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-trace-item-tracked-items"></a>Spore varesporede varer
Du kan vise hvor en varesporet vare er brukt, inkludert hvordan og når den ble mottatt eller produsert, overført, solgt, forbrukt eller returnert. Du kan også finne alle gjeldende forekomster av et bestemt serie- eller partinummer i databasen. Dette gjør du ved hjelp av funksjonene Varesporing og Naviger.  

 Disse funksjonene kan være spesielt nyttige i kvalitetskontroll når du må finne ut hvilke kunder som mottok produkter fra et bestemt partinummer, eller når du må finne ut hvilket parti en defekt komponent kom fra.  

 I vinduet **Varesporing** kan du spore fremover og bakover i en sekvens med bokførte lagertransaksjoner for serie- eller partinummeret.  

 Du kan ikke se transaksjonssekvensen i vinduet **Naviger**, men du kan se alle postene for serie- eller partinummeret, både bokførte poster og åpne poster.  

 De to funksjonene kan brukes i kombinasjon ved å overføre et sporet serie- eller partinummer til vinduet **Naviger** hvis du vil fullføre et fullstendig sporingsscenario. Hvis du vil ha mer informasjon, kan du se [Gjennomgang: spore serie-/partinumre](walkthrough-tracing-serial-lot-numbers.md).  

## <a name="to-trace-item-tracked-items"></a>Slik sporer du varesporede varer  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Varesporing**, og velg deretter den relaterte koblingen.  
2.  Angi de bestemte varenumrene eller et filter på varenumrene du vil spore, i filterfeltene øverst i vinduet.  
3.  Velg om du også vil vise hvor komponentene for varen kommer fra, i feltet **Vis komponenter**. Alternativene i dette feltet er som følger.  

    |Felt|Beskrivelse|  
    |----------------------------------|---------------------------------------|  
    |**Nei**|Velg dette alternativet hvis du ikke vil vise noen komponenter.|  
    |**Bare varesporet**|Velg dette alternativet hvis du bare vil vise komponenter som har parti- eller serienumre.|  
    |**Alle**|Velg dette alternativet hvis du vil vise alle komponentene.|  

4.  Velg metoden du vil bruke til å spore varen, i feltet **Sporingsmetode**. Du kan velge mellom følgende alternativer  

    |Felt|Beskrivelse|  
    |----------------------------------|---------------------------------------|  
    |**Forbruk->opprinnelse**|Denne metoden sporer varen fra der den ble brukt, til der den kom fra. Hvis en produsert vare for eksempel ble solgt til en kunde, vises dette i **Varesporing**-vinduet med følgeseddellinjen først, som du deretter kan utvide for å vise hvilken produksjonsordre den kom fra.|  
    |**Opprinnelse->forbruk**|Denne metoden sporer varen fra der den kom inn på lageret, til der den ble brukt. Hvis en produsert vare ble solgt til en kunde, vises dette i **Varesporing**-vinduet med den ferdige produksjonsordren først, som du deretter kan utvide for å vise følgeseddellinjer der varen ble brukt.|  

5.  Velg **Spor** for å kjøre sporingen.  

> [!NOTE]  
>  Hvis du har mottatt samme parti i flere transaksjoner, vises kanskje ikke alle transaksjonene i vinduet **Varesporing**. Det vises bare utlignede transaksjoner.  

> [!NOTE]  
>  Hvis ytterligere transaksjonshistorikk under en varesporingslinje allerede er sporet av en annen linje ovenfor, er det merket av for **Allerede sporet**. For en enklere visning vises ikke slike underliggende linjer.  
>   
>  Når du skal søke etter varesporingslinjer der transaksjonsloggen allerede er sporet, velger du knappen **Gå til allerede sporet**. Den aktuelle varesporingslinjen velges, og alle underliggende linjer utvides.  

## <a name="to-find-item-tracked-items-with-navigate"></a>Slik søker du etter varesporede varer med Naviger:  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Naviger**, og velg deretter den relaterte koblingen.  
2.  På hurtigfanen **Varesporing**, under **Serienr.** og **Partinr.** angir du varesporingsnumrene du vil spore.  
3.  Velg **Søk** for å finne alle forekomster av serie- eller partinummeret i databasen.  

## <a name="see-also"></a>Se også  
[Lager](inventory-manage-inventory.md)  
[Designdetaljer: Varesporing](design-details-item-tracking.md)
[Designdetaljer: Varesporing og reservasjoner](design-details-item-tracking-and-reservations.md)  
[Reservere varer](inventory-how-to-reserve-items.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
[Gjennomgang: spore serie-/partinumre](walkthrough-tracing-serial-lot-numbers.md)

