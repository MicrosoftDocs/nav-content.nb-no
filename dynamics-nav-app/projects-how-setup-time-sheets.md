---
title: Definere timelister
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 6cbacce79ce185d6ed00ea8383259d1b28f9e11b
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-time-sheets"></a><span data-ttu-id="0101f-102">Definere timelister</span><span class="sxs-lookup"><span data-stu-id="0101f-102">How to: Set Up Time Sheets</span></span>
<span data-ttu-id="0101f-103">Timelister i Dynamics NAV håndterer tidsregistrering i ukentlige intervaller på sju dager.</span><span class="sxs-lookup"><span data-stu-id="0101f-103">Time sheets in Dynamics NAV handle time registration in weekly increments of seven days.</span></span> <span data-ttu-id="0101f-104">Du kan bruke dem til å spore tiden som brukes på prosjekter, og du kan bruke dem til å registrere enkel registrering av ressurstid.</span><span class="sxs-lookup"><span data-stu-id="0101f-104">You use them to track the time used on jobs, and you can use them to record simple resource time registration.</span></span> <span data-ttu-id="0101f-105">Før du kan bruke timelister, må du angi hvordan du vil at de skal settes opp og konfigureres.</span><span class="sxs-lookup"><span data-stu-id="0101f-105">Before you can use time sheets, you must specify how you want them to be set up and configured.</span></span>

<span data-ttu-id="0101f-106">Når du har definert hvordan organisasjonen vil bruke timelister, kan du angi om og hvordan timelister er godkjent.</span><span class="sxs-lookup"><span data-stu-id="0101f-106">After you have set up how your organization will use time sheets, you can specify if and how time sheets are approved.</span></span> <span data-ttu-id="0101f-107">Avhengig av behovene i organisasjonen, kan du angi:</span><span class="sxs-lookup"><span data-stu-id="0101f-107">Depending on the needs of your organization, you can designate:</span></span>

- <span data-ttu-id="0101f-108">En eller flere brukere som administrator for timeliste og godkjenning for alle timelister.</span><span class="sxs-lookup"><span data-stu-id="0101f-108">One or more users as the time sheet administrator and approver for all time sheets.</span></span>
- <span data-ttu-id="0101f-109">En godkjenner av timelister for hver ressurs.</span><span class="sxs-lookup"><span data-stu-id="0101f-109">A time sheet approver for each resource.</span></span>

<span data-ttu-id="0101f-110">Når du har definert timelister, kan du opprette timelister for ressurser, tilordne dem til planleggingslinjer og bokføre timelistelinjer.</span><span class="sxs-lookup"><span data-stu-id="0101f-110">When you have set up time sheets, you can create time sheets for resources, assign them to job planning lines, and post time sheet lines.</span></span> <span data-ttu-id="0101f-111">Se [Bruke timelister](projects-how-use-time-sheets.md) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="0101f-111">For more information, see [How to: Use Time Sheets](projects-how-use-time-sheets.md).</span></span>

## <a name="to-set-up-general-information-for-time-sheets"></a><span data-ttu-id="0101f-112">Slik definerer du generell informasjon for timelister</span><span class="sxs-lookup"><span data-stu-id="0101f-112">To set up general information for time sheets</span></span>  

1. <span data-ttu-id="0101f-113">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Ressursoppsett** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="0101f-113">In the top right corner, choose the **Search for Page or Report** icon, enter **Resources Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="0101f-114">Fyll ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="0101f-114">Fill in the fields as necessary.</span></span> <span data-ttu-id="0101f-115">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="0101f-115">Choose a field to read a short description of the field or link to more information.</span></span>
3. <span data-ttu-id="0101f-116">For feltet **Timeliste etter prosjektgodkjenning** velger du ett av følgende alternativer.</span><span class="sxs-lookup"><span data-stu-id="0101f-116">For the **Time Sheet by Job Approval** field, select one of the following options.</span></span>

|<span data-ttu-id="0101f-117">Alternativ</span><span class="sxs-lookup"><span data-stu-id="0101f-117">Option</span></span> |<span data-ttu-id="0101f-118">Beskrivelse</span><span class="sxs-lookup"><span data-stu-id="0101f-118">Description</span></span>|
|---|---|
|<span data-ttu-id="0101f-119">**Aldri**</span><span class="sxs-lookup"><span data-stu-id="0101f-119">**Never**</span></span>|<span data-ttu-id="0101f-120">Brukeren i feltet **Bruker-ID for godkjenner av timeliste:** på ressurskortet godkjenner timelisten.</span><span class="sxs-lookup"><span data-stu-id="0101f-120">The user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span></span>|
|<span data-ttu-id="0101f-121">**Alltid**</span><span class="sxs-lookup"><span data-stu-id="0101f-121">**Always**</span></span>|<span data-ttu-id="0101f-122">Brukeren i feltet **Ansvarlig person** på prosjektkortet godkjenner timelisten.</span><span class="sxs-lookup"><span data-stu-id="0101f-122">The user in the **Person Responsible** field on the job card approves the time sheet.</span></span>|
|<span data-ttu-id="0101f-123">**Bare maskin**´</span><span class="sxs-lookup"><span data-stu-id="0101f-123">**Machine Only**´</span></span>|<span data-ttu-id="0101f-124">Hvis timelisten for maskin er knyttet til et prosjekt, godkjenner brukeren i feltet **Ansvarlig person** på prosjektkortet, timelisten.</span><span class="sxs-lookup"><span data-stu-id="0101f-124">If the machine time sheet is linked with a job, then the user in the **Person Responsible** field on the job card approves the time sheet.</span></span> <span data-ttu-id="0101f-125">Hvis timelisten for maskin er knyttet til en ressurs, godkjenner brukeren i feltet **Bruker-ID for godkjenner av timeliste:** på ressurskortet, timelisten.</span><span class="sxs-lookup"><span data-stu-id="0101f-125">If the machine time sheet is linked with a resource, then the user in the **Time Sheet Approver User ID** field on the resource card approves the time sheet.</span></span>

## <a name="to-assign-a-time-sheet-administrator"></a><span data-ttu-id="0101f-126">Slik tilordner du en timelisteadministrator</span><span class="sxs-lookup"><span data-stu-id="0101f-126">To assign a time sheet administrator</span></span>  

1. <span data-ttu-id="0101f-127">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Brukeroppsett** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="0101f-127">In the top right corner, choose the **Search for Page or Report** icon, enter **User Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="0101f-128">Legg til en ny bruker hvis brukerlisten ikke inkluderer personen som du vil skal være ansvarlig for timelisteregistrering.</span><span class="sxs-lookup"><span data-stu-id="0101f-128">Add a new user, if the user list does not include the person who you want to be the time sheet administrator.</span></span> <span data-ttu-id="0101f-129">Hvis du vil ha mer informasjon, kontakt systemansvarlig.</span><span class="sxs-lookup"><span data-stu-id="0101f-129">For more information, please contact your administrator.</span></span>  
3. <span data-ttu-id="0101f-130">Velg en bruker som administrator for en timeliste, og merk deretter av for **Administrator for timeliste**</span><span class="sxs-lookup"><span data-stu-id="0101f-130">Select a user to be a time sheet administrator, and then select the **Time Sheet Admin.**</span></span> <span data-ttu-id="0101f-131">.</span><span class="sxs-lookup"><span data-stu-id="0101f-131">check box.</span></span>  

<span data-ttu-id="0101f-132">**Tips**: Det anbefales at du velger bare én bruker som administrator for timelisten i et selskap.</span><span class="sxs-lookup"><span data-stu-id="0101f-132">**Tip**: It is recommended that you designate only one user to be the time sheet administrator for a company.</span></span> <span data-ttu-id="0101f-133">I den følgende fremgangsmåten setter du opp en timelisteeier og -godkjenner, der godkjenneren av timelisten er tilordnet for hver ressurs.</span><span class="sxs-lookup"><span data-stu-id="0101f-133">In the following procedure, you set up a time sheet owner and approver where the time sheet approver is assigned for each resource.</span></span>  

## <a name="to-assign-a-time-sheets-owner-and-approver"></a><span data-ttu-id="0101f-134">Slik tilordner du en timelisteeier og -godkjenner</span><span class="sxs-lookup"><span data-stu-id="0101f-134">To assign a time sheets owner and approver</span></span>  

1. <span data-ttu-id="0101f-135">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Ressurser** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="0101f-135">In the top right corner, choose the **Search for Page or Report** icon, enter **Resources**, and then choose the related link.</span></span>
2. <span data-ttu-id="0101f-136">Merk ressursen du vil definere muligheten til å bruke timelister for, og merk deretter av for **Bruk timeliste**.</span><span class="sxs-lookup"><span data-stu-id="0101f-136">Select the resource for which you want to set up the ability to use time sheets, and then select the **Use Time Sheet** check box.</span></span>  
3. <span data-ttu-id="0101f-137">Angi ID-en for eieren av timelisten i feltet **Bruker-ID for eier av timeliste:**.</span><span class="sxs-lookup"><span data-stu-id="0101f-137">In the **Time Sheet Owner User ID** field, enter the ID of the owner of the time sheet.</span></span> <span data-ttu-id="0101f-138">Eieren kan angi tidsbruk på en timeliste og sende den til godkjenning.</span><span class="sxs-lookup"><span data-stu-id="0101f-138">The owner can enter time usage on a time sheet and submit it for approval.</span></span> <span data-ttu-id="0101f-139">Når ressursen er en person, er denne personen vanligvis også eieren.</span><span class="sxs-lookup"><span data-stu-id="0101f-139">In general, when the resource is a person, that person is also the owner.</span></span>  
4. <span data-ttu-id="0101f-140">Angi ID-en for godkjenneren av timelisten i feltet **Bruker-ID for godkjenner av timeliste**.</span><span class="sxs-lookup"><span data-stu-id="0101f-140">In the **Time Sheet Approver User ID** field, enter the ID of the approver of the time sheet.</span></span> <span data-ttu-id="0101f-141">Godkjenneren kan godkjenne, avvise eller åpne på nytt en timeliste.</span><span class="sxs-lookup"><span data-stu-id="0101f-141">The approver can approve, reject, or reopen a time sheet.</span></span>  

<span data-ttu-id="0101f-142">**Merk**: Du kan ikke endre ID-en for godkjenneren av timelisten hvis det finnes timelister som ennå ikke er behandlet og som har statusen **Sendt** eller **Åpen**.</span><span class="sxs-lookup"><span data-stu-id="0101f-142">**Note**: You cannot change the ID of the time sheet approver if there are time sheets that have not yet been processed and have the status of **Submitted** or **Open**.</span></span>

## <a name="see-also"></a><span data-ttu-id="0101f-143">Se også</span><span class="sxs-lookup"><span data-stu-id="0101f-143">See Also</span></span>
[<span data-ttu-id="0101f-144">Konfigurere prosjektstyring</span><span class="sxs-lookup"><span data-stu-id="0101f-144">Set Up Project Management</span></span>](projects-setup-projects.md)  
[<span data-ttu-id="0101f-145">Administrere prosjekter</span><span class="sxs-lookup"><span data-stu-id="0101f-145">Manage Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="0101f-146">Finans</span><span class="sxs-lookup"><span data-stu-id="0101f-146">Finance</span></span>](finance-setup.md)  
<span data-ttu-id="0101f-147">[Håndtere kjøp](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="0101f-147">[Manage Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="0101f-148">[Håndtere salg](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="0101f-148">[Manage Sales](sales-manage-sales.md)    </span></span>  
[<span data-ttu-id="0101f-149">Arbeide med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="0101f-149">Work With Dynamics NAV</span></span>](ui-work-product.md)  

