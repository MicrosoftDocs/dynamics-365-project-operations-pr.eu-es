---
title: Proiektuaren antolaketa-erregistroak
description: Artikulu honek Project Scheduling erregistroak erabiltzen lagunduko dizuten informazioa eta laginak eskaintzen ditu Project Scheduling Service eta Project Scheduling APIekin erlazionatutako hutsegiteen jarraipena egiteko.
author: ruhercul
ms.date: 11/30/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: c57419642e90e4def01f2cd2474c9e82dc162b86
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8923680"
---
# <a name="project-scheduling-logs"></a>Proiektuaren antolaketa-erregistroak

_**Honi dagokio:** Baliabideetan edo hornituta ez dauden agertokietarako proiektuen eragiketak, Lite inplementazioa - fakturazio proforma jorratu_, _proiektua_

Microsoft Dynamics 365 Project Operations erabilerak [Weberako proiektua](https://support.microsoft.com/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5) bere programazio-motor nagusi gisa. Estandarra erabili beharrean Microsoft Dataverse Web aplikazioen programazio-interfazeak (API), Project Operations-ek Project Scheduling API berriak erabiltzen ditu proiektuko zereginak, baliabide-esleipenak, ataza-menpekotasunak, proiektu-kuboak eta proiektu-taldeetako kideak sortzeko, eguneratzeko eta ezabatzeko. Hala ere, sortu, eguneratu edo ezabatu eragiketak lanaren banaketa egituraren (WBS) entitateetan programatikoki exekutatzen direnean, akatsak gerta daitezke. Akats hauen eta eragiketen historiaren jarraipena egiteko, bi administrazio-erregistro berri ezarri dira: **Eragiketa multzoa** eta **Proiektuak Planifikatzeko Zerbitzua (PSS)**. Erregistro hauetara sartzeko, joan hona **Ezarpenak** \> **Ordutegien Integrazioa**.

Ondorengo ilustrazioak Proiektuaren Programazio-erregistroen datu-eredua erakusten du.

![Proiektuaren Programazioaren erregistroetarako datu-eredua.](media/LOGDATAMODEL.jpg)

## <a name="operation-set-log"></a>Eragiketa Ezarri erregistroa

Eragiketa-multzoaren erregistroak eragiketa-multzo baten exekuzioaren jarraipena egiten du, sorta batean sortu, eguneratu edo ezabatzeko eragiketa bat edo asko exekutatzeko, proiektuetan, proiektu-zereginetan, baliabide-esleipenetan, ataza-menpekotasunean, proiektu-ontzietan edo proiektu-taldekideetan. The **Funtzionamendua Egoeran** eremuak eragiketa multzoaren egoera orokorra erakusten du. Eragiketa-multzoaren karga-kargaren xehetasunak erlazionatutako Eragiketa-multzoaren xehetasun-erregistroetan jasotzen dira.

### <a name="operation-set"></a>Eragiketa multzoa

Ondoko taulan, honekin erlazionatutako eremuak erakusten dira **Eragiketa multzoa** entitate.

| Eskemaren izena            | Deskribapenak                                                                                                  | DisplayName            |
|-----------------------|--------------------------------------------------------------------------------------------------------------|------------------------|
| msdyn_completedon     | Eragiketa ezarri edo huts egin den data/ordua.                                                | CompletedOn            |
| msdyn_correlationid   | The **korrelazioId** eskaeraren balioa.                                                                  | CorrelationId          |
| msdyn_description     | Eragiketa-multzoaren deskribapena.                                                                        | Deskribapenak            |
| msdyn_executedon      | Erregistroa exekutatu zeneko data/ordua.                                                                       | Exekuzio-data            |
| msdyn_operationsetId  | Entitate-instantziaren identifikatzaile bakarra.                                                                   | OperationSet           |
| msdyn_Project         | Eragiketa multzoarekin zerikusia duen proiektua.                                                            | Project                |
| msdyn_projectid       | The **projectId** eskaeraren balioa.                                                                      | ProjectId (zaharkituta) |
| msdyn_projectName     | Ez da aplikagarria.                                                                                              | Ez da aplikagarria         |
| msdyn_PSSErrorLog     | Eragiketa-multzoarekin lotuta dagoen Project Scheduling Service errore-erregistroaren identifikatzaile bakarra. | PSS errore-erregistroa          |
| msdyn_PSSErrorLogName | Ez da aplikagarria.                                                                                              | Ez da aplikagarria         |
| msdyn_status          | Eragiketa multzoaren egoera.                                                                             | Fasea                 |
| msdyn_statusName      | Ez da aplikagarria.                                                                                              | Ez da aplikagarria         |
| msdyn_useraadid       | The Azure Active Directory (Azure AD) eskaerari dagokion erabiltzailearen objektuaren IDa.                     | UserAADID              |

### <a name="operation-set-detail"></a>Eragiketa-multzoaren xehetasuna

Ondoko taulan, honekin erlazionatutako eremuak erakusten dira **Eragiketa-multzoaren xehetasuna** entitate.

| Eskemaren izena                 | Deskribapenak                                                                                 | DisplayName           |
|----------------------------|---------------------------------------------------------------------------------------------|-----------------------|
| msdyn_cdspayload           | Serializatua Dataverse eskaera egiteko eremuak.                                            | CdsPayload            |
| msdyn_entityname           | Eskaera egiteko entitatearen izena.                                                     | EntityName            |
| msdyn_httpaditza             | Eskaera metodoa.                                                                         | HTTP aditza (zaharkitua) |
| msdyn_httpverbName         | Ez da aplikagarria.                                                                             | Ez da aplikagarria        |
| msdyn_operationset         | Erregistroari dagokion eragiketa-multzoaren identifikatzaile bakarra.                      | OperationSet          |
| msdyn_operationssetdetailId | Entitate-instantziaren identifikatzaile bakarra.                                                  | OperationSet xehetasuna   |
| msdyn_operationsetName     | Ez da aplikagarria.                                                                             | Ez da aplikagarria        |
| msdyn_operationtype        | Eragiketa-multzoaren eragiketa motaren xehetasuna.                                             | OperationType         |
| msdyn_operationtypeName    | Ez da aplikagarria.                                                                             | Ez da aplikagarria        |
| msdyn_psspayload           | Serializatutako Proiektua Planifikatzeko Zerbitzua eskaeraren eremuak.                           | PssPayload            |
| msdyn_recordid             | Eskaeraren erregistroaren identifikatzailea.                                                       | Erregistroaren IDa             |
| msdyn_requestnumber        | Automatikoki sortutako zenbakia, eskaerak jaso ziren ordena identifikatzen duena. | Eskaera-zenbakia        |

## <a name="project-scheduling-service-error-logs"></a>Project Scheduling Service erroreen erregistroak

Project Scheduling Service errore-erregistroek Project Scheduling Service saiatzean gertatzen diren hutsegiteak jasotzen dituzte **Gorde** edo **Ireki** operazioa. Erregistro hauek sortzen diren hiru eszenatoki onartzen dira:

- Erabiltzaileak abiarazitako ekintzek huts egiten dute (adibidez, ezin da esleipena sortu pribilegioak falta direlako).
- Proiektuak Planifikatzeko Zerbitzuak ezin du programatikoki sortu, eguneratu, ezabatu edo kaskadako beste eragiketarik egin entitate batean.
- Erabiltzaileak erroreak izaten ditu erregistro bat irekitzen ez denean (adibidez, proiektu bat irekitzen denean edo taldekide baten informazioa eguneratzen denean).

### <a name="project-scheduling-service-log"></a>Proiektua Planifikatzeko Zerbitzuaren erregistroa

Ondorengo taulak Project Scheduling Service erregistroan sartzen diren eremuak erakusten ditu.

| Eskemaren izena          | Deskribapenak                                                                    | DisplayName    |
|---------------------|--------------------------------------------------------------------------------|----------------|
| msdyn_CallStack     | Salbuespenaren dei-pila.                                               | Dei-pila     |
| msdyn_correlationid | Errorearen korrelazio IDa.                                               | CorrelationId  |
| msdyn_errorcode     | Gordetzeko erabiltzen den eremua Dataverse errore-kodea edo HTTP errore-kodea. | Errore-kodea     |
| msdyn_HelpLink      | Laguntza publikorako dokumentaziorako esteka.                                       | Laguntza-esteka      |
| msdyn_log           | Proiektuak Antolatzeko Zerbitzuaren erregistroa.                                   | Egunkaria            |
| msdyn_project       | Erroreen erregistroarekin lotutako proiektua.                             | Project        |
| msdyn_projectName   | Proiektuaren izena eragiketa-multzoaren kargari eutsiko bazaio. | Ez da aplikagarria |
| msdyn_psserrorlogId | Entitate-instantziaren identifikatzaile bakarra.                                     | PSS errore-erregistroa  |
| msdyn_SessionId     | Proiektuaren saioaren IDa.                                                        | Saioaren IDa     |

## <a name="error-log-cleanup"></a>Errorea erregistroa garbitzean

Lehenespenez, bai Project Scheduling Service erroreen erregistroak bai Operation Set erregistroa garbitu daitezke 90 egunez behin. 90 egun baino zaharragoak diren erregistroak ezabatu egingo dira. Hala ere, balioa aldatuz **msdyn_StateOperationSetAge** eremuan **Proiektuaren Parametroak** orrialdean, administratzaileek garbiketa-tartea doi dezakete, 1 eta 120 egun artean egon dadin. Balio hau aldatzeko hainbat metodo daude eskuragarri:

- Pertsonalizatu **Proiektuaren parametroa** entitatea orri pertsonalizatu bat sortuz eta gehituz **Stale Operations Set Age** eremua.
- Erabili bezero-kodea erabiltzen duen [WebApi softwarea garatzeko kit (SDK)](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-webapi/updaterecord).
- Erabili Xrm SDK erabiltzen duen Service SDK kodea **eguneratuErregistroa** metodoa (Client API reference) ereduetan oinarritutako aplikazioetan. Power Apps deskribapen bat eta onartzen dituen parametroak biltzen ditu **eguneratuErregistroa** metodoa.

    ```C#
    Xrm.WebApi.retrieveMultipleRecords('msdyn_projectparameter').then(function (response) {
        parameter = response.entities[0];
        var staleOperationValue = prompt("All records older than (x) days will be deleted, please enter X between 1 to 90 days", 1)
        var newData = {};
        newData.msdyn_projectparameterid = parameter.msdyn_projectparameterid;
        newData.msdyn_staleoperationsetage = parseInt(staleOperationValue);
        Xrm.WebApi.updateRecord("msdyn_projectparameter", parameter.msdyn_projectparameterid, newData).then(
            function success(result) {
                console.log("Project Parameter: Stale Operation Expiry is set to: " + newData.msdyn_staleoperationsetage);
                // perform operations on record update
                Xrm.WebApi.retrieveMultipleRecords('msdyn_projectparameter')
                .then(function (response2) { console.log("Confirmed Project Parameter: Stale Operation Expiry is set to: " + response2.entities[0].msdyn_staleoperationsetage) });
            },
            function (error) {
                console.log("Failed to Update Project Ednpoint with error: " + error.message);
            // handle error conditions
            }
        );
    });
    ```
