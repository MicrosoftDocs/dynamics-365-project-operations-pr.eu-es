---
title: Azpikontratatutako baliabideen esleipenen kostuak kalkulatzea
description: Artikulu honek nola nolabait azaltzen du Microsoft Dynamics 365 Project Operations azpikontratatutako baliabideen esleipenen kostuen estimazioa kalkulatzen du.
author: rumant
ms.date: 09/14/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 9fded1baa63d2defc134994c858dfc6c09f75082
ms.sourcegitcommit: 08eb3be9eda44e9446c43ed9b6aefd58d77927c5
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/15/2022
ms.locfileid: "9522639"
---
# <a name="cost-estimation-of-subcontracted-resource-assignments"></a>Azpikontratatutako baliabideen esleipenen kostuak kalkulatzea

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Azpikontratatutako proiektuko taldekideen ataza-esleipenak kostua erabiltzen da **Erosketa** lotutako taldekideen erregistroan azpikontratuari atxikitako prezioen zerrenda. Langileen baliabideen esleipenak kostua erabiliz langileen baliabideen ataza-esleipenak balioesten direnetik desberdina da **Kostua** proiektuaren kontratazio-unitateari atxikita dagoen prezio-zerrenda. 

Azpikontratatutako proiektuko taldekideen ataza-esleipenak kostua erabiltzen da Erosketa lotutako taldekideen erregistroan azpikontratuari atxikitako prezioen zerrenda. Erosketa prezioak baliabide bakoitzerako berariaz ere ezar daitezke. Baliabide espezifikoen prezio horiei lehentasuna emango zaie proiektu-talde izendatutako kideen lan-esleipenak lan-kontratuko langileak direnean. 

Funtzio espezifikoko erosketa-prezioa erabiltzearen lehentasuna baliabideen araberako prezioen dimentsioaren lehentasunaren ezarpenak ezartzen du **Parametroak > Zenbatekoetan oinarritutako prezioen dimentsioak**.

Azpikontraten erosketa-prezioen dimentsioen konfigurazioan oinarritutako prezioak modu dinamikoan eratortzeko funtzionalitate hau lanaldi osoko langileen kostu eta faktura-tasak eratorritakoaren antzekoa da. 

## <a name="creating-task-assignments-for-getting-cost-estimates-of-subcontractor-resources"></a>Azpikontratistaren baliabideen kostuen estimazioak lortzeko ataza-esleipenak sortzea

Azpikontratentzako zereginak bi modutara sor daitezke: 
- Erabili **Zereginak** fitxa.
- Erabili **Taldea** fitxa.

### <a name="creating-resources-assignments-using-the-tasks-tab"></a>Baliabideen esleipenak sortzea Zereginak fitxa erabiliz
Erabiliz **Baliabideak** zerrendan **Zereginak** ataza zehatz baterako, zeregin esleipen bat sor dezakezu izendun baliabide baterako edo baliabide generiko baterako. Baliabide izendun bat hautatzen baduzu **Esleitutako Baliabideak** zereginean goitibeherako goitibeherakoa eta baliabide hau kontratu-langile bat da, izendatutako baliabidea zereginari esleitzen zaio eta dagokion proiektu-taldekidearen erregistroa sortzen da langile mota gisa ezarrita **Lan-kontratuko langilea** eta **Baliotasuna** ezarri **Baliogabea**. Hurrengo urrats gisa, proiektuko taldekideen erregistroa ireki eta azpikontratu eta azpikontratu lerro bat hautatu beharko duzu. Honek zereginen esleipena eguneratuko du azpikontratu eta azpikontratu lerroari erreferentzia bat izateko eta taldekideen egoera ere eguneratuko du **Baliozkoa**.

Taldekide generiko bat sortzea aukeratzen baduzu **Esleitutako Baliabideak** atazaren goitibeherakoa, **Taldekideen sorkuntza orokorra** elkarrizketa-koadroak azpikontratua eta azpikontratazio lerroa hautatzeko aukera emango dizu. Baliabide generikoa zereginari esleitzen zaionean eta dagokion proiektuko taldeko kideen erregistroa sortzen denean, proiektuko taldeko kideen erregistroa langile mota gisa ezarrita dagoela ikusiko duzu **Lan-kontratuko langilea** eta **Baliotasuna** ezarri **Baliozkoa**.

### <a name="creating-project-team-members-using-the-team-tab"></a>Proiektuko taldekideak sortzea Taldea fitxa erabiliz
Proiektuko Taldea fitxa erabiliz, taldekide generiko bat edo izendun bat sor dezakezu. Taldekidea sortzerakoan, azpikontratazioa eta azpikontratua lerroa hauta ditzakezu. Taldekidea sortu ondoren, taldekideari zeregin bat esleitu beharko diozu **Esleitutako Baliabideak** zereginaren goitibeherakoa. 

## <a name="updating-estimates"></a>Estimazioak eguneratzea
Proiektuko taldeko kideak zereginak esleitu ondoren, atalera nabigatu beharko duzu **Estimazioak** fitxan proiektuan eta hautatu **Eguneratu prezioak** azpikontratistaren baliabideen esleipenen kostu-tasak azpikontratuari atxikitako erosketa-prezioen zerrendan oinarrituta eguneratzen direla ziurtatzeko. Ez dira esleitu gabeko zereginetarako kalkuluak sortzen Microsoft Dynamics 365 Project Operations-en. Ondorioz, zereginen esleipenak sortu beharko dituzu zure proiektuko hainbat ataza prezioa eta kostua emateko. 

> [OHARRA!] Proiektuko taldekideek duten **Langile mota** bezala **Lan-kontratuko langilea** baina ez dute azpikontratu erreferentziarik bezala markatzen dira **Baliogabea** gainean **Proiektuko taldekideak** sareta. Egoera hori duen proiektu-taldekideren bat baldin badago, ireki proiektu-taldearen erregistroa eta eguneratu eskuz azpikontratazio eta azpikontratazio-lerroaren eremuak, finantza-kostuen estimazioak azpikontratistaren kostua zehatz-mehatz isla dezan **Estimazioak** fitxa. 


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
