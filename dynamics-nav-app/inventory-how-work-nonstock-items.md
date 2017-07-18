---
title: Arbeide med katalogvarer
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
ms.openlocfilehash: 2b49d95904732dcf091fd060a96006fdcb477ec1
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-nonstock-items"></a>Arbeide med katalogvarer
Du kan tilby bestemte varer til kundene for å gjøre det mer bekvemmelig for dem, som du ikke vil ha på lager før du begynner å selge dem. Når du vil begynne å ha slike varer på lager, kan du konvertere dem til vanlige varekort på to måter.

- Fra et katalogvarekort kan du opprette et nytt varekort basert på en mal.
- Fra en salgsordrelinje med et tomt **Vare**-felt, velger du en katalogvare. Når du bokfører salget, opprettes det automatisk et varekort for katalogvaren.

**Merk**: Du kan ikke velge en katalogvare fra **Salgsfaktura**-vinduet. Du kan velge en katalogvare fra **Tilbud**-vinduet, men katalogvaren vil ikke bli konvertert til en vanlig vare når du bruker **Lag ordre**-funksjonen.

En katalogvare har vanligvis varenummeret til leverandøren som leverer den. For å gjøre det mulig å konvertere et katalogvarekort til et vanlig varekort, må du først definere hvordan varenummerering for leverandør skal konverteres til din egen varenummerering.   

## <a name="to-create-a-nonstock-item"></a>Slik oppretter du en katalogvare:
Katalogvarekort har mye mindre informasjon enn vanlige varekort fordi du bare bruker dem til tilbud i salgstilbud og på andre måter. Derfor må de konverteres til vanlige varekort før du kan bokføre salgstransaksjoner for dem.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Katalogvarer** og velger deretter den relaterte koblingen.
2. Velg handlingen **Ny**.
2. Fyll ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.

## <a name="to-set-up-how-nonstock-item-numbers-are-converted-to-your-own-numbering"></a>Slik definerer du hvordan katalogvarenumre konverteres til din egen nummerering:  
For å gjøre det mulig å konvertere et katalogvarekort til et vanlig varekort, må du først definere hvordan varenummereringen for leverandøren skal konverteres til ditt eget varenummereringsformat.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Katalogvare - oppsett** og velger deretter den relaterte koblingen.
2. Fyll ut feltene etter behov.

## <a name="to-convert-a-nonstock-item-to-a-normal-item"></a>Slik konverterer du en katalogvare til en vanlig vare:
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Katalogvarer** og velger deretter den relaterte koblingen.
2. Åpne kortet for katalogvaren som du vil konvertere til en vanlig vare.
3. I vinduet **Kort for katalogvare** velger du handlingen **Opprett vare**.

Et nytt varekort forhåndsutfylt med informasjon fra katalogvaren og en relevant varemal opprettes. Du kan deretter fylle ut eller redigere felt på det nye varekortet etter behov. Hvis du vil ha mer informasjon, kan du se [Registrere nye produkter](inventory-how-register-new-products.md).

## <a name="to-sell-a-nonstock-item-and-convert-it-to-a-normal-item"></a>Slik selger du en katalogvare og konverterer den til en vanlig vare:
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Ordrer** og velger deretter den relaterte koblingen.
2. Velg handlingen **Ny**. Fyll ut feltene på hurtigfanen **Generelt** som for ordrer.
3. På en ny salgslinje lar du **Vare**-feltet stå tomt, velger **Linje**, **Funksjoner**, og velger deretter **Katalogvarer**.

    Katalogvaren konverteres til en vanlig vare. Et nytt varekort forhåndsutfylt med informasjon fra katalogvaren og en relevant varemal opprettes.
4. I **Katalogvarer**-vinduet velger du katalogvaren du vil selge, og velger deretter **OK**-knappen.
5. Når ordren er fullført, kan du velge handlingen **Bokfør**.

Du kan deretter fylle ut eller redigere felt på det nye varekortet etter behov. Hvis du vil ha mer informasjon, kan du se [Registrere nye produkter](inventory-how-register-new-products.md).

**Merk**: En varekryssreferansepost opprettes automatisk for leverandøren av varen mellom leverandørens varenummer og det nye varenummeret ditt.

## <a name="see-also"></a>Se også
[Registrere en nye produkter](inventory-how-register-new-products.md)  
[Håndtere lager](inventory-manage-inventory.md)  
[Arbeide med Dynamics NAV](ui-work-product.md)

