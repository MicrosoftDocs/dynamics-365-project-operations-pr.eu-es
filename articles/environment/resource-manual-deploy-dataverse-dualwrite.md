---
title: Inplementatu eskuz Project Operations-en Dataverse aplikazioa idazketa dualaren bateragarritasunarekin
description: Artikulu honek proiektuaren eragiketak eskuz nola zabaldu azaltzen du Dataverse aplikazioa idazketa bikoitza onartzen duen.
author: stsporen
ms.date: 06/18/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: a25e2a59f1c069057c6689825ce52b13d842af71
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/18/2022
ms.locfileid: "9028549"
---
# <a name="manually-deploy-the-project-operations-dataverse-app-with-dual-write-support"></a>Inplementatu eskuz Project Operations-en Dataverse aplikazioa idazketa dualaren bateragarritasunarekin

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Artikulu honek Microsoft eskuz nola zabaldu azaltzen du Dynamics 365 Project Operations urtean Microsoft Dataverse beraz, idazketa bikoitza onartzen du. Project Operations-ek ingurunearen konfigurazioa hautematen dute eta idazketa bikoitzerako laguntza gehigarria gehitzen dute aurrez aurreko baldintzak betetzen badira.

Inplementazioan zehar Microsoft Dynamics Lifecycle Services (LCS), artikulu honetako argibideak jarraitu badituzu, salta dezakezu Microsoft Power Platform integrazioa (lehen bezala ezagutzen zen Common Data Service ingurunea).

Dataverse-ko Project Operations-ek idazketa bikoitza onartzeko inplementazio prozesuak du lau urrats nagusi ditu:

1. [Ingurune berri bat sortu Dataverse-n idazketa bikoitza onartzen duena](#create).
2. [Gehitu idazketa bikoitzaren aurrebaldintzak inguruneari](#prerequisites).
3. [Gehitu Project Operations Dataverse aplikazioan](#dataverse).
4. [Estekatu inguruneak](#link).

## <a name="create-a-new-environment-in-dataverse-that-supports-dual-write"></a><a name="create"></a>Sortu ingurune bat Dataverse-n idazketa bikoitza onartzen duena

Prozedura hau osatzeko, administratzaile gisa hasi behar duzu saioa.

1. Ireki [Power Platform administratzaile zentroa](https://admin.powerplatform.com), eta hasi saioa administratzaile gisa.
2. Sortu ingurune bat eta jarri izena.
3. Hautatu ingurune mota. Probako eskaintzan izena eman baduzu, hautatu **Proba (harpidetzan oinarrituta)**.
4. Berretsi inplementazioaren eskualdea.
5. Gaitu **Sortu datu-base bat ingurune honetarako** aukera. 
6. Berretsi hizkuntza, eta, ondoren, egiaztatu moneta bat datorrela finantza- eta operazio-aplikazioetako diruarekin.
7. Gaitu **Dynamics 365 aplikazioak** aukera, eta baieztatu **Aplikazio hauek automatikoki zabaldu** eremua ezarrita dagoela **Bat ere ez** gisa.
8. Gehitu segurtasun taldea, segurtasun taldea beharrezkoa bada.
9. Hautatu **Gorde** ingurunea sortzeko.
10. Itxaron inplementazioa amaitu arte eta ingurunea **Prest** egoeran egon arte.

## <a name="add-dual-write-prerequisites-to-the-environment"></a><a name="prerequisites"></a>Gehitu idazketa bikoitzaren aurrebaldintzak inguruneari

Idazketa dualaren euskarriak funtsezko entitateei gehitzen zaizkien eremu osagarriak biltzen ditu, adibidez **Enpresa** entitatea. Lehendik dagoen ingurune bati idazketa bikoitzeko laguntza gehitzen ari bazara, baliteke datuak eguneratu beharko izatea laguntza gaitzeko. Datuak abiarazteko moduari buruzko informazioa lortzeko, ikusi [Bootstrap enpresaren datuak](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data). Idazketa bikoitzari buruzko informazio gehiago lortzeko, ikusi [Idazketa bikoitzeko sistemaren eskakizunak](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req).

Osatu prozedura hau idazketa bikoitzaren aurrebaldintzak zure inguruneari gehitzeko.

1. Ireki sortu berri duzun ingurunea eta joan hona **Baliabidea** \> **Dynamics 365 aplikazioak**.
2. Aukeratu **Idazketa dualeko oinarrizko soluzioa** aplikazioen zerrendan eta instalatu.
3. Itxaron instalazioa amaitu arte. Aukeratu **Idazketa dualaren aplikazioa antolatzeko soluzioa** aplikazioen zerrendan eta instalatu.

## <a name="add-the-project-operations-dataverse-app"></a><a name="dataverse"></a>Gehitu Project Operations Dataverse aplikazioan

Project Operations instalatu aurretik aurreko izapideak burutu badituzu soilik egin dezakezu prozedura hau. Instalazioan zehar, sistemak ingurumenaren konfigurazioa aztertzen du eta beharrezkoa bada idazketa bikoitzeko laguntza gehitzen du.

1. Ireki sortu duzun ingurunea eta joan hona **Baliabidea** \> **Dynamics 365 aplikazioak**.
2. Aukeratu **Microsoft Dynamics 365 Project Operations** aplikazioen zerrendan eta instalatu.

## <a name="link-your-environments"></a><a name="link"></a>Estekatu inguruneak

Ondoren Dataverse ingurunea zabalduta dago, esteka konfigura dezakezu zure finantza eta eragiketa aplikazioetan. Jarraitu urratsak: [Erabili idazketa bikoitzeko morroia zure inguruneak lotzeko](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment).
