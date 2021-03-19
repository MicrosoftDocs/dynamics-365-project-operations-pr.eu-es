---
title: Kudeatu baliabideak
description: Gai honek baliabideak kudeatzeko moduari buruzko informazioa eskaintzen du.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 05/13/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 1d47be6c11ced70b94b7497dfbc0c67d1a3f631b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274983"
---
# <a name="manage-resources"></a><span data-ttu-id="2f66d-103">Kudeatu baliabideak</span><span class="sxs-lookup"><span data-stu-id="2f66d-103">Manage resources</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="2f66d-104">Dynamics 365 Project Service Automation-ek baliabideen kudeaketako panela biltzen du baliabideen eskaeraren eta erakundearen erabileraren ikuspegi orokorra eskaintzen duena.</span><span class="sxs-lookup"><span data-stu-id="2f66d-104">Dynamics 365 Project Service Automation includes a resource manager dashboard that provides a visual overview of resource demand and utilization throughout the organization.</span></span> <span data-ttu-id="2f66d-105">Panel honetako diagramak erabil ditzakezu informazioa ikusteko:</span><span class="sxs-lookup"><span data-stu-id="2f66d-105">You can use the charts on this dashboard to visualize the following information:</span></span>

- <span data-ttu-id="2f66d-106">**Baliabideen eskaria**: **Baliabide aktiboen eskaera** taulan aurkeztu diren baliabideak erakusten dira.</span><span class="sxs-lookup"><span data-stu-id="2f66d-106">**Resource demand** – The **Active Resource Request** chart shows resources that have been submitted.</span></span> <span data-ttu-id="2f66d-107">Baliabideak funtzioaren edo proiektuaren arabera biltzen dira.</span><span class="sxs-lookup"><span data-stu-id="2f66d-107">The resources are aggregated by either role or project.</span></span>
- <span data-ttu-id="2f66d-108">**Bidali gabeko baliabideen eskaria**: **Esleitu gabeko baliabideen eskaria** taulan aurkeztu ez diren baliabide-eskakizun guztiak erakusten dira.</span><span class="sxs-lookup"><span data-stu-id="2f66d-108">**Unsubmitted resource demand** – The **Unassigned Resource Demand** chart shows all the resource requirements that haven't been submitted.</span></span> <span data-ttu-id="2f66d-109">Baliabideen kudeatzaileei eskaera ez dela irmoa ikusten dute eta baliabide eskaera bidez bidaltzen laguntzen die.</span><span class="sxs-lookup"><span data-stu-id="2f66d-109">It helps resource managers view demand that isn't firm and might be submitted through a resource request.</span></span>
- <span data-ttu-id="2f66d-110">**Erabilera erabilgarriak azken astean**: **Erabilera funtzioa** taulan ikus daiteke erakundearen benetako fakturazioaren portzentajea bere eginkizunaren arabera fakturazioaren aldera.</span><span class="sxs-lookup"><span data-stu-id="2f66d-110">**Billable utilization for the past week** – The **Utilization by Role** chart shows the percentage of the organization's actual billable utilization by role against its target billable utilization by role.</span></span>

    > [!NOTE]
    > <span data-ttu-id="2f66d-111">**Erabilera funtzioa** taula eskuragarri egoteko, sortu UpdateRoleUtilization lan-fluxua exekutatzen duen lana.</span><span class="sxs-lookup"><span data-stu-id="2f66d-111">To make the **Utilization by Role** chart available, create a job that runs the UpdateRoleUtilization workflow.</span></span> <span data-ttu-id="2f66d-112">Lan errepikari hau zazpi egunez behin egiten da aurreko zazpi egunetako erabilgarritasuna kalkulatzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-112">This recurring job runs every seven days to calculate billable utilization for the previous seven days.</span></span> <span data-ttu-id="2f66d-113">Emaitzak funtzioaren arabera batu dira.</span><span class="sxs-lookup"><span data-stu-id="2f66d-113">The results are aggregated by role.</span></span>

## <a name="manage-project-team-members"></a><span data-ttu-id="2f66d-114">Proiektu-taldekideak kudeatu</span><span class="sxs-lookup"><span data-stu-id="2f66d-114">Manage project team members</span></span>

<span data-ttu-id="2f66d-115">Proiektuaren kudeatzaileek baliabideen kudeatzailearen panela erabil dezakete proiektuetan baliabideak kudeatzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-115">Project managers can use the resource manager dashboard to manage the resources on projects.</span></span> <span data-ttu-id="2f66d-116">Adibidez, taldekide bat zuzenean gehitu dezakete proiektu batean eta taldekide bat erreserbatu baliabide generiko batek harrapatutako baliabide eskakizunak betetzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-116">For example, they can add a team member directly to a project and book a team member to fulfill the resource requirements that were captured by a generic resource.</span></span>

### <a name="add-a-team-member-directly-to-a-project"></a><span data-ttu-id="2f66d-117">Gehitu taldekidea zuzenean proiektu bati</span><span class="sxs-lookup"><span data-stu-id="2f66d-117">Add a team member directly to a project</span></span>

<span data-ttu-id="2f66d-118">Taldekide bat zuzenean proiektu batean gehitzeko, **Proiektuak** orrialdean **Taldea** fitxan, aukeratu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="2f66d-118">To add a team member directly to a project, on the **Projects** page, on the **Team** tab, select **New**.</span></span> <span data-ttu-id="2f66d-119">**Sorrera bizkorra: proiektuko taldekidea** elkarrizketa-koadroa agertuko da.</span><span class="sxs-lookup"><span data-stu-id="2f66d-119">The **Quick Create:Project Team Member** dialog box appears.</span></span> <span data-ttu-id="2f66d-120">Elkarrizketa-koadro honetan zeregin hauek egin ditzakezu:</span><span class="sxs-lookup"><span data-stu-id="2f66d-120">In this dialog box, you can perform these tasks:</span></span>

- <span data-ttu-id="2f66d-121">**Erreserbatu izendatutako baliabidea**: **Baliabide erreserbagarria** eremuan, hautatu baliabidearen izena.</span><span class="sxs-lookup"><span data-stu-id="2f66d-121">**Book a named resource** – In the **Bookable Resource** field, select the name of the resource.</span></span> <span data-ttu-id="2f66d-122">Ondoren, hautatu funtzioa, zehaztu epea eta hautatu esleipen metodoa.</span><span class="sxs-lookup"><span data-stu-id="2f66d-122">Then select the role, set the period, and select an allocation method.</span></span> <span data-ttu-id="2f66d-123">Aukeratu duzun izena duen baliabidea proiektuari gehitzen zaio hautatutako esleipen metodoa eta baliabideen egutegia erabiliz.</span><span class="sxs-lookup"><span data-stu-id="2f66d-123">The named resource that you selected is added to the project by using the selected allocation method and the resources calendar.</span></span>
- <span data-ttu-id="2f66d-124">**Gehitu baliabide generikoa**: utzi **Baliabide erreserbagarria** eremua hutsik eta, ondoren, hautatu funtzioa, ezarri aldia eta hautatu hobetsitako esleipen metodoa.</span><span class="sxs-lookup"><span data-stu-id="2f66d-124">**Add a generic resource** – Leave the **Bookable resource** field blank, and then select the role, set the period, and select the preferred allocation method.</span></span> <span data-ttu-id="2f66d-125">Baliabide generiko bat gehitzen zaio taldeari leku-marka gisa, taldean izena duten baliabide erabiltzen diren eskaera-eredua mantentzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-125">A generic resource is added to the team as a placeholder to hold the demand pattern that is used to book named resources on the team.</span></span> <span data-ttu-id="2f66d-126">Baldintza proiektuaren egutegiaren arabera egiten da.</span><span class="sxs-lookup"><span data-stu-id="2f66d-126">The requirement is made according to the project calendar.</span></span>
- <span data-ttu-id="2f66d-127">**Gehitu izendatutako baliabidea taldeari baliabideen ahalmena kontsumitu gabe**: **Baliabide erreserbagarria** eremuan, hautatu baliabide bat.</span><span class="sxs-lookup"><span data-stu-id="2f66d-127">**Add a named resource to the team without consuming resource capacity** – In the **Bookable Resource** field, select a resource.</span></span> <span data-ttu-id="2f66d-128">Ondoren, hautatu aldia eta hautatu **Ez** esleipen metodoa.</span><span class="sxs-lookup"><span data-stu-id="2f66d-128">Then select the period, and select **None** as the allocation method.</span></span> <span data-ttu-id="2f66d-129">Baliabidea taldeari gehitzen zaio, baina baliabidearen ahalmena ez da erreserba bidez kontsumitzen.</span><span class="sxs-lookup"><span data-stu-id="2f66d-129">The resource is added to the team, but the resource's capacity isn't consumed through a booking.</span></span>

### <a name="book-a-team-member-to-fulfill-resource-requirements-for-a-generic-resource"></a><span data-ttu-id="2f66d-130">Erreserbatu taldekide bat baliabide generiko baterako eskakizunak betetzeko</span><span class="sxs-lookup"><span data-stu-id="2f66d-130">Book a team member to fulfill resource requirements for a generic resource</span></span>

<span data-ttu-id="2f66d-131">PSAn, baliabide generikoak proiektu talde batean erreserbatu ditzakezu eta zeregina, behar den gaitasuna eta nola banatzen den zehaztu dezakezu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-131">In PSA, you can book a generic resource on a project team, and can specify the role, the required capacity, and how that capacity is distributed.</span></span> <span data-ttu-id="2f66d-132">Baliabidearen eskakizunean, baliabide generikoarekin lotutako atributuak zehaztu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-132">On the resource requirement, you can specify attributes that are associated with the generic resource.</span></span> <span data-ttu-id="2f66d-133">Ezaugarri horien artean beharrezkoak diren trebetasunak, nahiago den antolakuntza-unitatea eta hobetsitako baliabideak daude.</span><span class="sxs-lookup"><span data-stu-id="2f66d-133">These attributes include required skills, the preferred organizational unit, and preferred resources.</span></span>

<span data-ttu-id="2f66d-134">Jarraitu urrats hauek garatzaileentzako baliabide generiko batean eskatutako trebetasunak zehazteko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-134">Follow these steps to specify required skills on a generic resource for a developer.</span></span>

1. <span data-ttu-id="2f66d-135">**Proiektuak** orrialdean **Taldea** fitxan, hautatu **Berria** baliabide generikoa erreserbatzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-135">On the **Projects** page, on the **Team** tab, select **New** to book a generic resource.</span></span>

    ![Balio generikoa taldean erreserbatuta](media/Resource-Management-image9.png)

2. <span data-ttu-id="2f66d-137">**Taldekide guztiak** ikuspegian, **Baliabideen eskakizuna** zutabean, hautatu esteka baliabide generikorako beharrezkoak diren trebetasunak gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-137">In the **All Team Members** view, in the **Resource Requirement** column, select the link to add required skills for the generic resource.</span></span>

    ![Eskakizun esteka](media/Resource-Management-image10.png)

3. <span data-ttu-id="2f66d-139">**Baliabideen eskakizuna** orrian, **Trebetasunak** saretan agertzen denean, hautatu elipsia (**...**) eta hautatu **Gehitu eskakizun berriaren ezaugarria** sustatzailearentzako beharrezkoak diren gaitasunak gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-139">On the **Resource Requirement** page that appears, in the **Skills** grid, select the ellipsis (**...**) and then select **Add New Requirement Characteristic** to add the required skills for your developer.</span></span>

    ![Eskakizunen ezaugarri-komando berria hautatu](media/Resource-Management-image11.png)

4. <span data-ttu-id="2f66d-141">**Sorrera bizkorra: eskakizunaren ezaugarria** elkarrizketa-koadroan **Ezaugarria** eremuan agertzen denean, hautatu eskatutako trebetasuna.</span><span class="sxs-lookup"><span data-stu-id="2f66d-141">In the **Quick Create: Requirement Characteristic** dialog box that appears, in the **Characteristic** field, select the required skill.</span></span> <span data-ttu-id="2f66d-142">Ondoren, **Balorazioaren balioa** eremuan, hautatu trebetasun horren maila.</span><span class="sxs-lookup"><span data-stu-id="2f66d-142">Then, in the **Rating value** field, select the proficiency level for that skill.</span></span> <span data-ttu-id="2f66d-143">Azkenean, **Baliabideen eskakizuna** eremuan, ezarri eskakizuna baliabide iturriak antolakuntza unitateetatik edo baita izendatutako baliabideak ere.</span><span class="sxs-lookup"><span data-stu-id="2f66d-143">Finally, in the **Resource Requirement** field, set the requirement to source resources from organizational units or even named resources.</span></span> <span data-ttu-id="2f66d-144">Bukatu duzunean, hautatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="2f66d-144">When you've finished, select **Save**.</span></span>

    ![Sorrera bizkorra: eskakizunaren elkarrizketa-koadroa](media/Resource-Management-image12.png)

5. <span data-ttu-id="2f66d-146">**Baliabideen eskakizuna** orrian, hautatu **Liburua** baliabide eskakizuna betetzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-146">On the **Resource Requirement** page, select **Book** to fulfill the resource requirement.</span></span>

    ![Liburuaren botoia Baliabide Eskakizuna orrian](media/Resource-Management-image13.png)

    <span data-ttu-id="2f66d-148">Baliabide generikoak ere hauta ditzakezu **Taldekide guztiak** saretan eta gero hautatu **Liburua**.</span><span class="sxs-lookup"><span data-stu-id="2f66d-148">You can also select the generic resource in the **All Team Members** grid and then select **Book**.</span></span>

    ![Erreserbatu botoia Taldekide guztien sarearen gainetik](media/Resource-Management-image14.png)

    > [!NOTE]
    > <span data-ttu-id="2f66d-150">Adibide honetan, 40 ordu behar dira baina ez erreserbatu gabeko orduak, baliabide generikoek erreserbaziorik ez dutelako.</span><span class="sxs-lookup"><span data-stu-id="2f66d-150">In this example, there are 40 required hours but no actual booked hours, because generic resources don't have bookings.</span></span> <span data-ttu-id="2f66d-151">Gainera, ez dira ordu esleituak, baliabide generikoa zuzenean taldeari gehitu zitzaiolako.</span><span class="sxs-lookup"><span data-stu-id="2f66d-151">Additionally, there are no assigned hours, because the generic resource was added directly to the team.</span></span> <span data-ttu-id="2f66d-152">Ez da zereginen esleipena erabiliz gehitu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-152">It wasn't added by using task assignment.</span></span>

    <span data-ttu-id="2f66d-153">**Programazio laguntzailea** orrialdean, erabilgarri dauden baliabideak iragazi ditzakezu baliabideen eskakizunean zehazten diren baldintzen arabera.</span><span class="sxs-lookup"><span data-stu-id="2f66d-153">On the **Scheduling Assistant** page, you can filter available resources by the requirements that are specified on the resource requirement.</span></span> <span data-ttu-id="2f66d-154">Baliabideak Antolaketa taulan zehaztutako sailkapen parametroen arabera ordenatzen dira.</span><span class="sxs-lookup"><span data-stu-id="2f66d-154">Resources are sorted according to the sorting parameters that are specified on the Schedule Board.</span></span>

    ![Antolaketa-laguntzailearen orria](media/Resource-Management-image15.png)

    <span data-ttu-id="2f66d-156">Hona hemen maiz erabiltzen diren iragazki batzuk:</span><span class="sxs-lookup"><span data-stu-id="2f66d-156">Here are some filters that are often used:</span></span>

    - <span data-ttu-id="2f66d-157">**Ezaugarriak puntuazioarekin batera**: gaitasunak, ziurtagiriak eta baliabideen beste ezaugarri batzuen arabera iragazi, gaitasunen balorazioez gain.</span><span class="sxs-lookup"><span data-stu-id="2f66d-157">**Characteristics along with a rating** – Filter by skills, certifications, and other resource qualities, in addition to ratings of proficiency.</span></span>
    - <span data-ttu-id="2f66d-158">**Funtzioak**: iragazi baliabide erreserbagarrietan esleitzen zaizkion funtzio lehenetsiak.</span><span class="sxs-lookup"><span data-stu-id="2f66d-158">**Roles** – Filter by the default roles that are assigned to bookable resources.</span></span>
    - <span data-ttu-id="2f66d-159">**Antolamendu unitateak**: erreserbatu baliabideak esleitzen zaizkion antolaketa unitateen arabera.</span><span class="sxs-lookup"><span data-stu-id="2f66d-159">**Organizational units** – Filter bookable resources by the organizational units that they are assigned to.</span></span>

6. <span data-ttu-id="2f66d-160">Hasierako eskakizunaren emaitzarekin konforme ez bazaude, iragazkiaren irizpideak alda ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-160">If you aren't satisfied with the results of the initial requirement search, you can change the filter criteria.</span></span> <span data-ttu-id="2f66d-161">Zabaldu **Iragazkiaren ikuspegia** orria ezkerrean eta ondoren hautatu **Bilatu** baliabide osagarriak aurkitzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-161">Expand the **Filter View** pane on the left, and then select **Search** to find additional resources.</span></span>

    ![Iragazi ikuspegiaren panela](media/Resource-Management-image16.png)

7. <span data-ttu-id="2f66d-163">Emaitzak nola ordenatzen diren aldatzeko, hautatu **Ordenatu**.</span><span class="sxs-lookup"><span data-stu-id="2f66d-163">To change how the results are sorted, select **Sort**.</span></span>

    ![Ordena komandoa](media/Resource-Management-image17.png)

8. <span data-ttu-id="2f66d-165">Hautatu baliabideak eskakizunean zehaztutako eskaeraren arabera, saretaren goiko aldean adierazten den moduan.</span><span class="sxs-lookup"><span data-stu-id="2f66d-165">Select resources according to the demand that is specified on the requirement, as indicated at the top of the grid.</span></span> <span data-ttu-id="2f66d-166">Saretako gelaxken aukera garbitu eta baliabide-ahalmena irekita utzi dezakezu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-166">You can clear the selection of cells in the grid and leave that resource capacity open.</span></span> <span data-ttu-id="2f66d-167">Baliabide bakarra aldi berean erreserbatu daiteke.</span><span class="sxs-lookup"><span data-stu-id="2f66d-167">Only one resource at a time can be selected as booked.</span></span>

9. <span data-ttu-id="2f66d-168">Aukeratu **Liburua** hautatutako baliabidea erreserbatzea eta Antolaketa taula irekita uztea, baliabide osagarriak aukeratu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-168">Select **Book** to book the selected resource and leave the Schedule Board open, so that you can select additional resources.</span></span> <span data-ttu-id="2f66d-169">Bestela, hautatu **Liburua eta irteera** hautatutako baliabidea erreserbatzeko eta Antolaketa taula ixteko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-169">Alternatively, select **Book & Exit** to book the selected resource and close the Schedule Board.</span></span>

    ![Erreserbatzeko baliabidea](media/Resource-Management-image19.png)

    <span data-ttu-id="2f66d-171">Erreserbatutako orduen jakinarazpena jasotzen duzu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-171">You receive a notification about booked hours.</span></span> <span data-ttu-id="2f66d-172">Eskariaren adierazleek erreserba-eskakizuna betetzen den eta zenbat geratzen den erakusten dute.</span><span class="sxs-lookup"><span data-stu-id="2f66d-172">The demand indicators show how much the booking requirement is satisfied and how much remains.</span></span> <span data-ttu-id="2f66d-173">Aukeratutako baliabidearen ahalmena zenbat kontsumitzen den ere ikus dezakezu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-173">You can also see how much of the selected resource's capacity is consumed.</span></span> <span data-ttu-id="2f66d-174">Aukeratu **Zabaldu** baliabide erreserbagarriei buruzko xehetasun gehiago ikusteko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-174">Select **Expand** to view more details about resource bookings.</span></span>

9. <span data-ttu-id="2f66d-175">Itzuli **Taldekide guztiak** ikuspegira.</span><span class="sxs-lookup"><span data-stu-id="2f66d-175">Return to the **All Team Members** view.</span></span> <span data-ttu-id="2f66d-176">Saretan, ohartu baliabide generikoa izena duen baliabide ordez aldatu dela, eta 40 ordu zerrendatzen direla baliabide horretarako erreserbatuta.</span><span class="sxs-lookup"><span data-stu-id="2f66d-176">In the grid, notice that the generic resource has been replaced by the named resource, and 40 hours are listed as booked for that resource.</span></span>

    ![Taldekide guztien sareta eguneratua](media/Resource-Management-image20.png)

    > [!NOTE]
    > <span data-ttu-id="2f66d-178">Ez dira esleitutako orduak erakusten, zuzenean taldean erreserbatu direlako.</span><span class="sxs-lookup"><span data-stu-id="2f66d-178">No assigned hours are shown, because they were booked directly on the team.</span></span> <span data-ttu-id="2f66d-179">Ez zuten zereginen zereginaz baliatu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-179">They weren't booked by using task assignment.</span></span>

## <a name="assign-generic-resources-to-tasks-and-generate-resource-requirements"></a><span data-ttu-id="2f66d-180">Esleitu baliabide generikoak zereginei eta sortu baliabide eskakizunak</span><span class="sxs-lookup"><span data-stu-id="2f66d-180">Assign generic resources to tasks and generate resource requirements</span></span>

<span data-ttu-id="2f66d-181">PSAn, zereginak sor ditzakezu eta gero baliabide generikoak esleitu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-181">In PSA, you can create tasks and then assign generic resources to them.</span></span> <span data-ttu-id="2f66d-182">Horrela, baliabideen eskaera tokiko ordezkariek ordezkatu dezakete zure egutegia eta finantza-zenbakiak zenbatzen dituzun bitartean.</span><span class="sxs-lookup"><span data-stu-id="2f66d-182">In this way, resource demand can be represented by placeholders while you estimate your schedule and financial numbers.</span></span> <span data-ttu-id="2f66d-183">Baliabide generikoetarako baliabide eskakizunak sor ditzakezu eta bete.</span><span class="sxs-lookup"><span data-stu-id="2f66d-183">You can then generate resource requirements for the generic resources and fulfill them.</span></span>

1. <span data-ttu-id="2f66d-184">**Proiektuak** orrialdean **Antolaketa** fitxan, aukeratu **Gehitu** zeregin bat sortzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-184">On the **Projects** page, on the **Schedule** tab, select **Add** to create a task.</span></span>

    ![Zeregin berria sortuta](media/Resource-Management-image21.png)

2. <span data-ttu-id="2f66d-186">**Baliabideak** eremuan aukeratu **Baliabideen hautatzailea** sinboloa.</span><span class="sxs-lookup"><span data-stu-id="2f66d-186">In the **Resources** field, select the **Resource Picker** symbol.</span></span> <span data-ttu-id="2f66d-187">Baliabide hautatzailea proiektuan dauden taldekideak agertzen dira.</span><span class="sxs-lookup"><span data-stu-id="2f66d-187">The Resource Picker appears and shows existing team members for the project.</span></span>

    ![Baliabideen hautatzailea](media/Resource-Management-image22.png)

3. <span data-ttu-id="2f66d-189">Idatzi baliabide generiko berriaren izena eta, ondoren, hautatu **Sortu**.</span><span class="sxs-lookup"><span data-stu-id="2f66d-189">Enter the name of the new generic resource, and then select **Create**.</span></span>

    ![Sartu den baliabide generiko berri baten izena](media/Resource-Management-image23.png)

4. <span data-ttu-id="2f66d-191">**Sorrera bizkorra: proiektuko taldekidea** elkarrizketa-koadroan **Funtzioa** eremuan agertzen denean, hautatu baliabide generikorako funtzioa.</span><span class="sxs-lookup"><span data-stu-id="2f66d-191">In the **Quick Create: Project Team Member** dialog box that appears, in the **Role** field, select the role for the generic resource.</span></span> <span data-ttu-id="2f66d-192">**Baliabide-unitatea** eremuan, hautatu baliabide generikoa lortzeko antolakuntza-unitatea.</span><span class="sxs-lookup"><span data-stu-id="2f66d-192">In the **Resourcing Unit** field, select the organizational unit for the generic resource.</span></span> <span data-ttu-id="2f66d-193">Ondoren, hautatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="2f66d-193">Then select **Save**.</span></span>

    ![Sorrera bizkorra: proiektuko taldekidea elkarrizketa-koadroa](media/Resource-Management-image24.png)

    <span data-ttu-id="2f66d-195">Taldekide generikoa orain zereginera esleituta dago.</span><span class="sxs-lookup"><span data-stu-id="2f66d-195">The generic team member is now assigned to the task.</span></span>

    ![Taldekide generikoa zereginera esleituta dago.](media/Resource-Management-image25.png)

    <span data-ttu-id="2f66d-197">**Taldea** fitxan, taldekide generikoko berria ikusiko duzu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-197">On the **Team** tab, you will see the new generic team member.</span></span> <span data-ttu-id="2f66d-198">Kontuan izan orduak bakarrik esleituta dituela.</span><span class="sxs-lookup"><span data-stu-id="2f66d-198">Notice that it has only assigned hours.</span></span> <span data-ttu-id="2f66d-199">Ordu horiek taldekide generikoari esleitzen zaizkion zeregin guztien batura dira.</span><span class="sxs-lookup"><span data-stu-id="2f66d-199">These hours are the sum of all tasks that are assigned to the generic team member.</span></span> <span data-ttu-id="2f66d-200">Taldekide generikoak oraindik ez du ordurik edo baliabide eskakizunik behar.</span><span class="sxs-lookup"><span data-stu-id="2f66d-200">The generic team member doesn't yet have required hours or a resource requirement.</span></span>

    ![Taldekide generikoa Taldea fitxan](media/Resource-Management-image26.png)

5. <span data-ttu-id="2f66d-202">Orain taldekide generikoa beste zeregin batzuei esleitu diezaiekezu Baliabide hautatzailea erabiliz.</span><span class="sxs-lookup"><span data-stu-id="2f66d-202">You can now assign the generic team member to other tasks by using the Resource Picker.</span></span>

    ![Baliabide hautatzailean taldekide generikoa](media/Resource-Management-image27.png)

    <span data-ttu-id="2f66d-204">Baliabide generikoa zereginetan esleitzen amaitu duzunean, baliabide generikorako baliabide eskakizuna sor dezakezu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-204">When you've finished assigning the generic resource to tasks, you can generate a resource requirement for the generic resource.</span></span>

5. <span data-ttu-id="2f66d-205">**Taldea** fitxa, hautatu baliabide generikoa eta ondoren hautatu **Sortu eskakizuna**.</span><span class="sxs-lookup"><span data-stu-id="2f66d-205">On the **Team** tab, select the generic resource, and then select **Generate Requirement**.</span></span>

    ![Sortu eskakizuna komandoa](media/Resource-Management-image28.png)

    <span data-ttu-id="2f66d-207">Baldintza sortzen denean, taldekide generikoak orduak eta esteka beharko ditu baliabideen eskakizuna lortzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-207">When the requirement is generated, the generic team member will have required hours and a link for the resource requirement.</span></span>

    ![Baliabidearen eskakizunaren esteka](media/Resource-Management-image29.png)

    <span data-ttu-id="2f66d-209">Erreserba izena duen baliabide batek osatu eta bete ostean, baliabide generikoa taldetik kenduko da eta izena duen baliabidearen bidez ordezkatuko da.</span><span class="sxs-lookup"><span data-stu-id="2f66d-209">After you book a named resource, the generic resource is removed from the team and replaced by the named resource.</span></span>

    ![Baliabide generikoa izena duen baliabidearen ordez](media/Resource-Management-image30.png)

    <span data-ttu-id="2f66d-211">**Antolaketa** fitxan, baliabide generikoen esleipenak izena duen baliabidearen bidez kendu eta ordezkatu egingo dira.</span><span class="sxs-lookup"><span data-stu-id="2f66d-211">On the **Schedule** tab, the generic resource assignments are removed and replaced by the named resource.</span></span>

    ![Antolaketa fitxan, baliabide generikoen esleipenak izena duen baliabidearen bidez ordezkatuta](media/Resource-Management-image31.png)

    > [!NOTE]
    > <span data-ttu-id="2f66d-213">Jokabide hau izena duen baliabide bat baliabide generikoen eskakizuna guztiz erreserbatzen denean gertatzen da.</span><span class="sxs-lookup"><span data-stu-id="2f66d-213">This behavior occurs only when a named resource is fully booked for the generic resource requirement.</span></span> <span data-ttu-id="2f66d-214">Izena duen baliabide batek partzialkui baliabide generikoen eskakizuna ordezkatzen duenean edo izena duten baliabide anitzek baliabide generikoen eskakizuna ordezkatzen dutenean, baliabide generikoa zereginari esleitzen zaio.</span><span class="sxs-lookup"><span data-stu-id="2f66d-214">When either a named resource partially replaces the generic resource requirement or multiple named resources replace the generic resource requirement, the generic resource remains assigned to the task.</span></span>

    <span data-ttu-id="2f66d-215">Hurrengo irudian, 80 orduko zereginak bost eguneko iraupena izan dezan aurreikusi da (egunean 16 ordu bost egunetan zehar) eta **Funtzionala** izena duen baliabide generikoari esleitu zaio.</span><span class="sxs-lookup"><span data-stu-id="2f66d-215">In the following illustration, an 80-hour task has been planned for a five-day duration (16 hours per day over five days) and assigned to the generic resource that is named **Functional**.</span></span>

    ![Laurogei ordu eta bost eguneko zeregina Funtzionala baliabide generikoari esleituta](media/Resource-Management-image32.png)

    <span data-ttu-id="2f66d-217">Eskakizuna sortzen duzunean, 80 orduz bost egunetan zehar izaten da.</span><span class="sxs-lookup"><span data-stu-id="2f66d-217">When you generate the requirement, it's for 80 hours over five days.</span></span>

    ![80 egunetan sortutako eskakizuna bost egunetan zehar](media/Resource-Management-image33.png)

    <span data-ttu-id="2f66d-219">Eskuragarri dauden baliabideak egunean zortzi orduz bakarrik funtzionatzen dutenez, bi baliabide behar dira baldintza betetzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-219">Because available resources work only eight hours per day, two resources are needed to fulfill the requirement.</span></span>

    ![Bigarren baliabidea](media/Resource-Management-image35.png)

    <span data-ttu-id="2f66d-221">**Taldea** fitxan, ikus dezakezu baliabide generikoak ez duela ordurik behar, baina esleitutako orduak betetzea osatzen duten bi baliabideekin batera agertzen dira.</span><span class="sxs-lookup"><span data-stu-id="2f66d-221">On the **Team** tab, you can now see that the generic resource has no required hours, but the assigned hours still appear together with the two named resources that make up the fulfillment.</span></span>

    ![Bi baliabide izendatu dira Taldea fitxan](media/Resource-Management-image36.png)

    <span data-ttu-id="2f66d-223">**Antolaketa** fitxan, baliabide generikoa zereginari esleitzen zaio.</span><span class="sxs-lookup"><span data-stu-id="2f66d-223">On the **Schedule** tab, the generic resource remains assigned to the task.</span></span>

    ![Baliabide generikoak Antolaketa fitxan](media/Resource-Management-image37.png)

<span data-ttu-id="2f66d-225">PSAk ez ditu bi baliabideak zereginera esleitzen, jokaera horrek aurreikusteko antolaketa txikiagoa sortuko lukeelako.</span><span class="sxs-lookup"><span data-stu-id="2f66d-225">PSA doesn't assign both resources to the task, because that behavior would produce a less predictable schedule.</span></span> <span data-ttu-id="2f66d-226">Adibide erraz honetan, erraza da orduak bi baliabideen artean banatzea.</span><span class="sxs-lookup"><span data-stu-id="2f66d-226">In this simple example, it's easy to divide the hours equally between two resources.</span></span> <span data-ttu-id="2f66d-227">Hala ere, zeregin anitz eta baliabide anitz biltzen dituzten eszenatoki konplexuagoetan, PSAk zeregin ugaritan baliabide ugarietarako jasotzen diren erreserbak nola esleitu behar litzaizkion hipotesi batzuk egin beharko lituzke.</span><span class="sxs-lookup"><span data-stu-id="2f66d-227">However, in more complex scenarios that involve multiple tasks and multiple resources, PSA would have to make assumptions about how it should allocate the bookings that are received for multiple resources across multiple tasks.</span></span>

<span data-ttu-id="2f66d-228">Hori dela eta, gertakari horietan, proiektuaren arduraduna arduratzen da erreserba anitzak analizatzeaz eta behar izanez gero esleitzea.</span><span class="sxs-lookup"><span data-stu-id="2f66d-228">Therefore, in these scenarios, the project manager is responsible for parsing the multiple bookings and assigning them as needed.</span></span> <span data-ttu-id="2f66d-229">Erreserbak esleitzeko, proiektuaren arduradunak zereginak baliabide generikoetatik esleitzen dizkio izendatutako baliabideei, eta ondoren erabiltzen du **Kontziliazioa** ikuspegia, esleipena erreserbak funtzionatzen duela ziurtatzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-229">To allocate the bookings, the project manager assigns the tasks from the generic resources to the named resources and then uses the **Reconciliation** view to make sure that the allocation works with the bookings.</span></span>

### <a name="edit-a-resource-requirement"></a><span data-ttu-id="2f66d-230">Baliabidearen eskakizuna editatu</span><span class="sxs-lookup"><span data-stu-id="2f66d-230">Edit a resource requirement</span></span>

<span data-ttu-id="2f66d-231">Baliabideen eskakizuna sortu ondoren, proiektu-kudeatzaileak edo baliabideen kudeatzaileak xehetasunak editatu nahi ditu bilaketa-irizpideak afinatzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-231">After a resource requirement has been created, a project manager or resource manager might want to edit the details to refine the search criteria when the Schedule Board is used.</span></span> <span data-ttu-id="2f66d-232">Baliabideen eskakizuna editatzeko, jarraitu urrats hauek.</span><span class="sxs-lookup"><span data-stu-id="2f66d-232">To edit the resource requirement, follow these steps.</span></span>

1. <span data-ttu-id="2f66d-233">**Proiektuak** orrialdean **Taldea** fitxan, hautatu baliabide generikoko edozein eskakizunerako esteka.</span><span class="sxs-lookup"><span data-stu-id="2f66d-233">On the **Projects** page, on the **Team** tab, select the link to any requirement on a generic resource.</span></span>
2. <span data-ttu-id="2f66d-234">**Baliabideen eskakizuna** agertzen den orrian, hainbat atributu eguneratu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-234">On the **Resource Requirement** page that appears, you can update several attributes.</span></span> <span data-ttu-id="2f66d-235">Hona hemen zenbait adibideak:</span><span class="sxs-lookup"><span data-stu-id="2f66d-235">Here are some examples:</span></span>

    - <span data-ttu-id="2f66d-236">Izena</span><span class="sxs-lookup"><span data-stu-id="2f66d-236">Name</span></span>
    - <span data-ttu-id="2f66d-237">Hasiera-data</span><span class="sxs-lookup"><span data-stu-id="2f66d-237">From Date</span></span>
    - <span data-ttu-id="2f66d-238">Amaiera-data</span><span class="sxs-lookup"><span data-stu-id="2f66d-238">To Date</span></span>
    - <span data-ttu-id="2f66d-239">Iraupena</span><span class="sxs-lookup"><span data-stu-id="2f66d-239">Duration</span></span>
    - <span data-ttu-id="2f66d-240">Baliabide mota</span><span class="sxs-lookup"><span data-stu-id="2f66d-240">Resource Type</span></span>

<span data-ttu-id="2f66d-241">**Baliabideen eskakizuna** orrialdean, proiektuaren kudeatzaileak edo baliabideen kudeatzaileak informazio hau ere defini dezake:</span><span class="sxs-lookup"><span data-stu-id="2f66d-241">On the **Resource Requirement** page, the project manager or resource manager can also define the following information:</span></span>

- <span data-ttu-id="2f66d-242">Trebetasunak</span><span class="sxs-lookup"><span data-stu-id="2f66d-242">Skills</span></span>
- <span data-ttu-id="2f66d-243">Funtzioak</span><span class="sxs-lookup"><span data-stu-id="2f66d-243">Roles</span></span>
- <span data-ttu-id="2f66d-244">Baliabideen hobespenak</span><span class="sxs-lookup"><span data-stu-id="2f66d-244">Resource preferences</span></span>
- <span data-ttu-id="2f66d-245">Hobetsitako erakunde-unitateak</span><span class="sxs-lookup"><span data-stu-id="2f66d-245">Preferred organizational unit</span></span>

### <a name="update-resource-bookings-after-they-are-booked-on-a-project"></a><span data-ttu-id="2f66d-246">Eguneratu baliabideen erreserbak proiektu batean erreserbatu ondoren</span><span class="sxs-lookup"><span data-stu-id="2f66d-246">Update resource bookings after they are booked on a project</span></span>

<span data-ttu-id="2f66d-247">Baliabide generikoak edo izena dutenak proiektu talde batean gehitu ondoren, baliabidearen erreserbak alda ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-247">After you've added a generic or named resource to a project team, you can change the resource's bookings.</span></span>

1. <span data-ttu-id="2f66d-248">**Proiektuak** orrialdean **Taldea** fitxan, aukeratu taldekidea eta gero hautatu **Mantendu erreserbak**.</span><span class="sxs-lookup"><span data-stu-id="2f66d-248">On the **Projects** page, on the **Team** tab, select a team member, and then select **Maintain Bookings**.</span></span>

    ![Antolaketa-panela ireki da hautatutako taldekideentzat](media/Resource-Management-image40.png)

    <span data-ttu-id="2f66d-250">Antolaketa-panela agertzen da eta proiektuko taldekideen erreserbak agertzen dira.</span><span class="sxs-lookup"><span data-stu-id="2f66d-250">The Schedule Board appears and shows the project team member's bookings.</span></span> <span data-ttu-id="2f66d-251">Zabaldu taldekidearen erregistroa proiektu honen aurka erreserbatu diren orduak eta taldekidearen ahalmena kontsumitzen duten gainerako proiektuak ikusteko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-251">Expand the team member's record to view the hours that have been booked against this project and other projects that are consuming the team member's capacity.</span></span>

2. <span data-ttu-id="2f66d-252">Hautatu eta arrastatu erreserba luzatzeko edo laburtzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-252">Select and drag the booking to extend or shorten it.</span></span> <span data-ttu-id="2f66d-253">**Sortu Baliabideen Erreserba** elkarrizketa-koadroa agertuko da erreserba egokitzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-253">A **Create Resource Booking** dialog box appears that lets you adjust the booking.</span></span>

    ![Sortu baliabide-erreserba elkarrizketa-koadroa](media/Resource-Management-image41.png)

3. <span data-ttu-id="2f66d-255">Egin klik eskuineko botoiarekin erreserban.</span><span class="sxs-lookup"><span data-stu-id="2f66d-255">Right-click the booking.</span></span> <span data-ttu-id="2f66d-256">Jarraian, ekintza hauek burutzeko lasterbide menua erabil dezakezu:</span><span class="sxs-lookup"><span data-stu-id="2f66d-256">You can then use the shortcut menu to complete the following actions:</span></span>

    - <span data-ttu-id="2f66d-257">Aldatu erreserbaren egoera.</span><span class="sxs-lookup"><span data-stu-id="2f66d-257">Change the booking status.</span></span>
    - <span data-ttu-id="2f66d-258">Editatu erreserba.</span><span class="sxs-lookup"><span data-stu-id="2f66d-258">Edit the booking.</span></span>
    - <span data-ttu-id="2f66d-259">Proiektuko taldeko baliabide bat ordeztu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-259">Substitute a resource on the project team.</span></span>

### <a name="change-the-booking-status"></a><span data-ttu-id="2f66d-260">Aldatu erreserbaren egoera</span><span class="sxs-lookup"><span data-stu-id="2f66d-260">Change the booking status</span></span>

<span data-ttu-id="2f66d-261">Lehenetsitako edo pertsonalizatutako erreserba egoera alda dezakezu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-261">You can change any default or custom booking status.</span></span>

![Komandoaren egoera aldatu](media/Resource-Management-image42.png)

<span data-ttu-id="2f66d-263">Egoera hauek daude PSA aplikazioan:</span><span class="sxs-lookup"><span data-stu-id="2f66d-263">The following statuses are included in PSA:</span></span>

- <span data-ttu-id="2f66d-264">**Utzita**: egoera honek baliabideen erreserba bertan behera uzten du eta baliabidearen ahalmena askatzen du.</span><span class="sxs-lookup"><span data-stu-id="2f66d-264">**Canceled** – This status cancels a resource's booking and frees up the resource's capacity.</span></span>
- <span data-ttu-id="2f66d-265">**Erreserba gogorra**: egoera honek baliabideen ahalmena kontsumitzen du.</span><span class="sxs-lookup"><span data-stu-id="2f66d-265">**Hard Book** – This status consumes a resource's capacity.</span></span> <span data-ttu-id="2f66d-266">Erreserbak normalean egoera hau du **Mantendu Erreserbak** **Taldekide guztiak** saretatik **Proiektuak** orrian irekitzen duzunean.</span><span class="sxs-lookup"><span data-stu-id="2f66d-266">A booking typically has this status when you open **Maintain Bookings** from the **All Team Members** grid on the **Projects** page.</span></span>
- <span data-ttu-id="2f66d-267">**Erreserba biguna**: egoera honek baliabide bat gehitzen dio taldeari baina ez du baliabidearen ahalmena kontsumitzen.</span><span class="sxs-lookup"><span data-stu-id="2f66d-267">**Soft Book** – This status adds a resource to a team but doesn't consume the resource's capacity.</span></span> <span data-ttu-id="2f66d-268">Baliabidea lan potentzialerako erreserbatu dela adierazten du, baina hala ere, gaitasuna badu beste lan batzuetan behar bada.</span><span class="sxs-lookup"><span data-stu-id="2f66d-268">It indicates that the resource has been reserved for potential work but still has capacity if it's needed on other jobs.</span></span> <span data-ttu-id="2f66d-269">Baliabideen erabilgarritasun orokorraren iritziz, erreserba leunek erreserba gogorrak baino beste egoera bat dute.</span><span class="sxs-lookup"><span data-stu-id="2f66d-269">In the view of overall resource availability, soft bookings have a different status than hard bookings.</span></span>
- <span data-ttu-id="2f66d-270">**Proposatua**: egoera honek baliabideen kudeatzailearen edo proiektuaren kudeatzailearen proposamena adierazten du.</span><span class="sxs-lookup"><span data-stu-id="2f66d-270">**Proposed** – This status represents a resource manager's or project manager's proposal for a resource.</span></span> <span data-ttu-id="2f66d-271">Proposamenek ez dute baliabide baten ahalmena kontsumitzen eta baliabidea ez da proiektuko taldeari gehitzen.</span><span class="sxs-lookup"><span data-stu-id="2f66d-271">Proposals don't consume the capacity of a resource, and the resource isn't added to the project team.</span></span> <span data-ttu-id="2f66d-272">Baliabidea taldean erreserbatzeko, proiektuaren zuzendariak proposamena onartu behar du.</span><span class="sxs-lookup"><span data-stu-id="2f66d-272">To hard-book the resource on the team, the project manager must accept the proposal.</span></span>

### <a name="submit-resource-requests"></a><span data-ttu-id="2f66d-273">Bidali baliabide-eskaerak</span><span class="sxs-lookup"><span data-stu-id="2f66d-273">Submit resource requests</span></span>

<span data-ttu-id="2f66d-274">Baliabide-kudeatzaile batek bete behar duen eskaera (baliabide-eskakizuna) egiteko erabiltzen dira baliabide eskakizunak.</span><span class="sxs-lookup"><span data-stu-id="2f66d-274">Resource requests are used to carry the demand (resource requirement) that must be fulfilled by a resource manager.</span></span> <span data-ttu-id="2f66d-275">Dagoeneko taldean dagoen baliabide generikoa lortzeko, baliabide eskaera zuzenean bidal dezakezu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-275">For a generic resource that is already on the team, you can submit a resource request directly.</span></span> <span data-ttu-id="2f66d-276">Baliabide eskaera bi eratara bete daiteke:</span><span class="sxs-lookup"><span data-stu-id="2f66d-276">A resource request can be fulfilled in two ways:</span></span>

- <span data-ttu-id="2f66d-277">Baliabideen kudeatzaileak eskaera zuzenean betetzen du.</span><span class="sxs-lookup"><span data-stu-id="2f66d-277">The resource manager directly fulfills the request.</span></span> <span data-ttu-id="2f66d-278">+Kasu honetan, baliabide generikoa izena duen baliabide erreserba gogorraren ordez ordezkatuko da.</span><span class="sxs-lookup"><span data-stu-id="2f66d-278">In this case, the generic resource is replaced by a hard booking that has a named resource.</span></span>
- <span data-ttu-id="2f66d-279">Baliabideen kudeatzaileak baliabide bat proposatzen dio proiektuaren kudeatzaileari, eta proiektuaren kudeatzaileak proposatutako baliabidea onartu edo arbuiatu egiten du.</span><span class="sxs-lookup"><span data-stu-id="2f66d-279">The resource manager proposes a resource to the project manager, and the project manager approves or rejects the proposed resource.</span></span>

#### <a name="direct-fulfillment-of-resource-requests"></a><span data-ttu-id="2f66d-280">Baliabideen eskaerak zuzenean betetzea</span><span class="sxs-lookup"><span data-stu-id="2f66d-280">Direct fulfillment of resource requests</span></span>

<span data-ttu-id="2f66d-281">Baliabide-eskakizuna sortzen denean, proiektu-kudeatzaileak baliabide generiko baterako baliabide-eskaera aurkez dezake baliabidea hautatuz eta ondoren hautatuta **Bidali eskaera** aukera.</span><span class="sxs-lookup"><span data-stu-id="2f66d-281">When a resource requirement is generated, a project manager can submit a resource request for a generic resource by selecting the resource and then selecting **Submit Request**.</span></span>

![Bidali eskaera botoia](media/Resource-Management-image45.png)

<span data-ttu-id="2f66d-283">Baliabideari buruzko iruzkinak eskaera betetzen ari den baliabide kudeatzaileari eman diezaiokezu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-283">Comments about the resource can be provided to the resource manager who is fulfilling the request.</span></span> <span data-ttu-id="2f66d-284">Eskaera bidali ondoren, **Egoera** eremua taldekidearentzako aldatu egingo da **Bidalita** egoerara.</span><span class="sxs-lookup"><span data-stu-id="2f66d-284">After the request is submitted, the **Status** field for the team member is changed to **Submitted**.</span></span>

![Aukerako iruzkinak sartu](media/Resource-Management-image46.png)

<span data-ttu-id="2f66d-286">Baliabideen kudeatzaileak eskaera betetzen duenean, taldekide generikoa izena duen baliabidearen ordez ordezkatuko da **Taldekide guztiak** saretan.</span><span class="sxs-lookup"><span data-stu-id="2f66d-286">When the resource manager fulfills the request, the generic team member is replaced by the named resource in the **All Team Members** grid.</span></span>

![Taldekide generikoa izena duen baliabidearengatik ordezkatu dute Taldekide guztiak sartean](media/Resource-Management-image47.png)

#### <a name="use-a-resource-proposal-for-resource-requests"></a><span data-ttu-id="2f66d-288">Erabili baliabide proposamen bat baliabide eskaeretarako</span><span class="sxs-lookup"><span data-stu-id="2f66d-288">Use a resource proposal for resource requests</span></span>

<span data-ttu-id="2f66d-289">Baliabideen eskaera zuzenean erreserbatu beharrean, baliabideen kudeatzaileak proiektuaren kudeatzaileari baliabidea proposatu diezaioke.</span><span class="sxs-lookup"><span data-stu-id="2f66d-289">Instead of directly booking a resource on a resource request, a resource manager can propose a resource to the project manager.</span></span> <span data-ttu-id="2f66d-290">Baliabideen kudeatzaile batek aukera hau erabil dezake eskakizunekin bat datorrenean eskuragarri ez dagoenean.</span><span class="sxs-lookup"><span data-stu-id="2f66d-290">A resource manager might use this option when an exact match for the requirements isn't available.</span></span> <span data-ttu-id="2f66d-291">Baliabideen kudeatzaileak baliabide bat proposatzen duenean, proiektuaren kudeatzaileak ikusten du **Egoera** eremua taldekide generikorako aldatu egingo dela **Beharrak berrikustea** egoerara.</span><span class="sxs-lookup"><span data-stu-id="2f66d-291">When a resource manager proposes a resource, the project manager sees that the **Status** field for the generic team member is changed to **Needs Review**.</span></span>

![Taldekide generikoaren egoera Beharrak berrikustea egoerara aldatu da](media/Resource-Management-image48.png)

<span data-ttu-id="2f66d-293">Proposatutako baliabidea proposamenaren erreserbaren eragina bistaratzearekin batera ikusteko, egin klik bikoitza **Beharrak berrikustea** egoera duen taldekidean.</span><span class="sxs-lookup"><span data-stu-id="2f66d-293">To view the proposed resource together with a visualization of the effect of the proposal's booking, double-click the team member that has a status of **Needs Review**.</span></span> <span data-ttu-id="2f66d-294">Ondoren hautatu **Proposatutako baliabideak** fitxa.</span><span class="sxs-lookup"><span data-stu-id="2f66d-294">Then select the **Proposed Resources** tab.</span></span>

![Baliabide proposatuak fitxa](media/Resource-Management-image49.png)

<span data-ttu-id="2f66d-296">Aukeratu **Onartu proposamen guztiak** proposatutako baliabide guztiak onartzeko edo **Proposamen guztiak arbuiatu** arbuiatzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-296">Select **Accept All Proposals** to accept all proposed resources or **Reject All Proposals** to reject them.</span></span> <span data-ttu-id="2f66d-297">Proposatutako baliabideak onartzen badituzu, proiektuan erreserbatu egiten dira taldekide gisa eta baliabide generikoak ordezkatzen dituzte.</span><span class="sxs-lookup"><span data-stu-id="2f66d-297">If you accept the proposed resources, they are hard-booked on the project as team members and replace the generic resources.</span></span>

> [!NOTE]
> <span data-ttu-id="2f66d-298">Proposatutako baliabide guztiak onartu edo baztertu beharko dituzu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-298">You must either accept or reject all proposed resources.</span></span> <span data-ttu-id="2f66d-299">Ezin dituzu partzialki onartu edo arbuiatu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-299">You can't partially accept or reject them.</span></span>

### <a name="substitute-a-resource-on-the-project-team"></a><span data-ttu-id="2f66d-300">Proiektuko taldeko baliabide bat ordeztu</span><span class="sxs-lookup"><span data-stu-id="2f66d-300">Substitute a resource on the project team</span></span>

<span data-ttu-id="2f66d-301">Batzuetan, proiektuko kudeatzaileak proiektuan erreserbatutako taldekide bat ordezkatu behar du.</span><span class="sxs-lookup"><span data-stu-id="2f66d-301">Sometimes, a project manager must substitute a booked team member on a project.</span></span>

1. <span data-ttu-id="2f66d-302">**Proiektuak** orrialdean **Taldea** fitxan, aukeratu ordezkoa behar duen baliabidea eta gero hautatu **Mantendu erreserbak**.</span><span class="sxs-lookup"><span data-stu-id="2f66d-302">On the **Projects** page, on the **Team** tab, select the resource that needs a substitute, and then select **Maintain Bookings**.</span></span>
2. <span data-ttu-id="2f66d-303">Zabaldu baliabidea esleitutako proiektuak ikusteko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-303">Expand the resource to view the projects that it's assigned to.</span></span>

    ![Esleitutako proiektuak erakusteko zabaldutako baliabidea](media/Resource-Management-image50.png)

3. <span data-ttu-id="2f66d-305">Egin klik proiektuan eskuineko botoiarekin, eta, ondoren, hautatu **Baliabidea ordezkatu**.</span><span class="sxs-lookup"><span data-stu-id="2f66d-305">Right-click the project, and then select **Substitute Resource**.</span></span>
4. <span data-ttu-id="2f66d-306">Uneko baliabidea ordezkatu nahi duzun baliabidea ezagutzen baduzu, hautatu edo idatzi izena eta, ondoren, hautatu **Esleitu berriro**.</span><span class="sxs-lookup"><span data-stu-id="2f66d-306">If you know the resource that you want to substitute for the current resource, select or type the name, and then select **Re-assign**.</span></span>

    ![Ordezko baliabidea zehaztea](media/Resource-Management-image51.png)

    <span data-ttu-id="2f66d-308">Bestela, jarraitu urrats hauei baliabidea bilatzeko:</span><span class="sxs-lookup"><span data-stu-id="2f66d-308">Alternatively, follow these steps to search for a resource:</span></span>

    1. <span data-ttu-id="2f66d-309">Hautatu **Bilatu ordezkoa**.</span><span class="sxs-lookup"><span data-stu-id="2f66d-309">Select **Find Substitution**.</span></span>

        ![Ordezko baliabidea bilatzea](media/Resource-Management-image52.png)

        <span data-ttu-id="2f66d-311">Antolaketa laguntzaileak eskuragarri dauden ordezkoen zerrenda itzultzen du.</span><span class="sxs-lookup"><span data-stu-id="2f66d-311">The Schedule Assistant returns a list of available substitutes.</span></span> <span data-ttu-id="2f66d-312">Antolaketa laguntzailean, erabilgarri dauden baliabideak iragazi ditzakezu ordezko egoki bat bilatzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-312">In the Schedule Assistant, you can further filter the available resources to find a suitable substitute.</span></span>

        ![Erabilgarri dauden ordezkoen zerrenda.](media/Resource-Management-image53.png)

    2. <span data-ttu-id="2f66d-314">Baliabidea ordezkatzeko, hautatu nahi duzun baliabidea eta, gero, hautatu **Ordezkatu**.</span><span class="sxs-lookup"><span data-stu-id="2f66d-314">To substitute the resource, select the resource that you want, and then select **Substitute**.</span></span>

        ![Ordeztu hautatutako baliabidea](media/Resource-Management-image54.png)

    <span data-ttu-id="2f66d-316">Erreserbak eta zereginak baliabide berriarekin ordezkatuko dira.</span><span class="sxs-lookup"><span data-stu-id="2f66d-316">The bookings and assignments are substituted with the new resource.</span></span>

    ![Erreserbak eta zereginak baliabide berriarekin ordezkatuko dira](media/Resource-Management-image55.png)

## <a name="reconcile-team-member-bookings-and-assignments"></a><span data-ttu-id="2f66d-318">Kontziliatu taldekideen erreserbak eta esleipenak</span><span class="sxs-lookup"><span data-stu-id="2f66d-318">Reconcile team member bookings and assignments</span></span>

<span data-ttu-id="2f66d-319">Taldekideentzat, erreserbak eta zereginak bateratu egiten dira.</span><span class="sxs-lookup"><span data-stu-id="2f66d-319">For team members, bookings and assignments are loosely coupled.</span></span> <span data-ttu-id="2f66d-320">Alegia, baliabideek zereginak izan ditzakete baina erreserbarik ez, edo erreserbak izan ditzakete baina zereginik ez.</span><span class="sxs-lookup"><span data-stu-id="2f66d-320">In other words, resources can have assignments but no bookings, or they can have bookings but no assignments.</span></span> <span data-ttu-id="2f66d-321">Egokiena, erreserbak eta zereginak lerrokatuta egotea izango litzateke, baliabideek zereginak betetzeko gaitasuna konprometituta izan dezaten.</span><span class="sxs-lookup"><span data-stu-id="2f66d-321">Ideally, bookings and assignments should be aligned, so that resources have committed capacity to perform the task assignments.</span></span> <span data-ttu-id="2f66d-322">Hala ere, erreserbak erabilgarritasunean oinarrituta egon litezke, eta zereginen aldaketak proiektuak aurrera egin ahala alda litezke.</span><span class="sxs-lookup"><span data-stu-id="2f66d-322">However, the bookings might be based on availability, and task timings might change as the project continues.</span></span> <span data-ttu-id="2f66d-323">Hori dela eta, erreserbak eta zereginen akoplamendu solteak malgutasuna ematen du.</span><span class="sxs-lookup"><span data-stu-id="2f66d-323">Therefore, the loose coupling of bookings and assignments provides flexibility.</span></span>

<span data-ttu-id="2f66d-324">PSAk proiektu-kudeatzaileei taldekideen erreserbak eta proiektuko taldeen zereginak bateratzeko aukera ematen dien **Kontziliazioa** fitxa du.</span><span class="sxs-lookup"><span data-stu-id="2f66d-324">PSA has a **Reconciliation** tab that lets project managers reconcile team members' bookings and their assignments for project teams.</span></span>

![Kontziliazioa fitxa](media/Resource-Management-image56.png)

<span data-ttu-id="2f66d-326">**Kontziliazioa** fitxak erreserbak eta zereginak erakusten ditu zereginen esleipen bakoitzaren mailan taldekide bakoitzarentzat.</span><span class="sxs-lookup"><span data-stu-id="2f66d-326">The **Reconciliation** tab shows bookings and assignments down to the level of the individual task assignment for each team member.</span></span> <span data-ttu-id="2f66d-327">Denbora erakusten ditu gelaxkatan, hilabetetik egunera arteko epeak.</span><span class="sxs-lookup"><span data-stu-id="2f66d-327">It shows hours in cells that represent time periods from months down to days.</span></span>

<span data-ttu-id="2f66d-328">Fitxak proiektuaren guztizko garbi osoa ere erakusten du, zutabe guztiekin batera.</span><span class="sxs-lookup"><span data-stu-id="2f66d-328">The tab also shows an overall net total for the project, together with a total column.</span></span>

<span data-ttu-id="2f66d-329">Baliabide bakoitzerako, fitxak taldekidearen erreserben desberdintasunak kalkulatzen ditu eta taldekideen zereginen esleipenekin bateratzen ditu.</span><span class="sxs-lookup"><span data-stu-id="2f66d-329">For each resource, the tab calculates the difference between the team member's bookings and a rollup of the team member's task assignments.</span></span> <span data-ttu-id="2f66d-330">Egokiena, aldea 0 (zero) izatea da.</span><span class="sxs-lookup"><span data-stu-id="2f66d-330">Ideally, this difference should be 0 (zero).</span></span> <span data-ttu-id="2f66d-331">Beste modu batera esanda, ez litzateke alderik egon behar erreserbaren eta esleipenen artean.</span><span class="sxs-lookup"><span data-stu-id="2f66d-331">In other words, there should be no difference between bookings and assignments.</span></span> <span data-ttu-id="2f66d-332">Desberdintasunak koloreztatuta eta itzalpean daude bi baldintzetan arreta jartzeko:</span><span class="sxs-lookup"><span data-stu-id="2f66d-332">Differences are colored and shaded to draw attention to two conditions:</span></span>

- <span data-ttu-id="2f66d-333">**Erreserba eskasia**: erreserba eskasia gertatzen da baliabideek erreserbak baino esleipen gehiago dituztenean.</span><span class="sxs-lookup"><span data-stu-id="2f66d-333">**Booking shortage** – A booking shortage occurs when a resource has more assignments than bookings.</span></span> <span data-ttu-id="2f66d-334">Ez denez erreserbatu gaitasun hori, baliteke proiektu-kudeatzaileak baldintza hori zuzentzea baliabideen erreserbak hedatuz defizita estaltzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-334">Because this capacity hasn't been reserved, a project manager might want to correct this condition by extending the resource's bookings to cover the deficit.</span></span>
- <span data-ttu-id="2f66d-335">**Gehiegizko erreserbak** - Gehiegizko erreserbak baliabide bat proiektuan erreserbatuta dagoenean baina zereginetara esleitu ez denean gertatzen da.</span><span class="sxs-lookup"><span data-stu-id="2f66d-335">**Excess bookings** – Excess bookings occur when a resource has been booked to the project but hasn't been assigned to tasks.</span></span> <span data-ttu-id="2f66d-336">Baldintza hau onargarria izan daiteke zereginen esleipena gertatu baino lehen proiektuan erreserbatu den kasuetan.</span><span class="sxs-lookup"><span data-stu-id="2f66d-336">This condition might be acceptable in the cases where the resource was booked to the project before task assignment occurred.</span></span> <span data-ttu-id="2f66d-337">Hala ere, baliteke beste kasu batzuetan baliabidea ez izatea aurreikusita zereginei esleitzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-337">However, in other cases, the resource isn't planned to be assigned to tasks.</span></span> <span data-ttu-id="2f66d-338">Kasu horietan, proiektu-kudeatzaileak baliabidearen erreserbak bertan behera uztea pentsatu beharko luke, gaitasuna beste proiektu baterako erabili ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-338">In these cases, the project manager should consider canceling the resource's bookings, so that the capacity can be used for another project.</span></span>

<span data-ttu-id="2f66d-339">Zenbait kasutan, eguneko maila baino maila altuagoan ikusten baduzu (adibidez, hilabetearen maila), baliteke zero diferentzia garbia izatea baliabide batentzat (beste modu batera esanda, erreserbak = zereginak).</span><span class="sxs-lookup"><span data-stu-id="2f66d-339">In some cases, when you view time at a higher level than the day level (for example, the month level), you might see a net difference of zero for a resource (in other words, bookings = assignments).</span></span> <span data-ttu-id="2f66d-340">Hala ere, Astea mailari erreparatuz gero, baliteke 0 (zero) orduko esleipenak eta 40 orduko erreserbak daudela ikustea lehenengo astean, baina 40 orduko esleipenak eta 0 (zero) orduko erreserbak bigarren astean.</span><span class="sxs-lookup"><span data-stu-id="2f66d-340">However, if you view time at the week level, you might see that there are assignments of zero hours and bookings of 40 hours in the first week, but assignments of 40 hours and bookings of zero hours in the second week.</span></span> <span data-ttu-id="2f66d-341">Oro har, erreserbak eta zereginak bateratu egiten dira, baina aste batetik bestera desberdinak dira.</span><span class="sxs-lookup"><span data-stu-id="2f66d-341">Overall, the bookings and assignments are reconciled, but they differ from one week to the next.</span></span>

<span data-ttu-id="2f66d-342">Denbora-maila altuagoak ikusten dituzunean, **Kontziliazioa** fitxak gelaxkak adierazle bat du denbora maila baxuagoetan desberdintasunak daudela jakinarazteko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-342">When you view time at higher levels, cells in the **Reconciliation** tab have an indicator to inform you that there are differences at lower levels.</span></span> <span data-ttu-id="2f66d-343">Gelaxka batean klik bikoitza eginez, handiagotu dezakezu aldea ikusteko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-343">By double-clicking in a cell, you can zoom in to view the difference.</span></span> <span data-ttu-id="2f66d-344">Ondoren, egin klik eskuineko botoiarekin hurbiltzeko. Baliabide bat hautatuta eta, ondoren, erabilita **Hurrengo aldea** kontrola saretako tresna-barran, baliabide horren erreserbak eta zereginen arteko hurrengo diferentziara joan zaitezke.</span><span class="sxs-lookup"><span data-stu-id="2f66d-344">You can then right-click to zoom out. By selecting a resource and then using the **Next difference** control on the grid toolbar, you can go to the next difference between bookings and assignments for that resource.</span></span> <span data-ttu-id="2f66d-345">Ondoren, erabil dezakezu **Aurreko aldea** kontrola atzera egiteko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-345">You can then use the **Previous difference** control to go back.</span></span> <span data-ttu-id="2f66d-346">Alderantzizko adierazlea eta nabigazio portaera ere desaktiba ditzakezu **Ezarpenak** aukeran.</span><span class="sxs-lookup"><span data-stu-id="2f66d-346">You can also turn off the difference indicator and navigation behavior under **Settings**.</span></span>

![Diferentziaren adierazlea](media/Resource-Management-image57.png)

<span data-ttu-id="2f66d-348">Zereginen esleipenak dituzun baina erreserbarik ez baduzu, **Proiektuak** aorrian, **Kontziliazioa** fitxan, erreserba eskasia aukeratu dezakezu eta, ondoren, hautatu **Hedatu erreserba**.</span><span class="sxs-lookup"><span data-stu-id="2f66d-348">If you have task assignments for a resource but no bookings, on the **Projects** page, on the **Reconciliation** tab, select the booking shortage, and then select **Extend Booking**.</span></span> <span data-ttu-id="2f66d-349">**Luzatu Erreserba** elkarrizketa-koadroa agertuko da eta baliabidearen eskasiari aurre egiteko beharrezkoa den erreserba erakusten du.</span><span class="sxs-lookup"><span data-stu-id="2f66d-349">The **Extend Booking** dialog box appears and shows the booking that is needed to address the resource's shortage.</span></span> <span data-ttu-id="2f66d-350">Gainera, baliabideek dituzten erreserbak agertzen dira proiektu guztietan edo beste erakunde antolatzaile batzuetan.</span><span class="sxs-lookup"><span data-stu-id="2f66d-350">It also shows the resource's existing bookings across all projects or other schedulable entities.</span></span> <span data-ttu-id="2f66d-351">Aukeratzen baduzu **Ados** baliabidearen erreserba sortzeko, baliabidearen erabilgarritasuna edozein dela ere, gerta daiteke erreserba gehiegi egotea.</span><span class="sxs-lookup"><span data-stu-id="2f66d-351">If you select **OK** to create the booking for the resource, regardless of that resource's availability, you might cause overbooking.</span></span>

![Luzatu Erreserba elkarrizketa-koadroa](media/Resource-Management-image58.png)

<span data-ttu-id="2f66d-353">Orduan, proiektu-kudeatzaileak edo baliabide-kudeatzaileak antolaketa-panela erabil dezake baliabide batek bere ahalmenetatik harago gaitasunak gainditutako edozein egoera kudeatzeko.</span><span class="sxs-lookup"><span data-stu-id="2f66d-353">The project manager or resource manager can then use the Schedule Board to manage any situations where a resource is overbooked beyond its capacity.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]