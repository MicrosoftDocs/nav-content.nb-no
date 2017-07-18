---
title: Registrere en nye produkter
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
ms.openlocfilehash: df84a4d3e15035cd956c7612a12069844f5601d2
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-register-new-products"></a>Registrere en nye produkter

Produktene er grunnlaget for virksomheten din, varer eller tjenester som du handler med. Hvert produkt må være registrert som et varekort.

**Merk**: I Dynamics NAV brukes ordet “vare” for å referere til et produkt.

Varekort inneholder informasjonen som er nødvendig for å kjøpe, lagre, selge, levere og gjøre rede for produkter.

Varekortet kan være av typen Beholdning eller Tjeneste for å angi om produktet er en fysisk enhet eller arbeidstidsenhet. Bortsett fra noen av feltene som er relatert til de fysiske aspektene av en vare, fungerer alle felt på et varekort på samme måte for lagervarer og tjenester. Hvis du vil ha mer informasjon om hvordan du selger en vare, kan du se [Selge produkter](sales-how-sell-products.md) eller [Fakturere salg](sales-how-invoice-sales.md).

**Merk**: Hvis det finnes varemaler for ulike varetyper, vises et vindu når du oppretter et nytt kundekort der du kan velge en passende mal. Hvis det bare finnes én varemal, brukes alltid denne malen i nye varekort.

## <a name="to-create-a-new-item-card"></a>Opprette et nytt varekort
1. På Hjem-siden velger du handlingen **Varer** for å åpne listen over eksisterende varer.  
2. I vinduet **Varer** velger du handlingen **Ny**.

    Hvis det bare finnes én varemal, åpnes et nytt varekort med noen felt som er fylt ut med informasjon fra malen.
3. I vinduet **Velg en mal for en ny vare** velger du malen som du vil bruke for det nye varekortet.
4. Velg **OK**-knappen. Det åpnes et nytt varekort med noen felt som er fylt ut med informasjon fra malen.
5. Fortsette med å fylle ut eller endre feltet på varekortet etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.

I hurtigfanen **Salgspriser** kan du vise spesialpriser eller rabatter som skal gis for varen hvis bestemte kriterier oppfylles, for eksempel kunde, minimumsordreantall eller sluttdato. Hver rad representerer en spesialpris eller linjerabatt. Hver kolonne representerer et vilkår som må brukes for å garantere spesialprisen du angir i feltet **Enhetspris**, eller linjerabatten du angir i feltet **Linjerabatt-%**. Hvis du vil ha mer informasjon, kan du se [Registrere avtaler om salgspris, rabatt og betaling](sales-how-record-sales-price-discount-payment-agreements.md).

Varen er nå registrert, og varekortet er klart til å brukes på kjøps- og salgsdokumenter.

Hvis du vil bruke dette varekortet som en mal når du oppretter nye varekort, kan du lagre det som en mal. Hvis du vil ha mer informasjon, kan du se følgende avsnitt:

## <a name="to-save-the-item-card-as-a-template"></a>Lagre varekortet som en mal
1. I vinduet **Varekort** velger du handlingen **Lagre som mal**. **Varemal**  -vinduet åpnes og viser varekortet som en mal.
2. Fyll ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
3. Hvis du vil bruke dimensjoner i maler, velger du handlingen **Dimensjoner**. **Dimensjonsmaler**-vinduet åpnes med alle dimensjonskoder som er definert for varen.
4. Rediger eller angi dimensjonskoder som skal gjelde for nye varekort som opprettes ved hjelp av malen.
5. Når du har fullført den nye varemalen, kan du velge **OK**-knappen.

Varemalen legges til i listen over varemaler, slik at du kan bruke den til å opprette nye varekort.

## <a name="see-also"></a>Se også
  [Håndtere lager](inventory-manage-inventory.md)  
  [Håndtere kjøp](purchasing-manage-purchasing.md)  
  [Håndtere salg](sales-manage-sales.md)

