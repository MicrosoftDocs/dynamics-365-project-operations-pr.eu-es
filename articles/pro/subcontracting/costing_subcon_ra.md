---
title: Azpikontratatutako baliabideen esleipenen kostuen estimazioa
description: Gai honek Microsoft nola nolabait azaltzen du Dynamics 365 Project Operations azpikontratatutako baliabideen esleipenen kostuen estimazioa kalkulatzen du.
author: rumant
ms.date: 12/03/2021
ms.topic: article
ms.reviewer: tonyafehr
ms.author: rumant
ms.openlocfilehash: 5a94840a3735639532683153105fea85bea99c9d
ms.sourcegitcommit: 45893132bd8bfaf944ee0ac855484684dd1ee945
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/09/2021
ms.locfileid: "7902981"
---
# <a name="cost-estimation-of-subcontracted-resource-assignments"></a>Azpikontratatutako baliabideen esleipenen kostuen estimazioa

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Azpikontratatutako proiektuko taldekideen ataza-esleipenak kostua erabiltzen da **Erosketa** lotutako taldekideen erregistroan azpikontratuari atxikitako prezioen zerrenda. Hau desberdina da langileen baliabideen esleipenak kostua erabiliz, non langileen baliabideen ataza esleipenak kostua erabiliz **Kostua** proiektuaren kontratazio-unitateari atxikita dagoen prezio-zerrenda. 

Azpikontratatuta dauden proiektu-talde generikoko kideentzat, esleipenak azpikontratazioari atxikitako erosketa-prezio-zerrendan roletan oinarritutako prezioen konfigurazioa erabiliz kostatzen dira. Erosketa prezioak baliabide bakoitzerako berariaz ere ezar daitezke. Baliabide espezifikoen prezio horiei lehentasuna emango zaie proiektu-talde izendatutako kideen zereginen esleipenak lan-kontratuko langileak direnean. 

Funtzio espezifikoko erosketa-prezioa erabiltzearen lehentasuna baliabideen araberako prezioen dimentsioaren lehentasuna ezarrita dago.**Parametroak > Zenbatekoetan oinarritutako prezioen dimentsioak**.

Azpikontratisten erosketa-prezioen dimentsioen konfigurazioan oinarritutako prezioak dinamikoki deribatzeko funtzionalitate hau lanaldi osoko langileentzako kostuak eta fakturak tasak eratorritakoaren antzekoa da. 

## <a name="creating-task-assignments-for-getting-cost-estimates-of-subcontractor-resources"></a>Azpikontratistaren baliabideen kostuen estimazioak lortzeko ataza-esleipenak sortzea

Azpikontratentzako zereginak bi modutara sor daitezke: 
- erabiliz **Zereginak** fitxa.
- erabiliz **Taldea** fitxa.

### <a name="creating-resources-assignments-using-the-tasks-tab"></a>Baliabideen esleipenak sortzea Zereginak fitxa erabiliz
erabiliz **Baliabideak** zerrendan **Zereginak** ataza zehatz baterako, zeregin esleipen bat sor dezakezu izendun baliabide baterako edo baliabide generiko baterako. Baliabide izendun bat hautatzen baduzu **Esleitutako Baliabideak** zereginean goitibeherako goitibeherakoa eta baliabide hau lan-kontratuko langile bat da, izendatutako baliabidea zereginari esleitzen zaio eta dagokion proiektu-taldekidearen erregistroa sortzen da langile mota gisa ezarrita.**Lan-kontratuko langilea** eta **Baliotasuna** ezarri **Baliogabea**. Hurrengo urrats gisa, proiektuko taldekideen erregistroa ireki eta azpikontratu eta azpikontratu lerro bat hautatu beharko duzu. Honek zereginen esleipena eguneratuko du azpikontratu eta azpikontratazio lerroari erreferentzia bat izateko eta taldekideen egoera ere eguneratuko du.**Baliozkoa**.

Taldekide generiko bat sortzea aukeratzen baduzu **Esleitutako Baliabideak** atazaren goitibeherakoa, **Taldekideen sorkuntza orokorra** elkarrizketa-koadroak azpikontratua eta azpikontratazio lerroa hautatzeko aukera emango dizu. Baliabide generikoa zereginari esleitzen zaionean eta dagokion proiektu-taldekidearen erregistroa sortzen denean, proiektu-taldekidearen erregistroa langile mota gisa ezarrita dagoela ikusiko duzu.**Lan-kontratuko langilea** eta **Baliotasuna** ezarri **Baliozkoa**.

### <a name="creating-project-team-members-using-the-team-tab"></a>Proiektuko taldekideak sortzea Taldea fitxa erabiliz
Proiektuko Taldea fitxa erabiliz, taldekide generiko bat edo izendun bat sor dezakezu. Taldekidea sortzerakoan, azpikontratazioa eta azpikontratazio lerroa hautatzeko aukera duzu. Taldekidea sortu ondoren, taldekidea zeregin bat esleitu beharko duzu erabiliz **Esleitutako Baliabideak** zereginean goitibeherakoa. 

## <a name="updating-estimates"></a>Estimazioak eguneratzea
Proiektuko taldeko kideak zereginak esleitu ondoren, hona joan beharko duzu **Estimazioak** fitxan proiektuan eta hautatu **Eguneratu prezioak** azpikontratistaren baliabideen esleipenen kostu-tasak azpikontratuari atxikitako erosketa-prezioen zerrendan oinarrituta eguneratzen direla ziurtatzeko. Kontuan izan Microsoft-en esleitu gabeko zereginetarako estimazioak ez direla sortzen Dynamics 365 Project Operations. Ondorioz, zereginen esleipenak sortu beharko dituzu zure proiektuko hainbat ataza prezio eta kostua izateko. 

> [OHARRA!] Proiektuko taldekideek duten **Langile mota** gisa **Lan-kontratuko langilea** baina ez dute azpikontratu erreferentziarik bezala markatzen dira **Baliogabea** gainean **Proiektuko taldekideak** sareta. Egoera hori duen proiektu-taldekideren bat baldin badago, ireki proiektu-taldearen erregistroa eta eguneratu eskuz azpikontratazio eta azpikontratazio-lerroen eremuak, finantza-kostuen estimazioak azpikontratistaren kostua zehatz-mehatz isla dezan.**Estimazioak** fitxa. 


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
