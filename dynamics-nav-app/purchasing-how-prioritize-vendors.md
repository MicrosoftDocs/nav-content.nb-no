---
title: "Tilordne et prioritetsnivå til en leverandør"
description: "Du kan tilordne numre til leverandørene for å prioritere dem og forenkle betalingsforslag i Dynamics NAV."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supplier, payment priority
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 79458c1372c9f696a8331f2e7c83179dd42fb905
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-prioritize-vendors"></a>Prioritere leverandører
[!INCLUDE[d365fin](includes/d365fin_md.md)] kan foreslå ulike utbetalinger til leverandører, for eksempel betalinger som snart forfaller eller betalinger hvor en rabatt er tilgjengelig. Hvis du vil ha mer informasjon, kan du se [Betalingsforslag - leverandør](payables-how-suggest-vendor-payments.md).

Først må du prioritere leverandørene ved å tilordne numre til dem.

## <a name="to-prioritize-vendors"></a>Slik prioriterer du leverandører
1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Leverandører**, og velg deretter den relaterte koblingen.
2. Velg den aktuelle leverandøren, og velg deretter **Rediger**.
3. Angi et tall i feltet **Prioritet**.

[!INCLUDE[d365fin](includes/d365fin_md.md)] vurderer det laveste tallet, unntatt 0, til å ha høyest prioritet. Hvis du for eksempel bruker 1, 2 og 3, har 1 høyeste prioritet.

Hvis du ikke vil prioritere en leverandør, lar du feltet **Prioritet** stå tomt. Når du deretter bruker funksjonen for betalingsforslag, vises leverandøren i oversikten etter alle leverandørene som har et prioritetsnummer. Du kan angi et ubegrenset antall prioritetsnivåer.

## <a name="see-also"></a>Se også
[Definere kjøp](purchasing-setup-purchasing.md)  
[Administrere skyldige beløp](payables-manage-payables.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

