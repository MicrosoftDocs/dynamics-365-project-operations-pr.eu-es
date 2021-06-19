---
title: Konfiguratu kreditu-txartelaren integrazioa
description: Gai honetan gastuekin lotutako kreditu txarteleko transakzioekin nola lan egin azaltzen da.
author: suvaidya
ms.date: 04/02/2021
ms.topic: article
ms.prod: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 3555e894e206c2aafb30b0df1e52efadd69b0713
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001785"
---
# <a name="set-up-credit-card-integration"></a><span data-ttu-id="5285d-103">Konfiguratu kreditu-txartelaren integrazioa</span><span class="sxs-lookup"><span data-stu-id="5285d-103">Set up credit card integration</span></span>

<span data-ttu-id="5285d-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="5285d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5285d-105">Gastuei lotutako kreditu txartelaren eragiketak konfiguratu daitezke, aldian-aldiko programazioan automatikoki inportatzeko.</span><span class="sxs-lookup"><span data-stu-id="5285d-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="5285d-106">Bestela, transakzioak eskuz inporta daitezke beharrezkoak diren neurrian.</span><span class="sxs-lookup"><span data-stu-id="5285d-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="5285d-107">Kreditu txartelaren transakzioak kreditu-txartelaren transakzioen datuen entitatearen bidez inportatzen dira.</span><span class="sxs-lookup"><span data-stu-id="5285d-107">The credit card transactions are imported through the credit card transactions data entity.</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="5285d-108">Inportatu kreditu txartelaren eragiketak</span><span class="sxs-lookup"><span data-stu-id="5285d-108">Import credit card transactions</span></span>

<span data-ttu-id="5285d-109">Kreditu txartelaren eragiketak inportatzeko, jarraitu urrats hauei:</span><span class="sxs-lookup"><span data-stu-id="5285d-109">To import credit card transactions, follow these steps:</span></span>

1. <span data-ttu-id="5285d-110">**Kreditu-txartelaren eragiketak** orrialdean, hautatu **Inportazio transakzioak**.</span><span class="sxs-lookup"><span data-stu-id="5285d-110">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="5285d-111">Datuen kudeaketa lehen aldiz irekitzen ari bazara, sistemak datu-entitateen zerrenda eguneratu beharko du jarraitu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="5285d-111">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="5285d-112">**Izena** eremuan, sartu inportazio lanaren deskribapen bakarra.</span><span class="sxs-lookup"><span data-stu-id="5285d-112">In the **Name** field, enter a unique description for the import job.</span></span>
3. <span data-ttu-id="5285d-113">**Iturriaren datuen formatua** eremuan, hautatu inportatu beharreko kreditu txartelaren transakzioak dituen fitxategiaren formatua.</span><span class="sxs-lookup"><span data-stu-id="5285d-113">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="5285d-114">Hautatu **Kargatu** eta, ondoren, bilatu eta hautatu inportatzeko fitxategia.</span><span class="sxs-lookup"><span data-stu-id="5285d-114">Select **Upload**, and then find and select the file to import.</span></span>
5. <span data-ttu-id="5285d-115">Fitxategia kargatu ondoren, baliozkotu kreditu txartelaren transakzio fitxategiaren mapak eta kreditu-txartelaren transakzioen datu entitatearen zutabeak hautatu **Ikusi mapa** esteka fitxan.</span><span class="sxs-lookup"><span data-stu-id="5285d-115">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="5285d-116">Kartografia akatsak badaude, edo mapaketa aldatu behar baduzu, egin maparen aldaketak **Mapen bistaratzea** fitxa edo **Kartografia xehetasunak** fitxa.</span><span class="sxs-lookup"><span data-stu-id="5285d-116">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="5285d-117">Kreditu txartelaren eragiketak automatizatzeko, hautatu **Sortu aldizkako datuen lana**.</span><span class="sxs-lookup"><span data-stu-id="5285d-117">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="5285d-118">Kreditu txartelaren eragiketak zenbat aldiz inportatu behar diren zehazten duen errepikapena ezar dezakezu.</span><span class="sxs-lookup"><span data-stu-id="5285d-118">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="5285d-119">Bukatu duzunean, hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="5285d-119">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="5285d-120">Aukeratutako fitxategia orain inportatzeko, hautatu **Inportatu**.</span><span class="sxs-lookup"><span data-stu-id="5285d-120">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="5285d-121">Inportazioan zehar akatsak gertatzen badira, exekuzio erregistroa edo faseko datuak ikus ditzakezu inportazio arrakastatsua ziurtatzen laguntzeko konpondu behar dituzun akatsak ikusteko.</span><span class="sxs-lookup"><span data-stu-id="5285d-121">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help ensure a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="5285d-122">Fitxategi formatu bat baino gehiago inportatu behar badituzu, inportazio lan bereiziak sortu behar dituzu formatu mota bakoitzerako.</span><span class="sxs-lookup"><span data-stu-id="5285d-122">If you need to import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="5285d-123">Kargatu bajako langileentzako kreditu txartelaren eragiketak</span><span class="sxs-lookup"><span data-stu-id="5285d-123">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="5285d-124">Langilearen erregistroa amaitu ondoren, langilearen Active Directory domeinu zerbitzuak (AD DS) kontua desgaituta dago.</span><span class="sxs-lookup"><span data-stu-id="5285d-124">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="5285d-125">Hala ere, baliteke kreditu txartelarekin egindako transakzio aktiboak oraindik gastatu eta itzuli behar direnak.</span><span class="sxs-lookup"><span data-stu-id="5285d-125">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="5285d-126">**Kreditu txartelaren eragiketak** orrialdean, langilea berriro esleitu ahal izango duzu lotutako langilea amaitu den kreditu txartelarekin egindako edozein transakzioetarako.</span><span class="sxs-lookup"><span data-stu-id="5285d-126">On the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="5285d-127">Aukeratu kreditu txartelaren transakzio bat edo gehiago, eta hautatu **Transakzioak berriro esleitu**.</span><span class="sxs-lookup"><span data-stu-id="5285d-127">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="5285d-128">Kreditu txartelaren eragiketak esleitzeko beste langile bat hauta dezakezu.</span><span class="sxs-lookup"><span data-stu-id="5285d-128">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="5285d-129">Kreditu txartelaren eragiketak berriro esleitu ondoren, gastuen txostena aukeratu eta gastuen txostena itzultzeko ohiko prozesuaren bidez ordain daitezke.</span><span class="sxs-lookup"><span data-stu-id="5285d-129">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>

## <a name="delete-credit-card-transactions"></a><span data-ttu-id="5285d-130">Ezabatu kreditu txartelaren eragiketak</span><span class="sxs-lookup"><span data-stu-id="5285d-130">Delete credit card transactions</span></span> 

<span data-ttu-id="5285d-131">Batzuetan, kreditu txartelarekin egindako transakzioak inportatu ondoren, baliteke transakzio batzuk ezabatu behar izatea.</span><span class="sxs-lookup"><span data-stu-id="5285d-131">Sometimes, after credit card transactions are imported, certain transactions may need to be deleted.</span></span> <span data-ttu-id="5285d-132">Gerta liteke transakzioak bikoiztuak direlako edo baliteke datuak zehatzak ez izateagatik.</span><span class="sxs-lookup"><span data-stu-id="5285d-132">This could be because the transactions are duplicates or because the data might isn't accurate.</span></span> <span data-ttu-id="5285d-133">Administratzaileek **"Ezabatu kreditu txartelaren transakzioak"** funtzioa diren kreditu txarteleko eragiketak hautatu eta ezabatzeko **erantsita ez** gastuen txosten batera.</span><span class="sxs-lookup"><span data-stu-id="5285d-133">Admins can use the **"Delete credit card transactions"** feature to select and delete credit card transactions that are **not attached** to an expense report.</span></span> 

1. <span data-ttu-id="5285d-134">Joan **Aldizkako zereginak** > **Ezabatu kreditu txartelaren eragiketak**.</span><span class="sxs-lookup"><span data-stu-id="5285d-134">Go to **Periodic tasks** > **Delete credit card transactions**.</span></span>
2. <span data-ttu-id="5285d-135">Aukeratu **Iragazi** eta informazioa eman erregistroak identifikatzeko.</span><span class="sxs-lookup"><span data-stu-id="5285d-135">Select **Filter** and provide information to identify the records to include.</span></span>
3. <span data-ttu-id="5285d-136">Hautatu **Ados** erregistroak ezabatzeko.</span><span class="sxs-lookup"><span data-stu-id="5285d-136">Select **OK** to delete the records.</span></span> 

[!INCLUDE[footer-include](../includes/footer-banner.md)]
