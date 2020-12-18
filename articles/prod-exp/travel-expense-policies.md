---
title: Konfiguratu gastu-gidalerroak
description: Zure langileek Microsoft Dynamics 365 Finance-ko gastuen txostenak eta bidaia-eskaerak sartu eta bidaltzerakoan jarraitu behar dituzten gastu-politikak konfigura ditzakezu.
author: suvaidya
manager: AnnBe
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysPolicyListPage, TrvPolicyRule
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 6240a7be175800ce6f3b066de9e935ab370629ef
ms.sourcegitcommit: 13a4e58eddbb0f81aca07c1ff452c420dbd8a68f
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/30/2020
ms.locfileid: "4650079"
---
# <a name="set-up-expense-policies"></a><span data-ttu-id="80381-103">Konfiguratu gastu-gidalerroak</span><span class="sxs-lookup"><span data-stu-id="80381-103">Set up expense policies</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="80381-104">Zure langileek txostenak eta bidaia-eskaerak sartu eta bidaltzerakoan jarraitu behar dituzten gastu-politikak defini ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="80381-104">You can define policies that your workers must follow when entering and submitting expense reports and travel requisitions.</span></span>         
<span data-ttu-id="80381-105">Gastu politikak ezartzeak gastuak modu eraginkorrean kudeatzen lagun zaitzake.</span><span class="sxs-lookup"><span data-stu-id="80381-105">Implementing expense policies can help you manage expenses effectively.</span></span>         

<span data-ttu-id="80381-106">Adibidez, New Yorkeko hoteletako gastuei buruzko politika bat ezar dezakezu, gaueko gastuak ezin dituela USD 250 baino gehiago adierazi.</span><span class="sxs-lookup"><span data-stu-id="80381-106">For example, you can set a policy for hotel expenses in New York City, which states that the per night expense cannot exceed USD 250.</span></span>       
<span data-ttu-id="80381-107">Langile batek gastuen txostena edo bidaiaren eskaera aurkezten badu gelaren tarifak zenbateko hori gainditzen duenean, sistemak horren berri emango dio</span><span class="sxs-lookup"><span data-stu-id="80381-107">If a worker submits an expense report or a travel requisition in which the room rate exceeds this amount, the system will notify the</span></span>        
<span data-ttu-id="80381-108">Langileak gastuaren polizaren zenbatekoa gainditu duela.</span><span class="sxs-lookup"><span data-stu-id="80381-108">worker that the policy amount for the expense has been exceeded.</span></span> <span data-ttu-id="80381-109">Langileak zu jasotzean jasoko duen mezua konfigura dezakezu</span><span class="sxs-lookup"><span data-stu-id="80381-109">You can configure the message that the worker will receive when you</span></span>        
<span data-ttu-id="80381-110">Politika definitu.</span><span class="sxs-lookup"><span data-stu-id="80381-110">define the policy.</span></span>      
        
<span data-ttu-id="80381-111">Hiru politika mota defini ditzakezu:</span><span class="sxs-lookup"><span data-stu-id="80381-111">You can define three types of policies:</span></span>         
        
- <span data-ttu-id="80381-112">Abisua: Langileak gastuen txostena edo bidaia eskaera aurkezteko aukera ematen du baina gastua onartzaile guztientzat eta</span><span class="sxs-lookup"><span data-stu-id="80381-112">Warning – Allows the worker to submit an expense report or travel requisition but the expense will be marked for all approvers and</span></span>        
  <span data-ttu-id="80381-113">geroago salatzeko.</span><span class="sxs-lookup"><span data-stu-id="80381-113">for later reporting.</span></span>        

- <span data-ttu-id="80381-114">Errorea: Langileari gastua berrikusteko eskatzen dio politika betetzeko, gastuen txostena edo bidaia eskaera bidali aurretik.</span><span class="sxs-lookup"><span data-stu-id="80381-114">Error – Requires the worker to revise the expense to comply with the policy before submitting the expense report or travel requisition.</span></span>       
 
 - <span data-ttu-id="80381-115">Justifikazioa: Langileak edo zuzendariak polizaren zenbatekoa gainditu izanaren justifikazioa sartzeko eskatzen du, gastuen txostena edo bidaia eskaera aurkeztu aurretik.</span><span class="sxs-lookup"><span data-stu-id="80381-115">Justification – Requires the worker or a manager to enter a justification for exceeding the policy amount before submitting the expense report or travel requisition.</span></span>        

## <a name="policy-tips"></a><span data-ttu-id="80381-116">Politika aholkuak</span><span class="sxs-lookup"><span data-stu-id="80381-116">Policy tips</span></span>
<span data-ttu-id="80381-117">Hona hemen gastuak kudeatzeko politika berriak sortzen lagun zaitzaketen iradokizun batzuk.</span><span class="sxs-lookup"><span data-stu-id="80381-117">Here are a few suggestions that can assist you when creating new policies for expense management.</span></span> 
* <span data-ttu-id="80381-118">Gidalerroak indarrean daudenean, horrek esan nahi du gidalerroek ez dutela eragina izango gastua gertatu den egunaren ondorengo datarekin sortzen bada.</span><span class="sxs-lookup"><span data-stu-id="80381-118">Policies are date effective and won't take effect if the policy is created with a date after the date that the expense occurred.</span></span> <span data-ttu-id="80381-119">Adibidez, gaur 50 $ gehieneko otorduen gastua betearazteko politika berri bat sortzen ari bazara, atzotik sartutako lehendik dauden gastuak ez dira politika honen aurka egiaztatuko.</span><span class="sxs-lookup"><span data-stu-id="80381-119">For example, if you are creating a new policy today to enforce a maximum meal expense of $50, then any existing expenses entered as of yesterday won't be checked against this policy.</span></span>
* <span data-ttu-id="80381-120">Zehaztu daitekeen gastu-kategoria baterako politika sortzerakoan, kontuan hartu gastu-lerro motarako baldintza bat gehitzea.</span><span class="sxs-lookup"><span data-stu-id="80381-120">When creating a policy for an expense category that can be itemized, consider adding a condition for expense line type.</span></span> <span data-ttu-id="80381-121">Baliteke ordainagiria eskatzea bezalako politika batzuek ez dute zentzurik zerrendatutako lerroetan eta goiburuaren lerroan edo zehaztu gabeko lerroan soilik aplikatu behar dira.</span><span class="sxs-lookup"><span data-stu-id="80381-121">Some policies such as requiring a receipt may not make sense for itemized lines and should only be applied to the header line or a non-itemized line.</span></span> 
* <span data-ttu-id="80381-122">Gastuak kudeatzeko gidalerroak jatorrizko entitatearen arabera ebaluatzen dira lehenespenez.</span><span class="sxs-lookup"><span data-stu-id="80381-122">Expense management policies are evaluated against the source entity by default.</span></span> <span data-ttu-id="80381-123">Enpresen arteko eszenatokietan, helburuko entitatearekin (mailegu-entitatea) ebaluatzeko politika ezarri dezakezu.</span><span class="sxs-lookup"><span data-stu-id="80381-123">For intercompany scenarios, you can set the policy to be evaluated against the destination entity (borrowing entity) instead.</span></span> <span data-ttu-id="80381-124">Helburuko entitatearen aurkako gidalerroak exekutatzeko, aktibatu "Pertsona juridiko mailegu-hartzailearekiko Gastuen politika ebaluatzea" funtzioan **Ezaugarrien kudeaketa** lan eremua.</span><span class="sxs-lookup"><span data-stu-id="80381-124">To run the policies against the destination entity, turn on the "Evaluate Expense policy against borrowing legal entity" feature in the **Feature Management** workspace.</span></span>

## <a name="when-to-evaluate-policies"></a><span data-ttu-id="80381-125">Noiz ebaluatu politikak</span><span class="sxs-lookup"><span data-stu-id="80381-125">When to evaluate policies</span></span>

<span data-ttu-id="80381-126">Gastua kudeatzeko parametroetan, aukera bat dago gastuak kudeatzeko politikak ebaluatzeko lerro bat gordetzen denean edo gastuen txostena aurkezten denean.</span><span class="sxs-lookup"><span data-stu-id="80381-126">In expense management parameters, there is an option to either evaluate expense management policies when a line is saved or when an expense report is submitted.</span></span> <span data-ttu-id="80381-127">Lerro bat noiz gordetzen den ebaluatzea aukeratzen baduzu, horrela erabiltzaileek lehenago ikusiko dute zer egin behar duten beren gastuen txostena aldi berean osatzeko.</span><span class="sxs-lookup"><span data-stu-id="80381-127">If you choose to evaluate when a line is saved this ensures that users have earlier visibility into what they need to do to complete their expense report all at once.</span></span> <span data-ttu-id="80381-128">Bestela, gidalerroen ebaluazioa atzeratu eta denbora aurrez dezakezu amaieran baliozkotatzen bada, lan-fluxura bidalitakoan.</span><span class="sxs-lookup"><span data-stu-id="80381-128">Otherwise, you can delay policy evaluation and save time if you have validation occur at the end, during submission to workflow.</span></span>
