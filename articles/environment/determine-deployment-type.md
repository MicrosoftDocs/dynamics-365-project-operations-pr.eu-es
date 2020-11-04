---
title: Zehaztu inplementazio mota
description: Gai honek zure enpresako Proiektuaren eragiketen inplementazio mota zuzena determinatzen laguntzeari buruzko informazioa eskaintzen du.
author: stsporen
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 564f2878553fe3904a7c47c7e80a3b57c763a3b2
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071040"
---
# <a name="determine-your-deployment-type"></a>Zehaztu inplementazio mota

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

> [!IMPORTANT]
> Lizentzia erosi ondoren, hasi hemen Dynamics 365 Project Operations-en inplementazio eredu onena zehazteko [Instalazio gidatuko fluxua](https://aka.ms/provisionprojectoperations).
> Gidatutako instalazio-fluxua finkatu ondoren, kudeaketa-atarira zuzenduko zara zure instalazioa osatzeko. Instalazioa osatzeko, ikusi inplementazioaren xehetasunak.


## <a name="existing-customers-of-dynamics-using-dynamics-365-project-service-automation"></a>Dynamics 365 Project Service Automation erabiltzen duten Dynamics-eko lehengo bezeroak
Project Operations-ek Project Service Automation-ekin hornitutako gaitasunak biltzen ditu. Aurrerantzean bezero horien bertsio berritzeko bidea argitaratuko da.

## <a name="existing-customers-of-dynamics-365-finance-using-project-management-and-accounting"></a>Proiektu-kudeaketa eta kontabilitatea erabiltzen duten Dynamics 365 Finance-ren lehendik dauden bezeroak 

Proiektuen kudeaketa eta kontabilitate funtzionalitatea erabiltzen duten Finantzetako lehendik dauden bezeroek bere horretan jarraitzeko. Ikusi [Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations](#pma).


## <a name="deployment-types"></a>Inplementazio motak
Project Operations-ek zure eskakizunekin bat etortzeko hainbat aukera onartzen ditu. Dynamics 365 bezero berria edo lehendik zaren, Project Operations-ek zure beharrak onar ditzake.

Gure [Inplementazio galdetegia](https://aka.ms/provisionprojectoperations) inplementazio egokia zehazten lagunduko dizu. Emaitzek inplementazio mota hauetakoren batera bideratuko zaituzte:

- [Oinarrizko inplementazioa: kudeatu proformako fakturak](#lite)
- [Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations](#integrated)
- [Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations](#pma)

Project Operations-ek ingurune berean biltegiratutako / ekoizteko eskaerak eta ez hornitutako / baliabideetan oinarritutako agertokiak onartzen dituzte entitate juridikoen mailako konfigurazioen bidez. Adibidez, Contosok hornitutako / ekoizteko eskaeren gaitasunak erabil ditzake AEBetako fabrikazio instalazioetan (Entitate juridikoa = Contoso Manufacturing United States). Contosok hornituta ez dauden / baliabideetan oinarritutako gaitasunak erabil ditzake Erresuma Batuko Contoso Robotics Arms zerbitzuaren instalazioetan (Entitate juridikoa = Contoso Robotics United Kingdom).

### <a name="lite-deployment---deal-to-proforma-invoicing"></a><a  name="lite"></a>Oinarrizko inplementazioa: kudeatu proformako fakturak

Lite inplementazioak gaitasun hauek ditu:

- Proiektuaren plangintza Microsoft Project weberako
- Dimentsio anitzeko prezioak
- Baliabide-kudeaketa bateratua
- Denboraren jarraipena
- Oinarrizko gastua
- Faktura-proposamena

#### <a name="deployment-steps"></a>Inplementazio-urratsak
Erabili proiektuaren eragiketen hedapen eredu onena [Inplementazio-galdetegia](https://aka.ms/provisionprojectoperations).

Inplementazio honetarako, ikusi [Izena eman aurrebista harpidetzak lortzeko](lite-preview-subscription-sign-up.md) eta [Ingurune berria hornitzea](lite-deployment.md). 


### <a name="project-operations-for-resourcenon-stocked-scenarios"></a><a name="integrated"></a>Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations
Baliabideen / hornitu gabeko eszenatokien Poject Operations-ek gaitasun hauek biltzen ditu:
  
- Proiektuaren plangintza Microsoft Project weberako
- Dimentsio anitzeko prezioak
- Baliabide-kudeaketa bateratua
- Denboraren jarraipena
- Oinarrizko gastua
- Gastu osoa
- OCR agiria
- Fakturazio osoa
- Diru-sarreren aitorpena

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
- Materialen inguruko laguntza

#### <a name="deployment-steps"></a>Inplementazio-urratsak
Erabili proiektuaren eragiketen hedapen eredu onena [Inplementazio-galdetegia](https://aka.ms/provisionprojectoperations).

Inplementazio honetarako, ikusi [Izena eman aurrebista harpidetzak lortzeko](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) eta [Ingurune berria hornitzea](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json). 

