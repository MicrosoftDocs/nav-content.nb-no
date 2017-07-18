---
title: Arbeide med sjekker
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
ms.openlocfilehash: 421516a7580a90d6eabc8ecfcc841215839994c9
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-checks"></a>Arbeide med sjekker
Dynamics NAV støtter elektronisk og manuell utstedelse av sjekker. Begge metodene bruker utbetalingskladden til å utstede sjekker til leverandører. Du kan også kansellere sjekker og vise sjekkposter.

Prosessen med å utstede sjekker foreslår utbetalinger, oppretter poster og skriver ut de maskinelle sjekkene.

Skriveren må være riktig konfigurert for sjekkskjemaene, og du må definere hvilke sjekkoppsett som skal brukes. Hvis du vil ha mer informasjon, kan du se [Definere sjekkoppsett](finance-setup-how-define-check-layouts.md)

## <a name="to-issue-checks"></a>Utstede sjekker
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Betalingskladder** og velger deretter den relaterte koblingen.
2. Fyll ut kladden med relevante betalinger, for eksempel ved hjelp av funksjonen Betalingsforslag - leverandør. Hvis du vil ha mer informasjon, kan du se [Betalingsforslag - leverandør](payables-how-suggest-vendor-payments.md).
3. I **Bankbetalingstype**-feltet på kladdelinjer for betaling som du vil gjøre med sjekker, velger du ett av følgende alternativer:

 - **Maskinell sjekk**: Velg dette alternativet hvis du vil at programmet skal opprette og senere skrive ut en sjekk på beløpet på betalingskladdelinjen. Du må skrive ut sjekkene før du kan bokføre kladdelinjene. Du kan bare velge **Maskinell sjekk** hvis **Motkontotype** eller **Kontotype** er **Bankkonto**.

 - **Manuell sjekk**: Velg dette alternativet hvis du manuelt har skrevet en sjekk og vil at programmet skal opprette en tilhørende sjekkpost på dette beløpet. Når du bruker dette alternativet, kan du ikke skrive ut sjekker fra Dynamics NAV. Du kan bare velge **Manuell sjekk** hvis **Motkontotype** eller **Kontotype** er **Bankkonto**.

    **Merk**: Du må skrive ut maskinelle sjekkene før du kan bokføre de relaterte kladdelinjene.
4. Velg **Skriv ut sjekk** for maskinelle sjekker.
5. Fyll ut feltene etter behov i vinduet **Sjekk**. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
6. Velg **Skriv ut**.

**Merk**: Hvis du vil skrive ut sjekker i flere valutaer fra forskjellige bankkonti, må du utføre kjørselen **Skriv ut sjekk** separat for hver enkelt valuta og angi riktig bankkonto.

## <a name="to-cancel-printed-checks-that-are-not-posted"></a>Kansellere utskrevne sjekker som ikke er bokført
Du kan kansellere ikke-bokførte sjekker etter at de er skrevet ut, ved hjelp av handlingen **Kanseller sjekk** i vinduet **Betalingskladd**.
1. I vinduet **Betalingskladd** velger du **Kanseller sjekk**, og deretter velger du hvilke sjekker som skal kanselleres.

## <a name="to-void-checks"></a>Kansellere sjekker
Når sjekkbetaliner er bokført, kan du bare kansellere (void) sjekker fra de resulterende bankpostene.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Bankkonti** og velger deretter den relaterte koblingen.
2. Velg relevant bankkonto, velg handlingene **Rediger** og **Sjekkposter**.
3. I vinduet **Sjekkposter** velger du handlingen **Kanseller sjekk**.
4. Merk av for **Kanseller sjekk**.
5. Velg **OK**-knappen.

## <a name="see-also"></a>Se også
[Administrere skyldige beløp](payables-manage-payables.md)  
[Definere bankvesen](bank-setup-banking.md)  

