---
title: Zer berri 2022eko iraila - Project Operations lite/ren inplementazioa
description: Gai honek informazioa eskaintzen du 2022ko irailaren Microsoft Dynamics 365 Project Operations lite-ren inplementazio arinaren bertsioan eskuragarri dauden kalitate-eguneratzeei buruz.
author: ramagadu
ms.date: 09/28/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ramagadu
ms.openlocfilehash: a02ac7a69489bc7974eb0e63c11fa5de74795b78
ms.sourcegitcommit: b3a70bc4f2850cff5c2b7114cff7bd61ec298143
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/06/2022
ms.locfileid: "9634837"
---
# <a name="whats-new-september-2022---project-operations-lite-deployment"></a>Zer berri 2022eko iraila - Project Operations lite/ren inplementazioa

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Gai hau Microsoft Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

- Project Operations Dataverse inguruneko bertsioan 4.46.0.60

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

| Ezaugarrien eremua | Eginbidearen izena | Informazio gehiago |
| --- | --- | --- |
| Abaguneen kudeaketa | **Eskaintzen aktibazioa eta berrikuspenak**<br>Project Operations-ek salmenta-prozesuaren laguntza osoa dakar. Proiektuaren eskaintzak aktibatu daitezke eskaintza irakurtzeko soilik den eta berrikusten den egoera bat irudikatzeko. Aktibatutako eskaintzak berrikus daitezke berrikuspen-zenbaki handitua duten eskaintza berriak sortzeko. Aktibatutako proiektuaren eskaintzak edo eskaintzen berrikuspenak irabazi edo galduta gisa itxi daitezke. | [Aktibatu eta berrikusi proiektuaren eskaintza](/dynamics365/project-operations/sales/activation-and-revision) |
| Fakturazioa eta prezioak | **Ordu-eremuaren prezio agnostikoa lehenetsita**<br>Project Operations-ek ordu-eremuaren data agnostiko baten kontzeptua sartu du proiektuaren erreal guztietan. Eremu berri bat, **Transakzio data**, orain egunkari-lerroetan eta errealetan eskuragarri dago, eta transakzioa gertatu zeneko data gordetzeko erabiliko da, baina data hori Ordu Unibertsal Koordinatuan bihurtu gabe. Data hori beheranzko prozesuetarako erabiliko da, hala nola prezioen lehenetsia eta fakturak sortzeko. | <p>[Erabaki proiektuetan oinarritutako estimazio eta benetako datuen salmenta-prezioak](/dynamics365/project-operations/pro/pricing-costing/cost-price-resolution-sales)</p><p>[Erabaki proiektuetan oinarritutako aurreikuspenen eta benetako datuen salmenta-prezioak](/dynamics365/project-operations/pro/pricing-costing/sales-price-resolution-sales)</p> |
| Fakturazioa eta prezioak | **Datarekin eraginkor bihurtzen den prezioen gainidazketa Project Operations-en**<br>Data-eraginkorra den prezioak gainidaztea prezioen zerrendan prezio zehatzak gainidazteko edo aldatzeko modu bat eskaini. | [Dataren araberako prezioen gainidazketak](/dynamics365/project-operations/pricing-costing/dateffective_price_overrides) |
| Denbora eta gastua | **Onartzaile globala**<br>Ezaugarri honek software hornitzaile independentea (ISV) eta onespen zentralizatua ahalbidetzen du, proiektuaren edo taldekideen egoera edozein dela ere. | [Segurtasuna eta onarpenak](/dynamics365/project-operations/approvals/approvals-security) |
|Proiektuaren antolaketa eta jarraipena|**Erabili Proiektuak programatzeko APIak Planifikazio entitateekin eragiketak egiteko** </br> </br>Baliabideen esleipenaren sestra editatzeko APIari esker, garatzaileek programatikoki zehazten dute zereginen esleipendun baten esfortzua onartzen den edozein data-barrutitan, denbora-mailako esfortzuen planifikazio zehatzagoa lortzeko.|[Erabili Proiektuak programatzeko APIak Planifikazio entitateekin eragiketak egiteko](/dynamics365/project-operations/project-management/schedule-api-preview)|

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Fakturazioa eta prezioak | 2754422 | Material eta gastuen estimazioak ez dira Dynamics 365 Finance-ra iristen proiektuak kopiatzen direnean Dataverse-n. |
| Denbora eta gastua | 2787409 | Balio ez duen onartzaile batek proiektua ez den denbora-sarrera onar dezake. |
| Abaguneen kudeaketa | 2788907 | Errore-mezu eguneratua, markak dituzten eskaera-lerroen esklusibotasuna baliozkotzeko. |
| Denbora eta gastua | 2842253 | Denbora onartzeko salbuespen nulua kudeatzea. |
| Fakturazioa eta prezioak | 2844181 | Korrelazio IDa ez lortzeak blokeatzen du faktura sortzea. |
| Fakturazioa eta prezioak | 2876628 | QLD, CLD - Estimazio-prezio-zerrendaren ebazpenak prezio-zerrendako data-tarte-eremuak erabili behar ditu. |
| Azpikontratazioa | 2893222 | Azpikontratazio-lerro baterako rolik ez bada zehazten, posible izan beharko litzateke lerro hori hautatzea taldekide batean edozein roltarako. |
