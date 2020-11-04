---
title: Konfiguratu kreditu-txartelaren integrazioa
description: Gai honetan gastuekin lotutako kreditu txartelaren eragiketak nola inportatu eta nola mantendu azaltzen da.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 12c7971204b485ee7cb222cd9cffdfdfde93dcf4
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070999"
---
# <a name="set-up-credit-card-integration"></a><span data-ttu-id="6e64d-103">Konfiguratu kreditu-txartelaren integrazioa</span><span class="sxs-lookup"><span data-stu-id="6e64d-103">Set up credit card integration</span></span>

<span data-ttu-id="6e64d-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="6e64d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="6e64d-105">Gastuei lotutako kreditu txartelaren eragiketak konfiguratu daitezke, aldian-aldiko programazioan automatikoki inportatzeko.</span><span class="sxs-lookup"><span data-stu-id="6e64d-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="6e64d-106">Bestela, transakzioak eskuz inporta daitezke beharrezkoak diren neurrian.</span><span class="sxs-lookup"><span data-stu-id="6e64d-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="6e64d-107">Kreditu txartelaren transakzioak Kreditu txartelaren transakzioen datuen entitatearen bidez inportatzen dira.</span><span class="sxs-lookup"><span data-stu-id="6e64d-107">The credit card transactions are imported through the Credit card transactions data entity.</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="6e64d-108">Inportatu kreditu txartelaren eragiketak</span><span class="sxs-lookup"><span data-stu-id="6e64d-108">Import credit card transactions</span></span>

1. <span data-ttu-id="6e64d-109">**Kreditu-txartelaren eragiketak** orrialdean, hautatu **Inportazio transakzioak**.</span><span class="sxs-lookup"><span data-stu-id="6e64d-109">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="6e64d-110">Datuen kudeaketa lehen aldiz irekitzen ari bazara, sistemak datu-entitateen zerrenda eguneratu beharko du jarraitu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="6e64d-110">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="6e64d-111">**Izena** eremuan, sartu inportazio lanaren deskribapen bakarra.</span><span class="sxs-lookup"><span data-stu-id="6e64d-111">In the **Name** field, enter a unique description of the import job.</span></span>
3. <span data-ttu-id="6e64d-112">**Iturriaren datuen formatua** eremuan, hautatu inportatu beharreko kreditu txartelaren transakzioak dituen fitxategiaren formatua.</span><span class="sxs-lookup"><span data-stu-id="6e64d-112">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="6e64d-113">Hautatu **Kargatu** eta, ondoren, bilatu eta hautatu inportatzeko fitxategia.</span><span class="sxs-lookup"><span data-stu-id="6e64d-113">Select **Upload** , and then find and select the file to import.</span></span>
5. <span data-ttu-id="6e64d-114">Fitxategia kargatu ondoren, baliozkotu kreditu txartelaren transakzio fitxategiaren mapak eta Kreditu txartelaren transakzioen datu entitatearen zutabeak hautatu **Ikusi mapa** esteka fitxan.</span><span class="sxs-lookup"><span data-stu-id="6e64d-114">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the Credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="6e64d-115">Kartografia akatsak badaude, edo mapaketa aldatu behar baduzu, egin maparen aldaketak **Mapen bistaratzea** fitxa edo **Kartografia xehetasunak** fitxa.</span><span class="sxs-lookup"><span data-stu-id="6e64d-115">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="6e64d-116">Kreditu txartelaren eragiketak automatizatzeko, hautatu **Sortu aldizkako datuen lana**.</span><span class="sxs-lookup"><span data-stu-id="6e64d-116">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="6e64d-117">Kreditu txartelaren eragiketak zenbat aldiz inportatu behar diren zehazten duen errepikapena ezar dezakezu.</span><span class="sxs-lookup"><span data-stu-id="6e64d-117">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="6e64d-118">Bukatu duzunean, hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="6e64d-118">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="6e64d-119">Aukeratutako fitxategia orain inportatzeko, hautatu **Inportatu**.</span><span class="sxs-lookup"><span data-stu-id="6e64d-119">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="6e64d-120">Inportazioan zehar akatsak gertatzen badira, exekuzio erregistroa edo faseko datuak ikus ditzakezu inportazio arrakastatsua bermatzen laguntzeko konpondu behar dituzun akatsak ikusteko.</span><span class="sxs-lookup"><span data-stu-id="6e64d-120">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help guarantee a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="6e64d-121">Fitxategi formatu bat baino gehiago inportatu behar badituzu, inportazio lan bereiziak sortu behar dituzu formatu mota bakoitzerako.</span><span class="sxs-lookup"><span data-stu-id="6e64d-121">If you must import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="6e64d-122">Kargatu bajako langileentzako kreditu txartelaren eragiketak</span><span class="sxs-lookup"><span data-stu-id="6e64d-122">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="6e64d-123">Langilearen erregistroa amaitu ondoren, langilearen Active Directory domeinu zerbitzuak (AD DS) kontua desgaituta dago.</span><span class="sxs-lookup"><span data-stu-id="6e64d-123">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="6e64d-124">Hala ere, baliteke kreditu txartelarekin egindako transakzio aktiboak oraindik gastatu eta itzuli behar direnak.</span><span class="sxs-lookup"><span data-stu-id="6e64d-124">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="6e64d-125">Tik **Kreditu txartelaren eragiketak** orrialdean, langilea berriro esleitu ahal izango duzu lotutako langilea amaitu den kreditu txartelarekin egindako edozein transakzioetarako.</span><span class="sxs-lookup"><span data-stu-id="6e64d-125">From the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="6e64d-126">Aukeratu kreditu txartelaren transakzio bat edo gehiago, eta hautatu **Transakzioak berriro esleitu**.</span><span class="sxs-lookup"><span data-stu-id="6e64d-126">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="6e64d-127">Kreditu txartelaren eragiketak esleitzeko beste langile bat hauta dezakezu.</span><span class="sxs-lookup"><span data-stu-id="6e64d-127">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="6e64d-128">Kreditu txartelaren eragiketak berriro esleitu ondoren, gastuen txostena aukeratu eta gastuen txostena itzultzeko ohiko prozesuaren bidez ordain daitezke.</span><span class="sxs-lookup"><span data-stu-id="6e64d-128">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>
