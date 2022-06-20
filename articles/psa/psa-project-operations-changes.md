---
title: Project Service Automation-etik Project Operations-erako eginbideen aldaketak
description: Artikulu honetan Project Service Automation a ren ezaugarri-aldaketei buruzko informazio orokorra ematen da Dynamics 365 Project Operations.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/03/2022
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
ms.reviewer: johnmichalak
ms.openlocfilehash: 8a6030faf777051ea1003679589af4bdf97322ab
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8925335"
---
# <a name="feature-changes-from-project-service-automation-to-project-operations"></a>Project Service Automation-etik Project Operations-erako eginbideen aldaketak

Literen eguneratzea Dynamics 365 Project Service Automation Dynamics 365 Project Operations hiru fasetan emango da. Artikulu honetan, eguneraketa osatzen denean ikusi artean izan ditzakeen aldaketa nagusiei buruzko informazioa ematen da.

| Eguneratzeak ematea | 1. fasea <br>(2022ko urtarrila) | 2. fasea <br>(2022ko apirileko olatua) | 3. fasea  |
|------------------|------------------------|---------------------------|---------------------------|
| Ez lan-egiturarekiko mendekotasunik (WBS) proiektuetarako. | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| WBS-a proiektuaren eragiketetan gaur egun onartzen diren mugetan sartuta. | &nbsp; | :heavy_check_mark: | :heavy_check_mark: |
| WBSa gaur egun project operations-era onartutako mugetatik kanpo, Project-eko idazmahaiko bezeroarentzako euskarria barne. | &nbsp; | &nbsp; | :heavy_check_mark: |

## <a name="project-management"></a>Proiektuen kudeaketa

Erabiltzailearen esperientzian izandako aldaketa esanguratsuenak proiektuak planifikatzeko arloan izango dira. Project Operations-ek esperientzia moderno berri bat hartu du lanaren desglose-egitura bat administratzeko (WBS), Project for the Web-ek [emandako programazio-gaitasunak aprobetxatuz](https://support.microsoft.com/en-us/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5).

## <a name="differences-in-the-scheduling-experience"></a>Diferentziak programazio-esperientzian

Hurrengo taulan Project Service Automation eta Project Operations-en arteko programazio-desberdintasunak laburbiltzen dira.

|  Antolatzen     |   Project Operations   |   PSA   |
|-----------------|------------------------|---------|
| Proiektu-plantillak: proiektu bat sortzen denean proiektu-plantillak definitzeko eta aplikatzeko gaitasuna  |  &nbsp;    | :heavy_check_mark: |
| Proiektuaren lana (WBS) eta idazmahaiko bezeroa sakribatzeko egitura integratzea   |    &nbsp;  | :heavy_check_mark: |
| Murrizketak: beranduenez amaitzen denean hasten da  | :heavy_check_mark: |   &nbsp;  |
| Mugarriak - Zero iraupeneko lanak   | :heavy_check_mark:  |  &nbsp;  |
| Baliabideetan oinarritutako zereginek esleitutako baliabideen erabilgarritasuna errespetatuko dute   | :heavy_check_mark: |  &nbsp;    |
| Edizioa denbora-faseka: planak argitaratu eta eguneroko lan egin   |   &nbsp;  | :heavy_check_mark: |
| Programazio automatikoa/ eskuzkoa: erabili proiektuak programatzeko motorra lanak modu automatikoan edo eskuz programatzeko |  &nbsp; | :heavy_check_mark:  |
| Proiektu handiak zuzenean erabiltzailearen interfazean editatzea: ez mugarik editatu daitezkeen planen tamainarako  | 500eko lanen muga  | :heavy_check_mark:       |
| Ehuneko osoa: lanaren aurrerapena markatzea   | :heavy_check_mark:  |  &nbsp;  |
| [Proiektuaren programazio-moduak](../project-management/scheduling-modes.md) : proiektua unitate finko, ahalegin finko edo iraupen finko gisa definitzen du | :heavy_check_mark: | &nbsp; |
| Denbora-lerroa: programazioaren xehetasunak bistaratzeko eta interesa duten aldeekin komunikatzeko denbora-lerroaren ikusmena sortzen eta pertsonalizatzen du. | :heavy_check_mark:  | &nbsp; |
| Ahaleginean oinarritutako zereginak: programazio-motorrarekin bateragarritasuna, ahaleginak bultzatutako zeregin bat programatzeko  | :heavy_check_mark:  | &nbsp; |
| **Elkarrizketa-koadroa Lanaren informazioa** : lanaren xehetasunak elkarrizketa-koadro baten bidez gordetzea | :heavy_check_mark:  |  &nbsp;  |
| Arrastaka ibili eta askatu: lan anitzak aukeratu eta WBSn duten posizioa aldatu | :heavy_check_mark: | &nbsp;  |
| Ikuspegi malguak: lanaren atributuen bistarik granularrenak zehazten ditu   | :heavy_check_mark:  | &nbsp; |
| Ordenatu eta filtratu WBS  | :heavy_check_mark:  | &nbsp; |
| Ur-jauzirik gabeko proiektuak entregatzeko taulak bista  | :heavy_check_mark:   | &nbsp; |
| Denbora-lerroaren ikuspegia: WBS ikusi eta editatzeko erabiltzen den Gantt interaktiboaren diagrama   | :heavy_check_mark:  | &nbsp; |
| Teklatuko metodo laburtuak: erabili teklatu-metodo laburtuak eragiketa komunetarako, hala nola sangria aplikatu edo txertatu  | :heavy_check_mark:  |  &nbsp; |
| Maila anitzeko desegitea: egin analisi hipotetikoa, aldaketen eragina erabat ulertzeko, inbertituz eta eragiketa-multzo oso bat aplikatuz | :heavy_check_mark: | &nbsp; |
| Moztu/Copiar/Pegar - Lagundu programatutako garapenean, aplikazioen arteko programazio-xehetasunak kopiatuz eta erantsiz  | :heavy_check_mark: | &nbsp; |
| Lanak egiaztatzeko zerrendak: egiaztapen-zerrendako 20 elementu ere erantsi zeregin batera   | :heavy_check_mark: | &nbsp; |

## <a name="project-planning"></a>Proiektuaren antolaketa

**Proiektu-eragiketen proiektu-orriak** alde nabarmena du proiektu-zerbitzuen Automatizazioko Proiektu-orriarekin **alderatuta**.

Honako ekintza hauek Proiektuen **orritik** kendu dira, 1 fasearen eguneratzearen parte gisa:

  - **Ireki MS Project-en**
  - **Sortu txantiloia**
  - **Kendu esteka MS Project-etik**

**Proiektu-eragiketen proiektuaren** orrialdeak honako fitxa berri hauek biltzen ditu.

- **Materialaren aurreikuspenak**
- **Zereginak fakturatzeko konfigurazioa**

**Estatu** fitxa kanporatu egin da eta **Estatua** laburpen **fitxan** dago orain, proiektuaren programazio moduarekin.

   ![Proiektuaren orrialdearen eguneratzeak.](media/projectform.png)

**Programazioaren** izena Tarea **fitxara** aldatu da eta Weberako Project-ekin proiektuak planifikatzeko esperientzia berria aurkeztu du.

   ![Proiektuaren lan berriak.](media/tasktab.png)

## <a name="scheduling-modes"></a>Antolaketa moduak

Project Operations-ek [ezaugarri berri bat sartu du, programazio moduak](../project-management/scheduling-modes.md). Project Service Automation-en proiektu guztiek aurrez **zehaztutako** balio finkoa izango dute proiektuaren eragiketetan. Hala ere, proiektu berrietarako aurrez zehaztutako balioa **parametroak** > **programatzeko parametro parametroak** > **konfiguratuz administratu daiteke.** > **·**

   ![Programazio-modurako proiektu-parametroen konfigurazioa.](media/projectparameter.png)

## <a name="project-planning-limits"></a>Proiektuak planifikatzeko mugak

Project Operations Project for the Web-en oinarritzen da proiektuak programatzeko eragiketa guztietarako. Project for the Web-ek lanaren desglose-egitura administratzen du, hurrengo taularen mugak erabiliz.

| **Eremua**                                          | **Muga**             |
|----------------------------------------------------|-----------------------|
| Proiektu baterako gehieneko zereginak                  | 500                   |
| Proiektu baten gehieneko iraupena               | 3650 egun (10 urte)  |
| Proiektu baterako gehieneko baliabideak              | 300                   |
| Proiektu bateko gehieneko estekak (ondorengoak soilik) | 600                   |
| Proiektu baterako gehieneko eremu pertsonalizatuak          | 1,0                    |
| Gehieneko hierarkia-maila                            | 10 maila             |
| Gehieneko estekak (ondorengoa + aurrekoa)            | 20                    |
| Hosto-zereginaren gehienezko iraupena                      | 1250 egun             |
| Laburpen-zeregin baten gehieneko iraupena                 | 3650 egun (10 urte)  |
| Zeregin bati esleitutako gehieneko baliabideak               | 20 baliabide          |
| Zeregin baterako onartutako data-tartea                    | 2000/1/1 - 2149/12/31 |
| Zerrendako elementuak                                    | 20                    |

## <a name="project-planning-extensibility-and-development"></a>Proiektuen plangintzaren zabaltasuna eta garapena

Proiektu-eragiketak eguneratu ondoren, proiektuen programazioko API-ak erabili behar dituzu honako erakunde hauetan sortze-, eguneratze- eta ezabatze-eragiketak gauzatzeko:

|   Entitatearen izena           |   Entitatearen izen logikoa       |
|-------------------------|-----------------------------|
| Project                 | msdyn_project               |
| Proiektuaren zeregina            | msdyn_projecttask           |
| Proiektuaren zereginen mendekotasuna | msdyn_projecttaskdependency |
| Baliabide-esleipena     | msdyn_resourceassignment    |
| Proiektuaren ontzia          | msdyn_projectbucket         |
| Proiektu-taldeko kidea     | msdyn_projectteam           |

Gaur egun erakunde horiek inplikatzen dituzten pertsonalizazioak badituzu, kontsulta ezazu [proiektuen programazio-apis-ak erabiltzea programazio-erakundeekin eragiketak egiteko, inplementazio-jarraibideak](../project-management/schedule-api-preview.md) lortzeko.

## <a name="data-model-changes"></a>Aldaketak datu-ereduan

1. eguneratze fasearen parte gisa, datu-ereduan aldaketak daude. Aldaketa horiek, batez ere, dauden entitateen landa-aldaketak dira. 1. fasean, erakundeak, **msydn_project** eta **msdyn_projectteam** pertsonalizazioak erreaktoreizatzea dira. 

> [!IMPORTANT]
> Atal hau erakunde gehigarriekin eguneratuko da, etorkizuneko eguneratze-faseak osatu ahala.

Hurrengo zelaien ordez eremu berriak hartu dira.

|   Entity          |   Izen logiko zaharra   |   Izen logiko berria    |
|-------------------|----------------------|-----------------------|
| msdyn_project     | msdyn_actualhours    | msdyn_effortcompleted |
| msdyn_project     | msdyn_plannedhours   | msdyn_effort          |
| msdyn_project     | msdyn_remaininghours | msdyn_effortremaining |
| msdyn_project     | msdyn_scheduledend   | msdyn_finish          |
| msdyn_project     | msdyn_wbsduration    | msdyn_duration        |
| msdyn_projectteam | msdyn_assignedhours  | msdyn_effort          |
| msdyn_projectteam | msdyn_from           | msdyn_start           |
| msdyn_projectteam | msdyn_to             | msdyn_finish          |

Hurrengo alor nagusiak gehitu dira.

|   Entity          |   Izen logikoa                               |   Deskribapenak |
|-------------------|----------------------------------------------|---------------|
| msdyn_project     | msdyn_actualfeesales                         | Proiektuan tarifa errealen salmenten agregatua erakusten du. Project Service Automation-en bakarrik erabiltzeko. |
| msdyn_project     | msdyn_actualmaterialcost                     | Materialak proiektuan duen benetako kostua erakusten du. Project Service Automation-en bakarrik erabiltzeko. |
| msdyn_project     | msdyn_actualmaterialsales                    | Proiektuan materialaren benetako salmentak erakusten ditu. Project Service Automation-en bakarrik erabiltzeko. |
| msdyn_project     | msdyn_businesscase                           |                |
| msdyn_project     | msdyn_contractlineproject                    | Proiektu honi lotutako kontratu-lerroa. |
| msdyn_project     | msdyn_copyprojectcorrelationid               | Korrelazio-identifikatzailearekin lotutako **proiektuak kopiatzeko** erabiltzen den sistemaren barne-eremua da. Project Service Automation-en bakarrik erabiltzeko. |
| msdyn_project     | msdyn_copyprojectsessionid                   | Hau barne-sistemaren eremu bat da, horretarako erabiltzen da **Kopiatu proiektua** Saioaren Identifikatzaileari lotutakoa. Project Service Automation-en bakarrik erabiltzeko. |
| msdyn_project     | msdyn_globalrevisiontoken                    | Azken sinkronizazioa xRM Global Revision Token Proiektua antolatzeko zerbitzutik. |
| msdyn_project     | msdyn_msprojectdocument                      | Proiektuari dagokion Microsoft Project dokumentua. |
| msdyn_project     | msdyn_plannedmaterialcost                    | Proiektuan aurreikusitako materialaren kostuaren agregatua. Project Service Automation-en bakarrik erabiltzeko. |
| msdyn_project     | msdyn_plannedmaterialsales                   | Proiektuan aurreikusitako material salmentaren agregatua. Project Service Automation-en bakarrik erabiltzeko. |
| msdyn_project     | msdyn_programa                                | Proiektu hau dagokion programa. |
| msdyn_project     | msdyn_quotelineproject                       | Proiektu honekin lotutako aurrekontu-lerroa. |
| msdyn_project     | msdyn_replaylogheader                        | Erreprodukzio-erregistroen goiburua. |
| msdyn_project     | msdyn_schedulemode                           | Proiektuko zeregin guztietan erabiltzen den programazio modu lehenetsia.  |
| msdyn_project     | msdyn_taskearlieststart                      | Proiektuko edozein zereginen lehenengo hasiera-data.  |
| msdyn_project     | msdyn_valuestatement                         |                |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | Proiektu-taldekide hau kopiatu den proiektu-taldekidea. |
| msdyn_projectteam | msdyn_creategenericteammember eskakizunarekin | Sortu berri den taldekide generiko baterako baliabide-eskakizuna sortu behar den adierazten du.  |
| msdyn_projectteam | msdyn_deletestatus                           | Taldekidearen ezabatze-egoera Proiektua antolatzeko zerbitzura bidalitako ezabatze-eskaerarik dagoen eta espero den denbora-leihoan erantzuna behar bezala bidaltzen duen jarraitzeko. |
| msdyn_projectteam | msdyn_effortcompleted                        | Taldekideak bere zereginetan egindako esfortzuaren jarraipena egiten du. |
| msdyn_projectteam | msdyn_effortremaining                        | Taldekideak bere zereginetan oraindik egin beharreko ahaleginaren jarraipena egiten du. |
| msdyn_projectteam | msdyn_markedfordeletiontimer                 | Taldekideak Proiektua antolatzeko zerbitzura ezabatzeko eskaera bidaltzen duenetik taldekidea benetan ezabatzen den arte itxaronaldia Microsoft Dataverse.|
| msdyn_projectteam | msdyn_markedfordeletiontimestamp             | Taldekidea ezabatzeko eskaera Proiektua antolatzeko zerbitzura bidaltzen denean grabatu beharreko denbora-zigilua. |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | Proiektuaren taldeko kidea hau kopiatutako proiektuaren taldeko kidea erakusten du.  |

## <a name="project-templates"></a>Proiektuen txantiloiak

Project Operations-ek ez du proiektuen txantiloietarako laguntzarik eskaintzen. Hala ere, oinarrizko funtzionalitatearen zati handi bat erreplikatu dezakezu [Project Copy APIa](../project-management/dev-copy-project.md).

## <a name="desktop-add-in-support"></a>Mahaigaineko gehigarrien laguntza

Microsoft Project Desktop gehigarriaren euskarria ez da erabilgarri egongo eguneratzearen lehen 2 faseetan. 3. fasean, Project for Web-en gaur egun onartzen dituen mugak baino proiektu handiagoak dituzten bezeroek mahaigaineko gehigarria erabili ahal izango dute.

## <a name="editing-resource-assignment-contours"></a>Baliabideen esleipenaren sestrak editatzea

Baliabideen esleipenaren sestrak editatzeko aukera erabilgarri egongo da eguneratzearen 2. fasea erabilgarri dagoenean.

## <a name="billing-and-pricing"></a>Fakturazioa eta prezioak

Honako ezaugarri berriak gehitu dira Proiektuaren Eragiketetan. Ezaugarri hauek izaera gehigarriak dira eta ez dute eraginik Project Service Automation datu-ereduan.

- [Proiektuetan eta proiektuetako zereginetan materialaren erabilera erregistratzea](../material/material-usage-log.md)
- [Azpikontratazio kudeaketa](../pro/subcontracting/managing-subcontracts-overview.md)
- [Aurrerakinak eta atxikipenetan oinarritutako kontratuak](../pro/sales/set-up-advances-retainer-based-contracts-sales.md)
- [Kontratuaren egoera ez gainditzeko eta baliozkotzeak](../pro/proforma-invoicing/manage-nte-status-validations-sales.md)
- [Zereginetan oinarritutako fakturazioa](../pro/sales/mapping-projects-tasks-quote-line-sales.md)

## <a name="deprecated-components"></a>Zaharkitutako osagaiak

Ondorengo taulek bertsio zaharkituta dauden osagaien soluziora eguneratu ondoren mugitzen diren eremu zaharkitu guztiak dokumentatzen dituzte. Informazio gehiagorako eta irtenbiderako estekarako, ikus [Dynamics 365 Project Service Automation 3x Project Operations 4x zaharkitutako osagaietara](https://github.com/microsoft/Dynamics365-Project-Operations-PowerApps/tree/main/3x-4x-deprecated-solution).

### <a name="invoicedetail"></a>Fakturaren xehetasuna

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
|invoicedetail.msdyn_contractline    |

### <a name="msdyn_actual"></a>msdyn_actual

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_actual.msdyn_salescontractline                                                          |

### <a name="msdyn_characteristicreqforteammember"></a>msdyn_characteristicreqforteammember

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_characteristicreqforteammember.msdyn_characteristic                                     |
| msdyn_characteristicreqforteammember.msdyn_characteristicreqforteammemberid                   |
| msdyn_characteristicreqforteammember.msdyn_characteristictype                                 |
| msdyn_characteristicreqforteammember.msdyn_name                                               |
| msdyn_characteristicreqforteammember.msdyn_ratingvalue                                        |
| msdyn_characteristicreqforteammember.msdyn_resourcerequirementid                              |

### <a name="msdyn_contractlineinvoiceschedule"></a>msdyn_contractlineinvoiceschedule

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_contractlineinvoiceschedule.msdyn_contractline                                          |
| msdyn_contractlinesscheduleofvalue.msdyn_contractline                                          |
 
### <a name="msdyn_dataexport"></a>msdyn_dataexport

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_dataexport.msdyn_dataexportid                                                           |
| msdyn_dataexport.msdyn_datatoken                                                              |
| msdyn_dataexport.msdyn_entityname                                                             |
| msdyn_dataexport.msdyn_exportedrecordcount                                                    |
| msdyn_dataexport.msdyn_exportstatus                                                           |
| msdyn_dataexport.msdyn_linkedentitydata                                                       |
| msdyn_dataexport.msdyn_name                                                                   |
| msdyn_dataexport.msdyn_pagingdata                                                             |

### <a name="msdyn_fact"></a>msdyn_fact

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_fact.msdyn_salescontractline                                                            |

### <a name="msdyn_findworkevent"></a>msdyn_findworkevent

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_findworkevent.msdyn_bookableresource                                                    |
| msdyn_findworkevent.msdyn_findworkeventid                                                     |
| msdyn_findworkevent.msdyn_name                                                                |
| msdyn_findworkevent.msdyn_timestamp                                                           |
| msdyn_findworkevent.msdyn_type                                                                |
| msdyn_findworkevent.msdyn_value                                                               |
| msdyn_findworkevent.msdyn_work                                                                |

### <a name="msdyn_invoicelinetransaction"></a>msdyn_invoicelinetransaction

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_invoicelinetransaction.msdyn_invoiceline                                                |
| msdyn_invoicelinetransaction.msdyn_salescontractline                                          |

### <a name="msdyn_journalline"></a>msdyn_journalline

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_journalline.msdyn_salescontractline                                                     |

### <a name="msdyn_opportunitylineresourcecategory"></a>msdyn_opportunitylineresourcecategory

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylineresourcecategory.msdyn_billingtype                                       |
| msdyn_opportunitylineresourcecategory.msdyn_description                                       |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylineresourcecategoryid                 |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylinetransactionclassification          |
| msdyn_opportunitylineresourcecategory.msdyn_resourcecategory                                  |

### <a name="msdyn_opportunitylinetransaction"></a>msdyn_opportunitylinetransaction

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransaction.msdyn_accountcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_accountingdate                                         |
| msdyn_opportunitylinetransaction.msdyn_accountvendor                                          |
| msdyn_opportunitylinetransaction.msdyn_amount                                                 |
| msdyn_opportunitylinetransaction.msdyn_amount_base                                            |
| msdyn_opportunitylinetransaction.msdyn_amountmethod                                           |
| msdyn_opportunitylinetransaction.msdyn_basisamount                                            |
| msdyn_opportunitylinetransaction.msdyn_basisamount_base                                       |
| msdyn_opportunitylinetransaction.msdyn_basisprice                                             |
| msdyn_opportunitylinetransaction.msdyn_basisprice_base                                        |
| msdyn_opportunitylinetransaction.msdyn_basisquantity                                          |
| msdyn_opportunitylinetransaction.msdyn_billingtype                                            |
| msdyn_opportunitylinetransaction.msdyn_bookableresource                                       |
| msdyn_opportunitylinetransaction.msdyn_contactcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_contactvendor                                          |
| msdyn_opportunitylinetransaction.msdyn_customertype                                           |
| msdyn_opportunitylinetransaction.msdyn_description                                            |
| msdyn_opportunitylinetransaction.msdyn_documentdate                                           |
| msdyn_opportunitylinetransaction.msdyn_enddatetime                                            |
| msdyn_opportunitylinetransaction.msdyn_exchangeratedate                                       |
| msdyn_opportunitylinetransaction.msdyn_opportunityline                                        |
| msdyn_opportunitylinetransaction.msdyn_opportunitylinetransactionid                           |
| msdyn_opportunitylinetransaction.msdyn_percent                                                |
| msdyn_opportunitylinetransaction.msdyn_price                                                  |
| msdyn_opportunitylinetransaction.msdyn_price_base                                             |
| msdyn_opportunitylinetransaction.msdyn_pricelist                                              |
| msdyn_opportunitylinetransaction.msdyn_product                                                |
| msdyn_opportunitylinetransaction.msdyn_project                                                |
| msdyn_opportunitylinetransaction.msdyn_quantity                                               |
| msdyn_opportunitylinetransaction.msdyn_resourcecategory                                       |
| msdyn_opportunitylinetransaction.msdyn_resourceorganizationalunitid                           |
| msdyn_opportunitylinetransaction.msdyn_startdatetime                                          |
| msdyn_opportunitylinetransaction.msdyn_task                                                   |
| msdyn_opportunitylinetransaction.msdyn_transactioncategory                                    |
| msdyn_opportunitylinetransaction.msdyn_transactionclassification                              |
| msdyn_opportunitylinetransaction.msdyn_transactiontypecode                                    |
| msdyn_opportunitylinetransaction.msdyn_unit                                                   |
| msdyn_opportunitylinetransaction.msdyn_unitschedule                                           |
| msdyn_opportunitylinetransaction.msdyn_vendortype                                             |

### <a name="msdyn_opportunitylinetransactioncategory"></a>msdyn_opportunitylinetransactioncategory

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactioncategory.msdyn_billingtype                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_description                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactioncategoryid           |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactionclassification       |
| msdyn_opportunitylinetransactioncategory.msdyn_transactioncategory                            |

### <a name="msdyn_opportunitylinetransactionclassificatio"></a>msdyn_opportunitylinetransactionclassificatio

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactionclassificatio.msdyn_billingtype                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_description                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_include                                   |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunityline                           |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunitylinetransactionclassificatioid |
| msdyn_opportunitylinetransactionclassificatio.msdyn_transactionclassification                 |

### <a name="msdyn_orderlineresourcecategory"></a>msdyn_orderlineresourcecategory

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlineresourcecategory.msdyn_contractline                                            |

### <a name="msdyn_orderlinetransaction"></a>msdyn_orderlinetransaction

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransaction.msdyn_salescontractline                                            |
| msdyn_orderlinetransactioncategory.msdyn_contractline                                         |

### <a name="msdyn_orderlinetransactionclassification"></a>msdyn_orderlinetransactionclassification

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransactionclassification.msdyn_contractline                                   |

### <a name="msdyn_project"></a>msdyn_project

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_project.msdyn_actualdurationminutes                                                     |
| msdyn_project.msdyn_actualhours                                                               |
| msdyn_project.msdyn_template                                                                |
| msdyn_project.msdyn_plannedhours                                                              |
| msdyn_project.msdyn_projecttemplate                                                           |
| msdyn_project.msdyn_remaininghours                                                            |
| msdyn_project.msdyn_scheduldurationminutes                                                  |
| msdyn_project.msdyn_scheduledend                                                              |
| msdyn_project.msdyn_stagename                                                                 |
| msdyn_project.msdyn_wbsduration                                                               |


### <a name="msdyn_projecttask"></a>msdyn_projecttask

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttask.msdyn_actualdurationminutes                                                 |
| msdyn_projecttask.msdyn_actualeffort                                                          |
| msdyn_projecttask.msdyn_aggregationdirection                                                  |
| msdyn_projecttask.msdyn_assignedresources                                                     |
| msdyn_projecttask.msdyn_assignedteammembers                                                   |
| msdyn_projecttask.msdyn_autoscheduling                                                        |
| msdyn_projecttask.msdyn_costestimatecontour                                                   |
| msdyn_projecttask.msdyn_effortcontour                                                         |
| msdyn_projecttask.msdyn_islinetask                                                            |
| msdyn_projecttask.msdyn_numberofresources                                                     |
| msdyn_projecttask.msdyn_remaininghours                                                        |
| msdyn_projecttask.msdyn_resourceutilization                                                   |
| msdyn_projecttask.msdyn_salesestimatecontour                                                  |
| msdyn_projecttask.msdyn_scheduledhours                                                        |
| msdyn_projecttask.msdyn_wbsid                                                                 |

### <a name="msdyn_projecttaskstatususer"></a>msdyn_projecttaskstatususer

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttaskstatususer.msdyn_bookableresource                                            |
| msdyn_projecttaskstatususer.msdyn_description                                                 |
| msdyn_projecttaskstatususer.msdyn_expectedcompletiondate                                      |
| msdyn_projecttaskstatususer.msdyn_expectedhourstocompleted                                     |
| msdyn_projecttaskstatususer.msdyn_iscompleted                                                 |
| msdyn_projecttaskstatususer.msdyn_name                                                        |
| msdyn_projecttaskstatususer.msdyn_percentcomplete                                             |
| msdyn_projecttaskstatususer.msdyn_projecttaskid                                               |
| msdyn_projecttaskstatususer.msdyn_projecttaskstatusindicator                                  |
| msdyn_projecttaskstatususer.msdyn_projecttaskstatususerid                                     |

### <a name="msdyn_projectteam"></a>msdyn_projectteam

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteam.msdyn_applicantcount                                                        |
| msdyn_projectteam.msdyn_applicants eskuragarri dago                                                   |
| msdyn_projectteam.msdyn_assignedhours                                                         |
| msdyn_projectteam.msdyn_description                                                           |
| msdyn_projectteam.msdyn_from                                                                  |
| msdyn_projectteam.msdyn_hours eskatuta                                                        |
| msdyn_projectteam.msdyn_membershipstatus                                                      |
| msdyn_projectteam.msdyn_number                                                                |
| msdyn_projectteam.msdyn_to                                                                    |

### <a name="msdyn_projectteammembersignup"></a>msdyn_projectteammembersignup

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteammembersignup.msdyn_bookableresource                                          |
| msdyn_projectteammembersignup.msdyn_membershipstatus                                          |
| msdyn_projectteammembersignup.msdyn_name                                                      |
| msdyn_projectteammembersignup.msdyn_projectteammembersignupid                                 |
| msdyn_projectteammembersignup.msdyn_teammembership                                            |

### <a name="msdyn_projecttransactioncategory"></a>msdyn_projecttransactioncategory

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttransactioncategory.msdyn_billingtype                                            |
| msdyn_projecttransactioncategory.msdyn_name                                                   |
| msdyn_projecttransactioncategory.msdyn_project                                                |
| msdyn_projecttransactioncategory.msdyn_projecttransactioncategoryid                           |
| msdyn_projecttransactioncategory.msdyn_transactioncategory                                    |

### <a name="msdyn_quotelineinvoiceschedule"></a>msdyn_quotelineinvoiceschedule

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_quotelineinvoiceschedule.msdyn_quoteline                                                |
| msdyn_quotelineresourcecategory.msdyn_quoteline                                               |
| msdyn_quotelinesscheduleofvalue.msdyn_quoteline                                                |
| msdyn_quotelinetransaction.msdyn_quoteline                                                    |
| msdyn_quotelinetransactioncategory.msdyn_quoteline                                            |
| msdyn_quotelinetransactionclassification.msdyn_quoteline                                      |

### <a name="msdyn_resourceassignment"></a>msdyn_resourceassignment

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_resourceassignment.msdyn_hours                                                          |
| msdyn_resourceassignment.msdyn_fromdate                                                       |
| msdyn_resourceassignment.msdyn_msprojectclientid                                              |
| msdyn_resourceassignment.msdyn_todate                                                         |
| msdyn_resourceassignmentdetail.msdyn_duration                                                 |
| msdyn_resourceassignmentdetail.msdyn_from                                                     |
| msdyn_resourceassignmentdetail.msdyn_izena                                                     |
| msdyn_resourceassignmentdetail.msdyn_resourceassignmentdetailid                               |
| msdyn_resourceassignmentdetail.msdyn_resourceassignmentid                                     |

### <a name="salesorderdetail"></a>salmenta-eskaeraren xehetasuna

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| salesorderdetail.msdyn_quoteline                                                              |

