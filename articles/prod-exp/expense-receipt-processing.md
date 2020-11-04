---
title: Gastuen agiriak prozesatzea
description: Gai honetan ordainagirien karaktereen ezagutza optikoa (OCR) prozesatzeari buruzko informazioa ematen da. Eginbide hau Microsoft Dynamics 365 Finance-en sortutako gastuen txostenak sortzerakoan erabiltzailearen esperientzia hobetzeko diseinatuta dago.
author: stsporen
manager: AnnBe
ms.date: 05/14/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Operations, Core
ms.search.region: Global
ms.author: stsporen
ms.search.validFrom: 2019-11-20
ms.dyn365.ops.version: 10.0.8
ms.openlocfilehash: 31c08ea264e6caec3217f4b424275495f39123e3
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071194"
---
# <a name="expense-receipt-processing"></a><span data-ttu-id="aa1e6-104">Gastuen agiriak prozesatzea</span><span class="sxs-lookup"><span data-stu-id="aa1e6-104">Expense receipt processing</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="aa1e6-105">Gastuen sarrera hobetu da ordainagirien karaktereen ezagutza optikoa (OCR) prozesuaren bidez.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-105">Expense entry has been enhanced through the introduction of optical character recognition (OCR) processing for receipts.</span></span> <span data-ttu-id="aa1e6-106">Eginbide hau sortutako gastuen txostenak sortzerakoan erabiltzailearen esperientzia hobetzeko diseinatuta dago.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-106">This feature is designed to improve the user experience when expense reports are created.</span></span>

## <a name="key-features"></a><span data-ttu-id="aa1e6-107">Eginbide nagusiak</span><span class="sxs-lookup"><span data-stu-id="aa1e6-107">Key features</span></span>

- <span data-ttu-id="aa1e6-108">Merkatariaren izena, data eta zenbateko osoa ateratzen dira ordainagirietatik.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-108">The merchant name, date, and total amount are extracted from receipts.</span></span>
- <span data-ttu-id="aa1e6-109">Eginbidea erantsitako ordainagiriak lotu gabeko gastuen transakzioekin parekatzen saiatzen da.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-109">The feature tries to match unattached receipts to unattached expense transactions.</span></span>
- <span data-ttu-id="aa1e6-110">Erabiltzaileek ordainagirietatik eskuz sartutako gastu transakzioak sor ditzakete.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-110">Users can create manually entered expense transactions from receipts.</span></span>

## <a name="usage-examples"></a><span data-ttu-id="aa1e6-111">Erabilera-adibideak</span><span class="sxs-lookup"><span data-stu-id="aa1e6-111">Usage examples</span></span>

<span data-ttu-id="aa1e6-112">Gastu txostena sortzen denean kreditu txartelarekin egindako transakzioak jasotzen dituzten ordainagiriak automatikoki eransteko, egin hau:</span><span class="sxs-lookup"><span data-stu-id="aa1e6-112">To automatically attach receipts that include credit card transactions when an expense report is created, do the following:</span></span>

  1. <span data-ttu-id="aa1e6-113">Ireki **Gastuen kudeaketa** lan eremua.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-113">Open the **Expense management** workspace.</span></span>
  2. <span data-ttu-id="aa1e6-114">Gainean **Ordainagiriak** fitxa, egiaztatu lotu gabeko ordainagiriak badirela.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-114">On the **Receipts** tab, verify that unattached receipts exist.</span></span> <span data-ttu-id="aa1e6-115">Ordainagiriak ere karga ditzakezu **Ordainagiriak** fitxa.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-115">You can also upload receipts on the **Receipts** tab.</span></span>
  3. <span data-ttu-id="aa1e6-116">**Gastuak** fitxan, egiaztatu lotu gabeko gastuak badirela.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-116">On the **Expenses** tab, verify that unattached expenses exist.</span></span> <span data-ttu-id="aa1e6-117">Normalean, gastuen administratzaileak gastu horiek kreditu txartelaren hornitzailearen eskutik inportatzen ditu.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-117">Typically, the expense administrator imports these expenses from the credit card provider.</span></span>
  4. <span data-ttu-id="aa1e6-118">Aukeratu **Gastu txosten berria**.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-118">Select **New expense report**.</span></span> <span data-ttu-id="aa1e6-119">Kontuan izan gastuak eta ordainagiriak sar ditzakezula, orain ere, gastuen txostena sortzen duzunean.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-119">Notice that you can include expenses, and receipts, now as well, when you create an expense report.</span></span> <span data-ttu-id="aa1e6-120">Gastuak eta ordainagiriak gehitzen badituzu, ordainagirien gastuen pareko automatikoki abiaraziko da.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-120">If you add both expenses and receipts, automatic matching of the receipts against the expenses is triggered.</span></span>

<span data-ttu-id="aa1e6-121">Gastua sortzeko edo ordainagiriaren gastuarekin bat egiteko, egin hau:</span><span class="sxs-lookup"><span data-stu-id="aa1e6-121">To create an expense, or match an expense from a receipt, do the following:</span></span>

  1. <span data-ttu-id="aa1e6-122">Gastu txosten batean, **Ordainagiriak** fitxa, erantsi ordainagiria hautatuz **Gehitu ordainagiriak**.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-122">On an expense report, on the **Receipts** tab, attach a receipt by selecting **Add receipts**.</span></span>
  2. <span data-ttu-id="aa1e6-123">Ordainagiriaren kargatutako irudiaren azpian, ohar ezazu **Sortu** eta **Partidua** aukerak.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-123">Under the uploaded image of the receipt, notice the **Create** and **Match** options.</span></span>

      - <span data-ttu-id="aa1e6-124">Aukeratu **Sortu** eskuz sartutako gastuen transakzioa sortzeko eta ordainagiritik ateratako balioak betetzeko.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-124">Select **Create** to create a manually entered expense transaction and fill in the values that are extracted from the receipt.</span></span>
      - <span data-ttu-id="aa1e6-125">Hautatzen baduzu **Partidua** , sistema lehendik zegoen gastua ordainagiriarekin parekatzen saiatzen da.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-125">If you select **Match** , the system tries to match an existing expense to the receipt.</span></span>

## <a name="installation"></a><span data-ttu-id="aa1e6-126">Instalazioa</span><span class="sxs-lookup"><span data-stu-id="aa1e6-126">Installation</span></span>

<span data-ttu-id="aa1e6-127">Ezaugarri hau **Gastuen txostenak berriro imajinatu ziren** funtzioa gastuen esperientzia errazten laguntzeko.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-127">This feature works in combination with the **Expense reports re-imagined** feature to help simplify the expense experience.</span></span> <span data-ttu-id="aa1e6-128">Ezaugarri hau Tier 2+ inguruneetarako bakarrik dago erabilgarri, Sandbox eta Production.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-128">This feature is only available for Tier 2+ environments, which are Sandbox and Production.</span></span>

<span data-ttu-id="aa1e6-129">Gastu-gaitasun aurreratu hauek erabiltzeko, instalatu Microsoft Dynamics 365 Finance-rako Gastuen kudeaketa-zerbitzua gehigarria, eta aktibatu funtzioak zure instantzian.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-129">To use these advanced expense capabilities, install the Expense Management Service add-in for Microsoft Dynamics 365 Finance, and turn on the features in your instance.</span></span> <span data-ttu-id="aa1e6-130">Gehigarria zure proiektuan sar dezakezu Microsoft Dynamics Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="aa1e6-130">You can access the add-in from your project in Microsoft Dynamics Lifecycle Services (LCS).</span></span>

1. <span data-ttu-id="aa1e6-131">Hasi saioa LCS-n eta ireki nahi duzun ingurunea.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-131">Sign in to LCS, and open the desired environment.</span></span>
2. <span data-ttu-id="aa1e6-132">Joan **Xehetasun guztiak**.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-132">Go to **Full details**.</span></span>
3. <span data-ttu-id="aa1e6-133">Aukeratu **Mantendu** edo joan behera **Ingurumeneko gehigarriak** FastTab.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-133">Select **Maintain** , or scroll down to the **Environment add-ins** FastTab.</span></span>
4. <span data-ttu-id="aa1e6-134">Aukeratu **Instalatu gehigarri berria**.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-134">Select **Install a new add-in**.</span></span>
5. <span data-ttu-id="aa1e6-135">Hautatu **Gastuen kudeaketa-zerbitzua**.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-135">Select **Expense Management Service**.</span></span>
6. <span data-ttu-id="aa1e6-136">Jarraitu instalazio gida eta onartu baldintzak.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-136">Follow the installation guide, and agree to the terms and conditions.</span></span>
7. <span data-ttu-id="aa1e6-137">Hautatu **Instalatu**</span><span class="sxs-lookup"><span data-stu-id="aa1e6-137">Select **Install**.</span></span>

<span data-ttu-id="aa1e6-138">Urtean **Ezaugarrien kudeaketa** laneko eremua, aktibatu ezaugarri hauek:</span><span class="sxs-lookup"><span data-stu-id="aa1e6-138">In the **Feature management** workspace, turn on the following features:</span></span>

- <span data-ttu-id="aa1e6-139">Gastu-txostenen itxura berria</span><span class="sxs-lookup"><span data-stu-id="aa1e6-139">Expense reports re-imagined</span></span>
- <span data-ttu-id="aa1e6-140">Lotu automatikoki eta sortu gastua jasotzetik</span><span class="sxs-lookup"><span data-stu-id="aa1e6-140">Auto-match and create expense from receipt</span></span>

<span data-ttu-id="aa1e6-141">Ezaugarri hauek aktibatzean ekintza hauek gertatzen dira:</span><span class="sxs-lookup"><span data-stu-id="aa1e6-141">When you turn on these features the following actions occur:</span></span>

- <span data-ttu-id="aa1e6-142">Daudenak **Gastuen kudeaketa** lan-eremua lan-eremu berriarekin ordezkatzen da.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-142">The existing **Expense management** workspace is replaced with the new workspace.</span></span>
- <span data-ttu-id="aa1e6-143">Gastu eremuen ikusgarritasunerako menu elementu berria gehitzen da.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-143">A new menu item for expense field visibility is added.</span></span>
- <span data-ttu-id="aa1e6-144">Lehenengoa ireki dezakezu **Gastuen txostenak** orrialdera joanda **Gastuen kudeaketa> Nire gastuak> Gastuen txostenak**.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-144">You can still open the former **Expense reports** page by going to **Expense management > My expenses > Expense reports**.</span></span>
- <span data-ttu-id="aa1e6-145">Lan-fluxuek eta edozein onarpenek lehendik dauden gastuen txostenen orrialdera eramaten zaituzte.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-145">Workflows and any approvals still take you to the existing expense reports page.</span></span>
- <span data-ttu-id="aa1e6-146">Ordainagiriak bidez prozesatuko dira Microsoft Azure Cognitive Services-k eta metadatuak erauzi eta gehituko dira.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-146">Receipts will be processed through Microsoft Azure Cognitive Services, and metadata will be extracted and added.</span></span>
- <span data-ttu-id="aa1e6-147">Erantsitako loturarik gabeko ordainagiriak biltzen dituen gastu-txostena sortzeko aukera ematen duen aukera gehitzen da.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-147">An option is added that lets you create an expense report that includes matched unattached receipts.</span></span>
- <span data-ttu-id="aa1e6-148">Gastu txostenetan gehitzen den aukera batek ordainagiri batetik gastu lerro bat sortzeko aukera ematen du edo lehendik dagoen ordainagiria lehendik dagoen gastu lerro batekin parekatzen saiatzen da.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-148">An option that is added to expense reports lets you create an expense line from a receipt, or attempts to match an existing receipt to an existing expense line.</span></span>

<span data-ttu-id="aa1e6-149">Gastuen txostenak berriro imajinatutako eginbideari buruzko informazio gehiago lortzeko, ikusi [Gastuen txostenak berriro pentsatu ziren](ExpenseWorkspaceNew.md).</span><span class="sxs-lookup"><span data-stu-id="aa1e6-149">For more information about the Expense reports re-imagined feature, see [Expense reports reimagined](ExpenseWorkspaceNew.md).</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="aa1e6-150">Ohiko galderak</span><span class="sxs-lookup"><span data-stu-id="aa1e6-150">Frequently asked questions</span></span>

<span data-ttu-id="aa1e6-151">**Microsoft-ek nire datuak erabiltzen ditu bere modeloetarako?**</span><span class="sxs-lookup"><span data-stu-id="aa1e6-151">**Does Microsoft use my data for its models?**</span></span>

<span data-ttu-id="aa1e6-152">Ez, Microsoft-ek Ikaskuntza automatiko eredu orokorra eraiki du ordainagiriak prozesatzeko zerbitzurako.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-152">No, Microsoft has built a general machine learning model for its receipt processing service.</span></span> <span data-ttu-id="aa1e6-153">Eredu hau ez dago kargatutako ordainagirietan oinarrituta.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-153">This model isn't based on the receipts that you upload.</span></span>

<span data-ttu-id="aa1e6-154">**Non dago erabilgarri eta prozesatu eginbide hau?**</span><span class="sxs-lookup"><span data-stu-id="aa1e6-154">**Where is this feature available and processed?**</span></span>

<span data-ttu-id="aa1e6-155">Gaur egun, Estatu Batuak onartzen dira.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-155">Currently, the United States is supported.</span></span>

<span data-ttu-id="aa1e6-156">**Nora doaz nire ordainagiriak?**</span><span class="sxs-lookup"><span data-stu-id="aa1e6-156">**Where do my receipts go?**</span></span>

<span data-ttu-id="aa1e6-157">Finance-k Cognitive Service harremanetan jarriko da eremuko datuak ateratzeko.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-157">Finance will contact Cognitive Services to extract the field data.</span></span> <span data-ttu-id="aa1e6-158">Cognitive Service-k zure ordainagiriaren kopia mantenduko dute 24 orduz gehienez prozesamendua gertatu bitartean.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-158">Cognitive Services will retain a copy of your receipt for up to 24 hours while processing occurs.</span></span> <span data-ttu-id="aa1e6-159">Prozesamendua amaitu ondoren, Cognitive Services-ek ordainagiria kenduko du.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-159">After processing is completed, Cognitive Services will remove the receipt.</span></span> <span data-ttu-id="aa1e6-160">Ordainagiriak Finantzan gordetzen dira oraindik.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-160">Receipts are still stored in Finance.</span></span>

<span data-ttu-id="aa1e6-161">Informazio gehiagorako, ikus [Gaitu ordainagiriak ulertzeko inprimakia hautagaiaren gaitasun berriarekin](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span><span class="sxs-lookup"><span data-stu-id="aa1e6-161">For more information, see [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span></span>
