---
title: Gehitu entitate pertsonalizatuaren inprimaki berriak (Project Service Automation 2.x)
description: Gai honek entitate pertsonalizatuaren inprimakiak gehitzeko informazioa eskaintzen du, aukerak, eskaintzak, eskaerak edo fakturak sartzeko Dynamics 365 Project Service Automation 2.x-n
author: makk
ms.custom:
- dyn365-projectservice
ms.date: 3/14/2019
ms.topic: article
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 400d817ee7cbae6f6da95db4286ad6c4d6ff349a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6007981"
---
# <a name="add-new-custom-entity-forms-project-service-automation-2x"></a><span data-ttu-id="7b4f9-103">Gehitu entitate pertsonalizatuaren inprimaki berriak (Project Service Automation 2.x)</span><span class="sxs-lookup"><span data-stu-id="7b4f9-103">Add new custom entity forms (Project Service Automation 2.x)</span></span>

[!include [banner](../../includes/psa-now-project-operations.md)]

## <a name="type-field"></a><span data-ttu-id="7b4f9-104">Eremu mota</span><span class="sxs-lookup"><span data-stu-id="7b4f9-104">Type field</span></span> 

<span data-ttu-id="7b4f9-105">Dynamics 365 Project Service Automation oinarritzen da **Mota** (**msdyn\_ordertype**) eremuan abagunea, eskaintza, eskaera eta fakturak entitateetan, bereizteko **Lanean oinarritutako** erakunde horien bertsioak **elementua oinarritutako** eta **zerbitzu-oinarritutako** bertsioak.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-105">Dynamics 365 Project Service Automation relies on the **Type** (**msdyn\_ordertype**) field of the Opportunity, Quote, Order, and Invoice entities to distinguish **work-based** versions of these entities from **item-based** and **service-based** versions.</span></span> <span data-ttu-id="7b4f9-106">Entitate horien lanerako bertsioak PSAk kudeatzen ditu.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-106">Work-based versions of these entities are handled by PSA.</span></span> <span data-ttu-id="7b4f9-107">Bezeroaren eta zerbitzariaren aldean negozioen logika asko daude **Mota** eremuan.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-107">Lots of business logic on the client side and server side of the solution depends on the **Type** field.</span></span> <span data-ttu-id="7b4f9-108">Hori dela eta, garrantzitsua da eremua entitateak sortzen direnean balio zuzena izatea.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-108">Therefore, it's important that the field be initialized with a correct value when the entities are created.</span></span> <span data-ttu-id="7b4f9-109">Balio okerrak portaera okerrak sor ditzake eta baliteke zenbait negozio logikak ez izatea ondo funtzionatzea.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-109">An incorrect value can cause incorrect behaviors, and some business logic might not run correctly.</span></span>

## <a name="automatic-form-switching"></a><span data-ttu-id="7b4f9-110">Inprimakia aldatzea automatikoki</span><span class="sxs-lookup"><span data-stu-id="7b4f9-110">Automatic form switching</span></span>

<span data-ttu-id="7b4f9-111">Datuen ustelkeria eta salmenta-entitateen erregistro okerrak hastea eta editatzea eragiten duten ustekabeko jokabideak saihesteko, PSAk orain inprimakiak automatikoki aldatzeko logika dakar.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-111">To avoid potential data corruption and unexpected behaviors that are caused by incorrect initialization and editing of the sales entity records, PSA now includes logic for automatic form switching in out-of-box forms.</span></span> <span data-ttu-id="7b4f9-112">Logika honek erabiltzaileak lanerako bertsioarekin edo abagune, eskaintza, eskaera edo fakturako beste edozein erakunderekin lan egiteko inrpimaki egokira eramaten ditu.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-112">This logic takes users to the correct form for working with the work-based version or any other type of Opportunity, Quote, Order, or Invoice entity.</span></span> <span data-ttu-id="7b4f9-113">Erabiltzaileak abagunea, eskaintza, eskaera edo faktura entitate baten lanerako oinarritutako bertsioa irekitzen duenean, inprimakia aldatu egiten da **Proiektuaren informazioa** eremura.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-113">When a user opens the work-based version of an Opportunity, Quote, Order, or Invoice entity, the form is switched to **Project Information**.</span></span>

<span data-ttu-id="7b4f9-114">Inprimakia aldatzeko automatikoen logika maiztasunaren arteko esleipenean oinarritzen da **formId** balioa eta **msdyn\_ordertype** eremua.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-114">The automatic form switching logic relies on the mapping between the **formId** value and the **msdyn\_ordertype** field.</span></span> <span data-ttu-id="7b4f9-115">Kartelaz kanpoko inprimaki guztiak erantsi zaizkio esleipen horri.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-115">All out-of-box forms have been added to that mapping.</span></span> <span data-ttu-id="7b4f9-116">Hala ere, inprimaki pertsonalizatuak eskuz gehitu behar dira zein entitate kudeatu nahi duten adierazteko.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-116">However, custom forms must be manually added to indicate which version of the entity they are intended to handle.</span></span> <span data-ttu-id="7b4f9-117">Honetan oinarritzen da: **msdyn\_ordertype** eremua.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-117">This is based on the **msdyn\_ordertype** field.</span></span> <span data-ttu-id="7b4f9-118">Inprimakia aldatzea esleipenean falta bada, logika berezko inprimakira aldatuko da, gordetako balioan oinarrituta, **msdyn\_ordertype** entitatearen eremuan.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-118">If the form switching is missing from the mapping, logic will switch to the out-of-box form, based on the value that is saved in the **msdyn\_ordertype** field of the entity.</span></span>

## <a name="add-custom-forms-and-turn-on-the-form-switching-logic"></a><span data-ttu-id="7b4f9-119">Gehitu inprimaki pertsonalizatuak eta piztu inprimakia aldatzeko logika</span><span class="sxs-lookup"><span data-stu-id="7b4f9-119">Add custom forms and turn on the form switching logic</span></span>

<span data-ttu-id="7b4f9-120">Hurrengo adibidean, inprimaki pertsonalizatua nola gehitu daitekeen erakusten da, **Nire proiektuaren informazioa**, beraz, laneko abaguneekin lan egiteko.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-120">The following example shows how to add a custom form, **My Project Information**, so that it works with work-based opportunities.</span></span> <span data-ttu-id="7b4f9-121">Prozesu bera erabiltzen da inprimaki pertsonalizatuak gehitzeko, eskaintzekin, eskaeren eta fakturen bidez lan egiteko.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-121">The same process is used to add custom forms so that they work with quotes, orders, and invoices.</span></span>

<span data-ttu-id="7b4f9-122">Jarraitu urrats hauei bertsio pertsonalizatua sortzeko, **Proiektuaren informazioa** inprimakiarena.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-122">Follow these steps to create a custom version of the **Project Information** form.</span></span>

1. <span data-ttu-id="7b4f9-123">Abagunea erakundean, ireki **Proiektuaren informazioa** inprimakia eta gorde kopia **Nire proiektuaren informazioa** izenarekin.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-123">In the Opportunity entity, open the **Project Information** form, and save a copy under the name **My Project Information**.</span></span>
2. <span data-ttu-id="7b4f9-124">Ireki inprimaki berria eta, ondoren, egin ezazu propietateetan, ziurtatu inprimakiaren hasierako scriptak, **Proiektuaren informazioa** inprimakikoak, daudela.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-124">Open the new form, and then, in the properties, make sure that the form initialization scripts from the **Project Information** form are present.</span></span> 

    > [!IMPORTANT]
    > <span data-ttu-id="7b4f9-125">Ez kendu gidoiak.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-125">Don't remove the scripts.</span></span> <span data-ttu-id="7b4f9-126">Bestela, datu batzuk oker has daitezke.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-126">Otherwise, some data might be initialized incorrectly.</span></span>

3. <span data-ttu-id="7b4f9-127">Egiaztatu **Mota** (**msdyn\_ordertype**) eremua inprimakian dagoela.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-127">Verify that the **Type** (**msdyn\_ordertype**) field is present in the form.</span></span> 

    > [!IMPORTANT]
    > <span data-ttu-id="7b4f9-128">Ez kendu eremu hau</span><span class="sxs-lookup"><span data-stu-id="7b4f9-128">Don't remove this field.</span></span> <span data-ttu-id="7b4f9-129">Bestela, hasierako gidoiek huts egingo dute.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-129">Otherwise, the initialization scripts will fail.</span></span>

4. <span data-ttu-id="7b4f9-130">Aurkitu **formId** balioa inprimaki berriarena.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-130">Find the **formId** value of the new form.</span></span> <span data-ttu-id="7b4f9-131">Bi modutara bete dezakezu urrats hau:</span><span class="sxs-lookup"><span data-stu-id="7b4f9-131">You can complete this step in two ways:</span></span>

    - <span data-ttu-id="7b4f9-132">Esportatu **Nire proiektuaren informazioa** inprimakia kudeatu gabeko irtenbide baten zati gisa eta, ondoren, bilatu **formId** esportatutako soluzioaren customization.xml fitxategiaren balioa.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-132">Export the **My Project Information** form as part of an unmanaged solution, and then look up the **formId** value in the customization.xml file of the exported solution.</span></span>
    - <span data-ttu-id="7b4f9-133">Ireki **Nire proiektuaren informazioa** inprimakia inprimaki-editorean, eta ondoren bilatu globalki identifikatzaile bakarra (GIDA) **fromId** parametroaren ondoan URLan, hurrengo irudian erakusten den moduan.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-133">Open the **My Project Information** form in the form editor, and then look for the globally unique identifier (GUID) next to the **fromId** parameter in the URL, as shown in the following illustration.</span></span>

    ![formId balioa inprimaki berriarena, URLan](media/how-to-add-custom-forms-in-v2.0.png)

5. <span data-ttu-id="7b4f9-135">Sortu **msdyn\_ordertype** esleipenak **formId** baliorako msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js web baliabidea editatuz.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-135">Create an **msdyn\_ordertype** mapping for the **formId** value by editing the msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js web resource.</span></span> <span data-ttu-id="7b4f9-136">Kendu kodea baliabidetik eta jarri hurrengo kodearekin.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-136">Remove the code from the resource, and replace it with the following code.</span></span>

    ```javascript
    define(["require", "exports"], function (require, exports) {
        "use strict";
        var SalesDocumentCustomFormIds = (function () {
            function SalesDocumentCustomFormIds() {
            }
            SalesDocumentCustomFormIds.overwriteFormIds = function (mappedFormIds) {
                /*
                ---- Notes ----
                mappedFormIds[SalesEntity][OrderType] => The array of forms IDs that support particular entity and order type
                Add or overwrite customized formId for the particular entity and order type by calling:
                    mappedFormIds[<EntityType>][<msdyn_ordertype>].push("<formId>");
                Allowed msdyn_ordertype values for reference:
                    ServiceBased: 690970002 (Field Service version of the entity)
                    WorkBased: 192350001 (PSA version of the entity)
                    ItemBased: 192350000 (Regular out of the box entity)
                Uncomment and update one of the following lines to register custom PSA form for required entity:
                */      
                //mappedFormIds[1][192350001].push("<formId>"); //Quote
                //mappedFormIds[5][192350001].push("<formId>"); //Quote Line
                //mappedFormIds[2][192350001].push("<formId>"); //Sales Order
                //mappedFormIds[6][192350001].push("<formId>"); //Sales Order Line
                // In this example we have added new form for Opportunity
                mappedFormIds[0][192350001].push("192EE537-DCC4-45D3-B7AF-EA694B9113D2"); //Opportunity
                //mappedFormIds[4][192350001].push("<formId>"); //Opportunity Line
            };
            return SalesDocumentCustomFormIds;
        }());
        exports.default = SalesDocumentCustomFormIds;
    });
    ```

6. <span data-ttu-id="7b4f9-137">Gorde eta, gero, argitaratu pertsonalizazioak.</span><span class="sxs-lookup"><span data-stu-id="7b4f9-137">Save and then publish the customizations.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]