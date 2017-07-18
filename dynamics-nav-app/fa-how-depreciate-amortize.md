---
title: Avskrive eller amortisere aktiva
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
ms.openlocfilehash: af71f30681d436ed5da1cd6cb3c2e13f86558631
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-depreciate-or-amortize-fixed-assets"></a>Avskrive eller amortisere aktiva
Avskrivning brukes til å fordele aktivakostnader, for eksempel maskiner og utstyr, over den avskrivningsberettigede levetiden til aktivaet. Du må definere hvordan du vil at hvert enkelt aktiva skal avskrives.  

 Det finnes to måter å bokføre avskrivninger på:
- Automatisk, ved å utføre kjørselen **Beregn avskrivning**.
- Manuelt, ved hjelp av aktivafinanskladden.  

Dynamics NAV kan beregne daglig avskrivning slik at du kan beregne avskrivninger for en hvilken som helst periode. Du kan derfor analysere gjeldende operasjonsresultater på for eksempel månedlig, kvartalsvis eller årlig basis. Beregningen bruker et standardår på 360 dager og en standardmåned på 30 dager. Hvis du vil ha mer informasjon, kan du se [Avskrivningsmetoder](fa-depreciation-methods.md).

Hvis flere avdelinger bruker det samme aktivaet, kan periodisk avskrivning automatisk fordeles til disse avdelingene, etter en brukerdefinert fordelingstabell.  

Du kan kansellere feil avskrivningsposter med kjørselen **Kanseller aktivaposter**. Deretter kan du bokføre det riktige avskrivningsbeløpet ved å utføre kjørselen **Beregn avskrivning** på nytt. Når du retter feil, bokføres feilene som aktivafeilposter.  

Indeksregulering brukes til å justere verdier for generelle endringer i prisnivået. Du bruker kjørselen **Indeksreg. aktiva** til å beregne avskrivningsbeløpene på nytt.  

## <a name="to-calculate-a-depreciation-automatically"></a>Slik beregner du en avskrivning automatisk:
Du kan utføre kjørselen **Beregn avskrivninger** én gang i måneden, eller etter behov. Aktiva som er solgt, aktiva som er sperret eller inaktive, og aktiva som bruker den manuelle avskrivningsmetoden, ignoreres.    

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Beregn avskrivninger** og velger deretter den relaterte koblingen.  
2. Fyll ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
3. Velg **OK**-knappen.  

    Kjørselen beregner avskrivningen og oppretter linjer i aktivafinanskladden.  
4. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktivafinanskladder** og velger deretter den relaterte koblingen.

    I vinduet **Aktiva finanskladd** i **Antall avskrivningsdager**-feltet kan du se hvor mange avskrivningsdager det er beregnet.  
5. Velg handlingen **Bokfør**.

## <a name="to-post-a-depreciation-manually-from-the-fixed-asset-gl-journal"></a>Slik bokfører du en avskrivning manuelt fra aktivafinanskladden:
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktivafinanskladd** og velger deretter den relaterte koblingen.  
2. Opprett en innledende kladdelinje, og fyll ut feltene etter behov.
3. I feltet **Aktivabokf.type** velger du **Avskrivning**.
4. Velg **Sett inn aktivamotkonto**. En ny kladdelinje opprettes for motkontoen som er satt opp for bokføring av avskrivning. Hvis du vil ha mer informasjon, kan du se "Definere bokføringsgrupper for aktiva" i [Definere generell aktivainformasjon](fa-how-setup-general.md).
5. I fanebladet **Hjem** velger du **Bokfør** for å bokføre kladden.

Hvis du har definert aktivafordelingsnøkler for å fordele beløp på ulike avdelinger eller prosjekter, vil beløpene fordeles under bokføringen. Se [Definere generell aktivainformasjon](fa-how-setup-general.md) for mer informasjon.

## <a name="to-calculate-allocations-in-the-fixed-asset-gl-journal"></a>Slik beregner du fordelinger i aktivafinanskladden:
Hvis flere avdelinger bruker det samme aktivaet, kan periodisk avskrivning automatisk fordeles til disse avdelingene, etter en brukerdefinert fordelingstabell.  

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktivafinanskladd** og velger deretter den relaterte koblingen.   
Opprett en innledende linje, og fyll ut feltene etter behov.
3. I feltet **Aktivabokf.type** velger du **Fordeling**.
4. Velg **Sett inn aktivamotkonto**. En ny kladdelinje opprettes for motkontoen som er satt opp for fordelingsbokføring.
5. I fanebladet **Hjem** velger du **Bokfør** for å bokføre kladden.

## <a name="use-duplication-lists-to-prepare-to-post-to-multiple-depreciation-books"></a>Bruke duplikatoversikter til å forberede bokføring av flere avskrivningstablåer  
Når du fyller ut kladdelinjer som skal bokføres i et avskrivningstablå, kan du duplisere linjene i en separat kladd der de etterpå kan bokføres i et annet avskrivningstablå. Hvis du vil ha mer informasjon, kan du se "Slik bokfører du poster i ulike avskrivningstablåer".

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Avskrivningstablåer** og velger deretter den relaterte koblingen.  
2. Åpne det aktuelle avskrivningstablået, og merk deretter av for **Del av duplikasjonsoversikt**.  

**Viktig**: Hvis du har valgt feltet **Bruk duplikatoversikt**, må du ikke bruke nummerserier på kladden. Årsaken er at nummerserien for aktivafinanskladden ikke samsvarer med nummerserien for aktivakladden.

## <a name="to-post-entries-to-different-depreciation-books"></a>Slik bokfører du poster i ulike avskrivningstablåer  
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktivafinanskladd** og velger deretter den relaterte koblingen.
2. I kladden du vil bokføre avskrivning med, merker du av for **Bruk duplikatoversikt**.
3. Fyll ut feltene som gjenstår etter behov.
4. Velg handlingen **Bokfør**.
5. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktivakladder** og velger deretter den relaterte koblingen.

    **Aktivakladd**-vinduet inneholder nye linjer for ulike avskrivningstablåer i henhold til duplikatoversikten.   

6. Se gjennom eller rediger linjene, og velg deretter **Bokfør**.

**Merk**: Du kan også duplisere en post i et separat tablå ved å angi koden for avskrivningstablået i feltet **Duplikat i avskrivningstablå**, når du fyller ut en kladdelinje.

Du kan kopiere poster fra ett avskrivningstablå til et annet med kjørselen **Kopier avskrivningstablå**. Kjørselen oppretter kladdelinjer i kladden du har angitt i vinduet **Aktivakladdoppsett** for avskrivningstablået du vil kopiere til. Hvis du vil ha mer informasjon, kan du se følgende fremgangsmåte:

## <a name="to-copy-fixed-asset-ledger-entries-between-depreciation-books"></a>Slik kopierer du aktivaposter mellom avskrivningstablåer:  
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Avskrivningstablåer** og velger deretter den relaterte koblingen.
2. Åpne det aktuelle avskrivningstablåkortet, og velg deretter **Kopier avskrivningstablå**.  
3. I vinduet **Kopier avskrivningstablå** fyller du ut feltene etter behov.  
4. Velg **OK**-knappen.  

De kopierte linjene opprettes enten i aktivafinanskladden eller i aktivakladden, avhengig av om avskrivningstablået du kopierer, er integrert med Finans.

## <a name="see-also"></a>Se også
[Administrere aktiva](fa-manage.md)  
[Definere aktiva](fa-setup.md)  
[Finans](finance-setup.md)  
[Velkommen til Dynamics NAV](across-get-started.md)

