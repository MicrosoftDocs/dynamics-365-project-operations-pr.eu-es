---
title: Proiektuetako materialen aurreikuspen ekonomikoak
description: Gai honek proiektuan oinarritutako materialak definitzeko edo kalkulatzeko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 98e3611b2b3948aab09a3eadeac7b95b893812e9
ms.sourcegitcommit: 504c09365bf404c1f1aa9b5034c1e1e5bc9d0d54
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/31/2021
ms.locfileid: "5788827"
---
# <a name="financial-estimates-for-materials-on-projects"></a>Proiektuetako materialen aurreikuspen ekonomikoak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations proiektuen kudeatzaileek proiektu edo zeregin bakoitzerako proiektuan oinarritutako material kostuak definitzeko aukera ematen du. Estimazio material bakoitza proiektuko zeregin zehatz batekin lotu daiteke. Gastuak antolaketa mailan definitzen diren gastu kategoria desberdinetan sailkatzen dira. Prezioen zerrendan zehazten dira gastu-kategoria bakoitzaren prezioak eta kostuak. 

Osatu urrats hauek proiektuaren materialaren aurrekontua ikusi, gehitu edo ezabatzeko.

1. Joan **Proiektuak**, eta hautatu eguneratu nahi duzun proiektua.
2. **Materialen aurrekontuak** fitxa, ikusi proiektuaren materialen kalkuluen zerrenda.
3. Hautatu **Material berrien estimazioa** materialaren estimazio berria sortzeko. Edo hautatu ezabatzeko materialaren aurrekontua eta hautatu **Ezabatu materialaren aurrekontua**.

Ondorengo taulan fitxategien eremuei buruzko informazioa ematen da **Materialaren aurreikusitako lerroa** proiektu batean. 

| **Eremua** | **Azalpena** | **Downstream eragina** |
| --- | --- | --- |
| Ataza | Proiektuko zereginen zerrenda. Honek laburpen eta hosto nodo zereginak biltzen ditu. | Materiala kalkulatzeko lerro baterako zeregina hautatzen duzunean, kalkulatutako materialaren kostua eta zeregin baterako kalkulatutako material salmentak eragina izango dute. Eremu hau hutsik badago, aurreikusitako materiala proiektuaren mailan jarraipena eta laburpena egiten dira. |
| Hautatu produktua |  Zehatz dezakezu aurreikusitako lerro hau lehendik dagoen (katalogoa) produktu edo katalogotik kanpoko produktu batena den. | Eremu honek zehazten du katalogotik produktu bat hautatzen duzun edo produktuan idazten duzun. |
| Produktu | Produktuen katalogoko produktuaren IDa. Produktuaren IDa hautatzen duzunean, **Aukeratu produktua** eremuko balioa automatikoki eguneratzen da **Lehendik dagoen produktua** aukerara. IDa prezioen zerrendatik kostuak eta salmenta prezioak berreskuratzeko erabiltzen da. | Ez dago alor honen beherako eraginik. |
| Katalogotik kanpoko produktuaren deskribapena | Produktuaren izena idazteko testu eremua. Eremu hau erabili behar da **Idatzi** produktuan **Aukeratu produktua** eremua hautatuta dagoenean.| Ez dago alor honen beherako eraginik. |
| Hasiera-data | Materiala noiz erabiliko den aurreikusten da. | Ez dago alor honen beherako eraginik. |
| Salmenta-unitatea | Eremu honetako balio lehenetsia katalogoko produktuko unitate talde lehenetsitik dator. Eremu hau egunera dezakezu beste unitate talde bat hautatzeko. | Ez dago alor honen beherako eraginik. |
| Unitatea | Eremu honetako balioa hautatutako produktuaren unitate lehenetsia da. Eremu hau egunera dezakezu beste unitate bat hautatzeko. | Unitatea aldatzeak unitateko prezio eta kostu lehenetsi desberdinak lortzen ditu. |
| Kantitatea | Proiektuan erabiliko den produktuaren zenbateko estimatua. | Ez dago alor honen beherako eraginik. |
| Unitatearen kostua | Aukeratutako produktuaren eta unitate konbinazioaren kostu unitarioa aplikagarri den kostuen prezioen zerrendan ezarritako moduan. | Unitatearen kostua proiektuaren kostuaren monetan agertzen da beti. Prezio zerrendan produktu konbinatuaren eta unitatearen kostu unitarioa konfiguratu gabe badago, kostu unitarioa 0,00 izango da lehenetsita. |
| Unitate-prezioa | Aukeratutako produktuaren eta unitate konbinazioaren prezioa aplikagarri den salmenten prezioen zerrendan ezarritako moduan. | Unitatearen prezioa proiektuaren salmenten monetan agertzen da beti. Prezio zerrendan produktu konbinatuaren eta unitatearen prezio unitarioa konfiguratu gabe badago, prezio unitarioa 0,00 izango da lehenetsita.|
| Kostua guztira | Kopuru gisa kalkulatzen den kostuaren zenbatekoa \* unitateko kostua.| Kostuaren zenbatekoa proiektuaren kostuaren monetan agertzen da beti. |
| Salmentak, guztira | Kopuru gisa kalkulatzen den salmentaren zenbatekoa \* unitateko prezioa. | Salmenten zenbatekoa proiektuaren salmenten monetan agertzen da beti. |


[!INCLUDE[footer-include](../includes/footer-banner.md)]
