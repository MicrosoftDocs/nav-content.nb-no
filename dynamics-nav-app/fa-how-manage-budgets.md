---
title: Administrere aktivabudsjetter
description: "Du kan definere informasjon om fremtidige investeringer, salg og avskrivning av aktiva for å bidra til å klargjøre budsjetter og prognoser."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: forecast
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 52b5e72d4d0a3e2c914894c58c10f44cb42d9c9d
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-manage-budgets-for-fixed-assets"></a>Behandle budsjetter for aktiva
Du kan definere budsjetterte aktiva. Dette gjør det for eksempel mulig å ta med forventede anskaffelser og salg i rapporter.  

Når du skal forberede et budsjettert resultatregnskap, balansebudsjett og likviditetsbudsjett, må du ha opplysninger om fremtidige investeringer, salg og aktivaavskrivninger. Du finner disse opplysningene i rapporten **Aktiva - forventet verdi**. Før du skriver ut denne rapporten, må du forberede budsjettet.  

## <a name="to-budget-the-acquisition-cost-of-a-fixed-asset"></a>Slik budsjetterer du anskaffelseskost for et aktiva:
Når du skal forberede et budsjett, må du definere aktivakort for aktiva som du vil kjøpe senere. De budsjetterte aktivaene er definert som vanlige aktiva, men må være konfigurert slik at de ikke bokføres i Finans.

Når du bokfører anskaffelseskosten, angir du nummeret for det budsjetterte aktivaet i feltet **Budsjettert aktivanr.** Dermed bokføres en anskaffelseskost med motsatt fortegn for det budsjetterte aktivaet. Dette betyr at den totale anskaffelseskosten for det budsjetterte aktivaet er differansen mellom den budsjetterte og den faktiske anskaffelseskosten.

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Aktiva**, og velg deretter den relaterte koblingen.
2. Velg **Ny** for å opprette et nytt aktivakort for det budsjetterte aktivaet.
3. Merk av for **Budsjettert aktiva** for å hindre bokføring til finans.
4. Fyll ut resten av feltene, tilordne et avskrivningstablå, og bokfør deretter den første anskaffelseskosten med det budsjetterte aktivaet som er angitt i feltet **Budsjettert aktivanr.** på kladdelinjen. Hvis du vil ha mer informasjon, kan du se [Anskaffe aktiva](fa-how-acquire.md).

## <a name="to-budget-the-disposal-of-a-fixed-asset"></a>Slik budsjetterer du salget av et aktiva:
Hvis du planlegger å selge aktiva i budsjettperioden, kan du angi opplysninger om salgsprisen og salgsdatoen.

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Aktiva**, og velg deretter den relaterte koblingen.
2. Velg aktivaet som skal avhendes, og velg deretter **Avskrivningstablåer**-handlingen.
3. Fyll ut feltene **Forventet salgsdato** og **Forventet gevinst ved salg** i vinduet **Aktivaavskrivningstablå**. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-view-projected-disposal-values"></a>Slik viser du forventede salgsverdier
Hvis du vil se de forventede salgsverdiene og beregne tap og vinning, kan du bruke rapporten **Aktiva - forventet verdi**.

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Aktiva - forventet verdi**, og velg deretter den relaterte koblingen.
2. Fyll ut feltene etter behov.
3. Velg knappen **Skriv ut** eller **Forhåndsvisning**.

## <a name="to-budget-depreciation"></a>Slik budsjetterer du avskrivninger
Du kan bruke rapporten **Aktiva - forventet verdi** til å beregne fremtidig avskrivning. Rapporten viser den bokførte verdien og den akkumulerte avskrivningen ved begynnelsen og slutten av den valgte perioden, samt endringer i perioden.

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Aktiva - forventet verdi**, og velg deretter den relaterte koblingen.
2. Fyll ut feltene etter behov.
3. Hvis du vil se de samlede verdiene for alle aktiva, fjerner du avmerkingen for **Skriv ut per aktiva**.
4. La hurtigfanen **Aktiva** stå tom hvis du vil ha med alle aktivaene. I feltet **Budsjettert aktiva** angir du **Nei** hvis du ikke vil ha med budsjetterte aktiva, eller **Ja** hvis du bare vil se på de budsjetterte aktivaene.
5. Velg knappen **Skriv ut** eller **Forhåndsvisning**.

## <a name="see-also"></a>Se også
[Aktiva](fa-manage.md)  
[Definere aktiva](fa-setup.md)  
[Finans](finance.md)  
[Velkommen til [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

