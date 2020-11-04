---
title: Garatu proiektuaren txantiloiak Kopiatu proiektua eginbidearekin
description: Gai honek proiektuaren txantiloiak sortzeko proiektuari buruzko informazioa eskaintzen du Kopiatu proiektua ekintza pertsonalizatua erabiliz.
author: stsporen
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: cb49109e8c199bc4569702ae844a19985534294d
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070976"
---
# <a name="develop-project-templates-with-copy-project"></a>Garatu proiektuaren txantiloiak Kopiatu proiektua eginbidearekin

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations-ek proiektu bat kopiatu eta eginkizunak eginkizuna adierazten duten baliabide generikoetara itzultzeko gaitasuna onartzen du. Bezeroek funtzionalitate hau erabil dezakete oinarrizko proiektuen txantiloiak eraikitzeko.

Hautatzen duzunean **Kopiatu proiektua** , helburuko proiektuaren egoera eguneratzen da. Erabili **Egoeraren arrazoia** kopia ekintza noiz bukatu den jakiteko. **Kopiatu proiektua** hautatuz gero, proiektuaren hasiera-data uneko hasierako datara eguneratzen du xede-proiektuaren entitatean xede-datarik hautematen ez bada.

## <a name="copy-project-custom-action"></a>Kopiatu proiektuaren ekintza pertsonalizatua 

### <a name="name"></a>Eman izena 

**msdyn_CopyProjectV2**

### <a name="input-parameters"></a>Sarrerako parametroak
Hiru sarrera-parametro daude:

| Parametroa          | Idatzi   | Balioak                                                   | 
|--------------------|--------|----------------------------------------------------------|
| ProjectCopyOption  | String | **{"removeNamedResources":true}** edo **{"clearTeamsAndAssignments":true}** |
| SourceProject      | Entitate-erreferentzia | Jatorriko proiektua |
| Helburua             | Entitate-erreferentzia | Helburu Proiektua |


- **{"clearTeamsAndAssignments":true}** : Lehenetsitako portaera duzu proiektuarentzako Weberako eta zeregin guztiak eta taldekideak kenduko ditu.
- **{"removeNamedResources":true}** Proiektuaren eragiketen portaera lehenetsia, eta zereginak baliabide generikoetara itzuliko ditu.

Ekintzei buruzko informazio gehiagorako, ikusi [Erabili web API ekintzak](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)

## <a name="specify-fields-to-copy"></a>Zehaztu kopiatu beharreko eremuak 
Ekintza deitzen denean, **Kopiatu proiektua** proiektuaren ikuspegia aztertuko du **Kopiatu proiektuaren zutabeak** proiektua kopiatzerakoan zein eremu kopiatu zehazteko.
