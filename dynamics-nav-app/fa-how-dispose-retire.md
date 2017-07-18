---
title: Avhende eller trekke tilbake aktiva
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
ms.openlocfilehash: 795bb23e7c0b46be095b2bbdfe7705b3d7b1e4ee
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-dispose-of-or-retire-fixed-assets"></a>Avhende eller trekke tilbake aktiva
Når du selger eller på annen måte avhender et aktiva, må salgsverdien bokføres for å beregne og registrere tap eller vinning. En salgspost må være den siste posten som bokføres for et aktiva. Du kan bokføre mer enn én salgspost for aktiva som er delvis solgt. Summen av alle bokførte salgsbeløp må være et kreditbeløp.

 **Merk**: Hvis du bytter ut et aktiva med et annet, må du registrere både salget av det gamle aktivaet og innkjøpet av det nye (anskaffelsen). Hvis du vil ha mer informasjon, se [Anskaffe aktiva](fa-how-acquire.md).

## <a name="to-post-a-disposal-from-the-fixed-asset-gl-journal"></a>Slik bokfører du et salg fra aktivafinanskladden:  
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktivafinanskladder** og velger deretter den relaterte koblingen.  
2. Opprett en innledende kladdelinje, og fyll ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
3. I feltet **Aktivabokf.type** velger du **Salg**.
4. Velg **Sett inn aktivamotkonto**. En ny kladdelinje opprettes for motkontoen som er satt opp for salgsbokføring.

    **Merk**: Trinn 4 fungerer bare hvis du har definert følgende: I vinduet **Kort for bokf.grp.- aktiva** for bokføringsgruppen for aktivaet, inneholder **Konto for salg**-feltet finansdebetkontoen og **Motkonto for salg**-feltet inneholder finanskontoen du vil bokføre motposter for oppskrivning til. Hvis du vil ha mer informasjon, kan du se "Definere bokføringsgrupper for aktiva" i [Definere generell aktivainformasjon](fa-how-setup-general.md).
5. Velg handlingen **Bokfør**.

Hvis du selger eller på avhender deler av et aktiva, må du dele opp aktivaet før du kan registrere salgstransaksjonen. Hvis du vil ha mer informasjon, se [Overføre, dele opp eller kombinere aktiva](fa-how-trans-split-combine.md).

## <a name="to-view-disposal-ledger-entries"></a>Slik viser du salgsposter  
Når du selger eller avhender et aktiva, bokføres salgsverdien til finans der du kan se resultatet.   

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktiva** og velger deretter den relaterte koblingen.  
2. Velg aktivaet du vil vise poster for, og velg deretter **Avskrivningstablåer**.
3. Velg avskrivningstablået du vil vise poster for, og velg deretter **Poster**.
4. Velg en linje med **Salg** i **Bokføringskategori, aktiva**-feltet, og velg deretter **Naviger**.  
5. I **Naviger**-vinduet velger du finanspostlinjen og deretter **Vis**.
**Finansposter**-vinduet åpnes der du kan se postene som er resultat av salgsbokføringen.

## <a name="see-also"></a>Se også
[Administrere aktiva](fa-manage.md)  
[Definere aktiva](fa-setup.md)  
[Finans](finance-setup.md)  
[Velkommen til Dynamics NAV](across-get-started.md)

