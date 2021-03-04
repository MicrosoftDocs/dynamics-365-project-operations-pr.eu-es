---
title: Zehaztu inplementazio mota
description: Gai honek zure enpresako Proiektuaren eragiketen inplementazio mota zuzena determinatzen laguntzeari buruzko informazioa eskaintzen du.
author: stsporen
manager: Annbe
ms.date: 11/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: e9d3a5d8e6e1daafac72a3b4c0380b679d1869bd
ms.sourcegitcommit: 14aa380759214713d9bf560f5a7f619b7f4bd5b8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/05/2020
ms.locfileid: "4401203"
---
# <a name="determine-your-deployment-type"></a>Zehaztu inplementazio mota

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

> [!IMPORTANT]
> Lizentzia erosi ondoren, hasi hemen Dynamics 365 Project Operations-en inplementazio eredu onena zehazteko [Instalazio gidatuko fluxua](https://aka.ms/provisionprojectoperations).
> Gidatutako instalazio-fluxua finkatu ondoren, kudeaketa-atarira zuzenduko zara zure instalazioa osatzeko. Instalazioa osatzeko, ikusi inplementazioaren xehetasunak.


## <a name="existing-customers-of-dynamics-using-dynamics-365-project-service-automation"></a>Dynamics 365 Project Service Automation erabiltzen duten Dynamics-eko lehengo bezeroak
Project Operations-ek Project Service Automation-ekin hornitutako gaitasunak biltzen ditu. Bezero hauen bertsio berritzeko bide bat kaleratuko da 2021 bertsio 1 olatuan.

## <a name="existing-customers-of-dynamics-365-finance-using-project-management-and-accounting"></a>Proiektu-kudeaketa eta kontabilitatea erabiltzen duten Dynamics 365 Finance-ren lehendik dauden bezeroak 

Proiektuen kudeaketa eta kontabilitate funtzionalitatea erabiltzen duten Finantzetako lehendik dauden bezeroek bere horretan erabiltzen jarrai dezakete. Ikusi [Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations](#pma).


## <a name="deployment-types"></a>Inplementazio motak
Project Operations-ek zure eskakizunekin bat etortzeko hainbat aukera onartzen ditu. Dynamics 365 bezero berria edo lehendik zaren, Project Operations-ek zure beharrak onar ditzake.

Gure [Inplementazio galdetegia](https://aka.ms/provisionprojectoperations) inplementazio egokia zehazten lagunduko dizu. Emaitzek inplementazio mota hauetakoren batera bideratuko zaituzte:

- [Oinarrizko inplementazioa: kudeatu proformako fakturak](#lite)
- [Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations](#integrated)
- [Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations](#pma)

Project Operations-ek ingurune berean biltegiratutako / ekoizteko eskaerak eta ez hornitutako / baliabideetan oinarritutako agertokiak onartzen dituzte entitate juridikoen mailako konfigurazioen bidez. Adibidez, Contosok hornitutako / ekoizteko eskaeren gaitasunak erabil ditzake AEBetako fabrikazio instalazioetan (Entitate juridikoa = Contoso Manufacturing United States). Contosok hornituta ez dauden / baliabideetan oinarritutako gaitasunak erabil ditzake Erresuma Batuko Contoso Robotics Arms zerbitzuaren instalazioetan (Entitate juridikoa = Contoso Robotics United Kingdom).

### <a name="lite-deployment---deal-to-proforma-invoicing"></a><a  name="lite"></a>Oinarrizko inplementazioa: kudeatu proformako fakturak

Lite inplementazioak gaitasun hauek ditu:

- Dynamics 365 Sales aplikazioen esperientziak luzatzen dituzten proiektuen salmenta prozesua
- Proiektuaren plangintza Microsoft Project weberako
- Dimentsio anitzeko prezioak
- Baliabide-kudeaketa bateratua
- Denboraren jarraipena
- Oinarrizko gastua
- Proforma eta bezeroari begira fakturazioa 

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
- Materialen inguruko laguntza

#### <a name="deployment-steps"></a>Inplementazio-urratsak
Erabili proiektuaren eragiketen hedapen eredu onena [Inplementazio-galdetegia](https://aka.ms/provisionprojectoperations).

Inplementazio honetarako, ikusi [Izena eman aurrebista harpidetzak lortzeko](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) eta [Ingurune berria hornitzea](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json). 



[!INCLUDE[footer-include](../includes/footer-banner.md)]