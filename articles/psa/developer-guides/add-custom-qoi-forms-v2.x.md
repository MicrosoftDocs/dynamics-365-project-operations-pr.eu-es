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
ms.reviewer: johnmichalak
ms.openlocfilehash: ffc702bbe9cedb2a0cc8da8d8f58e48005950127
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8584305"
---
# <a name="add-new-custom-entity-forms-project-service-automation-2x"></a>Gehitu entitate pertsonalizatuaren inprimaki berriak (Project Service Automation 2.x)

[!include [banner](../../includes/psa-now-project-operations.md)]

## <a name="type-field"></a>Eremu mota 

Dynamics 365 Project Service Automation oinarritzen da **Mota** (**msdyn\_ordertype**) eremuan abagunea, eskaintza, eskaera eta fakturak entitateetan, bereizteko **Lanean oinarritutako** erakunde horien bertsioak **elementua oinarritutako** eta **zerbitzu-oinarritutako** bertsioak. Entitate horien lanerako bertsioak PSAk kudeatzen ditu. Bezeroaren eta zerbitzariaren aldean negozioen logika asko daude **Mota** eremuan. Hori dela eta, garrantzitsua da eremua entitateak sortzen direnean balio zuzena izatea. Balio okerrak portaera okerrak sor ditzake eta baliteke zenbait negozio logikak ez izatea ondo funtzionatzea.

## <a name="automatic-form-switching"></a>Inprimakia aldatzea automatikoki

Datuen ustelkeria eta salmenta-entitateen erregistro okerrak hastea eta editatzea eragiten duten ustekabeko jokabideak saihesteko, PSAk orain inprimakiak automatikoki aldatzeko logika dakar. Logika honek erabiltzaileak lanerako bertsioarekin edo abagune, eskaintza, eskaera edo fakturako beste edozein erakunderekin lan egiteko inrpimaki egokira eramaten ditu. Erabiltzaileak abagunea, eskaintza, eskaera edo faktura entitate baten lanerako oinarritutako bertsioa irekitzen duenean, inprimakia aldatu egiten da **Proiektuaren informazioa** eremura.

Inprimakia aldatzeko automatikoen logika maiztasunaren arteko esleipenean oinarritzen da **formId** balioa eta **msdyn\_ordertype** eremua. Kartelaz kanpoko inprimaki guztiak erantsi zaizkio esleipen horri. Hala ere, inprimaki pertsonalizatuak eskuz gehitu behar dira zein entitate kudeatu nahi duten adierazteko. Honetan oinarritzen da: **msdyn\_ordertype** eremua. Inprimakia aldatzea esleipenean falta bada, logika berezko inprimakira aldatuko da, gordetako balioan oinarrituta, **msdyn\_ordertype** entitatearen eremuan.

## <a name="add-custom-forms-and-turn-on-the-form-switching-logic"></a>Gehitu inprimaki pertsonalizatuak eta piztu inprimakia aldatzeko logika

Hurrengo adibidean, inprimaki pertsonalizatua nola gehitu daitekeen erakusten da, **Nire proiektuaren informazioa**, beraz, laneko abaguneekin lan egiteko. Prozesu bera erabiltzen da inprimaki pertsonalizatuak gehitzeko, eskaintzekin, eskaeren eta fakturen bidez lan egiteko.

Jarraitu urrats hauei bertsio pertsonalizatua sortzeko, **Proiektuaren informazioa** inprimakiarena.

1. Abagunea erakundean, ireki **Proiektuaren informazioa** inprimakia eta gorde kopia **Nire proiektuaren informazioa** izenarekin.
2. Ireki inprimaki berria eta, ondoren, egin ezazu propietateetan, ziurtatu inprimakiaren hasierako scriptak, **Proiektuaren informazioa** inprimakikoak, daudela. 

    > [!IMPORTANT]
    > Ez kendu gidoiak. Bestela, datu batzuk oker has daitezke.

3. Egiaztatu **Mota** (**msdyn\_ordertype**) eremua inprimakian dagoela. 

    > [!IMPORTANT]
    > Ez kendu eremu hau Bestela, hasierako gidoiek huts egingo dute.

4. Aurkitu **formId** balioa inprimaki berriarena. Bi modutara bete dezakezu urrats hau:

    - Esportatu **Nire proiektuaren informazioa** inprimakia kudeatu gabeko irtenbide baten zati gisa eta, ondoren, bilatu **formId** esportatutako soluzioaren customization.xml fitxategiaren balioa.
    - Ireki **Nire proiektuaren informazioa** inprimakia inprimaki-editorean, eta ondoren bilatu globalki identifikatzaile bakarra (GIDA) **fromId** parametroaren ondoan URLan, hurrengo irudian erakusten den moduan.

    ![formId balioa inprimaki berriarena, URLan.](media/how-to-add-custom-forms-in-v2.0.png)

5. Sortu **msdyn\_ordertype** esleipenak **formId** baliorako msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js web baliabidea editatuz. Kendu kodea baliabidetik eta jarri hurrengo kodearekin.

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

6. Gorde eta, gero, argitaratu pertsonalizazioak.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
