---
title: Vise objekter som webtjenester
description: "Publiserer [!INCLUDE[d365fin](includes/d365fin_md.MD)]-objekter som webtjenester, de er tilgjengelig på nettverket umiddelbart."
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7c2bb65caeed819088382f811eb179eaeda35a7c
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-publish-a-web-service"></a>Publisere en webtjeneste
Webtjenester er en lett måte å gjøre programfunksjonalitet tilgjengelig for en rekke eksterne systemer og brukere. [!INCLUDE[d365fin](includes/d365fin_md.md)] inneholder en rekke objekter som vises som webtjenester som standard på grunn av integrering med andre Microsoft-tjenester, men du kan også legge til andre webtjenester.  

Du kan definere en webtjeneste i Windows-klienten eller i webklienten. Du må deretter publisere webtjenesten slik at den er tilgjengelig for serviceforespørsler over nettverket. Brukere kan oppdage webtjenester ved å velge en webleser på en server og be om liste over tilgjengelige tjenester. Når du publiserer en webtjeneste, er den umiddelbart tilgjengelig på nettverket for godkjente brukere. Alle autoriserte brukere har tilgang til metadata for webtjenester, men bare brukere som har tilstrekkelige tillatelser, har tilgang til faktiske data.

## <a name="creating-and-publishing-a-web-service"></a>Opprette og publisere en webtjeneste  
 De følgende trinnene forklarer hvordan du oppretter og publiserer en webtjeneste.  

#### <a name="to-create-and-publish-a-web-service"></a>Slik oppretter og publiserer du en webtjeneste  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Webtjenester**, og velg deretter den relaterte koblingen.  

2.  På siden **Webtjenester** velger du **Ny**. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    > [!NOTE]  
    >  **Kodeenhet** og **Side** er gyldige typer for SOAP-webtjenester. **Side** og **Spørring** er gyldige typer for OData-webtjenester.  
    Hvis databasen inneholder flere selskaper, kan du også velge en objekt-ID som er spesifikk for ett av selskapene.  
    Tjenestenavnet er synlig for brukere av webtjenesten, og brukes som grunnlag for å identifisere og skjelne webtjenester, så du bør velge et meningsfullt navn.

3.  Merk avmerkingsboksen i kolonnen **Publisert**.  

     Når du publiserer webtjenesten i feltene **OData URL-adresse** og **SOAP-URL-adresse**, kan du se URL-adressene som er generert for webtjenesten. Du kan teste webtjenesten umiddelbart ved å velge koblingene i feltene **OData URL-adresse** og **SOAP-URL-adresse**. Du kan eventuelt kopiere feltets verdi, og lagre den for senere bruk.  

Når du publiserer en webtjeneste, er den tilgjengelig for eksterne parter. Du kan kontrollere tilgjengeligheten til denne webtjenesten ved hjelp av en leser, eller du kan velge koblingen i feltene **OData URL-adresse** og **SOAP-URL-adresse** i vinduet **Webtjenester**. Følgende fremgangsmåte viser hvordan du kan kontrollere webtjenestens tilgjengelighet for senere bruk.  

#### <a name="to-verify-the-availability-of-a-web-service"></a>Slik kontrollerer du tilgjengeligheten til en webtjeneste  

1.  Angi den aktuelle URL-adressen i nettleseren. Tabellen nedenfor viser hvilke typer URL-adresser som du kan angi. Bruk følgende format for din URI for SOAP-webtjenester.  

    <table>
    <tr>
    <th>Webtjenestetype</th>
    <th>Syntaks</th>
    <th>Eksempel</th>
    </tr>
    <tr>
    <td>SOAP</td>
    <td>https://*Server*:*SOAPWebServicePort*/*ServerInstance*/WS/*CompanyName*/salesDocuments/</td>
    <td>https://mycompany.financials.dynamics.com:7047/MS/WS/MyCompany/Page/salesDocuments?tenant=mycompany.financials.dynamics.com</td>
    </tr>
    <tr>
    <td>OData</td>
    <td>https://*Server*:*ODataWebServicePort*/*ServerInstance*/OData/Company('*CompanyName*')</td>
    <td>https://MyCompany.financials.dynamics.com:7048/MS/OData/Company('MyCompany')/salesDocuments?tenant=MyCompany.financials.dynamics.com

         The company name is case-sensitive.</td>
    </tr>
    </table>

2.  Se gjennom informasjone som vises i webleseren. Kontroller at du kan se navnet på webtjenesten som du har opprettet.  

 Når du åpner en webtjeneste, og du vil skrive data tilbake til [!INCLUDE[d365fin](includes/d365fin_md.md)], må du angi firmanavnet. Du kan angi selskapet som en del av URI-en som vist i eksemplene, eller du kan angi selskapet som en del av spørringsparameterne. Følgende URIer peker for eksempel til den samme OData web-tjenesten, og de er begge gyldige URIer.  

```  
https://localhost:7048/server/OData/Company('CRONUS International Ltd.')/Customer  
```  

```  
https://localhost:7048/server/OData/Customer?company='CRONUS International Ltd.'  
```  

## <a name="see-also"></a>Se også  
[Oppsett og administrasjon i Dynamics NAV](admin-setup-and-administration.md)  

