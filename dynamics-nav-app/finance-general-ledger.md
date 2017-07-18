---
title: "Økonomimodulen og kontoplanen"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 9965ddcad214e97c5e4858824395d6f651b3c003
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="the-general-ledger-and-the-chart-of-accounts"></a>Økonomimodulen og kontoplanen
Økonomimodulen lagrer dine økonomiske data, og kontoplanen viser kontoene som alle finansposter bokføres til. Dynamics NAV inneholder en standard kontoplan som er klar til å støtte forretningsvirksomheten din.

## <a name="general-ledger-setup-and-general-posting-setup"></a>Finansoppsett og generelt bokføringsoppsett
Økonomimodulen er kjernen av forretningsprosessene og konfigurasjonen av hvordan dataene posteres til økonomimodulen.
I vinduet **Finansoppsett** angir du hvordan du håndterer bestemte regnskapssaker i firmaet. Dette inkluderer for eksempel detaljopplysninger om fakturaavrunding, adresseformater og om du vil bruke en tilleggsrapporteringsvaluta.
I vinduet **Generelt bokføringsoppsett** angir du hvordan du vil definere kombinasjoner av firma- og varebokføringsgrupper. Fyll ut en linje for hver kombinasjon av firma- og varebokføringsgrupper.  

## <a name="the-chart-of-accounts"></a>Kontoplanen
Kontoplanen viser alle kontoer. Herfra kan du åpne ulike rapporter som viser finansposter og saldoer, og du kan avslutte resultatregnskapet. For hver konto kan du åpne finanskortet og legge til eller endre innstillinger. Du kan også vise en liste over bokføringsgrupper som du posterer til kontoen.  

Dynamics NAV hindrer deg i å slette en finanskonto som lagrer data som er nødvendige i kontoplanen.  

## <a name="account-categories"></a>Kontokategorier
Med kontokategorier kan du tilordne finanskontoer til kategoriene som en personlig tilpasning av strukturen i kontoutskrifter.  

Vinduet **Finanskontokategorier** viser eksisterende hovedkategorier og underkategorier og finanskonti som du har tilordnet hver kategori. Du kan opprette nye underkategorier og tilordne disse kategoriene til eksisterende kontoer.  

Du kan gruppere kontokategoriene ved å rykke inn individuelle underkategorier. Dette gjør det enkelt for deg å få en oversikt, fordi hver gruppering viser den totale saldoen. Du kan for eksempel opprette underkategorier for ulike typer aktiva, og deretter opprette kategorigrupper for anleggsmidler kontra omløpsmidler. Du kan opprette en kategorigruppe ved å rykke inn andre underkategorier under en linje i vinduet **Finanskontokategorier**.  

For hver underkategori kan du angi om kontoer i denne kategorien skal inkluderes i bestemte typer finansrapporter. Kontokategoriene bidra til å definere oppsettet for regnskapsoppgjør. Standard saldoutdrag har for eksempel én enkelt oppføring for kontanter under aktiva. Hvis du vil at saldoutdraget skal ha underoppføringene for håndkasse og sjekkontoen, kan du legge til to nye underkategorier, angi rapportdefinisjonen Kontantkontoer for hver av dem, og rykker dem inn under underkategorien Kontanter. Når du har generert kontokontoskjemaer basert på endringene, vil det neste utdraget deretter vise en total saldo for kontanter og to linjer med saldoer for håndkasse og sjekkontoen.     

##<a name="see-also"></a>Se også
[Finans](finance-setup.md)  
[Definere eller endre kontoplanen](finance-setup-setup-chart-accounts.md)  
[Kontoskjemaer](finance-setup-account-schedule.md)  

