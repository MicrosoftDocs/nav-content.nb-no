---
title: "Lese inn lønnstransaksjoner"
author: SorenGP
ms.custom: na
ms.date: 09/29/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: d5e70a0a1659c7facdeec3f0971eda43ff8a03cc
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-import-payroll-transactions"></a>Lese inn lønnstransaksjoner
For å ta høyde for lønnsutbetalinger og relaterte transaksjoner, må du importere og bokføre finansielle transaksjoner som er utført av lønnssystemet til Finans. Hvis du vil gjøre dette, importerer du først en CSV-fil. filen som du mottar fra lønnssystemet til vinduet **Finanskladd**. Deretter tilordner du eksterne kontoer i lønnsfilen til de relevante finanskontiene. Til slutt kan du bokføre lønnstransaksjoner etter kontotilordningen.

## <a name="to-import-a-payroll-file"></a>Slik importerer du en lønnsfil
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Finanskladder** og velger deretter den relaterte koblingen.
2. I den aktuelle finanskladden velger du handlingen **Importer lønnstransaksjoner**.
3. I vinduet **Importer** velger du den aktuelle lønnsfilen, og deretter velger du **OK**-knappen. Filen må være i CSV-format. 
4. Følg trinnene i vinduet **Importer lønnstransaksjoner** for å importere transaksjoner og tilordne forretningsforbindelser, og velg deretter **Fullfør**.

    Økonomijournalen er fylt med linjer som representerer transaksjoner der lønnsfilen og relevante kontiene i kolonnen **Finanskonto**.
4. Rediger eller bokfør kladdelinjene som for andre transaksjoner i Finans. Hvis du vil ha mer informasjon, kan du se [Arbeide med finanskladder](ui-work-general-journals.md).   

## <a name="see-also"></a>Se også
[Finans](finance-setup.md)  
[Arbeide med finanskladder](ui-work-general-journals.md)  

