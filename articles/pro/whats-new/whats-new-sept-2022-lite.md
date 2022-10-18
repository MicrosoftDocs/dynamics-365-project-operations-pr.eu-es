---
title: 2022ko iraileko berritasunak - Project Operations lite inplementatzea
description: Artikulu honek Microsoft-en 2022ko iraileko bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du Dynamics 365 Project Operations lite inplementazioa.
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
# <a name="whats-new-september-2022---project-operations-lite-deployment"></a>2022ko iraileko berritasunak - Project Operations lite inplementatzea

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Artikulu hau Microsoft-en osagai eta bertsio hauei aplikatzen zaie Dynamics 365 Project Operations:

- Proiektuaren Eragiketak a Dataverse ingurunearen bertsioa 4.46.0.60

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

| Ezaugarrien eremua | Ezaugarriaren izena | Informazio gehiago |
| --- | --- | --- |
| Abaguneen kudeaketa | **Aurrekontuen berrikuspena eta aktibazioa**<br>Project Operations-ek salmenta-prozesuaren laguntza osoa dakar. Proiektuaren aurrekontuak aktibatu daitezke aurrekontua irakurtzeko soilik den eta berrikusten den egoera bat irudikatzeko. Aktibatutako komatxoak berrikus daitezke berrikuspen-zenbaki handitua duten komatxo berriak sortzeko. Aktibatutako proiektuen aurrekontuak edo aurrekontuen berrikuspenak irabazi edo galdu gisa itxi daitezke. | [Aktibatu eta berrikusi proiektuaren eskaintza](/dynamics365/project-operations/sales/activation-and-revision) |
| Fakturazioa eta prezioak | **Ordu-eremuaren prezio agnostikoa lehenetsita**<br>Project Operations-ek ordu-eremuaren data agnostiko baten kontzeptua sartu du proiektuaren erreal guztietan. Eremu berri bat, **Transakzio data**, orain aldizkariko lerroetan eta errealetan eskuragarri dago, eta transakzioa gertatu zeneko data gordetzeko erabiliko da, baina data hori Ordu Unibertsal Koordinatuan bihurtu gabe. Data hori beheranzko prozesuetarako erabiliko da, hala nola prezioen lehenetsia eta fakturak sortzeko. | <p>[Proiektuetan oinarritutako estimazioen eta errealen kostu-tasak zehaztea](/dynamics365/project-operations/pro/pricing-costing/cost-price-resolution-sales)</p><p>[Zehaztu proiektuetan oinarritutako estimazioen eta benetakoen salmenta-prezioak](/dynamics365/project-operations/pro/pricing-costing/sales-price-resolution-sales)</p> |
| Fakturazioa eta prezioak | **Data-eraginkorra den prezioen baliogabetzea Proiektuen Eragiketetan**<br>Data-eraginkorra den prezioen baliogabetzeak prezioen zerrendako prezio zehatzak aldatzeko edo aldatzeko modua eskaintzen du. | [Data-eraginkorra den prezioak gainidaztea](/dynamics365/project-operations/pricing-costing/dateffective_price_overrides) |
| Denbora eta gastua | **Onartzaile globala**<br>Ezaugarri honek software hornitzaile independentea (ISV) eta onespen zentralizatua ahalbidetzen du, proiektuko proiektuaren edo taldekidearen egoera edozein dela ere. | [Segurtasuna eta onarpenak](/dynamics365/project-operations/approvals/approvals-security) |
|Proiektuaren antolaketa eta jarraipena|**Erabili Proiektuak programatzeko APIak Planifikazio entitateekin eragiketak egiteko** </br> </br>Baliabideen esleipenaren sestra editatzeko APIari esker, garatzaileek programatikoki zehazten dute zereginen esleipendun baten esfortzua onartzen den edozein data-barrutitan, denbora-mailako esfortzuen planifikazio zehatzagoa lortzeko.|[Erabili Proiektuak programatzeko APIak Planifikazio entitateekin eragiketak egiteko](/dynamics365/project-operations/project-management/schedule-api-preview)|

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Fakturazioa eta prezioak | 2754422 | Materialen eta gastuen kalkuluak ez dira Dynamics 365 Finance-era iristen proiektuak kopiatzean Dataverse. |
| Denbora eta gastua | 2787409 | Balio ez duen onartzaile batek proiektua ez den denbora-sarrera onar dezake. |
| Abaguneen kudeaketa | 2788907 | Errore-mezu eguneratua, banderak dituzten eskaera-lerroen esklusibotasuna baliozkotzeko. |
| Denbora eta gastua | 2842253 | Denbora onartzeko salbuespen nulua kudeatzea. |
| Fakturazioa eta prezioak | 2844181 | Korrelazio IDa ez lortzeak blokeatzen du faktura sortzea. |
| Fakturazioa eta prezioak | 2876628 | QLD, CLD - Estimazio-prezio-zerrendaren ebazpenak prezio-zerrendako data-tarte-eremuak erabili behar ditu. |
| Azpikontratazioa | 2893222 | Azpikontratazio-lerro baterako rolik ez bada zehazten, posible izan beharko litzateke lerro hori hautatzea taldekide batean edozein roltarako. |
