---
title: Registrere nye kunder
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 191a9d0b38425c2e36400050afa4fa89ccd2556a
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-register-new-customers"></a>Registrere nye kunder
Kunder er kilden til dine inntekter. Hver kunde du selger til, må være registrert som et kundekort.

Før du kan registrere nye kunder, må du definere forskjellige salgskoder som du kan velge fra når du fyller ut kundekort. Hvis du vil ha mer informasjon, kan du se [Definere salg](sales-setup-sales.md).

Kundekort inneholder informasjonen som er nødvendig for å selge produkter til kunden. Hvis du vil ha mer informasjon, kan du se [Fakturere salg](sales-how-invoice-sales.md) og [Registrere nye produkter](inventory-how-register-new-products.md).

**Merk**: Hvis det finnes kundemaler for ulike kundetyper, vises et vindu når du oppretter et nytt kundekort der du kan velge en passende mal. Hvis det bare finnes én kundemal, brukes alltid denne malen i nye kundekort.

## <a name="to-create-a-new-customer-card"></a>Opprette et nytt kundekort
1. På Hjem-siden velger du handlingen **Kunder** for å åpne listen over eksisterende kunder.  
2. I vinduet **Kunder** velger du handlingen **Ny**.

    Hvis det bare finnes én kundemal, åpnes et nytt kundekort med noen felt som er fylt ut med informasjon fra malen.

    Hvis det finnes mer enn én kundemal, åpnes et vindu der du kan velge en kundemal. I det tilfellet følger du de to neste trinnene.
3. I vinduet **Velg en mal for en ny kunde** velger du malen som du vil bruke for det nye kundekortet.
4. Velg **OK**-knappen. Det åpnes et nytt kundekort med noen felt som er fylt ut med informasjon fra malen.  
5. Fortsette med å fylle ut eller endre feltet på kundekortet etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.

I hurtigfanen **Salgspriser** kan du vise spesialpriser eller rabatter som skal gis til kunden hvis bestemte kriterier oppfylles, for eksempel vare, minimumsordreantall eller sluttdato. Hver rad representerer en spesialpris eller linjerabatt. Hver kolonne representerer et vilkår som må brukes for å garantere spesialprisen du angir i feltet **Enhetspris**, eller linjerabatten du angir i feltet **Linjerabatt-%**. Hvis du vil ha mer informasjon, kan du se [Registrere avtaler om salgspris, rabatt og betaling](sales-how-record-sales-price-discount-payment-agreements.md).

Kunden er nå registrert, og kundekortet er klart til å brukes på salgsdokumenter.

Hvis du vil bruke dette kundekortet som en mal når du oppretter nye kundekort, kan du lagre det som en mal. Hvis du vil ha mer informasjon, kan du se følgende avsnitt:

## <a name="to-save-the-customer-card-as-a-template"></a>Lagre kundekortet som en mal
1. I vinduet **Kundekort** velger du handlingen **Lagre som mal**. **Kundemal**  -vinduet åpnes og viser kundekortet som en mal.
2. Fyll ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
3. Hvis du vil bruke dimensjoner i maler, velger du handlingen **Dimensjoner**. **Dimensjonsmaler**-vinduet åpnes med alle dimensjonskoder som er definert for kunden.
4. Rediger eller angi dimensjonskoder som skal gjelde for nye kundekort som opprettes ved hjelp av malen.  
5. Når du har fullført den nye kundemalen, kan du velge **OK**-knappen.

Kundemalen legges til i listen over kundemaler, slik at du kan bruke den til å opprette nye kundekort.

## <a name="see-also"></a>Se også  
[Håndtere salg](sales-manage-sales.md)    
[Definere salg](sales-setup-sales.md)    
[Arbeide med Dynamics NAV](ui-work-product.md)

