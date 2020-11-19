---
title: Lanaren kostu-tasak konfiguratzea
description: Gai honek Project Operations-eko lanaren kostuak konfiguratzeari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/12/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 66a254ce4e7c7f25ac3ea303b73a01625988b0d9
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070947"
---
# <a name="setting-up-labor-cost-rates"></a>Lanaren kostu-tasak konfiguratzea 

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Prezio zerrenda bakoitzak prezio zerrendaren edukiarekin eta datarekin eraginkortasunarekin bat datozen lan tasen (rol prezioak) multzoa du.

1. Sortu prezioen zerrenda eta **Rolaren prezioa** fitxa, azpi-saretan, hautatu **Rol berria**.
2. **Sortu bizkor** orrian, hautatu rola eta antolakuntza unitatea.
3. Idatzi beharrezko eremuaren beste edozein informazio.

Hurrengo taulan kostuen prezioen zerrendan eskulan tasak sortzerakoan garrantzitsuak diren zenbait arlo biltzen dira.

| Eremua | Kokapena | Garrantzia, xedea eta orientazioa | Downstream eragina |
| --- | --- | --- | --- |
| Funtzioa | **Orokorra** fitxa eta **Sortu bizkor** orrialdeak | Hautatu kostu-tasa aplikatzen zaion funtzioa. | Sarrerako estimazioaren edo benetako eginkizuna lerro honekin parekatuko da rolaren kostua lehenetsi ahal izateko. |
| Baliabide-unitatea | **Orokorra** fitxa eta **Sortu bizkor** orrialdeak | Aukeratu enpresaren antolakuntza unitatea edo banaketa zeregin hori non erabiliko den. Adibidez, Fabrikam Indiako Robotika dibisioko garatzailea edo Fabrikam AEBetako Software dibisioaren garatzailea. | Sarrerako estimazioaren edo benetako baliabide-unitateak lerro honekin parekatuko da rolaren kostua lehenetsi ahal izateko. |
| Prezioa | **Orokorra** fitxa eta **Sortu bizkor** orrialdeak | Konfiguratu eginkizunaren kostua, konpainia hornitzailea eta hornikuntza unitateen konbinazioa. Adibidez, Fabrikam Indiako garatzaile bat 1000 INR kostatzen da edo Fabrikam USA garatzaile bat 150 USD kostatzen da. | Prezioa sarrerako aurrekontuaren kostu unitateko edo lineako benetako lerroaren kostu lehenetsia da **Denbora** transakzio klasea. |
| Moneta | **Orokorra** fitxa eta **Sortu bizkor** orrialdeak | Berez, moneta balioa kostuen prezioen zerrendako goiburuko monetatik dator, baina gainidatz daiteke. Adibidez, Fabrikam Indiako garatzaile batek 1000 INR kostatzen ditu. Fabrikam USA-ko garatzaile batek 150 USD kostatzen du. | Moneta sarrerako benetako datuen kostuaren lerroko unitate kostua lehenesten du **Denbora** transakzio klasea. Proiektuaren kalkuluen arabera, moneta-balioa proiektuaren monetara bihurtzen da eta kalkuluen denbora-faseko ikuspegian agertzen da. |
| Unitate-antolaketa | **Orokorra** fitxa eta **Sortu bizkor** orrialdeak | Unitatearen ordutegia Denbora lehenetsia da eta ezin da aldatu Role prezioaren entitatean, denbora unitateen bidez tarifa espresak erabiltzen direlako. | Ez du behera eragiten. |
| Unitatea | **Orokorra** fitxa eta **Sortu bizkor** orrialdeak | Berez, balioa kostuen prezioen zerrendako **Denbora-unitatea** eremuaren goiburuko monetatik dator. Balioa gainidatz daiteke. Adibidez, Fabrikam Indiako garatzaile batek 1000 INR kostatzen ditu **India eguna** bakoitzeko. Fabrikam USA-ko garatzaile batek 150 USD kostatzen du **AEB egun** bakoitzeko. | Sistemak unitateen eta bihurtze sistema erabiltzen du oinarrizko unitateetan kostu bakoitzeko bat kalkulatzeko sarrerako estimazioan edo benetako lerroan unitateko prezio lehenetsia kalkulatzeko. Adibidez, kalkulua 10 da **India egunak** lana merezi du Indiako garatzaile batek eta unitateak, **India eguna** 10 ordu gisa definitzen da. Estimazio lerro hori kostatzerakoan, aplikazioak honela kalkulatzen du aurrekontuaren unitateko kostua: 1000 INR / 10 ordu = 100 INR orduko, USD bihurtzen dena eta unitateko kostu gisa agertzen dena **Proiektuaren aurrekontuak** orrialdea. |

## <a name="transfer-pricing-and-costs-for-resources-outside-of-your-division-or-legal-entity"></a>Transferitu prezioak eta kostuak zure dibisio edo pertsona juridikotik kanpoko baliabideengatik

Proiektuetan oinarritutako enpresetan, ohikoa da proiektuetan lege-erakunde edo sail desberdinetako langileak proiektuetan lan egiteko erabiltzeko. Proiektu bat pertsona juridiko batek exekutatu dezake, baina proiektuan lan egiten duten langile edo aholkulariak pertsona juridiko beretik edo beste batetik etor daitezke, edo bien konbinazioa egon daiteke. Dynamics 365 Project Operations-en, proiektuaren entregaren jabe den pertsona juridikoa da **Enpresa titularra** eta banaketaren jabea da **Kontratazio Unitatea**. Baliabideak eskaintzen dituzten beste pertsona juridikoak dira **Enpresa hornitzaileak** eta baliabideak eskaintzen dituzten zatiketak dira **Baliabideak hornitzeko unitateak**. Herrialde gehienetan, enpresek hornitzaileen pertsona juridikoa edo zatiketa ziurtatu behar dute, enpresa jabeari eta kontratazio unitateari baliabideak erabiltzeagatik kobratzen dutela.

Adibidez, Fabrikam korporazioak Fabrikam India-Robotics-ek Fabrikam US-Robotics edo Fabrikam UK-Robotics-ekin kostu tasa txartela negoziatu duela ziurtatu behar du.

Fabrikam India-Robotic-eko garatzaile batek 100 $ kobratzen du Fabrikam US-Robotics-i mailegu bat ematean eta 150 $Fabrikam U-Robotics-i mailegu bat ematean.

### <a name="set-up-costs-for-outside-resources"></a>Ezarri kanpoko baliabideen kostuak

1. Sortu kostuen prezioen zerrenda, *Fabrikam US-Robotics kostuen tasak* eta ezarri data-barruti eraginkorra.
2. Kostuen prezioen zerrendan, ezarri tarifak ondoko taulako informazioa erabiliz. 

| Funtzioa | Baliabideen enpresa | Baliabide-unitatea | Kostuaren tasa |
| --- | --- | --- | --- |
| Garatzailea | Fabrikam India | Fabrikam India-Robotika | 100 USD |
| Garatzailea | Fabrikam Philippines | Fabrikam Philippines-Robotics | 90 $ |
| Garatzailea | Fabrikam US | Fabrikam US-Robotics | 150 $ |

3. Erantsi kostuen prezioen zerrenda Fabrikam US-Robotics erakunde unitateari.

### <a name="set-up-transfer-pricing-for-a-resource-in-the-appropriate-currency"></a>Konfiguratu baliabide baten transferentzia prezioak dagokion monetan 

Project Operations-en, baliabideen prezioak edozein monetan konfigura daitezke. Moneta prezioen zerrendaren goiburuan dagoena lehenetsita dago, baina alda daiteke.

Transferentzia prezioa konfiguratzeko adibidea erabiliz, informazioa aldatu egin daiteke:

Fabrikam korporazioak Fabrikam India-Robotics-ek Fabrikam US-Robotics edo Fabrikam UK-Robotics-ekin kostu tasa negoziatu duela ziurtatu behar du.

Fabrikam India-Robotics-eko garatzaile batek 5000 INR kobratzen du Fabrikam US-Robotics-i mailegu bat ematean eta 5500 INR Fabrikam UK-Robotics-i mailegu bat ematean.

Fabrikam US-Robotics-en kostuen prezioen zerrendan, kostuen tasak honela adieraz daitezke:

| Funtzioa | Baliabideen enpresa | Kostua |
| --- | --- | --- |
| Garatzailea | Fabrikam India | 5000 INR |
| Garatzailea | Fabrikam US | 115 USD |

Fabrikam UK-Robotics-en kostuen prezioen zerrendan, kostuen tasak honela adieraz daitezke:

| Funtzioa | Baliabideen enpresa | Kostua |
| --- | --- | --- |
| Garatzailea | Fabrikam India | 5500 INR |
| Garatzailea | Fabrikam UK | 115 GBP |

Kostuen prezioen zerrendak lan-tasak moneta anitzetan eman ditzake. Proiektuaren kostu estimazioa sortzerakoan, Project Operations-en eragiketek kostu tasa horiek proiektuaren monetara bihurtuko dituzte eta erabiltzaileari bistaratuko dizkiete. Denbora sarrera onartzen denean eta kostu erreala sortzen denean, kostu erreala kostu prezioen zerrendako bat datorren rolaren prezio lerro horren monetan tasatzen da. Proiektu bakarreko denboraren kostu errealak moneta anitzetan erregistratu daitezke. Hala ere, proiektuaren benetako eskulanaren kostuak bildu edo laburtzerakoan, Project Operations-ek eskulanaren kostu kopuru guztiak proiektuaren monetara bihurtuko dituzte, erabiltzaileak ikus ditzakeenak.