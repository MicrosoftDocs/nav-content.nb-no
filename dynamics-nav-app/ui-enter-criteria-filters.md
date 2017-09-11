---
title: "Angi vilkår i filtre"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: df386e1195db385ee053b69fec0f5082d8df4116
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---

# <a name="entering-criteria-in-filters"></a><span data-ttu-id="82312-102">Angi vilkår i filtre</span><span class="sxs-lookup"><span data-stu-id="82312-102">Entering Criteria in Filters</span></span>
<span data-ttu-id="82312-103">Når du vil søke etter data, for eksempel kundenavn, adresser eller produktgrupper, må du angi kriterier.</span><span class="sxs-lookup"><span data-stu-id="82312-103">When you want to search for data, such as customer names, addresses, or product groups, you enter criteria.</span></span> <span data-ttu-id="82312-104">I søkekriteriene kan du bruke alle tallene og bokstavene du vanligvis kan bruke i det spesifikke feltet.</span><span class="sxs-lookup"><span data-stu-id="82312-104">In search criteria you can use all the numbers and letters that you normally use in the specific field.</span></span> <span data-ttu-id="82312-105">I tillegg til dette kan du bruke spesielle symboler til å filtrere resultatene ytterligere.</span><span class="sxs-lookup"><span data-stu-id="82312-105">In addition, you can use special symbols to further filter the results.</span></span>

## <a name="searching-using-the-quick-filter"></a><span data-ttu-id="82312-106">Søke ved hjelp av hurtigfilteret</span><span class="sxs-lookup"><span data-stu-id="82312-106">Searching using the Quick Filter</span></span>
<span data-ttu-id="82312-107">Du kan legge til filtre på alle sider ved hjelp av hurtigfilteret.</span><span class="sxs-lookup"><span data-stu-id="82312-107">You can add filters to all pages by using the Quick Filter.</span></span> <span data-ttu-id="82312-108">Hurtigfilteret aktiveres ved å velge forstørrelsesikonet i øvre høyre hjørne på siden.</span><span class="sxs-lookup"><span data-stu-id="82312-108">The Quick Filter is enabled by choosing the magnifier icon in the top right corner of a page.</span></span> <span data-ttu-id="82312-109">Denne filtreringstypen brukes for rask angivelse av kriterier.</span><span class="sxs-lookup"><span data-stu-id="82312-109">This filtering type is used for a fast entry of criteria.</span></span>

<span data-ttu-id="82312-110">**Viktig**: Hurtigfilteret gjør det enkelt å filtrere data ved å skrive inn ren tekst, men gir også mange alternativer når det gjelder søkekriterier.</span><span class="sxs-lookup"><span data-stu-id="82312-110">**Important**: The Quick Filter provides an easy access to filter data by entering plain text, but does also provide a lot of search criteria options.</span></span> <span data-ttu-id="82312-111">Virkemåten for hurtigfilteret er avhengig av om du skriver inn ren tekst eller tekst som inneholder symboler.</span><span class="sxs-lookup"><span data-stu-id="82312-111">Depending on whether you enter plain text or text including symbols, the Quick Filter behaves differently.</span></span>  
- <span data-ttu-id="82312-112">Hvis du skriver inn ren tekst i søkevilkåret, tolkes søkekriteriene som et søk som ikke skiller mellom store og små bokstaver og som inneholder en bestemt tekst.</span><span class="sxs-lookup"><span data-stu-id="82312-112">If you enter plain text in the search criteria, the search criteria is interpreted as a case insensitive search that contains certain text.</span></span>  
- <span data-ttu-id="82312-113">Hvis du skriver inn tekst med symboler i søkekriteriene, tolkes søkekriteriene nøyaktig slik du skrev det inn, og søket skiller mellom store og små bokstaver.</span><span class="sxs-lookup"><span data-stu-id="82312-113">If you enter text including symbols in the search criteria, the search criteria is interpreted exactly as you entered it, and the search is case sensitive.</span></span>

### <a name="quick-filter-criteria"></a><span data-ttu-id="82312-114">Kriterier for hurtigfilter</span><span class="sxs-lookup"><span data-stu-id="82312-114">Quick filter criteria</span></span>
<!-- html syntax because symbols conflict with MarkDown syntax -->
<TABLE>
  <TR>
    <TH><span data-ttu-id="82312-115">Søkekriterier</span><span class="sxs-lookup"><span data-stu-id="82312-115">Search Criteria</span></span></TH>
    <TH><span data-ttu-id="82312-116">Tolkes som ...</span><span class="sxs-lookup"><span data-stu-id="82312-116">Interpreted as...</span></span></TH>
    <TH><span data-ttu-id="82312-117">Returnerer ...</span><span class="sxs-lookup"><span data-stu-id="82312-117">Returns...</span></span></TH>
  </TR>
  <TR>
    <TD><span data-ttu-id="82312-118">>man</span><span class="sxs-lookup"><span data-stu-id="82312-118">>man</span></span></TD>
    <TD><span data-ttu-id="82312-119">@*man*</span><span class="sxs-lookup"><span data-stu-id="82312-119">@*man*</span></span></TD>
    <TD><span data-ttu-id="82312-120">Alle poster som inneholder teksten mann og som ikke skiller mellom små og store bokstaver.</span><span class="sxs-lookup"><span data-stu-id="82312-120">All records that contain the text man and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="82312-121">>se</span><span class="sxs-lookup"><span data-stu-id="82312-121">>se</span></span></TD>
    <TD><span data-ttu-id="82312-122">@*se*</span><span class="sxs-lookup"><span data-stu-id="82312-122">@*se*</span></span></TD>
    <TD><span data-ttu-id="82312-123">Alle poster som inneholder teksten se og som ikke skiller mellom små og store bokstaver.</span><span class="sxs-lookup"><span data-stu-id="82312-123">All records that contain the text se and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="82312-124">>Man*</span><span class="sxs-lookup"><span data-stu-id="82312-124">>Man*</span></span></TD>
    <TD><span data-ttu-id="82312-125">Begynner med Man, og skiller mellom små og store bokstaver.</span><span class="sxs-lookup"><span data-stu-id="82312-125">Starts with Man and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="82312-126">Alle poster som starter med teksten Man.</span><span class="sxs-lookup"><span data-stu-id="82312-126">All records that start with the text Man.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="82312-127">'man'</span><span class="sxs-lookup"><span data-stu-id="82312-127">'man'</span></span></TD>
    <TD><span data-ttu-id="82312-128">En nøyaktig tekst som skiller mellom små og store bokstaver.</span><span class="sxs-lookup"><span data-stu-id="82312-128">An exact text and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="82312-129">Alle poster som samsvarer nøyaktig med man.</span><span class="sxs-lookup"><span data-stu-id="82312-129">All records that match man exactly.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="82312-130">@*man</span><span class="sxs-lookup"><span data-stu-id="82312-130">@*man</span></span></TD>
    <TD><span data-ttu-id="82312-131">Slutter med, og skiller ikke mellom små og store bokstaver.</span><span class="sxs-lookup"><span data-stu-id="82312-131">Ends with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="82312-132">Alle poster som slutter med man.</span><span class="sxs-lookup"><span data-stu-id="82312-132">All records that end with man.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="82312-133">@man*</span><span class="sxs-lookup"><span data-stu-id="82312-133">@man*</span></span></TD>
    <TD><span data-ttu-id="82312-134">Begynner med, og skiller ikke mellom små og store bokstaver.</span><span class="sxs-lookup"><span data-stu-id="82312-134">Starts with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="82312-135">Alle poster som starter med man.</span><span class="sxs-lookup"><span data-stu-id="82312-135">All records that start with man.</span></span></TD>
  </TR>
</TABLE>

<span data-ttu-id="82312-136">**Merk**: Du kan ikke bruke et jokertegn når du filtrerer på felt for opplisting, for eksempel feltet **Status** i salgsordrer.</span><span class="sxs-lookup"><span data-stu-id="82312-136">**Note**: You cannot use a wildcard when filtering on enumeration fields, such as the **Status** field on sales orders.</span></span> <span data-ttu-id="82312-137">Hvis du vil angi et filter for denne typen felt, kan du angi den numeriske verdien som en parameter for filtrering.</span><span class="sxs-lookup"><span data-stu-id="82312-137">To enter a filter for this type of field, you can enter the numeric value as a filtering parameter.</span></span> <span data-ttu-id="82312-138">I feltet **Status** på en ordre som har verdiene **Åpen**, **Frigitt**, **Venter på godkjenning** og **Venter på forskudd**, må du bruke verdiene **0**, **1**, **2** og **3** for å filtrere etter disse alternativene.</span><span class="sxs-lookup"><span data-stu-id="82312-138">For example, in the **Status** field on a sales order that has the values **Open**, **Released**, **Pending Approval**, and **Pending Prepayment**, use the values **0**, **1**, **2**, and **3** to filter for these options.</span></span>  

## <a name="see-also"></a><span data-ttu-id="82312-139">Se også</span><span class="sxs-lookup"><span data-stu-id="82312-139">See Also</span></span>
[<span data-ttu-id="82312-140">Arbeide med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="82312-140">Work with Dynamics NAV</span></span>](ui-work-product.md)

