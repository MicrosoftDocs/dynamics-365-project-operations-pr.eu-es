---
title: Proiektuetako gastuen aurreikuspen ekonomikoak
description: Gai honek proiektuan oinarritutako gastuak definitzeko edo kalkulatzeko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 03/19/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ad4901b1264289f1da881154bc147fc3f8da698f
ms.sourcegitcommit: 386921f44f1e9a8a828b140206d52945de07aee7
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/22/2021
ms.locfileid: "5701767"
---
# <a name="financial-estimates-for-expenses-on-projects"></a>Proiektuetako gastuen aurreikuspen ekonomikoak
_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations proiektuen kudeatzaileek proiektu edo zeregin bakoitzerako proiektuan oinarritutako gastuak definitzeko aukera ematen du. Gastu-elementu bakoitza proiektuko zeregin zehatz batekin lotu daiteke. Gastuak antolaketa mailan definitzen diren gastu kategoria desberdinetan sailkatzen dira. Prezioen zerrendan zehazten dira gastu-kategoria bakoitzaren prezioak eta kostuak. 

Bete urrats hauek proiektuaren gastua ikusi, gehitu edo ezabatzeko.

1. Joan **Proiektuak**, eta hautatu landu nahi duzun proiektua.
2. Aukeratu **Proiektuaren aurrekontuak** fitxa eta ikusi proiektuaren gastuen zerrenda.
3. Aukeratu **Gastu berria** gastu bat gehitzeko. Edo hautatu ezabatzeko gastua eta hautatu **Ezabatu gastua**.

Ondorengo taulan fitxategien eremuei buruzko informazioa ematen da **Gastuen aurreikusitako lerroa** proiektu batean. 

| **Eremua** | **Azalpena** | **Downstream eragina** |
| --- | --- | --- |
| Ataza | Proiektuko zereginen zerrenda. Honek laburpen eta hosto nodo zereginak biltzen ditu. | Gastua kalkulatzeko lerro baterako zeregina hautatzeak kalkulatutako gastuen kostuan eta zeregin baterako gastuen salmenten estimazioan eragina izango du. Eremu hau hutsik badago, aurreikusitako gastua proiektuaren mailan jarraipena eta laburpena egiten dira. |
| Kategoria | Aplikazioan gastu-kategoriak lotu dituzten transakzio-kategorien zerrenda. | Kategoria bat hautatzeak gastuak kalkulatzeko lerroan prezioak eta kostuak eragiten ditu. |
| Hasiera-data | Gastua aurreikusitako eguna. | Ez dago alor honen beherako eraginik. |
| Salmenta-unitatea | Eremu honetako balio lehenetsia hautatutako kategorian lehenetsitako konfiguratutako unitate taldetik dator. Eremu hau egunera dezakezu beste unitate talde bat hautatzeko. | Ez dago alor honen beherako eraginik. |
| Unitatea | Eremu honetako balio lehenetsia hautatutako kategoriaren unitate lehenetsia da. Eremu hau egunera dezakezu beste unitate bat hautatzeko. | Unitatea aldatzeak unitateko prezio eta kostu lehenetsi desberdinak lortzen ditu. |
| Kantitatea | Aurreikusitako gastuaren zenbatekoa. | Ez dago alor honen beherako eraginik. |
| Unitatearen kostua | Aukeratutako kategoriaren eta unitate konbinazioaren kostu unitarioa aplikagarri den kostuen prezioen zerrendan ezarritako moduan | Unitatearen kostua proiektuaren kostuaren monetan agertzen da beti. |
| Unitate-prezioa | Aukeratutako kategoriaren eta unitate konbinazioaren prezioa aplikagarri den salmenten prezioen zerrendan ezarritako moduan. | Unitatearen prezioa proiektuaren salmenten monetan agertzen da beti. |
| Kostua guztira | Kopuru gisa kalkulatzen den kostuaren zenbatekoa \* unitateko kostua.| Kostuaren zenbatekoa proiektuaren kostuaren monetan agertzen da beti. |
| Salmentak, guztira | Kopuru gisa kalkulatzen den salmentaren zenbatekoa \* unitateko prezioa. | Salmenten zenbatekoa proiektuaren salmenten monetan agertzen da beti. |


[!INCLUDE[footer-include](../includes/footer-banner.md)]
