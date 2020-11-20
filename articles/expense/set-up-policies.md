---
title: Gastuen politikak zehaztu
description: Zure langileek gastuen txostenak eta bidaia-eskaerak sartu eta bidaltzerakoan jarraitu behar dituzten gastu-politikak defini ditzakezu.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: c55cec132649daf9ee08ea4d8db3668860247934
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4128403"
---
# <a name="define-expense-policies"></a><span data-ttu-id="d7dfc-103">Gastuen politikak zehaztu</span><span class="sxs-lookup"><span data-stu-id="d7dfc-103">Define expense policies</span></span>

<span data-ttu-id="d7dfc-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="d7dfc-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d7dfc-105">Zure langileek txostenak eta bidaia-eskaerak sartu eta bidaltzerakoan jarraitu behar dituzten gastu-politikak defini ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-105">You can define policies that your workers must follow when entering and submitting expense reports and travel requisitions.</span></span>         
<span data-ttu-id="d7dfc-106">Gastu politikak ezartzeak gastuak modu eraginkorrean kudeatzen lagun zaitzake.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-106">Implementing expense policies can help you manage expenses effectively.</span></span>         

<span data-ttu-id="d7dfc-107">Adibidez, New Yorkeko hoteletako gastuei buruzko politika bat ezar dezakezu, gaueko gastuak ezin dituela USD 250 baino gehiago adierazi.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-107">For example, you can set a policy for hotel expenses in New York City, which states that the per night expense cannot exceed USD 250.</span></span>       
<span data-ttu-id="d7dfc-108">Langile batek gastuen txostena edo bidaiaren eskaera aurkezten badu gelaren tarifak zenbateko hori gainditzen duenean, sistemak horren berri emango dio</span><span class="sxs-lookup"><span data-stu-id="d7dfc-108">If a worker submits an expense report or travel requisition where the room rate exceeds this amount, the system will notify the</span></span>         
<span data-ttu-id="d7dfc-109">Langileak gastuaren polizaren zenbatekoa gainditu duela.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-109">worker that the policy amount for the expense has been exceeded.</span></span> <span data-ttu-id="d7dfc-110">Langileak zu jasotzean jasoko duen mezua konfigura dezakezu</span><span class="sxs-lookup"><span data-stu-id="d7dfc-110">You can configure the message that the worker will receive when you</span></span>        
<span data-ttu-id="d7dfc-111">Politika definitu.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-111">define the policy.</span></span>      
        
<span data-ttu-id="d7dfc-112">Hiru politika mota defini ditzakezu:</span><span class="sxs-lookup"><span data-stu-id="d7dfc-112">You can define three types of policies:</span></span>         
        
- <span data-ttu-id="d7dfc-113">**Abisua**: Langileak gastuen txostena edo bidaia eskaera aurkezteko aukera ematen du baina gastua onartzaile guztientzat eta</span><span class="sxs-lookup"><span data-stu-id="d7dfc-113">**Warning**: Allows the worker to submit an expense report or travel requisition but the expense will be marked for all approvers and</span></span>         
  <span data-ttu-id="d7dfc-114">geroago salatzeko.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-114">for later reporting.</span></span>        

- <span data-ttu-id="d7dfc-115">**Errorea**: Langileari gastua berrikusteko eskatzen dio politika betetzeko, gastuen txostena edo bidaia eskaera bidali aurretik.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-115">**Error**: Requires the worker to revise the expense to comply with the policy before submitting the expense report or travel requisition.</span></span>        
 
 - <span data-ttu-id="d7dfc-116">**Justifikazioa**: Langileak edo zuzendariak polizaren zenbatekoa gainditu izanaren justifikazioa sartzeko eskatzen du, gastuen txostena edo bidaia eskaera aurkeztu aurretik.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-116">**Justification**: Requires the worker or a manager to enter a justification for exceeding the policy amount before submitting the expense report or travel requisition.</span></span>        

## <a name="policy-tips"></a><span data-ttu-id="d7dfc-117">Politika aholkuak</span><span class="sxs-lookup"><span data-stu-id="d7dfc-117">Policy tips</span></span>
<span data-ttu-id="d7dfc-118">Hona hemen gastuak kudeatzeko politika berriak sortzen lagun zaitzaketen iradokizun batzuk:</span><span class="sxs-lookup"><span data-stu-id="d7dfc-118">Here are a few suggestions that can assist you when creating new policies for expense management:</span></span> 

- <span data-ttu-id="d7dfc-119">Gidalerroak indarrean daudenean, horrek esan nahi du gidalerroek ez dutela eragina izango gastua gertatu den egunaren ondorengo datarekin sortzen bada.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-119">Policies are date effective which means a policy won't take effect if it's created with a date after the date that the expense occurred.</span></span> <span data-ttu-id="d7dfc-120">Adibidez, politika berri bat sortzen duzu gaur 50 $ gehieneko otorduen gastua betearazteko.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-120">For example, you create a new policy today to enforce a maximum meal expense of $50.</span></span> <span data-ttu-id="d7dfc-121">Atzotik hasita sartutako gastuak ez dira politika honen aurka egiaztatuko.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-121">Any existing expenses entered as of yesterday won't be checked against this policy.</span></span>
- <span data-ttu-id="d7dfc-122">Zehaztu daitekeen gastu-kategoria baterako politika sortzerakoan, kontuan hartu gastu-lerro motarako baldintza bat gehitzea.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-122">When creating a policy for an expense category that can be itemized, consider adding a condition for expense line type.</span></span> <span data-ttu-id="d7dfc-123">Politika batzuek, hala nola ordainagiria eskatzeak, agian ez dute zentzurik banakako lerroetan.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-123">Some policies, such as requiring a receipt, may not make sense for itemized lines.</span></span> <span data-ttu-id="d7dfc-124">Egoera horretan, politika goiburuaren lerroan edo zehaztu gabeko lerroan soilik aplikatzen da.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-124">In this situation, the policy only is applied to the header line or a non-itemized line.</span></span> 
- <span data-ttu-id="d7dfc-125">Gastuak kudeatzeko gidalerroak jatorrizko entitatearen arabera ebaluatzen dira lehenespenez.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-125">Expense management policies are evaluated against the source entity by default.</span></span> <span data-ttu-id="d7dfc-126">Enpresen arteko eszenatokietan, helburuko entitatearekin (mailegu-entitatea) ebaluatzeko politika ezarri dezakezu.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-126">For intercompany scenarios, you can set the policy to be evaluated against the destination entity (borrowing entity) instead.</span></span> <span data-ttu-id="d7dfc-127">Helburuko entitatearen aurkako gidalerroak exekutatzeko, aktibatu **Pertsona juridiko mailegu-hartzailearekiko Gastuen politika ebaluatzea** funtzioan **Ezaugarrien kudeaketa** lan eremua.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-127">To run the policies against the destination entity, turn on the **Evaluate Expense policy against borrowing legal entity** feature in the **Feature Management** workspace.</span></span>

## <a name="when-to-evaluate-policies"></a><span data-ttu-id="d7dfc-128">Noiz ebaluatu politikak</span><span class="sxs-lookup"><span data-stu-id="d7dfc-128">When to evaluate policies</span></span>

<span data-ttu-id="d7dfc-129">Gastua kudeatzeko parametroetan, gastuak kudeatzeko politikak ebaluatzea hauta dezakezu lerro bat gordetzen denean edo gastuen txostena aurkezten denean.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-129">In expense management parameters, you can select to evaluate expense management policies when a line is saved or when an expense report is submitted.</span></span> <span data-ttu-id="d7dfc-130">Lerro bat noiz gordetzen den ebaluatzea aukeratzen baduzu, erabiltzaileek lehenago ikusiko dute zer egin behar duten beren gastuen txostena aldi berean osatzeko.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-130">If you choose to evaluate when a line is saved, users will have earlier visibility into what they need to do to complete their expense report all at once.</span></span> <span data-ttu-id="d7dfc-131">Bestela, gidalerroen ebaluazioa atzeratu eta denbora aurrez dezakezu amaieran baliozkotuz, lan-fluxura bidalitakoan.</span><span class="sxs-lookup"><span data-stu-id="d7dfc-131">Otherwise, you can delay policy evaluation and save time by validating at the end, during the submission to workflow.</span></span>
