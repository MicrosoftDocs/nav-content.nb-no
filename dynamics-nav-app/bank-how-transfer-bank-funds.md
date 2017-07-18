---
title: "Overføre bankkapital"
author: SorenGP
ms.custom: na
ms.date: 09/21/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f34bef80c64cbad0a0b20d4d021cefbdc5a1cb64
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-transfer-bank-funds"></a>Overføre bankkapital
Noen ganger har du behov for å overføre av et beløp fra én konto til en annen. Hvis du vil gjøre dette, må du bokføre transaksjonen i finanskladden. Oppgaven varierer avhengig av om bankkontoene bruker samme valuta eller forskjellige valutaer.

## <a name="to-post-a-transfer-between-bank-accounts-with-the-same-currency-code"></a>Bokføre en overføring mellom bankkonti med samme valutakode
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Finanskladd** og velger deretter den relaterte koblingen.
2. På en av kladdelinjene fyller du ut **Bokføringsdato** og **Bilagsnr.** -feltene.
3. Velg **Bankkonto** i **Kontotype**-feltet.
4. I **Kontonummer** -feltet velger du banken du vil overføre midler fra.
5. Angi beløpet som skal overføres i feltet **Beløp**.
6. Velg **Bankkonto** i **Motkontotype**-feltet.
7. I **Motkontonr.** -feltet velger du bankkontoen du vil overføre midler til.
8. Bokfør kladden.

## <a name="to-post-a-transfer-between-bank-accounts-with-different-currency-codes"></a>Slik bokfører du en overføring mellom bankkonti med ulike valutakoder
Hvis du vil overføre midler mellom bankkonti som bruker forskjellige valutaer, må du bokføre to linjer i finanskladden.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Finanskladd** og velger deretter den relaterte koblingen.
2. Opprett to kladdelinjer, og fyll ut **Bokføringsdato** og **Bilagsnr.** -feltene.
3. På den første kladdelinje angir du **Bankkonto** i **Type**-feltet.
4. I **Kontonummer** -feltet velger du bankkontoen du vil overføre midler fra.
5. I **Beløp**-feltet angir du beløpet i valutaen til bankkontoen. Angi kreditbeløp med minus som fortegn. Angi debetbeløp uten minus som fortegn.
6. Velg **Bankkonto** i **Motkontotype**-feltet.
7. I **Motkontonr.** -feltet velger du bankkontoen du vil overføre midler til.
8. På den andre kladdelinje angir du **Bankkonto** i **Type**-feltet.
9. I **Kontonummer** -feltet velger du bankkontoen du vil overføre midler til.
10. I **Beløp**-feltet angir du beløpet i valutaen til bankkontoen. Angi kreditbeløp med minus som fortegn. Angi debetbeløp uten minus som fortegn.
11. Velg **Bankkonto** i **Motkontotype**-feltet.  
12. I **Motkontonr.** -feltet velger du bankkontoen du vil overføre midler fra.

    **Merk**: Hvis valutakursene som brukes i kladden, ikke er de samme som valutakursene i vinduet **Valutakurser**, angir du en tredje linje for agio/disagio. Angi **Finanskonto** i **Kontotype**-feltet. Angi finanskontonummeret for agio eller disagio i **Kontonr.**-feltet. . Angi agio eller disagio i **Beløp**-feltet med eller uten et minustegn for henholdsvis kredit og debet.
13. Bokfør kladden.

## <a name="see-also"></a>Se også  
[Håndtere bankkonti](bank-manage-bank-accounts.md)  
[Definere bankvesen](bank-setup-banking.md)  
[Arbeide med finanskladder](ui-work-general-journals.md)

