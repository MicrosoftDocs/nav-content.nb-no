---
title: "Bokføre konserninterne dokumenter og kladder"
description: "Bruke konserninterne dokumenter til å bokføre transaksjoner med de konserninterne partnerne."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: IC, group, consolidation, affiliate, subsidiary
ms.date: 06/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 176c12271c55936e61235e3a726932aa02b29b74
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-work-with-intercompany-documents-and-journals"></a>Arbeide med konserninterne dokumenter og kladder
Du bruker konserninterne dokumenter eller kladder til å bokføre transaksjoner med de konserninterne partnerne. Når du bokfører et konserninternt dokument eller en kladdelinje i selskapet, opprettes det et tilsvarende dokument eller kladdelinje i den konserninterne utboksen som du kan overføre til partneren. Partneren kan deretter bokføre den tilsvarende transaksjonen i selskapet sitt, uten å måtte registrere dataene på nytt.

For salgs-og kjøpsdokumenter sikrer den konserninterne partnerkoden på den involverte kunden eller leverandøren at alle ordrer og fakturaer som genereres i forbindelse med transaksjoner med disse selskapene, produserer tilhørende bilag i partnerselskapet, noe som fører til riktig balansering av kontoene.

For konserninterne finanskladdelinjer trenger du ikke å angi kontoene for et individuelt sett med bøker, men ganske enkelt gi identifikasjonen av partnerselskapet. Tilsvarende konserinterne finanskladdelinjer opprettes deretter i partnerselskapet, noe som fører til balansering av bøkene i begge selskapene som er involvert i en transaksjon.

## <a name="to-fill-in-and-send-an-intercompany-sales-order"></a>Slik fyller du ut og sender en konsernintern ordre
Du kan sende ordrer, bestillinger og returordrer før bokføring. Fakturaer og kreditnotaer kan ikke sendes før de bokført.

Fremgangsmåten nedenfor beskriver hvordan du fyller ut og sender en konsernintern ordre. Den samme fremgangsmåten gjelder for konserninterne bestillinger og returordrer og for bokførte konserninterne fakturaer og kreditnotaer.  

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Ordrer**, og velg deretter den relaterte koblingen.  
2. Velg **Ny** for å opprette en ny ordre. Hvis du vil ha mer informasjon, kan du se [Selge produkter](sales-how-sell-products.md).  
3. Fyll ut feltene etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Kointroller at kunden er en konsernintern partner.
5. Hvis du vil sende ordren før du bokfører den, kan du velge **Send KI-ordre**.

> [!NOTE]
> Hvis du utfører trinn 4, blir ordren flyttet til den konserninterne utboksen der du kan sende den senere. Hvis du vil ha mer informasjon, se [Administrere den konserninterne innboksen og utboksen](intercompany-how-manage-intercompany-inbox.md).

## <a name="to-fill-in-and-post-an-intercompany-journal"></a>Slik fyller du ut og bokfører en konsernintern kladd
Når du bokfører en konsernintern kladdelinje i selskapet, opprettes det en tilsvarende kladdelinje i den konserninterne utboksen som du kan overføre til partneren. Partneren kan deretter bokføre den tilsvarende transaksjonen i selskapet sitt, uten å måtte registrere dataene på nytt.

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **KI-finanskladder**, og velg deretter den relaterte koblingen.  
2. Åpne den relevante kjørselen for kladden. Hvis du vil ha mer informasjon, kan du se [Arbeide med finanskladder](ui-work-general-journals.md).
3. Fyll ut feltene etter behov.
4. I feltet **Finanskontonr. for KI-partner** angir du nummeret til den konserninterne finanskontoen der beløpet skal bokføres i partnerens selskap.

    > [!NOTE]
    > Dette Feltet må fylles ut på en linje med en bankkonto eller finanskonto i feltet **Kontonr.** eller **Motkontonr.**.  
5. Velg handlingen **Bokfør**.

De involverte postene bokføres i selskapet ditt, og en kladd med tilhørende poster opprettes i den konserninterne utboksen som du kan sende til partnerselskapet. Hvis du vil ha mer informasjon, se [Administrere den konserninterne innboksen og utboksen](intercompany-how-manage-intercompany-inbox.md). 

## <a name="see-also"></a>Se også
[Behandle konserninterne transaksjoner](intercompany-manage.md)  
[Finans](finance.md)  
[Konfigurere finans](finance-setup-finance.md)  
[Arbeide med finanskladder](ui-work-general-journals.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

