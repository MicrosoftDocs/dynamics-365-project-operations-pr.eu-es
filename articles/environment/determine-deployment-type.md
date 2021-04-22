---
title: Zehaztu inplementazio mota
description: Gai honek zure enpresako Proiektuaren eragiketen inplementazio mota zuzena determinatzen laguntzeari buruzko informazioa eskaintzen du.
author: stsporen
manager: Annbe
ms.date: 03/15/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 715b117cae5418fc743ea870772278450fff5ae9
ms.sourcegitcommit: df30839484ef278675c5c712af0f7ba66ed9cdd3
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/17/2021
ms.locfileid: "5663579"
---
# <a name="determine-your-deployment-type"></a>Zehaztu inplementazio mota

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

> [!IMPORTANT]
> Lizentzia erosi eta gero, hasi Dynamics 365 Project Operations erabiliz [Instalazio gidatuko fluxua](https://aka.ms/provisionprojectoperations).
> Gidatutako instalazio-fluxua finkatu ondoren, kudeaketa-atarira zuzenduko zara zure instalazioa osatzeko. Instalazioa osatzeko, ikusi inplementazioaren xehetasunak.


## <a name="existing-customers-of-dynamics-using-dynamics-365-project-service-automation"></a>Dynamics 365 Project Service Automation erabiltzen duten Dynamics-eko lehengo bezeroak
Project Operations-ek Project Service Automation-ekin hornitutako gaitasunak biltzen ditu. Bezero hauen bertsio berritzeko bide bat kaleratuko da 2021 bertsio 1 olatuan.

## <a name="existing-customers-of-dynamics-365-finance-using-project-management-and-accounting"></a>Proiektu-kudeaketa eta kontabilitatea erabiltzen duten Dynamics 365 Finance-ren lehendik dauden bezeroak 

Proiektuen kudeaketa eta kontabilitate funtzionalitatea erabiltzen duten Finantzetako lehendik dauden bezeroek bere horretan erabiltzen jarrai dezakete. Ikusi [Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations](#pma).


## <a name="deployment-regions"></a>Inplementazio-eskualdeak
Project Operations inplementazioa onartzen duten eskualdeak zehazteko, ikusi [Erabilgarritasun geografikoa Dynamics 365 eta Power Platform txostena](https://dynamics.microsoft.com/en-us/geographic-availability/). Aukeratu **Ikusi txostena**, eta zabaldu **Dynamics 365 > Operations aplikazioak > Dynamics 365 Project Operations** onartutako eskualdeak ikusteko.

## <a name="deployment-types"></a>Inplementazio motak
Project Operations-ek zure eskakizunekin bat etortzeko hainbat aukera onartzen ditu. Dynamics 365 bezero berria edo lehendik zaren, Project Operations-ek zure beharrak onar ditzake.

Gure [Inplementazio galdetegia](https://aka.ms/provisionprojectoperations) inplementazio egokia zehazten lagunduko dizu. Emaitzek inplementazio mota hauetakoren batera bideratuko zaituzte:

- [Oinarrizko inplementazioa: kudeatu proformako fakturak](#lite)
- [Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations](#integrated)
- [Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations](#pma)

Project Operations-ek ingurune berean biltegiratutako / ekoizteko eskaerak eta ez hornitutako / baliabideetan oinarritutako agertokiak onartzen dituzte entitate juridikoen mailako konfigurazioen bidez. Adibidez, Contoso hornitutako / ekoizteko eskaerak AEBetako fabrikazio instalazioetan erabil ditzake (entitate juridikoa = Contoso Fabrikazio Estatu Batuak). Contoso baliabideetan oinarrituta ez dauden baliabideak erabil ditzake Contoso Erresuma Batuko Robotika Armak zaintzeko instalazioa (entitate juridikoa = Contoso Robotika Erresuma Batua).

### <a name="lite-deployment---deal-to-proforma-invoicing"></a><a  name="lite"></a>Oinarrizko inplementazioa: kudeatu proformako fakturak

Lite inplementazioak gaitasun hauek ditu:

- Dynamics 365 Sales aplikazioen esperientziak luzatzen dituzten proiektuen salmenta prozesua
- Proiektuaren plangintza Microsoft Project weberako
- Dimentsio anitzeko prezioak
- Baliabide-kudeaketa bateratua
- Denboraren jarraipena
- Oinarrizko gastua
- Proforma fakturazioa Proiektu zuzendariaren berrikuspen eta aldaketetarako 

#### <a name="deployment-steps"></a>Inplementazio-urratsak
Erabili proiektuaren eragiketen hedapen eredu onena [Inplementazio-galdetegia](https://aka.ms/provisionprojectoperations).

Inplementazio honetarako, ikusi [Izena eman aurrebista harpidetzak lortzeko](lite-preview-subscription-sign-up.md) eta [Ingurune berria hornitzea](lite-deployment.md). 


### <a name="project-operations-for-resourcenon-stocked-scenarios"></a><a name="integrated"></a>Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations
Baliabideen / hornitu gabeko eszenatokien Poject Operations-ek gaitasun hauek biltzen ditu:
 
- Dynamics 365 Sales aplikazioak luzatzen dituzten proiektuen salmenta prozesua
- Proiektuaren plangintza Microsoft Project weberako
- Dimentsio anitzeko prezioak
- Baliabide-kudeaketa bateratua
- Denboraren jarraipena
- Oinarrizko gastua
- Gastu osoa
- OCR agiria
- Proforma eta bezeroari begira fakturazioa 
- Proiektuen diru-sarreren aitorpena

#### <a name="deployment-steps"></a>Inplementazio-urratsak
Erabili proiektuaren eragiketen hedapen eredu onena [Inplementazio-galdetegia](https://aka.ms/provisionprojectoperations).

Inplementazio honetarako, ikusi [Izena eman aurrebista harpidetzak lortzeko](resource-sign-up-preview-subscription.md) eta [Ingurune berria hornitzea](resource-provision-new-environment.md). 


### <a name="project-operations-for-stockedproduction-order-scenarios"></a><a name="pma"></a>Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations

- Proiektuaren antolaketa WBS erabiliz
- Baliabideen kudeaketa
- Denboraren jarraipena
- Gastu osoa
- OCR agiria
- Fakturazio osoa
- Diru-sarreren aitorpena
- Produkzio-eskaerak
- Hornitutako materialen euskarria inbentarioarekin

#### <a name="deployment-steps"></a>Inplementazio-urratsak
Erabili proiektuaren eragiketen hedapen eredu onena [Inplementazio-galdetegia](https://aka.ms/provisionprojectoperations).

Inplementazio honetarako, ikusi [Izena eman aurrebista harpidetzak lortzeko](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) eta [Ingurune berria hornitzea](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json). 



[!INCLUDE[footer-include](../includes/footer-banner.md)]
