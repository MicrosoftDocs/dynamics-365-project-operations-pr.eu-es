---
title: Azpikontratatutako baliabideen esleipenen kostuak kalkulatzea
description: Gai honek Microsoft nola nolabait azaltzen du Dynamics 365 Project Operations azpikontratatutako baliabideen esleipenen kostuen estimazioa kalkulatzen du.
author: rumant
ms.date: 12/03/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: f276e12713261538d1e7520dac17243e578db433
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8596679"
---
# <a name="cost-estimation-of-subcontracted-resource-assignments"></a>Azpikontratatutako baliabideen esleipenen kostuak kalkulatzea

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Azpikontratatutako proiektuko taldekideen ataza-esleipenak kostua erabiltzen da **Erosketa** lotutako taldekideen erregistroan azpikontratuari atxikitako prezioen zerrenda. Hau desberdina da langileen baliabideen esleipenen kostua, non langileen baliabideen zereginen esleipenak kostua erabiliz **Kostua** proiektuaren kontratazio-unitateari atxikita dagoen prezio-zerrenda. 

Azpikontratatuta dauden proiektu-talde generikoko kideentzat, esleipenak azpikontratazioari atxikitako erosketa-prezio-zerrendan roletan oinarritutako prezioen konfigurazioa erabiliz kostatzen dira. Erosketa prezioak baliabide bakoitzerako berariaz ere ezar daitezke. Baliabide espezifikoen prezio horiei lehentasuna emango zaie proiektuko taldekide izendatuen lan-esleipenak kontratudun langileak direnean. 

Funtzio espezifikoa den erosketa-prezioa erabiltzearen lehentasuna baliabideen araberako prezioen dimentsioaren lehentasuna ezarrita dago.**Parametroak > Zenbatekoetan oinarritutako prezioen dimentsioak**.

Azpikontratisten erosketa-prezioen dimentsioen konfigurazioan oinarritutako prezioak dinamikoki deribatzeko funtzionalitate hau lanaldi osoko langileentzako kostuak eta fakturak tasak eratorritakoaren antzekoa da. 

## <a name="creating-task-assignments-for-getting-cost-estimates-of-subcontractor-resources"></a>Azpikontratistaren baliabideen kostuen estimazioak lortzeko ataza-esleipenak sortzea

Azpikontratentzako zereginak bi modutara sor daitezke: 
- erabiliz **Zereginak** fitxa.
- erabiliz **Taldea** fitxa.

### <a name="creating-resources-assignments-using-the-tasks-tab"></a>Baliabideen esleipenak sortzea Zereginak fitxa erabiliz
erabiliz **Baliabideak** zerrendan **Zereginak** ataza zehatz baterako, zeregin esleipen bat sor dezakezu izendun baliabide baterako edo baliabide generiko baterako. Baliabide izendun bat hautatzen baduzu **Esleitutako Baliabideak** zereginean goitibeherako goitibeherakoa eta baliabide hau lan-kontratuko langile bat da, izendatutako baliabidea zereginari esleitzen zaio eta dagokion proiektu-taldekidearen erregistroa sortzen da langile mota gisa ezarrita.**Lan-kontratuko langilea** eta **Baliotasuna** ezarri **Baliogabea**. Hurrengo urrats gisa, proiektuko taldekideen erregistroa ireki eta azpikontratu eta azpikontratu lerro bat hautatu beharko duzu. Honek zereginen esleipena eguneratuko du azpikontratu eta azpikontratu lerroari erreferentzia bat izateko eta taldekideen egoera ere eguneratuko du.**Baliozkoa**.

Taldekide generiko bat sortzea aukeratzen baduzu **Esleitutako Baliabideak** atazaren goitibeherakoa, **Taldekideen sorkuntza orokorra** elkarrizketa-koadroak azpikontratua eta azpikontratazio lerroa hautatzeko aukera emango dizu. Baliabide generikoa zereginari esleitzen zaionean eta dagokion proiektu-taldekidearen erregistroa sortzen denean, proiektu-taldekidearen erregistroa langile mota gisa ezarrita dagoela ikusiko duzu.**Lan-kontratuko langilea** eta **Baliotasuna** ezarri **Baliozkoa**.

### <a name="creating-project-team-members-using-the-team-tab"></a>Proiektuko taldekideak sortzea Taldea fitxa erabiliz
Proiektuko Taldea fitxa erabiliz, taldekide generiko edo izendun bat sor dezakezu. Taldekidea sortzerakoan, azpikontratazioa eta azpikontratua lerroa hauta ditzakezu. Taldekidea sortu ondoren, taldekidea zeregin bat esleitu beharko duzu erabiliz **Esleitutako Baliabideak** zereginean goitibeherakoa. 

## <a name="updating-estimates"></a>Estimazioak eguneratzea
Proiektuko taldeko kideak zereginak esleitu ondoren, atalera nabigatu beharko duzu **Estimazioak** fitxan proiektuan eta hautatu **Eguneratu prezioak** azpikontratistaren baliabideen esleipenen kostu-tasak azpikontratuari atxikitako erosketa-prezioen zerrendan oinarrituta eguneratzen direla ziurtatzeko. Ez dira esleitu gabeko zereginetarako kalkuluak sortzen Microsoft-en Dynamics 365 Project Operations. Ondorioz, zereginen esleipenak sortu beharko dituzu zure proiektuko hainbat ataza prezioa eta kostua emateko. 

> [OHARRA!] Proiektuko taldekideek duten **Langile mota** gisa **Lan-kontratuko langilea** baina ez dute azpikontratu erreferentziarik bezala markatzen dira **Baliogabea** gainean **Proiektuko taldekideak** sareta. Egoera hori duen proiektu-taldekideren bat baldin badago, ireki proiektu-taldearen erregistroa eta eguneratu eskuz azpikontratazio eta azpikontratazio-lerroen eremuak, finantza-kostuen estimazioak azpikontratistaren kostua zehatz-mehatz isla dezan.**Estimazioak** fitxa. 


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
