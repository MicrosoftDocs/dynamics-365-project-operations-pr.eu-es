---
title: Alderatu agiria gastuekin OCRa erabiliz
description: Gai honetan ordainagirien karaktereen ezagutza optikoa (OCR) prozesatzeari buruzko informazioa ematen da.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 02c1bafbe907a657689b610ae792f88085320903
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896986"
---
# <a name="match-a-receipt-to-an-expense-using-ocr"></a><span data-ttu-id="4b19f-103">Alderatu agiria gastuekin OCRa erabiliz</span><span class="sxs-lookup"><span data-stu-id="4b19f-103">Match a receipt to an expense using OCR</span></span>

<span data-ttu-id="4b19f-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="4b19f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="4b19f-105">Gastuen sarrera hobetu da ordainagirien karaktereen ezagutza optikoa (OCR) prozesuaren bidez.</span><span class="sxs-lookup"><span data-stu-id="4b19f-105">Expense entry has been enhanced through the introduction of optical character recognition (OCR) processing for receipts.</span></span> <span data-ttu-id="4b19f-106">Funtzionalitate hau gastuen txostenak sortzerakoan erabiltzailearen esperientzia hobetzeko diseinatuta dago.</span><span class="sxs-lookup"><span data-stu-id="4b19f-106">This functionality is designed to improve the user experience when creating expense reports.</span></span>

## <a name="key-features"></a><span data-ttu-id="4b19f-107">Eginbide nagusiak</span><span class="sxs-lookup"><span data-stu-id="4b19f-107">Key features</span></span>

- <span data-ttu-id="4b19f-108">Sistemak merkatariaren izena, data eta zenbateko osoa ateratzen ditu ordainagirietatik.</span><span class="sxs-lookup"><span data-stu-id="4b19f-108">The system extracts the merchant name, date, and total amount from receipts.</span></span>
- <span data-ttu-id="4b19f-109">Sistema erantsitako ordainagiriak lotu gabeko gastuen transakzioekin parekatzen saiatuko da.</span><span class="sxs-lookup"><span data-stu-id="4b19f-109">The system will try to match unattached receipts to unattached expense transactions.</span></span>
- <span data-ttu-id="4b19f-110">Ordainagirietatik eskuz sartutako gastu transakzioak sor ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="4b19f-110">You can create manually entered expense transactions from receipts.</span></span>

## <a name="attach-receipts-to-an-expense-report"></a><span data-ttu-id="4b19f-111">Erantsi ordainagiriak gastuen txostenean</span><span class="sxs-lookup"><span data-stu-id="4b19f-111">Attach receipts to an expense report</span></span>

<span data-ttu-id="4b19f-112">Gastu txostena sortzen denean kreditu txartelarekin egindako transakzioak jasotzen dituzten ordainagiriak automatikoki eransteko, jarraitu urrats hauek.</span><span class="sxs-lookup"><span data-stu-id="4b19f-112">To automatically attach receipts that include credit card transactions when an expense report is created, complete the following steps.</span></span>

  1. <span data-ttu-id="4b19f-113">Ireki **Gastuen kudeaketa** lan eremua.</span><span class="sxs-lookup"><span data-stu-id="4b19f-113">Open the **Expense management** workspace.</span></span>
  2. <span data-ttu-id="4b19f-114">Gainean **Ordainagiriak** fitxa, egiaztatu lotu gabeko ordainagiriak badirela.</span><span class="sxs-lookup"><span data-stu-id="4b19f-114">On the **Receipts** tab, verify that unattached receipts exist.</span></span> <span data-ttu-id="4b19f-115">Ordainagiriak ere karga ditzakezu **Ordainagiriak** fitxa.</span><span class="sxs-lookup"><span data-stu-id="4b19f-115">You can also upload receipts on the **Receipts** tab.</span></span>
  3. <span data-ttu-id="4b19f-116">**Gastuak** fitxan, egiaztatu lotu gabeko gastuak badirela.</span><span class="sxs-lookup"><span data-stu-id="4b19f-116">On the **Expenses** tab, verify that unattached expenses exist.</span></span> <span data-ttu-id="4b19f-117">Normalean, gastuen administratzaileak gastu horiek kreditu txartelaren hornitzailearen eskutik inportatzen ditu.</span><span class="sxs-lookup"><span data-stu-id="4b19f-117">Typically, the expense administrator imports these expenses from the credit card provider.</span></span>
  4. <span data-ttu-id="4b19f-118">Aukeratu **Gastu txosten berria**.</span><span class="sxs-lookup"><span data-stu-id="4b19f-118">Select **New expense report**.</span></span> <span data-ttu-id="4b19f-119">Kontuan izan gastuak eta ordainagiriak sar ditzakezula, orain ere, gastuen txostena sortzen duzunean.</span><span class="sxs-lookup"><span data-stu-id="4b19f-119">Notice that you can include expenses, and receipts, now as well, when you create an expense report.</span></span> <span data-ttu-id="4b19f-120">Gastuak eta ordainagiriak gehitzen badituzu, ordainagirien gastuen pareko automatikoki abiaraziko da.</span><span class="sxs-lookup"><span data-stu-id="4b19f-120">If you add both expenses and receipts, automatic matching of the receipts against the expenses is triggered.</span></span>

## <a name="create-or-match-receipts-to-an-expense-report"></a><span data-ttu-id="4b19f-121">Sortu edo bat etorri ordainagiriak gastuen txostenean</span><span class="sxs-lookup"><span data-stu-id="4b19f-121">Create or match receipts to an expense report</span></span>
<span data-ttu-id="4b19f-122">Gastua sortzeko edo ordainagiriaren gastuarekin bat egiteko, jarraitu urrats hauek.</span><span class="sxs-lookup"><span data-stu-id="4b19f-122">To create an expense, or match an expense from a receipt, complete the following steps.</span></span>

  1. <span data-ttu-id="4b19f-123">Gastu txosten batean, **Ordainagiriak** fitxa, erantsi ordainagiria hautatuz **Gehitu ordainagiriak**.</span><span class="sxs-lookup"><span data-stu-id="4b19f-123">On an expense report, on the **Receipts** tab, attach a receipt by selecting **Add receipts**.</span></span>
  2. <span data-ttu-id="4b19f-124">Ordainagiriaren kargatutako irudiaren azpian, ohar ezazu **Sortu** eta **Partidua** aukerak.</span><span class="sxs-lookup"><span data-stu-id="4b19f-124">Under the uploaded image of the receipt, notice the **Create** and **Match** options.</span></span>

      - <span data-ttu-id="4b19f-125">Aukeratu **Sortu** eskuz sartutako gastuen transakzioa sortzeko eta ordainagiritik ateratako balioak betetzeko.</span><span class="sxs-lookup"><span data-stu-id="4b19f-125">Select **Create** to create a manually entered expense transaction and fill in the values that are extracted from the receipt.</span></span>
      - <span data-ttu-id="4b19f-126">Hautatzen baduzu **Partidua**, sistema lehendik zegoen gastua ordainagiriarekin parekatzen saiatzen da.</span><span class="sxs-lookup"><span data-stu-id="4b19f-126">If you select **Match**, the system tries to match an existing expense to the receipt.</span></span>

## <a name="installation"></a><span data-ttu-id="4b19f-127">Instalazioa</span><span class="sxs-lookup"><span data-stu-id="4b19f-127">Installation</span></span>

<span data-ttu-id="4b19f-128">Gastu-gaitasun aurreratu hauek erabiltzeko, instalatu Microsoft Dynamics 365 Finance-rako Gastuen kudeaketa-zerbitzua gehigarria, eta aktibatu funtzioak zure instantzian.</span><span class="sxs-lookup"><span data-stu-id="4b19f-128">To use these advanced expense capabilities, install the Expense Management Service add-in for Microsoft Dynamics 365 Finance, and turn on the features in your instance.</span></span> <span data-ttu-id="4b19f-129">Gehigarria zure proiektuan sar dezakezu Microsoft Dynamics Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="4b19f-129">You can access the add-in from your project in Microsoft Dynamics Lifecycle Services (LCS).</span></span>

1. <span data-ttu-id="4b19f-130">Hasi saioa LCS-n eta ireki nahi duzun ingurunea.</span><span class="sxs-lookup"><span data-stu-id="4b19f-130">Sign in to LCS, and open the desired environment.</span></span>
2. <span data-ttu-id="4b19f-131">Joan **Xehetasun guztiak**.</span><span class="sxs-lookup"><span data-stu-id="4b19f-131">Go to **Full details**.</span></span>
3. <span data-ttu-id="4b19f-132">Aukeratu **Mantendu** edo joan behera **Ingurumeneko gehigarriak** FastTab.</span><span class="sxs-lookup"><span data-stu-id="4b19f-132">Select **Maintain**, or scroll down to the **Environment add-ins** FastTab.</span></span>
4. <span data-ttu-id="4b19f-133">Aukeratu **Instalatu gehigarri berria**.</span><span class="sxs-lookup"><span data-stu-id="4b19f-133">Select **Install a new add-in**.</span></span>
5. <span data-ttu-id="4b19f-134">Hautatu **Gastuen kudeaketa-zerbitzua**.</span><span class="sxs-lookup"><span data-stu-id="4b19f-134">Select **Expense Management Service**.</span></span>
6. <span data-ttu-id="4b19f-135">Jarraitu instalazio gida eta onartu baldintzak.</span><span class="sxs-lookup"><span data-stu-id="4b19f-135">Follow the installation guide, and agree to the terms and conditions.</span></span>
7. <span data-ttu-id="4b19f-136">Hautatu **Instalatu**</span><span class="sxs-lookup"><span data-stu-id="4b19f-136">Select **Install**.</span></span>

<span data-ttu-id="4b19f-137">Urtean **Ezaugarrien kudeaketa** laneko eremua, aktibatu ezaugarri hauek:</span><span class="sxs-lookup"><span data-stu-id="4b19f-137">In the **Feature management** workspace, turn on the following features:</span></span>

- <span data-ttu-id="4b19f-138">Gastu-txostenen itxura berria</span><span class="sxs-lookup"><span data-stu-id="4b19f-138">Expense reports re-imagined</span></span>
- <span data-ttu-id="4b19f-139">Lotu automatikoki eta sortu gastua jasotzetik</span><span class="sxs-lookup"><span data-stu-id="4b19f-139">Auto-match and create expense from receipt</span></span>

<span data-ttu-id="4b19f-140">Ezaugarri hauek aktibatzean ekintza hauek gertatzen dira:</span><span class="sxs-lookup"><span data-stu-id="4b19f-140">When you turn on these features the following actions occur:</span></span>

- <span data-ttu-id="4b19f-141">Daudenak **Gastuen kudeaketa** lan-eremua lan-eremu berriarekin ordezkatzen da.</span><span class="sxs-lookup"><span data-stu-id="4b19f-141">The existing **Expense management** workspace is replaced with the new workspace.</span></span>
- <span data-ttu-id="4b19f-142">Gastu eremuen ikusgarritasunerako menu elementu berria gehitzen da.</span><span class="sxs-lookup"><span data-stu-id="4b19f-142">A new menu item for expense field visibility is added.</span></span>
- <span data-ttu-id="4b19f-143">Lehenengoa ireki dezakezu **Gastuen txostenak** orrialdera joanda **Gastuen kudeaketa> Nire gastuak> Gastuen txostenak**.</span><span class="sxs-lookup"><span data-stu-id="4b19f-143">You can still open the former **Expense reports** page by going to **Expense management > My expenses > Expense reports**.</span></span>
- <span data-ttu-id="4b19f-144">Lan-fluxuek eta edozein onarpenek lehendik dauden gastuen txostenen orrialdera eramaten zaituzte.</span><span class="sxs-lookup"><span data-stu-id="4b19f-144">Workflows and any approvals still take you to the existing expense reports page.</span></span>
- <span data-ttu-id="4b19f-145">Ordainagiriak bidez prozesatuko dira Microsoft Azure Cognitive Services-k eta metadatuak erauzi eta gehituko dira.</span><span class="sxs-lookup"><span data-stu-id="4b19f-145">Receipts will be processed through Microsoft Azure Cognitive Services, and metadata will be extracted and added.</span></span>
- <span data-ttu-id="4b19f-146">Erantsitako loturarik gabeko ordainagiriak biltzen dituen gastu-txostena sortzeko aukera ematen duen aukera gehitzen da.</span><span class="sxs-lookup"><span data-stu-id="4b19f-146">An option is added that lets you create an expense report that includes matched unattached receipts.</span></span>
- <span data-ttu-id="4b19f-147">Gastu txostenetan gehitzen den aukera batek ordainagiri batetik gastu lerro bat sortzeko aukera ematen du edo lehendik dagoen ordainagiria lehendik dagoen gastu lerro batekin parekatzen saiatzen da.</span><span class="sxs-lookup"><span data-stu-id="4b19f-147">An option that is added to expense reports lets you create an expense line from a receipt, or attempts to match an existing receipt to an existing expense line.</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="4b19f-148">Ohiko galderak</span><span class="sxs-lookup"><span data-stu-id="4b19f-148">Frequently asked questions</span></span>

<span data-ttu-id="4b19f-149">**Microsoft-ek nire datuak erabiltzen ditu bere modeloetarako?**</span><span class="sxs-lookup"><span data-stu-id="4b19f-149">**Does Microsoft use my data for its models?**</span></span>

<span data-ttu-id="4b19f-150">Ez, Microsoft-ek Ikaskuntza automatiko eredu orokorra eraiki du ordainagiriak prozesatzeko zerbitzurako.</span><span class="sxs-lookup"><span data-stu-id="4b19f-150">No, Microsoft has built a general machine learning model for its receipt processing service.</span></span> <span data-ttu-id="4b19f-151">Eredu hau ez dago kargatutako ordainagirietan oinarrituta.</span><span class="sxs-lookup"><span data-stu-id="4b19f-151">This model isn't based on the receipts that you upload.</span></span>

<span data-ttu-id="4b19f-152">**Non dago erabilgarri eta prozesatu eginbide hau?**</span><span class="sxs-lookup"><span data-stu-id="4b19f-152">**Where is this feature available and processed?**</span></span>

<span data-ttu-id="4b19f-153">Gaur egun, Estatu Batuak onartzen dira.</span><span class="sxs-lookup"><span data-stu-id="4b19f-153">Currently, the United States is supported.</span></span>

<span data-ttu-id="4b19f-154">**Nora doaz nire ordainagiriak?**</span><span class="sxs-lookup"><span data-stu-id="4b19f-154">**Where do my receipts go?**</span></span>

<span data-ttu-id="4b19f-155">Finance-k Cognitive Service harremanetan jarriko da eremuko datuak ateratzeko.</span><span class="sxs-lookup"><span data-stu-id="4b19f-155">Finance will contact Cognitive Services to extract the field data.</span></span> <span data-ttu-id="4b19f-156">Cognitive Service-k zure ordainagiriaren kopia mantenduko dute 24 orduz gehienez prozesamendua gertatu bitartean.</span><span class="sxs-lookup"><span data-stu-id="4b19f-156">Cognitive Services will retain a copy of your receipt for up to 24 hours while processing occurs.</span></span> <span data-ttu-id="4b19f-157">Prozesamendua amaitu ondoren, Cognitive Services-ek ordainagiria kenduko du.</span><span class="sxs-lookup"><span data-stu-id="4b19f-157">After processing is completed, Cognitive Services will remove the receipt.</span></span> <span data-ttu-id="4b19f-158">Ordainagiriak Finantzan gordetzen dira oraindik.</span><span class="sxs-lookup"><span data-stu-id="4b19f-158">Receipts are still stored in Finance.</span></span>

<span data-ttu-id="4b19f-159">Informazio gehiagorako, ikus [Gaitu ordainagiriak ulertzeko inprimakia hautagaiaren gaitasun berriarekin](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span><span class="sxs-lookup"><span data-stu-id="4b19f-159">For more information, see [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span></span>