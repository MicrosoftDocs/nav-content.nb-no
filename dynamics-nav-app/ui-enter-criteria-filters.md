---
title: "Angi vilkår i filtre"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 8eab393a0a77f9f1595ca1247c7549e68b491cb2
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="entering-criteria-in-filters"></a>Angi vilkår i filtre
Når du vil søke etter data, for eksempel kundenavn, adresser eller produktgrupper, må du angi kriterier. I søkekriteriene kan du bruke alle tallene og bokstavene du vanligvis kan bruke i det spesifikke feltet. I tillegg til dette kan du bruke spesielle symboler til å filtrere resultatene ytterligere.

## <a name="searching-using-the-quick-filter"></a>Søke ved hjelp av hurtigfilteret
Du kan legge til filtre på alle sider ved hjelp av hurtigfilteret. Hurtigfilteret aktiveres ved å velge forstørrelsesikonet i øvre høyre hjørne på siden. Denne filtreringstypen brukes for rask angivelse av kriterier.

**Viktig**: Hurtigfilteret gjør det enkelt å filtrere data ved å skrive inn ren tekst, men gir også mange alternativer når det gjelder søkekriterier. Virkemåten for hurtigfilteret er avhengig av om du skriver inn ren tekst eller tekst som inneholder symboler.  
- Hvis du skriver inn ren tekst i søkevilkåret, tolkes søkekriteriene som et søk som ikke skiller mellom store og små bokstaver og som inneholder en bestemt tekst.  
- Hvis du skriver inn tekst med symboler i søkekriteriene, tolkes søkekriteriene nøyaktig slik du skrev det inn, og søket skiller mellom store og små bokstaver.

### <a name="quick-filter-criteria"></a>Kriterier for hurtigfilter
<!-- html syntax because symbols conflict with MarkDown syntax -->
<TABLE>
  <TR>
    <TH>Søkekriterier</TH>
    <TH>Tolkes som ...</TH>
    <TH>Returnerer ...</TH>
  </TR>
  <TR>
    <TD>>man</TD>
    <TD>@*man*</TD>
    <TD>Alle poster som inneholder teksten mann og som ikke skiller mellom små og store bokstaver.</TD>
  </TR>
  <TR>
    <TD>>se</TD>
    <TD>@*se*</TD>
    <TD>Alle poster som inneholder teksten se og som ikke skiller mellom små og store bokstaver.</TD>
  </TR>
  <TR>
    <TD>>Man*</TD>
    <TD>Begynner med Man, og skiller mellom små og store bokstaver.</TD>
    <TD>Alle poster som starter med teksten Man.</TD>
  </TR>
  <TR>
    <TD>'man'</TD>
    <TD>En nøyaktig tekst som skiller mellom små og store bokstaver.</TD>
    <TD>Alle poster som samsvarer nøyaktig med man.</TD>
  </TR>
  <TR>
    <TD>@*man</TD>
    <TD>Slutter med, og skiller ikke mellom små og store bokstaver.</TD>
    <TD>Alle poster som slutter med man.</TD>
  </TR>
  <TR>
    <TD>@man*</TD>
    <TD>Begynner med, og skiller ikke mellom små og store bokstaver.</TD>
    <TD>Alle poster som starter med man.</TD>
  </TR>
</TABLE>

**Merk**: Du kan ikke bruke et jokertegn når du filtrerer på felt for opplisting, for eksempel feltet **Status** i salgsordrer. Hvis du vil angi et filter for denne typen felt, kan du angi den numeriske verdien som en parameter for filtrering. I feltet **Status** på en ordre som har verdiene **Åpen**, **Frigitt**, **Venter på godkjenning** og **Venter på forskudd**, må du bruke verdiene **0**, **1**, **2** og **3** for å filtrere etter disse alternativene.  

## <a name="see-also"></a>Se også
[Arbeide med Dynamics NAV](ui-work-product.md)

