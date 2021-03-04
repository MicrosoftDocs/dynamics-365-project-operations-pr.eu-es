---
title: Nola egin ditzaket Proiektua Faseak negozio-prozesuaren fluxua?
description: Proiektua faseen negozio-prozesuaren fluxua pertsonalizatzeko ikuspegi orokorra.
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 10/11/2018
ms.topic: article
author: JohnPBurrows
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 1d0168f187e6b0880713aac04bd87dbc2209197d
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5148988"
---
# <a name="how-do-i-customize-the-project-stages-business-process-flow"></a><span data-ttu-id="3688a-103">Nola egin ditzaket Proiektua Faseak negozio-prozesuaren fluxua?</span><span class="sxs-lookup"><span data-stu-id="3688a-103">How do I customize the Project Stages business process flow?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-2-4x-9-0-platform](../includes/cc-applies-to-psa-app-2-4x-9-0-platform.md)]
[!INCLUDE[cc-applies-to-psa-app-1x-8-2-platform](../includes/cc-applies-to-psa-app-1x-8-2-platform.md)]

<span data-ttu-id="3688a-104">Muga ezagun bat dago Project Service-ren aplikazioan eta negozio-prozesuaren fluxuko Proiektu-faseek bat etorri behar dute ingelesezko izenekin (**Quote**, **Plan**, **Close**).</span><span class="sxs-lookup"><span data-stu-id="3688a-104">There's a known limitation in earlier versions of the Project Service application that the names of the stages in the Project Stages business process flow must exactly match the expected English names (**Quote**, **Plan**, **Close**).</span></span> <span data-ttu-id="3688a-105">Bestela, eta negozio-logika, relies izenak Ingelesez fasea arabera, zer ez du funtzionatzen bezala.</span><span class="sxs-lookup"><span data-stu-id="3688a-105">Otherwise, the business logic, which relies on the English stage names, doesn't work as expected.</span></span> <span data-ttu-id="3688a-106">Why dagoen bai ekintzak esaterako ikusten ez **modura Aldaketa Prozesu** edo **Editatu Prozesua** proiektua inprimakian erabilgarri, eta pertsonalizatu negozio-prozesuaren fluxua encouraged ez dago.</span><span class="sxs-lookup"><span data-stu-id="3688a-106">That's why you don't see familiar actions such as **Switch Process** or **Edit Process** available on the project form, and customizing the business process flow isn't encouraged.</span></span> 

<span data-ttu-id="3688a-107">Muga honi 2.4.5.48 bertsioan edo berriagoan ekin zaio.</span><span class="sxs-lookup"><span data-stu-id="3688a-107">This limitation has been addressed in version 2.4.5.48 and later.</span></span> <span data-ttu-id="3688a-108">Artikulu honek iradokitako konponbideak ematen ditu, bertsio berriagoen negozio-prozesuaren fluxu lehenetsia pertsonalizatu nahi baduzu.</span><span class="sxs-lookup"><span data-stu-id="3688a-108">This article provides suggested workarounds if you need to customize the default business process flow for earlier versions.</span></span>  

## <a name="business-logic-requires-an-exact-match-with-english-stage-names"></a><span data-ttu-id="3688a-109">Negozio-logika Ingelesez fasea izenekin bat etor zehatzak behar du</span><span class="sxs-lookup"><span data-stu-id="3688a-109">Business logic requires an exact match with English stage names</span></span>

<span data-ttu-id="3688a-110">Proiektua Faseak negozio-prozesuaren fluxua drives hurrengo ditzake aplikazioan negozio-logika ditu:</span><span class="sxs-lookup"><span data-stu-id="3688a-110">The Project Stages business process flow includes business logic that drives the following behaviors in the app:</span></span>
- <span data-ttu-id="3688a-111">Proiektuan eskaintza batekin erlazionatuta dagoenean, kodea ezartzen negozio-prozesuaren fluxua, **Quote** fasea.</span><span class="sxs-lookup"><span data-stu-id="3688a-111">When the project is associated with a quote, the code sets the business process flow to the **Quote** stage.</span></span>
- <span data-ttu-id="3688a-112">Proiektuan kontratu batekin erlazionatuta dagoenean, kodea ezartzen negozio-prozesuaren fluxua, **Plan** fasea.</span><span class="sxs-lookup"><span data-stu-id="3688a-112">When the project is associated with a contract, the code sets the business process flow to the **Plan** stage.</span></span>
- <span data-ttu-id="3688a-113">Negozio-prozesuaren fluxua aurreratuaren duzunean, **Close** fasea proiektua erregistroa den desaktibatutako.</span><span class="sxs-lookup"><span data-stu-id="3688a-113">When the business process flow is advanced to the **Close** stage, the project record is deactivated.</span></span> <span data-ttu-id="3688a-114">Proiektuan desaktibatzen denean, proiektu-inprimakia eta zereginen xehetasunen egitura (WBS) irakurtzeko soilik dira, izena duten baliabideen erreserbak argitaratuta daude, eta erlazionatutako prezio-zerrendak desaktibatuta daude.</span><span class="sxs-lookup"><span data-stu-id="3688a-114">When the project is deactivated, the project form and work breakdown structure (WBS) are set to read-only, the named resource bookings are released, and any associated price lists are deactivated.</span></span>

<span data-ttu-id="3688a-115">Negozio logikoak ingelesezko izenetan oinarritzen dira proiektu-faseetarako.</span><span class="sxs-lookup"><span data-stu-id="3688a-115">This business logic relies on the English names for the project stages.</span></span> <span data-ttu-id="3688a-116">Hau izenak Ingelesez fasea atalean mendekotasunarekin zergatik Proiektua Faseak negozio-prozesuaren fluxua pertsonalizazio ez encouraged, zergatik ez ikusi, ohiko negozio-prozesuaren fluxuaren ekintzak bezala bezalaxe nagusian arrazoia **modura Aldaketa Prozesu** edo **Editatu Prozesua** proiektua entitatean.</span><span class="sxs-lookup"><span data-stu-id="3688a-116">This dependency on the English stage names is the main reason why customization of the Project Stages business process flow isn't encouraged, as well as why you don’t see the common business process flow actions like **Switch Process** or **Edit Process** on the project entity.</span></span>

## <a name="what-happens-if-the-stage-names-dont-match-the-english-names"></a><span data-ttu-id="3688a-117">Fase izenak Ingelesez izenekin bat ez baduzu gertatzen dena?</span><span class="sxs-lookup"><span data-stu-id="3688a-117">What happens if the stage names don't match the English names?</span></span>

<span data-ttu-id="3688a-118">Aplikazioa bertsioan Project Service 8.2 plataforma, 1.x fasea izenak aplikazioan negozio-prozesuaren fluxua duzunean ez izenekin bat datoz Ingelesez fasea negozio-logika ezartzen eskaintzak edo kontratuak fasea eskuineko edo ixten proiektua, zehazki, egin.</span><span class="sxs-lookup"><span data-stu-id="3688a-118">In the Project Service app version 1.x on the 8.2 platform, when the stage names in the business process flow don’t match the English stage names exactly, the business logic that sets the right stage for quotes or contracts, or that closes the project, is skipped.</span></span> <span data-ttu-id="3688a-119">Ez dago errore-mezuak bistaratuko dira.</span><span class="sxs-lookup"><span data-stu-id="3688a-119">No error messages are displayed.</span></span> <span data-ttu-id="3688a-120">Beraz agertzen dela Proiektua Faseak negozio-prozesuaren fluxua pertsonaliza ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="3688a-120">Therefore it appears that you are able to customize the Project Stages business process flow.</span></span> <span data-ttu-id="3688a-121">Hala ere, eskaintza, kontratuak, lanean prozesu automatikoen ikusi ez eta proiektua itxi.</span><span class="sxs-lookup"><span data-stu-id="3688a-121">However, you won’t see any of the automatic processes working for quotes, contracts, and project close.</span></span>

<span data-ttu-id="3688a-122">Project Service aplikazioa bertsioan 2.4.4.30 edo aurrekoa 9.0 plataforma, gertatu da bat asko arkitekturala aldatu negozio-prozesuaren fluxuak, eskatzen bat berriro idatzi negozio prozesuaren fluxu negozioen logikan.</span><span class="sxs-lookup"><span data-stu-id="3688a-122">In the Project Service app version 2.4.4.30 or earlier on the 9.0 platform, there was a significant architectural change to business process flows, which required a re-write of the business process flow business logic.</span></span> <span data-ttu-id="3688a-123">Ondorioz, prozesu-fasearen izenak aurreikusitako izenak Ingelesez ez badatoz bat, jasotzen errore-mezu bat.</span><span class="sxs-lookup"><span data-stu-id="3688a-123">As a result, if the process stage names don’t match the expected English names, you do receive an error message.</span></span> 

<span data-ttu-id="3688a-124">Beraz, Proiektua Faseak negozio-prozesuaren fluxua proiektua entitate pertsonalizatu nahi badituzu soilik gehi ditzakezu brand berria faseak lehenetsia negozio-prozesuaren fluxua proiektua entitaterako, zu, **Eskaintza**, **Plana** eta **Itxi** gisa faseak-da.</span><span class="sxs-lookup"><span data-stu-id="3688a-124">Therefore, if you want to customize the Project Stages business process flow for the project entity, you can only add brand new stages to the default business process flow for the project entity, while keeping the **Quote**, **Plan**, and **Close** stages as-is.</span></span> <span data-ttu-id="3688a-125">Murrizketa hau kontutan duzun duzun ez lortu erroreak negozio-prozesuaren fluxua izenak Ingelesez fasea expects negozio-logika ziurtatzen.</span><span class="sxs-lookup"><span data-stu-id="3688a-125">This restriction ensures that you don’t get errors from the business logic that expects the English stage names in the business process flow.</span></span>

<span data-ttu-id="3688a-126">2.4.5.48 bertsioan edo berriagoan, artikulu honetan azaldutako negozio-logika negozio-prozesuaren fluxu lehenetsitik kendu da proiektu-entitaterako.</span><span class="sxs-lookup"><span data-stu-id="3688a-126">In version 2.4.5.48 or later, the business logic described in this article has been removed from the default business process flow for the project entity.</span></span> <span data-ttu-id="3688a-127">Horren bertsioa edo berriagoa bertsioa berritzen ahalko dituzu pertsonalizatu edo ordezkatu lehenetsitako negozio-prozesuaren fluxua bat izatea.</span><span class="sxs-lookup"><span data-stu-id="3688a-127">Upgrading to that version or later will let you customize or replace the default business process flow with one of your own.</span></span> 

## <a name="workarounds-for-earlier-versions"></a><span data-ttu-id="3688a-128">Aurreko bertsioetarako konponbideak</span><span class="sxs-lookup"><span data-stu-id="3688a-128">Workarounds for earlier versions</span></span>

<span data-ttu-id="3688a-129">Aukera ez bertsio-berritzen, Proiektua Faseak negozio-prozesuaren fluxua bi moduetan bateko proiektua entitate pertsonaliza dezakezu:</span><span class="sxs-lookup"><span data-stu-id="3688a-129">If upgrading isn't an option, you can customize the Project Stages business process flow for the project entity in one of these two ways:</span></span>

1. <span data-ttu-id="3688a-130">Gehitu faseak gehigarria lehenetsia konfigurazioa, izenak Ingelesez fasea retaining da **Eskaintza**, **Antolatu**, eta **Itxi**.</span><span class="sxs-lookup"><span data-stu-id="3688a-130">Add additional stages to the default configuration, while retaining the English stage names for **Quote**, **Plan**, and **Close**.</span></span>


![Lehenetsitako konfigurazio-fluxuari faseak gehitzeak-Eginbideei](media/FAQ-Customize-BPF-1.png)
 
2. <span data-ttu-id="3688a-132">Zure negozio-prozesuaren fluxua sortzeko eta egin nagusia negozio-prozesuaren fluxua entitaterako proiektua, nahi dituzun fase guztiak izenak duzu lezake.</span><span class="sxs-lookup"><span data-stu-id="3688a-132">Create your own business process flow and make it the primary business process flow for the project entity, which lets you have any stage names you want.</span></span> <span data-ttu-id="3688a-133">Hala ere, estandarra proiektua faseak bera erabili nahi baduzu **Eskaintza**, **Antolatu**, eta **Itxi**, zenbait pertsonalizazio izen pertsonalizatuak fasea desaktibatu driven egin behar duzu.</span><span class="sxs-lookup"><span data-stu-id="3688a-133">However, if you want to use the same standard project stages **Quote**, **Plan**, and **Close**, you need to do some customizations that are driven off your custom stage names.</span></span> <span data-ttu-id="3688a-134">Konplexu logika duzu oraindik batzuek eragin bakarrik desaktibatu proiektua erregistroa zein, proiektua ixten da.</span><span class="sxs-lookup"><span data-stu-id="3688a-134">The more complex logic is in the closing of the project, which you can still trigger by just deactivating the project record.</span></span>

![BPF pertsonalizazioa](media/FAQ-Customize-BPF-2.png)

### <a name="additional-considerations-for-project-service-app-version-24430-or-earlier-on-platform-90"></a><span data-ttu-id="3688a-136">Project Service aplikazioa bertsioa 2.4.4.30 edo aurrekoa plataforma 9.0 considerations gehigarria</span><span class="sxs-lookup"><span data-stu-id="3688a-136">Additional considerations for Project Service app version 2.4.4.30 or earlier on platform 9.0</span></span>

<span data-ttu-id="3688a-137">Project Service 2.4.4.30 edo aurrekoa plataforma 9.0, pertsonalizatutako negozio-prozesuaren fluxuko batekin, **Fasearen Izena** erabilitako entitatearen proiektua eremua, **Proiektua Fasea** diagrama eta proiektua zerrenda-ikuspegietako ez eguneratu delako coupled Proiektua Faseak negozio prozesuaren fluxu lehenetsia.</span><span class="sxs-lookup"><span data-stu-id="3688a-137">In Project Service 2.4.4.30 or earlier on platform 9.0, with a custom business process flow the **Stage Name** field on the project entity used in the **Project By Stage** chart and project list views won’t update, because it’s coupled to the default Project Stages business process flow.</span></span> <span data-ttu-id="3688a-138">Urrats hauekin arazoarekin bideratuko dira:</span><span class="sxs-lookup"><span data-stu-id="3688a-138">You can address this issue with the following steps:</span></span>

- <span data-ttu-id="3688a-139">Uneko negozio prozesu-fluxuaren fasearen erabiltzailearen advances pertsonalizatutako negozio-prozesuaren fluxua bidez gisa eguneratu diren islatzeko eremu pertsonalizatu bat gehitu.</span><span class="sxs-lookup"><span data-stu-id="3688a-139">Add a custom field to capture the current business process flow stage that is updated as the user advances through the custom business process flow.</span></span>

- <span data-ttu-id="3688a-140">Aldatu, **Proiektua Fasea** ordez lehenetsitako konfigurazio-eremu pertsonalizatua zure lan egin nahi duzun diagrama.</span><span class="sxs-lookup"><span data-stu-id="3688a-140">Modify the **Project By Stage** chart to work with your custom field instead of the default configuration.</span></span>

### <a name="steps-to-create-your-own-business-process-flow-for-the-project-entity"></a><span data-ttu-id="3688a-141">Urratsak sortzeko zure negozio-prozesuaren fluxu proiektua entitate</span><span class="sxs-lookup"><span data-stu-id="3688a-141">Steps to create your own business process flow for the project entity</span></span>

<span data-ttu-id="3688a-142">Proiektu-entitatearen negozio-prozesuaren fluxua sortzeko, egin hau:</span><span class="sxs-lookup"><span data-stu-id="3688a-142">To create your own business process flow for the project entity do the following:</span></span>

1. <span data-ttu-id="3688a-143">Joan **Ezarpenak** > **Prozesu-zentroak** atalera.</span><span class="sxs-lookup"><span data-stu-id="3688a-143">Go to **Settings** > **Process Center**.</span></span> <span data-ttu-id="3688a-144">Ez da negozio-prozesuaren fluxu ere kopiatzen Project Service-ren negozio-logika duen delako Proiektua Faseak kopiatu.</span><span class="sxs-lookup"><span data-stu-id="3688a-144">Don’t copy the Project Stages business process flow because that also copies the Project Service business logic.</span></span>

  ![Sortu prozesua](media/FAQ-Customize-BPF-3.png)

2. <span data-ttu-id="3688a-146">Prozesu-Diseinatzailea sortzeko erabili nahi dituzun fase izenak.</span><span class="sxs-lookup"><span data-stu-id="3688a-146">Use the Process Designer to create the stage names you want.</span></span> <span data-ttu-id="3688a-147">Funtzionalitate bera fase lehenetsi gisa nahi duzun **Eskaintza**, **Antolatu**, eta **Itxi**, zure pertsonalizatutako negozio-prozesuaren fluxu baten fasearen izenak oinarrituta sortu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="3688a-147">If you want the same functionality as the default stages for **Quote**, **Plan**, and **Close**, you’ll have to create that based on your custom business process flow’s stage names.</span></span>

   ![Eginbideei-Prozesua Diseinatzailea erabiltzen BPF pertsonalizatu](media/FAQ-Customize-BPF-4.png) 

3. <span data-ttu-id="3688a-149">Prozesu-Diseinatzailea, sakatu **Ordenatu Prozesu-Fluxua** pertsonalizatutako negozio-prozesuaren fluxua nagusia negozio-prozesuaren fluxua proiektua entitate batek da Proiektua Faseak negozio-prozesuaren fluxua gaineko batera mugituz, zerrendaren goiko aldean jartzeko.</span><span class="sxs-lookup"><span data-stu-id="3688a-149">In the Process Designer, click **Order Process Flow** to make the custom business process flow the primary business process flow for the project entity by moving it above the Project Stages business process flow to the top of the list.</span></span>


   [<span data-ttu-id="3688a-150">Eskaera-Prozesuaren Fluxu erabiliz-Eginbideei</span><span class="sxs-lookup"><span data-stu-id="3688a-150">Screenshot of using Order Process Flow</span></span>](media/FAQ-Customize-BPF-5-720.png)

### <a name="the-following-steps-apply-to-project-service-app-24430-or-earlier-on-the-90-platform"></a><span data-ttu-id="3688a-151">Jarraitu urrats hauek Proiektua Zerbitzu aplikazioa 2.4.4.30, edo aurrekoa 9.0 plataforma aplikatu</span><span class="sxs-lookup"><span data-stu-id="3688a-151">The following steps apply to Project Service app 2.4.4.30 or earlier on the 9.0 platform</span></span>

4. <span data-ttu-id="3688a-152">Pertsonalizatutako negozio-prozesuaren fluxu pertsonalizatuak faseak islatzeko proiektua entitateetan eremu pertsonalizatu berri bat gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="3688a-152">Add a new custom field to the project entity to capture the custom stages in your custom business process flow.</span></span> <span data-ttu-id="3688a-153">Negozio-logika (plugin edo lan-fluxuaren) pertsonalizatutako negozio-prozesuaren fluxua fasea eguneratzen eremua eguneratzeko, gehitu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="3688a-153">You’ll need to add business logic (plugin/workflow) to update this field when the stage on the custom business process flow is updated.</span></span>

   ![Pertsonalizatu Proiektua entitate-Eginbideei](media/FAQ-Customize-BPF-6-720.png)

5. <span data-ttu-id="3688a-155">Aldatu, **Proiektua Fasea** eremu pertsonalizatu berri zure faseak erabili nahi duzun diagrama.</span><span class="sxs-lookup"><span data-stu-id="3688a-155">Modify the **Project By Stage** chart to use your new custom field for stages.</span></span>

   ![Eginbideei erabiltzearen arriskua Proiektua Fasea diagrama](media/FAQ-Customize-BPF-7-720.png)

6. <span data-ttu-id="3688a-157">Eremu pertsonalizatu berri zure faseak gehitzeko proiektua entitatearentzat ikuspegiak edozein aldatu.</span><span class="sxs-lookup"><span data-stu-id="3688a-157">Modify any views for the project entity to include your new custom field for stages.</span></span>

   ![Aldatu entitate Proiektua ikuspegiak Eginbideei](media/FAQ-Customize-BPF-8-720.png)

