---
title: Velg metoden for elektroniske betalinger
description: "Behandle betalinger til leverandører i -vinduet ved å eksportere en fil sammen med betalingsinformasjonen fra kladdelinjene."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 5502f9c50f00456b7a3b04a1cdce25e647671b29
ms.contentlocale: nb-no
ms.lasthandoff: 12/01/2017

---
# <a name="make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer"></a><span data-ttu-id="000a9-103">Betale med tjenesten for bankdatakonvertering eller SEPA-kredittoverføring</span><span class="sxs-lookup"><span data-stu-id="000a9-103">Make Payments with Bank Data Conversion Service or SEPA Credit Transfer</span></span>
<span data-ttu-id="000a9-104">Nå kan du behandle betalinger til leverandører i vinduet **Betalingskladd** ved å eksportere en fil sammen med betalingsinformasjonen fra kladdelinjene.</span><span class="sxs-lookup"><span data-stu-id="000a9-104">In the **Payment Journal** window, you can process payments to your vendors by exporting a file together with the payment information from the journal lines.</span></span> <span data-ttu-id="000a9-105">Du kan deretter laste opp filen til nettbanken der de relaterte pengeoverføringene behandles.</span><span class="sxs-lookup"><span data-stu-id="000a9-105">You can then upload the file to your electronic bank where the related money transfers are processed.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="000a9-106"> støtter formatet for SEPA-kreidttoverføring, men andre formater for elektroniske betalinger kan være tilgjengelige i ditt land/region.</span><span class="sxs-lookup"><span data-stu-id="000a9-106"> supports the SEPA Credit Transfer format, but in your country/region, other formats for electronic payments may be available.</span></span>   

 <span data-ttu-id="000a9-107">Hvis du vil gjøre det mulig å foreta SEPA-kredittoverføringer, må du først opprette en bankkonto, en leverandør og finanskladden som utbetalingskladden er basert på.</span><span class="sxs-lookup"><span data-stu-id="000a9-107">To enable SEPA credit transfers, you must first set up a bank account, a vendor, and the general journal batch that the payment journal is based on.</span></span> <span data-ttu-id="000a9-108">Deretter gjør du klar betalinger til leverandører ved å fylle ut vinduet **Betalingskladd** med forfalte betalinger som har angitte bokføringsdatoer.</span><span class="sxs-lookup"><span data-stu-id="000a9-108">You then prepare payments to vendors by automatically filling the **Payment Journal** window with due payments with specified posting dates.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="000a9-109">Når du har bekreftet at betalingene er behandlet av banken, kan du begynne å bokføre utbetalingskladdelinjene.</span><span class="sxs-lookup"><span data-stu-id="000a9-109">When you have verified that the payments are successfully processed by the bank, you can proceed to post the payment journal lines.</span></span>  

 <span data-ttu-id="000a9-110">Tabellen nedenfor beskriver en sekvens av oppgaver, og har koblinger til emnene som beskriver dem.</span><span class="sxs-lookup"><span data-stu-id="000a9-110">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="000a9-111">**Hvis du vil**</span><span class="sxs-lookup"><span data-stu-id="000a9-111">**To**</span></span>|<span data-ttu-id="000a9-112">**Se**</span><span class="sxs-lookup"><span data-stu-id="000a9-112">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="000a9-113">Aktiverer tjenesten for bankdatakonvertering for å konvertere en kontoutdragsfil til et format du kan importere, eller konvertere den eksporterte betalingsfilen til formatet som banken krever.</span><span class="sxs-lookup"><span data-stu-id="000a9-113">Activate the Bank Data Conversion Service feature to have any bank statement file converted to a format that you can import or to have your exported payment files converted to the format that your bank requires.</span></span>|[<span data-ttu-id="000a9-114">Konfigurere tjeneste for konvertering av bankdata</span><span class="sxs-lookup"><span data-stu-id="000a9-114">How to: Set Up the Bank Data Conversion Service</span></span>](bank-how-setup-bank-data-conversion-service.md)|  
|<span data-ttu-id="000a9-115">Definere en bankkonto, leverandør og en utbetalingskladd for SEPA-kredittoverføring.</span><span class="sxs-lookup"><span data-stu-id="000a9-115">Set up a bank account, a vendor, and a payment journal for SEPA credit transfer.</span></span>|[<span data-ttu-id="000a9-116">Definere SEPA-kredittoverføring</span><span class="sxs-lookup"><span data-stu-id="000a9-116">How to: Set Up SEPA Credit Transfer</span></span>](finance-how-to-set-up-sepa-credit-transfer.md)|  
|<span data-ttu-id="000a9-117">Fylle ut utbetalingskladden med linjer for utestående leverandørfordringer, med mulighet til å sette inn bokføringsdatoer basert på forfallsdatoen til de relaterte kjøpsdokumentene.</span><span class="sxs-lookup"><span data-stu-id="000a9-117">Fill the payment journal with lines for due payments to vendors, with the option to insert posting dates based on the due date of the related purchase documents.</span></span>|[<span data-ttu-id="000a9-118">Administrere skyldige beløp</span><span class="sxs-lookup"><span data-stu-id="000a9-118">Manage Payables</span></span>](payables-manage-payables.md)|  
|<span data-ttu-id="000a9-119">Eksportere utbetalingskladdelinjer til en fil i SEPA-kredittoverføringsformatet.</span><span class="sxs-lookup"><span data-stu-id="000a9-119">Export payment journal lines to a file in the SEPA Credit Transfer format.</span></span>|[<span data-ttu-id="000a9-120">Fremgangsmåte: Eksportere betalinger til en bankfil</span><span class="sxs-lookup"><span data-stu-id="000a9-120">How to: Export Payments to a Bank File</span></span>](payables-how-export-payments-bank-file.md)|  
|<span data-ttu-id="000a9-121">Gå gjennom hvilke betalinger som er eksportert til hvilke filer.</span><span class="sxs-lookup"><span data-stu-id="000a9-121">Review which payments have been exported and into which files.</span></span>|<span data-ttu-id="000a9-122">Kredittoverføringsregistre</span><span class="sxs-lookup"><span data-stu-id="000a9-122">Credit Transfer Registers</span></span>|  
|<span data-ttu-id="000a9-123">Bokfør betalingene når den elektroniske betalingen er behandlet av banken.</span><span class="sxs-lookup"><span data-stu-id="000a9-123">When the electronic payment is successfully processed by the bank, post the payments.</span></span>|[<span data-ttu-id="000a9-124">Arbeide med finanskladder</span><span class="sxs-lookup"><span data-stu-id="000a9-124">Working with General Journals</span></span>](ui-work-general-journals.md)|  

## <a name="see-also"></a><span data-ttu-id="000a9-125">Se også</span><span class="sxs-lookup"><span data-stu-id="000a9-125">See Also</span></span>  
[<span data-ttu-id="000a9-126">Konfigurere tjeneste for konvertering av bankdata</span><span class="sxs-lookup"><span data-stu-id="000a9-126">How to: Set Up the Bank Data Conversion Service</span></span>](bank-how-setup-bank-data-conversion-service.md)  
[<span data-ttu-id="000a9-127">Definere SEPA-kredittoverføring</span><span class="sxs-lookup"><span data-stu-id="000a9-127">How to: Set Up SEPA Credit Transfer</span></span>](finance-how-to-set-up-sepa-credit-transfer.md)  
<span data-ttu-id="000a9-128">[Administrere skyldige beløp](payables-manage-payables.md) </span><span class="sxs-lookup"><span data-stu-id="000a9-128">[Manage Payables](payables-manage-payables.md) </span></span>  
[<span data-ttu-id="000a9-129">Arbeide med finanskladder</span><span class="sxs-lookup"><span data-stu-id="000a9-129">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="000a9-130">Innkreve betalinger med SEPA Direct Debit</span><span class="sxs-lookup"><span data-stu-id="000a9-130">Collecting Payments with SEPA Direct Debit</span></span>](finance-collect-payments-with-sepa-direct-debit.md)   

