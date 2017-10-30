---
title: Definere dokumentutskrift
description: "I [!INCLUDE[navnow](../../includes/navnow_md.md)] kan du skrive ut salgsrapportene som bruker de nødvendige girospesifikasjonene, ved bruk av forskjellige papirtyper og -skuffer."
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
ms.openlocfilehash: 435c7f029d525526fb3e0af505dfb85c1fc0aa2d
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-document-printing"></a>Definere dokumentutskrift
I [!INCLUDE[navnow](../../includes/navnow_md.md)] kan du skrive ut salgsrapportene som bruker de nødvendige girospesifikasjonene, ved bruk av forskjellige papirtyper og -skuffer.  

Du må vurdere hvordan skriveren og skriverdriveren tolker denne informasjonen når du bruker skuffnumre og papirkilder for norske salgsdokumenter. Du må kanskje angi andre skuffnumre for din spesifikke skriver.  

> [!NOTE]  
>  KID-informasjon skrives også ut der giroopplysningene skrives ut.  

Følgende dokumenter krever en utskrevet giro:  

- Fakturaer  
- Kreditnotaer  
- Rentenotaer  
- Purringer  

Den norske versjonen av [!INCLUDE[navnow](../../includes/navnow_md.md)] inneholder følgende sett med salgsdokumenter.  

|**Valg**|Description|  
|-------------|---------------------------------------|  
|1|Standard [!INCLUDE[navnow](../../includes/navnow_md.md)]-dokumenter. Ingen giroinformasjon skrives ut.|  
|2|Giroen skrives ut på hver side. Den siste siden skriver ut girosummen.|  

## <a name="to-set-up-paper-trays"></a>Slik definerer du papirskuffer:  

1.  Velg ikonet ![Søk etter side eller rapport](../../media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Skrivervalg**, og velg deretter den relaterte koblingen.  
2.  Velg rapporten.  
3.  Velg handlingen **Salgsdok.arkskuff - oppsett**.  
4.  Velg en papirkilde i **Første side - papirkilde**-feltet.  
5.  Feltet **Første side - skuffnr.** viser automatisk den valgte papirkilden. Du kan også angi et skuffnummer manuelt.  

    > [!IMPORTANT]  
    >  Ikke alle skrivere har samme papirkildenavn. Du kan angi et nummer i feltet **Skuffnr.**. Nummeret kan tilsvare en papirkilde. Du finner nummeret som en bestemt skriver bruker, i den tekniske dokumentasjonen for skriveren.  

    Feltet **Andre sider** og **Giroside** defineres på samme måte.  

6.  Velg **OK**.  

## <a name="see-also"></a>Se også  
 [Papirkilder og skuffnumre](paper-sources-and-tray-numbers.md)   
 [Norsk giro og OCR-B-skrift](norwegian-giro-and-ocr-b-font.md)   
 [Opprette KID-numre for salgsdokumenter](how-to-set-up-kid-numbers-on-sales-documents.md)

