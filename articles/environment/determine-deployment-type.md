---
title: Inplementazio motak
description: Gai honek zure enpresako Proiektuaren eragiketen inplementazio mota zuzena determinatzen laguntzeari buruzko informazioa eskaintzen du.
author: stsporen
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: c3cf378caae4510482a8ee6771bf2e6decfe3b48
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948728"
---
# <a name="deployment-types"></a>Inplementazio motak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

> [!IMPORTANT]
> Lizentzia erosi ondoren, hasi hemen Dynamics 365 Project Operations-en inplementazio eredu onena zehazteko [Instalazio gidatuko fluxua](https://aka.ms/provisionprojectoperations).
> Gidatutako instalazio-fluxua finkatu ondoren, kudeaketa-atarira zuzenduko zara zure instalazioa osatzeko. Instalazioa osatzeko, ikusi beheko inplementazioaren xehetasunak.


## <a name="existing-customers-of-dynamics-using-dynamics-365-project-service-automation"></a>Dynamics 365 Project Service Automation erabiltzen duten Dynamics-eko lehengo bezeroak
Project Operations-ek Project Service Automation-ekin hornitutako gaitasunak biltzen ditu. Aurrerantzean bezero horien bertsio berritzeko bidea argitaratuko da.

## <a name="existing-customers-of-dynamics-365-finance-using-project-management-and-accounting"></a>Proiektu-kudeaketa eta kontabilitatea erabiltzen duten Dynamics 365 Finance-ren lehendik dauden bezeroak 

Proiektuen kudeaketa eta kontabilitate funtzionalitatea erabiltzen duten Finantzetako lehendik dauden bezeroek bere horretan jarrai dezakete. Ikusi [Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations](#pma).

Project Operations-ek zure eskakizunekin bat etortzeko hainbat aukera onartzen ditu. Dynamics 365 bezero berria edo lehendik zaren, Project Operations-ek zure beharrak onar ditzake.

Gure [Inplementazio galdetegia](https://aka.ms/provisionprojectoperations) inplementazio egokia zehazten lagunduko dizu. Emaitzek inplementazio mota hauetakoren batera bideratuko zaituzte:

- [Oinarrizko inplementazioa: kudeatu proformako fakturak](#lite)
- [Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations](#integrated)
- [Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations](#pma)

Project Operations-ek ingurune berean biltegiratutako / ekoizteko eskaerak eta ez hornitutako / baliabideetan oinarritutako agertokiak onartzen dituzte entitate juridikoen mailako konfigurazioen bidez. Adibidez, Contosok hornitutako / ekoizteko eskaeren gaitasunak balia ditzake AEBetako fabrikazio-instalazioetan (entitate juridikoa = Contoso Manufacturing United States) eta ez ditu hornitutako / baliabideetan oinarritutako gaitasunak Erresuma Batuko Contoso Robotics Arms zerbitzuaren instalazioetan (Entitate juridikoa = Contoso Robotics United Erresuma).

## <a name="a-namelitelite-deployment---deal-to-proforma-invoicing"></a><a name="lite"><a/>Oinarrizko inplementazioa: kudeatu proformako fakturak
Lite inplementazioak gaitasun hauek ditu:

- Proiektuaren plangintza Microsoft Project weberako
- Dimentsio anitzeko prezioak
- Baliabide-kudeaketa bateratua
- Denboraren jarraipena
- Oinarrizko gastua
- Faktura-proposamena

### <a name="deployment-steps"></a>Inplementazio-urratsak:
Erabili proiektuaren eragiketen hedapen eredu onena [Inplementazio-galdetegia](https://aka.ms/provisionprojectoperations).

Inplementazio honetarako, ikusi [Izena eman aurrebista harpidetzak lortzeko](lite-preview-subscription-sign-up.md) eta [Ingurune berria hornitzea](lite-deployment.md). 


## <a name="a-nameintegratedproject-operations-for-resourcenon-stocked-scenarios"></a><a name="integrated"><a/>Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations
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

### <a name="deployment-steps"></a>Inplementazio-urratsak:
Erabili proiektuaren eragiketen hedapen eredu onena [Inplementazio-galdetegia](https://aka.ms/provisionprojectoperations).

Inplementazio honetarako, ikusi [Izena eman aurrebista harpidetzak lortzeko](resource-sign-up-preview-subscription.md) eta [Ingurune berria hornitzea](resource-provision-new-environment.md). 


## <a name="project-operations-for-stockedproduction-order-scenarios"></a><a name="pma"></a>Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations

- Proiektuaren antolaketa WBS erabiliz
- Baliabideen kudeaketa
- Denboraren jarraipena
- Gastu osoa
- OCR agiria
- Fakturazio osoa
- Diru-sarreren aitorpena
- Produkzio-eskaerak
- Materialen inguruko laguntza

### <a name="deployment-steps"></a>Inplementazio-urratsak:
Erabili proiektuaren eragiketen hedapen eredu onena [Inplementazio-galdetegia](https://aka.ms/provisionprojectoperations).

Inplementazio honetarako, ikusi [Izena eman aurrebista harpidetzak lortzeko](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) eta [Ingurune berria hornitzea](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json). 



