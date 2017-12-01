---
title: "Anbefalte fremgangsmåter for globalt planleggingsoppsett"
description: Hurtigfanen **Planlegging** i vinduet **Produksjonsoppsett** inneholder flere felt som definerer globale regler for forsyningsplanlegging.
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b6437c809af79c1c0c24126aaa38e6da6120d066
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="setup-best-practices-global-planning-setup"></a>Anbefalte fremgangsmåter for oppsett: Oppsett for global planlegging
Hurtigfanen **Planlegging** i vinduet **Produksjonsoppsett** inneholder flere felt som definerer globale regler for forsyningsplanlegging.  

 Tabellen nedenfor inneholder anbefalte fremgangsmåter for hvordan du konfigurerer valgte globale planleggingsparameterfelt. Hvis du vil ha mer informasjon om et felt, velger du koblingen i kolonnen **Oppsettfelt**.  

|Oppsettfelt|Anbefalt fremgangsmåte|Merknad|  
|-----------------|-------------------|-------------|  
|Bruk prognose på lokasjoner|Velg dette alternativet hvis du har prognoser for bestemte plasseringer.||  
|Komponenter ved lokasjon|Hvis varene ikke er definert som lagerføringsenheter, velger du lokasjonskoden for hovedlageret.|Dette gjelder også hvis du bare bruker bestillingsforslaget.|  
|Tomt overflytnivå|Velg **Tillat standardberegning** hvis du migrerer fra Microsoft Dynamics NAV 5.0 eller tidligere.|Bruk bare hvis du vil tillate at alle eller noen av varene flyter over gjenbestillingspunktet.|  
|Standard avdempingsperiode|Velg mellom 1D og 5D.<br /><br /> Hvis planlegging er nytt for brukerne i [!INCLUDE[d365fin](includes/d365fin_md.md)], angir du en lengre periode.|Når brukere har satt seg bedre inn i de forskjellige årsakene til handlingsmeldinger, kan avdempingsperioden forkortes for å tillate flere endringsforslag.|  
|Standard avdempingsantall|Angi mellom 5 og 20 prosent av varens partistørrelse.||  

## <a name="see-also"></a>Se også  
 [Anbefalte fremgangsmåter for oppsett: Forsyningsplanlegging](setup-best-practices-supply-planning.md)   
 [Designdetaljer: Forsyningsplanlegging](design-details-supply-planning.md)   
 [Konfigurere komplekse moduler ved å bruke anbefalte fremgangsmåter](set-up-complex-application-areas-using-best-practices.md)  
 [Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

