---
title: Opprette bankkonti
description: Du kan avstemme bankkonti i Dynamics NAV med kontoutdrag fra banken.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: feed, stream
ms.date: 09/26/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3581615fe94006aa9245f5e66fe6cf475b22acfb
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-bank-accounts"></a>Opprette bankkonti
Du bruker bankkonti i [!INCLUDE[d365fin](includes/d365fin_md.md)] til å holde orden på banktransaksjonene dine. Konti kan utstedes i norske kroner eller i fremmed valuta. Når du har opprettet bankkonti, kan du bruke mulighetene for utskriving av sjekker (gjelder ikke Norge).

## <a name="to-set-up-bank-accounts"></a>Slik setter du opp bankkonti
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bankkonti**, og velg deretter den relaterte koblingen.
2. I vinduet **Bankkonti** velger du handlingen **Ny**.
3. Fyll ut feltene etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]
> For å kunne fylle ut **Saldo**-feltet med en inngående balanse, må du bokføre en bankkontopost med det aktuelle beløpet. Du kan gjøre dette ved å utføre en bankkontoavstemming. Hvis du vil ha mer informasjon, kan du se [Avstemme bankkonti separat](bank-how-reconcile-bank-accounts-separately.md). Du kan eventuelt også implementere den inngående balansen som en del av en generell dataoppretting i nye selskaper ved hjelp av det assisterte oppsettet for **Overfør forretningsdata**. Hvis du vil ha mer informasjon, kan du se [Velkommen til [!INCLUDE[d365fin](includes/d365fin_md.md)](index.md).

## <a name="to-set-up-your-bank-account-for-import-or-export-of-bank-files"></a>Opprette din bankkonto for import eller eksport av bankfilene
Felt i hurtigafnen **Overføring** i vinduet **Bankkontokort** er relatert til import og eksport av bankfeeder og filer. Hvis du vil ha mer informasjon, kan du se [Konfigurere konverteringstjenesten for bankdata](bank-how-setup-bank-data-conversion-service.md)

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Bankkonti**, og velg deretter den relaterte koblingen.
2. Åpne kortet for en bankkonto som du vil eksportere eller importere bankfiler for.
3. Fyll ut feltene på hurtigfanen **Overføring** etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   Andre fileksporttjenester og formater krever ulike oppsettsverdier i vinduet **Bankkort**. Du blir informert om feil eller manglende oppsettsverdier når du prøver å eksportere filen. Les derfor de korte beskrivelsene av feltene nøye, eller se relaterte fremgangsmåteeemner. Hvis du for eksempel eksporterer en betalingsfil for Nord-Amerika elektronisk pengeoverføring (EFT) krever at både feltet **Nr. for siste remitteringsmelding** og feltet **Transittnr.** er fylt ut. Hvis du vil ha mer informasjon, kan du se [Eksportere betalinger til en bankfil](payables-how-export-payments-bank-file.md).

## <a name="to-set-up-vendor-bank-accounts-for-export-of-bank-files"></a>Opprette dine leverandørbankkonti for import eller eksport av bankfilene
Felt i hurtigafnen **Overføring** i vinduet **Leverandørs bankkort** er relatert til eksport av bankfeeder og filer. Hvis du vil ha mer informasjon, kan du se [Konfigurere tjeneste for konvertering av bankdata](bank-how-setup-bank-data-conversion-service.md) og [Eksportere betalinger til en bankfil](payables-how-export-payments-bank-file.md).

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Leverandører**, og velg deretter den relaterte koblingen.
2. Åpne kortet for en leverandør med en bankkonto som du vil eksportere betalingsbankfiler til.
3. Velg **Bankkonti**-handlingen.
3. I vinduet **Leverandørs bankkort**, i hurtigfanen **Overføring**, fyller du ut feltene etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-the-opening-balance-on-new-bank-accounts"></a>Angi den inngående balansen på nye bankkonti


## <a name="see-also"></a>Se også
[Konfigurere banktjenester](bank-setup-banking.md)  
[Håndtere bankkonti](bank-manage-bank-accounts.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

