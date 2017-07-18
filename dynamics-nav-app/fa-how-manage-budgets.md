---
title: Behandle budsjetter for aktiva
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 47b5e0abcae4fab92da5dd9c1bda350a37ec0358
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-manage-budgets-for-fixed-assets"></a>Behandle budsjetter for aktiva
Du kan definere budsjetterte aktiva. Dette gjør det mulig å ta med eventuelle forventede anskaffelser og salg i rapporter.  

 Når du skal forberede et budsjettert resultatregnskap, balansebudsjett og likviditetsbudsjett, må du ha opplysninger om fremtidige investeringer, salg og aktivaavskrivninger. Du finner disse opplysningene i rapporten **Aktiva - forventet verdi**. Før du skriver ut denne rapporten, må du forberede budsjettet.  

## <a name="to-budget-the-acquisition-cost-of-a-fixed-asset"></a>Slik budsjetterer du anskaffelseskost for et aktiva:
Når du skal forberede et budsjett, må du definere aktivakort for aktiva som du vil kjøpe senere. De budsjetterte aktivaene er definert som vanlige aktiva, men må være konfigurert slik at de ikke bokføres i Finans.

Når du bokfører anskaffelseskosten, angir du nummeret for det budsjetterte aktivaet i **Budsjettert aktivanr.**-feltet . Dermed bokføres en anskaffelseskost med motsatt fortegn for det budsjetterte aktivaet. Dette betyr at den totale anskaffelseskosten for det budsjetterte aktivaet er differansen mellom den budsjetterte og den faktiske anskaffelseskosten.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktiva** og velger deretter den relaterte koblingen.
2. Velg **Ny** for å opprette et nytt aktivakort for det budsjetterte aktivaet.
3. Merk av for **Budsjettert aktiva** for å hindre bokføring til finans.
4. Fyll ut resten av feltene, tilordne et avskrivningstablå, og bokfør deretter den første anskaffelseskosten med det budsjetterte aktivaet som er angitt i **Budsjettert aktivanr.**-feltet på kladdelinjen. Hvis du vil ha mer informasjon, se [Anskaffe aktiva](fa-how-acquire.md).

## <a name="to-budget-the-disposal-of-a-fixed-asset"></a>Slik budsjetterer du salget av et aktiva:
Hvis du planlegger å selge aktiva i budsjettperioden, kan du angi opplysninger om salgsprisen og salgsdatoen.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktiva** og velger deretter den relaterte koblingen.
2. Velg aktivaet som skal avhendes, og velg deretter **Avskrivningstablåer**-handlingen.
3. Fyll ut feltene **Forventet salgsdato** og **Forventet gevinst ved salg** i vinduet **Aktivaavskrivningstablå**. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.

## <a name="to-view-projected-disposal-values"></a>Slik viser du forventede salgsverdier
Hvis du vil se de forventede salgsverdiene og beregne tap og vinning, kan du bruke rapporten **Aktiva - forventet verdi**.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktiva - forventet verdi** og velger deretter den relaterte koblingen.
2. Fyll ut feltene etter behov.
3. Velg knappen **Skriv ut** eller **Forhåndsvisning**.

## <a name="to-budget-depreciation"></a>Slik budsjetterer du avskrivninger
Du kan bruke rapporten **Aktiva - forventet verdi** til å beregne fremtidig avskrivning. Rapporten viser den bokførte verdien og den akkumulerte avskrivningen ved begynnelsen og slutten av den valgte perioden, samt endringer i perioden.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktiva - forventet verdi** og velger deretter den relaterte koblingen.
2. Fyll ut feltene etter behov.
3. Hvis du vil se de samlede verdiene for alle aktiva, fjerner du avmerkingen for **Skriv ut per aktiva**.
4. La hurtigfanen **Aktiva** stå tom hvis du vil ha med alle aktivaene. I feltet **Budsjettert aktiva** angir du **Nei** hvis du ikke vil ha med budsjetterte aktiva, eller **Ja** hvis du bare vil se på de budsjetterte aktivaene.
5. Velg knappen **Skriv ut** eller **Forhåndsvisning**.

## <a name="see-also"></a>Se også
[Administrere aktiva](fa-manage.md)  
[Definere aktiva](fa-setup.md)  
[Finans](finance-setup.md)  
[Velkommen til Dynamics NAV](across-get-started.md)

