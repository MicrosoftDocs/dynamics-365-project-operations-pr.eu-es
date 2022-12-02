---
title: Proiektuaren antolaketa-erregistroak
description: Artikulu honek Proiektuak antolatzeko erregistroak erabiltzen lagunduko dizuten informazioa eta laginak eskaintzen ditu Proiektuak antolatzeko zerbitzua eta Proiektuak antolatzeko APIarekin erlazionatutako hutsegiteen jarraipena egiteko.
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

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako Project Operations, Lite hedapena - proformaren fakturazioari aurre egin,_, _Project for the Web_

Microsoft Dynamics 365 Project Operations-ek erabiltzen du [Project for the Web](https://support.microsoft.com/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5) bere programazio-motor nagusi gisa. Microsoft Dataverse Web-aplikazioen programazio-interfazeak (API) estandarra erabili beharrean, Project Operations-ek Project Scheduling API berriak erabiltzen ditu proiektuko zereginak, baliabide-esleipenak, zereginen menpekotasunak, proiektu-kuboak eta proiektu-taldeetako kideak sortzeko, eguneratzeko eta ezabatzeko. Dena den, sortu, eguneratu edo ezabatzeko eragiketak zereginen xehetasunen egitura (WBS) entitateetan programatikoki exekutatzen direnean, akatsak gerta daitezke. Errore horien eta eragiketen historiaren jarraipena egiteko, bi administrazio-erregistro berri ezarri dira: **Eragiketa multzoa** eta **Proiektuak Planifikatzeko Zerbitzua (PSS)**. Erregistro hauetara sartzeko, joan hona **Ezarpenak** \> **Ordutegien Integrazioa**.

Ondorengo ilustrazioak Proiektuaren Programazioaren erregistroen datu-eredua erakusten du.

![Proiektuaren antolaketaren erregistrorako datu-eredua.](media/LOGDATAMODEL.jpg)

## <a name="operation-set-log"></a>Eragiketa multzoaren konfigurazioa

Eragiketa-multzoaren erregistroak eragiketa-multzo baten exekuzioaren jarraipena egiten du sorta batean sortu, eguneratu edo ezabatzeko eragiketa bat edo asko exekutatzeko, proiektuetan, proiektu-zereginetan, baliabide-esleipenetan, ataza-menpekotasunean, proiektu-ontzietan edo proiektu-taldekideetan. **Egoerako eragiketa** eremuak eragiketa multzoaren egoera orokorra erakusten du. Eragiketa-multzoaren karga-kargaren xehetasunak erlazionatutako Eragiketa-multzoaren xehetasun-erregistroetan jasotzen dira.

### <a name="operation-set"></a>Eragiketa multzoa

Taula honetan **Eragiketa multzoa** entitatearekin erlazionatutako eremuak erakusten dira.

| Eskemaren izena            | Deskribapenak                                                                                                  | DisplayName            |
|-----------------------|--------------------------------------------------------------------------------------------------------------|------------------------|
| msdyn_completedon     | Eragiketa multzoa osatu edo huts egin zueneko data eta ordua.                                                | CompletedOn            |
| msdyn_correlationid   | Erregistroaren **correlationId** balioa.                                                                  | CorrelationId          |
| msdyn_description     | Eragiketa multzoaren azalpena.                                                                        | Deskribapenak            |
| msdyn_executedon      | Erregistroa exekutatu zen data eta ordua.                                                                       | Exekuzio-data            |
| msdyn_operationsetId  | Entitatearen instantzien identifikatzaile esklusiboa.                                                                   | OperationSet           |
| msdyn_Project         | Eragiketa multzoarekin erlazionatutako proiektua.                                                            | Project                |
| msdyn_projectid       | Erregistroaren **projectId** balioa.                                                                      | ProjectId (zaharkituta) |
| msdyn_projectName     | Ez da aplikagarria.                                                                                              | Ez da aplikagarria         |
| msdyn_PSSErrorLog     | Eragiketa multzoarekin lotuta dagoen Project Scheduling Service errore-erregistroaren identifikatzaile bakarra. | PSS errore-erregistroa          |
| msdyn_PSSErrorLogName | Ez da aplikagarria.                                                                                              | Ez da aplikagarria         |
| msdyn_status          | Eragiketa multzoaren egoera.                                                                             | Fasea                 |
| msdyn_statusName      | Ez da aplikagarria.                                                                                              | Ez da aplikagarria         |
| msdyn_useraadid       | Eskaera dagokion erabiltzailearen Azure Active Directory (Azure AD) objektuaren IDa.                     | UserAADID              |

### <a name="operation-set-detail"></a>Eragiketa multzoaren xehetasuna

Taula honetan **Eragiketa multzoaren xehetasuna** entitatearekin erlazionatutako eremuak erakusten dira.

| Eskemaren izena                 | Deskribapenak                                                                                 | DisplayName           |
|----------------------------|---------------------------------------------------------------------------------------------|-----------------------|
| msdyn_cdspayload           | Eskaeraren serializatutako Dataverse eremuak.                                            | CdsPayload            |
| msdyn_entityname           | Eskaerako entitatearen izena.                                                     | EntityName            |
| msdyn_httpverb             | Eskaera egiteko metodoa.                                                                         | HTTP aditza (zaharkitua) |
| msdyn_httpverbName         | Ez da aplikagarria.                                                                             | Ez da aplikagarria        |
| msdyn_operationset         | Erregistro hau dagokion eragiketa multzoaren identifikatzaile esklusiboa.                      | OperationSet          |
| msdyn_operationsetdetailId | Entitatearen instantzien identifikatzaile esklusiboa.                                                  | OperationSet xehetasuna   |
| msdyn_operationsetName     | Ez da aplikagarria.                                                                             | Ez da aplikagarria        |
| msdyn_operationtype        | Eragiketa multzoaren eragiketa motaren xehetasuna.                                             | OperationType         |
| msdyn_operationtypeName    | Ez da aplikagarria.                                                                             | Ez da aplikagarria        |
| msdyn_psspayload           | Serializatutako Proiektua Planifikatzeko Zerbitzua eskaeraren eremuak.                           | PssPayload            |
| msdyn_recordid             | Eskaera-erregistroaren identifikatzailea.                                                       | Erregistroaren IDa             |
| msdyn_requestnumber        | Eskaerak jasotako ordena identifikatzen duen automatikoki sortutako zenbakia. | Eskaera-zenbakia        |

## <a name="project-scheduling-service-error-logs"></a>Proiektuen antolaketa-zerbitzuaren errore-egunkaria

Project Scheduling Service errore-erregistroek Project Scheduling Service **Gorde** edo **Ireki** eragiketa egiten saiatzen denean gertatzen diren hutsegiteak jasotzen dituzte. Erregistro hauek sortzen diren hiru eszenatoki onartzen dira:

- Erabiltzaileak abiarazitako ekintzek huts egiten dute (adibidez, ezin da esleipena sortu pribilegioak falta direlako).
- Proiektuak Antolatzeko Zerbitzuak ezin du programazioz sortu, eguneratu, ezabatu edo ur-jauziko beste eragiketarik egin entitate batean.
- Erabiltzaileak erroreak izaten ditu erregistro bat irekitzen ez denean (adibidez, proiektu bat irekitzen denean edo taldekide baten informazioa eguneratzen denean).

### <a name="project-scheduling-service-log"></a>Proiektuen antolaketa-zerbitzuaren egunkaria

Taula honetan barne hartzen diren eremuak erakusten ditu, proiektuak antolatzeko zerbitzuaren egunkarian.

| Eskemaren izena          | Deskribapenak                                                                    | DisplayName    |
|---------------------|--------------------------------------------------------------------------------|----------------|
| msdyn_CallStack     | Salbuespenaren dei-pila.                                               | Dei-pila     |
| msdyn_correlationid | Errorearen korrelazio IDa.                                               | CorrelationId  |
| msdyn_errorcode     | Dataverse errore-kodea edo HTTP errore-kodea gordetzeko erabiltzen den eremua. | Errore-kodea     |
| msdyn_HelpLink      | Laguntza publikoaren dokumentaziorako esteka.                                       | Laguntza-esteka      |
| msdyn_log           | Proiektuak Antolatzeko Zerbitzuaren erregistroa.                                   | Egunkaria            |
| msdyn_project       | Errore-egunkariarekin erlazionatutako proiektua.                             | Project        |
| msdyn_projectName   | Proiektuaren izena eragiketa-multzoaren kargari eutsiko bazaio. | Ez da aplikagarria |
| msdyn_psserrorlogId | Entitatearen instantzien identifikatzaile esklusiboa.                                     | PSS errore-erregistroa  |
| msdyn_SessionId     | Proiektuaren saio IDa.                                                        | Saioaren IDa     |

## <a name="error-log-cleanup"></a>Errore-erregistroaren garbiketa

Lehenespenez, bai Project Scheduling Service erroreen erregistroak bai Operation Set erregistroa garbitu daitezke 90 egunean behin. Erregistro guztiak 90 egun baino zaharragoak ezabatuko dira. Hala ere, balioa aldatuz **msdyn_StateOperationSetAge** eremuarena **Proiektuaren Parametroak** orrialdean, administratzaileek garbiketa-tartea doi dezakete, 1 eta 120 egun artekoa izan dadin. Balio hau aldatzeko hainbat metodo daude eskuragarri:

- Pertsonalizatu **Proiektuaren parametroa** entitatea orri pertsonalizatu bat sortuz eta gehituz **Eragiketa multzo zaharkituaren adina** eremua.
- Erabili bezero-kodea [WebApi softwarea garatzeko kita (SDK)](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-webapi/updaterecord) erabiltzen duena.
- Erabili Xrm SDK erabiltzen duen Service SDK kodea **updateRecord** metodoa (bezeroaren API erreferentzia) ereduetan oinarritutako aplikazioetan. Power Apps-e deskribapen bat eta onartzen dituen parametroak biltzen ditu **updateRecord** metodorako.

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
