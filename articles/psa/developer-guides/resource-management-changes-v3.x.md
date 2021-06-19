---
title: Baliabide-kudeaketa gida (Project Service Automation 3.x)
description: Gai honek baliabideak kudeatzeko eremuan izandako aldaketen inguruko informazioa ematen du.
author: makk
ms.custom:
- dyn365-projectservice
ms.date: 03/18/2019
ms.topic: article
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: e888d55b93c40e08e51bd4480853fec37f2b6333
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6007801"
---
# <a name="resource-management-changes-project-service-automation-3x"></a>Baliabide-kudeaketa gida (Project Service Automation 3.x)

[!include [banner](../../includes/psa-now-project-operations.md)]

Gai honen atalek Dynamics 365 Project Service Automation aplikazioaren 3.x bertsioako baliabideak kudeatzeko eremuan egin diren aldaketen inguruko informazioa ematen dute.

## <a name="project-estimates"></a>Proiektuaren aurreikuspenak

**msdyn \_projecttask** entitatean (**Proiektuaren zeregina**) oinarrituta egon beharrean, proiektuaren aurreikuspenak **msdyn \_resourceassignment** entitatean (**Baliabide-esleipena**) oinarritzen dira. Baliabide-esleipenak zereginen planifikazioa eta prezioak egiteko "egia iturri" bihurtu dira.

## <a name="line-tasks"></a>Lerro-zereginak

PSA aplikazioaren 3.x bertsioan, lerro-zereginak zaharkituta daude. Esleipenek zeregin osoa adierazten dute lerro-zereginen ordez.

Hurrengo adibidean, "Probako zeregina" izeneko zeregina A eta B taldeko kideei nola esleitu zaien ikusten da PSA-ren aurreko bertsioetan eta PSA-ren 3.x bertsioan.

- **PSA-ren 3.x bertsioaren aurretik:**

    - Probako zeregina

        - Probako zeregina - 1. lerro-zeregina

            - Esleipena Ari

        - Probako zeregina - 2. lerro-zeregina

            - Esleipena Bri

- **PSA-ren 3.x bertsioa:**

    - Probako zeregina

        - Esleipena Ari
        - Esleipena Bri

## <a name="unassigned-assignment"></a>Esleitu gabeko esleipena

PSA-ren 3.x bertsion, esleitu gabeko esleipena **NULUA** taldekidea eta **NULUA** baliabideari esleitutako esleipena da. Esleipen gabeko esleipenak bi egoeratan gerta daitezke:

- Zeregin bat sortu bada, baina oraindik taldekideren bati esleitu ez bazaio, esleitu gabeko esleipena sortzen da beti. 
- Zeregin bateko esleipendun guztiak kentzen badira, zeregin horretarako esleitu gabeko esleipena sortzen da berriro.

## <a name="scheduling-fields-on-the-project-task-entity"></a>Proiektuaren zereginen entitateko eremuak antolatzea

**msdyn \_projecttask** entitateko eremuak zaharkituta geratu dira, **msdyn \_resourceassignment** entitatera mugitu dira edo orain **msdyn \_projectteam** entitatean (**Proiektu-taldeko kidea**) aipatzen dira.

| Zaharkitutako eremua on msdyn\_projecttask atalean (Proiektuaren zeregina) | Eremu berria msdyn\_resourceassignment atalean (Baliabideen esleipena) | Iruzkina |
|---|---|---|
| msdyn\_assignedresources | Bat ere ez | |
| msdyn\_assignedteammembers | Bat ere ez | |
| msdyn\_numberofresources | Bat ere ez | |
| msdyn\_scheduledhours | Bat ere ez | |
| msdyn\_effortcontour | msdyn\_plannedwork | Eremuan gordetako JavaScript Object Notation (JSON) datuen egituraren formatua aldatu da. |

## <a name="schedule-contour"></a>Antolaketaren ingerada

Antolaketaren ingerada **Aurreikusitako lana** eremuan gordetzen da (**msdyn \_plannedwork**) **Baliabide-esleipena** entitate bakoitzean (**msdyn \_resourceassignment**).

### <a name="structure"></a>Egitura

Antolaketaren ingeradaren egitura berria antolatutako egun bakoitzerako definitzen diren denbora-tarte malguek osatzen dute. Denbora-tarte bakoitzean propietate hauek daude:

- **Hasi** – Eguneko lanaldiaren hasiera, proiektuaren egutegiaren arabera.
- **Amaitu** – Eguneko lanaldiaren amaiera, proiektuaren egutegiaren arabera.
- **Orduak** – Egunean esleitzen zaion ordu kopurua.

**Adibidea**

Adibide honek proiektuaren egutegia erabiltzen du, non laneguna goizeko 9etatik arratsaldeko 5etara den UTC-8 ordu-zonan.

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

### <a name="auto-scheduling-and-manual-scheduling"></a>Programazio automatikoa eta eskuzko programazioa

Zeregin bat automatikoki programatuta badago, orduak aurrez kargatzen dira eta zereginen iraupena murriztu liteke.

**Adibidea**

Honako zeregin hau automatikoki programatuta dago 3 egunetan 18 ordu egiteko (2018ko abenduaren 3tik 2018ko abenduaren 5era).

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

Zeregin bat eskuz programatuta badago, orduak uniformeki banatzen dira data guztietan.

**Adibidea**

Honako zeregin hau eskuz programatuta dago 3 egunetan 18 ordu egiteko (2018ko abenduaren 3tik 2018ko abenduaren 5era).

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":6},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":6},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":6}]
```

### <a name="assignment-unit"></a>Esleipen-unitatea

Esleipen-unitatea zaharkituta gelditu da PSA aplikazioaren 3.x bertsioan. Zereginaren ahalegin orduak berdin banatzen dira eguneko, esleitutako baliabide guztien artean.

**Adibidea**

Adibide honetan, zeregina bi baliabideri esleitzen zaie eta automatikoki antolatuta dago 3 egunez 36 ordu egiteko (2018ko abenduaren 3tik 2018ko abenduaren 5era).

- 1. esleipena:

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

- 2. esleipena:

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

## <a name="pricing-dimensions"></a>Prezio-dimentsioak

PSA-ren 3.x bertsioan, baliabide zehatzei buruzko prezioen dimentsioaren eremuak (adibidez, **Funtzioa** eta **Antolaketa-unitatea**) kendu dira **msdyn \_projecttask** erakundetik. Eremu horiek dagoeneko proiektu-taldeko kidetik (**msdyn\_projectteam**), baliabide-esleipenekoa (**msdyn\_resourceassignment**), eskura daitezke proiektuaren aurreikuspenak sortzen direnean. Beste eremu bat, **msdyn\_organizationaluni**, gehitu da **msdyn\_projectteam** entitatean.

| Zaharkitutako eremua on msdyn\_projecttask atalean (Proiektuaren zeregina) | Horren ordez erabiltzen den msdyn\_projectteam (proiektu-taldeko kidea) ataleko eremua |
|---|---|
| msdyn\_resourcecategory | msdyn\_resourcecategory |
| msdyn\_organizationalunit | msdyn\_organizationalunit |

## <a name="contours"></a>Ingeradak

Prezioen eta aurreikuspenen ingarada eremuak zeharkitu egin dira **msdyn\_projecttask** entitatean. **msdyn\_resourceassignment** entitatera mugitu dira.

| Zaharkitutako eremua on msdyn\_projecttask atalean (Proiektuaren zeregina) | Eremu berria msdyn\_resourceassignment atalean (Baliabideen esleipena) |
|---|---|
| msdyn\_costestimatecontour | msdyn\_plannedcostcontour |
| msdyn\_salesestimatecontour | msdyn\_plannedsalescontour |

Hurrengo eremuak **msdyn\_resourceassignment** entitatera gehitu dira:

* msdyn\_plannedcost
* msdyn\_plannedsales

Aurreikusitako, benetako eta gainerako kostuen eta salmenten eremuak aldatu gabe daude **msdyn\_projecttask** entitatean:

* msdyn\_plannedcost
* msdyn\_plannedsales
* msdyn\_actualcost
* msdyn\_actualsales
* msdyn\_remainingcost
* msdyn\_remainingsales


[!INCLUDE[footer-include](../../includes/footer-banner.md)]