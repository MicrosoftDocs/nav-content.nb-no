---
title: Avhende eller trekke tilbake aktiva
description: "Du må bokføre en salgsverdi når du kasserer, selger eller trekker tilbake et aktivum."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: scrap
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f6e90150a2fd14be13746dcbc91a6fca82d39738
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-dispose-of-or-retire-fixed-assets"></a>Avhende eller trekke tilbake aktiva
Når du selger eller på annen måte avhender et aktiva, må salgsverdien bokføres for å beregne og registrere tap eller vinning. En salgspost må være den siste posten som bokføres for et aktiva. Du kan bokføre mer enn én salgspost for aktiva som er delvis solgt. Summen av alle bokførte salgsbeløp må være et kreditbeløp.  

> [!NOTE]  
>   Hvis du bytter ut et aktivum med et annet, må du registrere både salget av det gamle aktivumet (salg) og innkjøpet av det nye (anskaffelse). Hvis du vil ha mer informasjon, kan du se [Anskaffe aktiva](fa-how-acquire.md).  

## <a name="to-post-a-disposal-from-the-fixed-asset-gl-journal"></a>Slik bokfører du et salg fra aktivafinanskladden:
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Aktivafinanskladder**, og velg deretter den relaterte koblingen.  
2. Opprett en innledende kladdelinje, og fyll ut feltene etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. I feltet **Aktivabokf.type** velger du **Salg**.  
4. Velg **Sett inn aktivamotkonto**. En ny kladdelinje opprettes for motkontoen som er satt opp for salgsbokføring.  

    > [!NOTE]  
>   Trinn 4 fungerer bare hvis du har definert følgende: I vinduet **Kort for bokf.grp.- aktiva** for bokføringsgruppen for aktivumet, inneholder feltet **Konto for salg** finansdebetkontoen, og feltet **Motkonto for salg** inneholder finanskontoen du vil bokføre motposter for oppskrivning til. Hvis du vil ha mer informasjon, kan du se "Definere bokføringsgrupper for aktiva" i [Definere generell aktivainformasjon](fa-how-setup-general.md).  
5. Velg handlingen **Bokfør**.  

    Hvis du selger eller på avhender deler av et aktiva, må du dele opp aktivaet før du kan registrere salgstransaksjonen. Hvis du vil ha mer informasjon, kan du se [Overføre, dele opp eller kombinere aktiva](fa-how-trans-split-combine.md).  

## <a name="to-view-disposal-ledger-entries"></a>Slik viser du salgsposter
Når du selger eller avhender et aktiva, bokføres salgsverdien til finans der du kan se resultatet.  

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Aktiva**, og velg deretter den relaterte koblingen.  
2. Velg aktivaet du vil vise poster for, og velg deretter **Avskrivningstablåer**.  
3. Velg avskrivningstablået du vil vise poster for, og velg deretter **Poster**.  
4. Velg en linje med **Salg** i **Bokføringskategori, aktiva**-feltet, og velg deretter **Naviger**.  
5. I **Naviger**-vinduet velger du finanspostlinjen og deretter **Vis**.  

**Finansposter**-vinduet åpnes der du kan se postene som er resultat av salgsbokføringen.  

## <a name="see-also"></a>Se også
[Aktiva](fa-manage.md)  
[Definere aktiva](fa-setup.md)  
[Finans](finance.md)  
[Velkommen til [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

