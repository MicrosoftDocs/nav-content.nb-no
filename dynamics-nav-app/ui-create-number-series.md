---
title: Opprette nummerserier
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
ms.openlocfilehash: e42e5ed139b2487fea13ef0fd57757035764addd
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---

# <a name="create-number-series"></a><span data-ttu-id="3526e-102">Opprette nummerserier</span><span class="sxs-lookup"><span data-stu-id="3526e-102">Create Number Series</span></span>

<span data-ttu-id="3526e-103">For hvert selskap som opprettes, må du tilordne unike identifikasjonskoder til elementer som for eksempel hovedbokkontoer, kunde- og leverandørkontoer, fakturaer og dokumenter.</span><span class="sxs-lookup"><span data-stu-id="3526e-103">For each company that you set up, you need to assign unique identification codes to things such as general ledger accounts, customer and vendor accounts, invoices, and documents.</span></span> <span data-ttu-id="3526e-104">Nummerering er ikke bare viktig for identifikasjonsformål.</span><span class="sxs-lookup"><span data-stu-id="3526e-104">Numbering is important not only for identification.</span></span> <span data-ttu-id="3526e-105">Med et godt utformet nummereringssystem er det enklere å styre og analysere selskapet, og antall feil som forekommer ved dataregistrering reduseres.</span><span class="sxs-lookup"><span data-stu-id="3526e-105">A well-designed numbering system also makes the company more manageable and easy to analyze, and can reduce the number of errors that occur in data entry.</span></span>

<span data-ttu-id="3526e-106">Du kan lage et komplett nummereringssystem med et ubegrenset antall nummerserier.</span><span class="sxs-lookup"><span data-stu-id="3526e-106">You can set up a complete numbering system with an unlimited number of number series.</span></span> <span data-ttu-id="3526e-107">Du kan bruke nummerserier for alle typer dokumenter og kladder, så vel som for hoveddata som for eksempel kunder, varer og jobber.</span><span class="sxs-lookup"><span data-stu-id="3526e-107">You can use number series for all types of documents and journals, as well as for master data such as customers, items, and jobs.</span></span>

<span data-ttu-id="3526e-108">Du kan kombinere bruken av nummerserier med manuell nummerering.</span><span class="sxs-lookup"><span data-stu-id="3526e-108">You can combine the use of number series with manual numbering.</span></span>

<span data-ttu-id="3526e-109">Et nummereringssystem lager du ved å opprette én eller flere koder for hver hoveddatatype eller dokumenttype.</span><span class="sxs-lookup"><span data-stu-id="3526e-109">You create a numbering system by setting up one or more codes for each type of master data or document.</span></span> <span data-ttu-id="3526e-110">Du kan for eksempel opprette én kode for å nummerere kunder, en annen kode for å nummerere salgsfakturaer, og enda en kode for å nummerere dokumenter i finanskladder.</span><span class="sxs-lookup"><span data-stu-id="3526e-110">For example, you can set up one code for numbering customers, another code for numbering sales invoices, and another code for numbering documents in general journals.</span></span>

<span data-ttu-id="3526e-111">Når du har opprettet en kode, må du opprette minst én nummerserielinje.</span><span class="sxs-lookup"><span data-stu-id="3526e-111">After you have set up a code, you set must set up at least one number series line.</span></span> <span data-ttu-id="3526e-112">Nummerserielinjen inneholder informasjon som for eksempel første og siste nummer i serien, samt startdato.</span><span class="sxs-lookup"><span data-stu-id="3526e-112">The number series line contains information such as the first and last number in the series and the starting date.</span></span> <span data-ttu-id="3526e-113">Du kan opprettet mer enn én nummerserielinje per nummerseriekode, med ulik startdato for hver linje.</span><span class="sxs-lookup"><span data-stu-id="3526e-113">You can set up more than one number series line per number series code, with a different starting date for each line.</span></span> <span data-ttu-id="3526e-114">Seriene brukes i rekkefølge, og hver serie starter på sin respektive startdato.</span><span class="sxs-lookup"><span data-stu-id="3526e-114">The series will be used consecutively, starting each series on the respective starting date.</span></span>

<span data-ttu-id="3526e-115">Hvis du vil bruke mer enn én nummerseriekode for én type hoveddata - det vil si hvis du for eksempel vil bruke ulike nummerserier for ulike varekategorier - kan du bruke nummerserieforbindelser.</span><span class="sxs-lookup"><span data-stu-id="3526e-115">If you want to use more than one number series code for one type of master data - for example, if you want to use different number series for different categories of items - you can use number series relationships.</span></span>

<span data-ttu-id="3526e-116">I tillegg til numrene du tilordner manuelt eller ved hjelp av nummereringssystemet, blir det automatisk tilordnet fortløpende nummerering av alle transaksjoner (poster).</span><span class="sxs-lookup"><span data-stu-id="3526e-116">In addition to the numbers that you assign manually or by use of the numbering system, all transactions (ledger entries) are automatically assigned consecutive numbers.</span></span> <span data-ttu-id="3526e-117">Disse numrene kan ses i **Løpenr.**</span><span class="sxs-lookup"><span data-stu-id="3526e-117">These numbers can be seen in the **Entry No.**</span></span> <span data-ttu-id="3526e-118">-feltet i alle postvinduene.</span><span class="sxs-lookup"><span data-stu-id="3526e-118">field in all the ledger entry windows.</span></span> <span data-ttu-id="3526e-119">Du kan ikke endre eller slette disse numrene.</span><span class="sxs-lookup"><span data-stu-id="3526e-119">You cannot modify or delete these numbers.</span></span>

## <a name="to-create-relationships-between-number-series"></a><span data-ttu-id="3526e-120">Slik oppretter du forbindelser mellom nummerserier</span><span class="sxs-lookup"><span data-stu-id="3526e-120">To create relationships between number series</span></span>
<span data-ttu-id="3526e-121">Hvis du har opprettet mer enn én nummerseriekode for den samme typen grunnleggende opplysninger eller transaksjoner, kan du opprette forbindelser mellom kodene.</span><span class="sxs-lookup"><span data-stu-id="3526e-121">If you have set up more than one number series code for the same kind of basic information or transactions, you can create relationships between the codes.</span></span> <span data-ttu-id="3526e-122">Denne funksjonen kan hjelpe deg med å velge mellom koder når du bruker et nummer.</span><span class="sxs-lookup"><span data-stu-id="3526e-122">This feature can assist you in deciding among the codes when you use a number.</span></span>

1. <span data-ttu-id="3526e-123">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Nummerserie** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="3526e-123">In the top right corner, choose the **Search for Page or Report** icon, enter **No. Series**, and then choose the related link.</span></span>
2. <span data-ttu-id="3526e-124">Velg linjen med nummerserien du vil opprette forbindelser for, og velg deretter **Forbindelser**.</span><span class="sxs-lookup"><span data-stu-id="3526e-124">Select the line with the number series you want to create relationships for and then choose **Relationships**.</span></span>
3. <span data-ttu-id="3526e-125">I **Seriekode**-feltet angir du koden for nummerserien du vil knytte til serien du valgte i trinn 2.</span><span class="sxs-lookup"><span data-stu-id="3526e-125">In the **Series Code** field, enter the code for the number series that you want to relate to the series you selected in step 2.</span></span>
4. <span data-ttu-id="3526e-126">Legg til en linje for hver kode du vil knytte til den valgte nummerserien.</span><span class="sxs-lookup"><span data-stu-id="3526e-126">Add a line for each code that you want to relate to the selected number series.</span></span>
5. <span data-ttu-id="3526e-127">Lukk vinduet.</span><span class="sxs-lookup"><span data-stu-id="3526e-127">Close the window.</span></span>

<span data-ttu-id="3526e-128">Når du så registrerer noe som trenger et nummer, kan du bruke forbindelsene du har opprettet til å velge mellom nummerseriene som er koblet til hverandre.</span><span class="sxs-lookup"><span data-stu-id="3526e-128">Now when you set up something that requires a number, you can use the relationships you created to select among the related number series.</span></span>

## <a name="see-also"></a><span data-ttu-id="3526e-129">Se også</span><span class="sxs-lookup"><span data-stu-id="3526e-129">See Also</span></span>
[<span data-ttu-id="3526e-130">Arbeide med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="3526e-130">Work with Dynamics NAV</span></span>](ui-work-product.md)

