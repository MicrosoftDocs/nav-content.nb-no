---
title: Foreta direkte leveringer
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
ms.openlocfilehash: f636de789dc6b006a449ec59c390fab85e62b443
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-make-drop-shipments"></a>Foreta direkte leveringer
En direkte levering er levering av varer fra en av leverandørene dine, direkte til en av kundene dine.

Når en ordre merkes for direkte levering, og du oppretter en bestilling som angir kunden i **Salg til kundenr.**-feltet, kan du koble de to dokumentene og dermed be leverandøren levere direkte til kunden.

## <a name="to-create-a-sales-order-for-drop-shipment"></a>Slik oppretter du en ordre med direkte levering:
Hvis du vil klargjøre en direkte levering, kan du opprette en ordre for en vare som vanlig, bortsett fra at du må vise på salgslinjen at salget krever direkte levering.

1. Opprett en ordre for en vare. Hvis du vil ha mer informasjon, kan du se [Selge produkter](sales-how-sell-products.md).
2. På ordrelinjen for varen for direkte levering, merker du av for **Direkte levering**.

## <a name="to-create-the-purchase-order-for-drop-shipment"></a>Slik oppretter du bestillingen med direkte levering:
Hvis du vil klargjøre en direkte levering for varen som skal selges, oppretter du en bestilling som vanlig, bortsett fra at du må angi på bestillingen at den må leveres til kunden, ikke til deg selv.

1. Opprett en bestilling. Ikke fyll ut noen felt på linjene. Hvis du vil ha mer informasjon, kan du se [Registrere kjøp](purchasing-how-record-purchases.md).
2. I feltet **Salg til-kundenr.** velger du kunden som du selger til.
3. Velg **Direkte levering**-handlingen, og velg deretter **Hent ordre**-handlingen.
4. I **Salgsliste**-vinduet merker du ordren som du har forberedt i "Slik oppretter du en ordre med direkte levering".
5. Velg **OK**-knappen.

Linjeinformasjonen fra ordren settes inn på bestillingslinjene.

Nå kan du angi at leverandøren skal levere varene til kunden, for eksempel, ved å sende bestillingen på e-post som en PDF-fil.     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a>Slik viser du den tilknyttede bestillingen fra ordren:
1. Velg ordrelinjen med direkte levering, velg **Ordre**-handlingen, velg **Direkte levering**-handlingen, og velg deretter **Bestilling**-handlingen.

Den tilknyttede bestillingen åpnes.

## <a name="to-post-a-drop-shipment"></a>Bokføre en direkte levering
Når leverandøren har levert varene, kan du bokføre ordren som levert. Du kan også bokføre bestillingen, men bare med **Motta**-alternativet til ordren er fakturert.
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Ordrer** og velger deretter den relaterte koblingen.
2. Åpne ordren som du laget i "Slik oppretter du en ordre med direkte levering".
3. I **Levere (antall)**-feltet angir du hvor mye av ordreantallet som skal leveres, hele eller deler av ordreantallet.
3. Velg handlingen **Bokfør** eller **Bokfør og send**.
4. Velg **Levere** hvis du vil fakturere senere, eller **Levere og fakturere** hvis du vil fakturere med en gang.

## <a name="see-also"></a>Se også
[Selge produkter](sales-how-sell-products.md)    
[Registrere kjøp](purchasing-how-record-purchases.md)  
[Håndtere salg](sales-manage-sales.md)  
[Håndtere lager](inventory-manage-inventory.md)      
[Arbeide med Dynamics NAV](ui-work-product.md)

