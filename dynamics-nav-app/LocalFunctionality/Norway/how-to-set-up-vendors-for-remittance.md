---
title: "Angi leverandører for remittering"
description: "Forbedringer i den norske versjonen inkluderer automatisk betaling til leverandører. Dette reduserer sjansen for at feil skal oppstå på grunn av manuell registrering av data. Du må angi leverandørinformasjon for å betale leverandører ved hjelp av remitteringssystemet."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 59e27dab8e933e126d185036ce943c708b55b46b
ms.contentlocale: nb-no
ms.lasthandoff: 10/26/2017

---
# <a name="how-to-set-up-vendors-for-remittance"></a>Angi leverandører for remittering
[!INCLUDE[navnow](../../includes/navnow_md.md)]inkluderer forbedringer i den norske versjonen for automatisk betaling til leverandører. Dette reduserer sjansen for at feil skal oppstå på grunn av manuell registrering av data. Du må angi leverandørinformasjon for å betale leverandører ved hjelp av remitteringssystemet.  

## <a name="to-set-up-a-vendor-for-remittance"></a>Slik angir du en leverandør for remittering  

1.  Velg ikonet ![Søk etter side eller rapport](../../media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Leverandører**, og velg deretter den relaterte koblingen.  
2.  Velg handlingen **Rediger**.  
3.  I hurtigfanen **Generelt** fyller du ut feltene som beskrevet i tabellen nedenfor.  

    |Felt|Description|  
    |---------------------------------|---------------------------------------|  
    |**Navn**|Angi leverandørens navn. Dette feltet benyttes ved remittering mot Bankenes Betalingssentral (BBS).|  
    |**Adresse**|Angi leverandørens adresse. Dette feltet benyttes ved remittering mot BBS.|  
    |**Adresse 2**|Angi en tilleggslinje for adressen til leverandøren, om nødvendig. Dette feltet benyttes ved remittering mot BBS.|  
    |**Postnummer**|Angi et gyldig postnummer med fire sifre for remittering innenlands.|  
    |**Lands-/regionkode**|Angi en gyldig lands-/regionkode for en utenlandsk adresse.|  

4.  I hurtigfanen **Betalinger** fyller du ut feltene som beskrevet i tabellen nedenfor.  

    |Felt|Description|  
    |---------------------------------|---------------------------------------|  
    |**Remittering**|Velg dette alternativet hvis leverandøren skal remitteres.|  
    |**Remitteringskontokode**|Angi kontokoden som skal benyttes for leverandøren.|  
    |**Mottaker bankkontonr.**|Angi bankkontonummeret som skal benyttes ved remittering til leverandøren.|  

5.  Velg handlingen **Remitteringsopplysninger**.  
6.  I hurtigfanen **Generelt** fyller du ut feltene som beskrevet i tabellen nedenfor.  

    |Felt|Description|  
    |---------------------------------|---------------------------------------|  
    |**Remitteringskontokode**|Angi koden til remitteringskontoen som benyttes av leverandøren.|  
    |**Remitteringsavtalekode**|Angi koden for avtalen som kontoen er koblet til.|  
    |**Mottaker bankkontonr.**|Angi leverandørens kontonummer som benyttes ved remittering.|  

7.  I hurtigfanen **Innland** fyller du ut feltene som beskrevet i tabellen nedenfor.  

    |Felt|Description|  
    |---------------------------------|---------------------------------------|  
    |**Egen leverandør mottakerref.**|Velg dette alternativet for å benytte mottakerreferansen fra leverandøren.|  
    |**Mottakerref. 1-- fakt.**|Skriv inn teksten som skal skrives ut på betalingsfakturaen.|  
    |**Mottaker ref. 1 - kred.**|Skriv inn teksten som skal skrives ut på betalingsfakturaen ved fradrag av en kreditnota.|  

    Hvis du benytter remittering til BBS, vises teksten fra **Mottakerref. - fakt.** og **Mottakerref. - kred.** på betalingsspesifikasjonen på linje én til tre, kolonne én og to. Du kan sette inn opptil 80 tegn i spesifikasjon av betaling.  

    Teksten i mottakerreferansefeltene kan formateres automatisk ved hjelp av spesielle koder. Se [Referansekoder for mottaker](recipient-reference-codes.md) for mer informasjon.  

8.  I hurtigfanen **Betaling utland** fyller du ut feltene som beskrevet i tabellen nedenfor.  

    |Felt|Description|  
    |---------------------------------|---------------------------------------|  
    |**Mottakerref. utland**|Skriv inn teksten som skal skrives ut på betalingsfakturaen.|  
    |**Varslingsanvisninger**|Velg ett av følgende alternativer for å angi hvordan en varslingsanvisning skal sendes fra mottakerens bank til mottakeren.<br /><br /> -   **Ingen** - ingen bekreftelse sendes.<br />-   **Telefon** - bekreftelse gis via telefon.<br />-   **Faks** - bekreftelse sendes på faks.<br />-   **Annet** - en tekstmelding vises i feltet **Advarseltekst**.|  
    |**Advarseltekst**|Angir advarselsteksten som skal brukes hvis du har angitt **Annet** i feltet **Varslingsanvisninger**.|  
    |**Mottakerbekreftelse**|Velg dette alternativet for å angi hvordan betalingsbekreftelsen sendes til mottakeren.|  
    |**Lands-/regionkode for teleks**|Angi lands-/regionkoden hvis bekreftelsen sendes via teleks.|  
    |**Teleks/telefaksnr.**|Angi teleks- eller faksnummer hvis bekreftelsen sendes via teleks eller faks.|  
    |**Mottakerkontakt**|Angi navnet på kontaktpersonen hvis en teleks- eller faksbekreftelse sendes til mottakeren.|  
    |**Omkostninger innland**|Angi hvem som belastes omkostninger innenlands i forbindelse med betalingen.<br /><br /> -   **Belastes avsender** - avsenderen belastes.<br />-   **Belastes mottaker** - mottakeren belastes.<br />-   **Standard** - banken avgjør hvem som belastes. Vanligvis blir dette avsenderen.|  
    |**Omkostninger utland**|Angi hvem som belastes for betalinger utland.<br /><br /> -   **Belastes avsender** - avsenderen belastes.<br />-   **Belastes mottaker** - mottakeren belastes.<br />-   **Standard** - banken avgjør hvem som belastes. Vanligvis blir dette avsenderen.|  
    |**Betalingsartkode utland**|Skriv inn en tosifret kode for betalingstypen.|  
    |**Spesifikasjon (Norges Bank)**|Angi informasjon for sentralbanken i landet. Kontakt banken din for å få mer informasjon.|  

9. I hurtigfanen **Bank utenlands** fyller du ut feltene som beskrevet i tabellen nedenfor.  

    |Felt|Description|  
    |---------------------------------|---------------------------------------|  
    |**SWIFT**|Angi SWIFT-adressen (Society for Worldwide Interbank Financial Telecommunication) som mottakerens bank identifiseres i henhold til.|  
    |**Banknavn**|Angi bankens navn.|  
    |**Bankadresse 1**|Angi adressen til mottakers bank.|  
    |**Lands-/regionkode for mottakers bank**|Angi lands-/områdekoden for mottakeren. Dette feltet er obligatorisk og må være i overensstemmelse med ISO-standarder.|  
    |**SWIFT remb.bank**|Angi SWIFT-adressen for refusjon til mottakerens korresponderende bank.|  

10. Velg **OK**.  

## <a name="see-also"></a>Se også  
 [Elektroniske betalinger til leverandører i Norge](electronic-payments-to-vendors-in-norway.md)   
 [Sette opp remitteringsavtaler](how-to-set-up-remittance-agreements.md)   
 [Opprette remitteringskontoer](how-to-create-remittance-accounts.md)   
 [Mottakerreferansekoder](recipient-reference-codes.md)   
 [Opprette remitteringsforslag](how-to-create-remittance-suggestions.md)   
 [Opprette manuelle remitteringsoppdrag](how-to-create-manual-remittance-payments.md)   
 [Definere betalingslinjeinformasjon](how-to-set-up-payment-line-information.md)   
 [Kontrollere remitteringsoppdrag](how-to-test-remittance-payments.md)   
 [Eksportere remitteringsoppdrag](how-to-export-remittance-payments.md)   
 [Typer betalingsreturfiler](types-of-payment-returns-files.md)   
 [Importere betalingsreturdata](how-to-import-payment-return-data.md)   
 [Slette remitteringsoppdrag](how-to-delete-remittance-payment-orders.md)   
 [Remitteringsfeil](remittance-errors.md)   
 [Vise remitteringsfeilkoder](how-to-view-remittance-error-codes.md)   
 [Annullere betalinger](how-to-cancel-payments.md)

