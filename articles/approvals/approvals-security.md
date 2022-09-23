---
title: Segurtasuna eta homologazioak
description: Artikulu honek Microsoft-en onarpenekin lan egiteko segurtasun-konfigurazioari buruzko informazioa eskaintzen du Dynamics 365 Project Operations.
author: stsporen
ms.date: 08/29/2022
ms.topic: security
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: bc33f63f66bdcf1470e5d9386cfc3661774436fd
ms.sourcegitcommit: b2d05f898daa552179d67fdf4c060c93a9c66bd1
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/16/2022
ms.locfileid: "9525398"
---
# <a name="security-and-approvals"></a>Segurtasuna eta homologazioak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Microsoft Dynamics 365 Project Operations bi segurtasun-rol erabiltzen ditu denbora, gastu eta material-sarrerak onartzeko:

- Proiektuaren onartzailea
- Proiektuaren onartzailea administratzailea

## <a name="project-approver"></a>Proiektuaren onartzailea

Izan behar duzu **Proiektuaren onespena** segurtasun-funtzio proiektuaren denbora, gastu eta material sarrerak onartzeko. Dagokion entitateetarako sarbidea ere izan behar duzu, adibidez **Proiektua**. Sarbide hori duen norbaitek eslei dezake **Proiektuaren arduraduna** rola. Gainera, proiektuko taldekidea izan behar duzu eta onartzaile gisa markatuta egon behar duzu.

Proiektuak ez diren sarrerak onartzeko, bidaltzailearen kudeatzailea izan behar duzu.

## <a name="project-approver-admin"></a>Proiektuaren onartzailea administratzailea

> [!NOTE]
> The [Onarpen multzoak](approval-sets.md) eginbidea gaituta egon behar da Project Approver Admin funtzioa erabili ahal izateko.

The **Proiektuaren onartzailea administratzailea** segurtasun-funtzio-ek erabiltzaileei politikak saihesteko aukera ematen die eta proiektu guztietan sarrerak onartzeko aukera ematen du. Rol hau esleitzeak taldekide izatea eta onartzaile gisa markatzea eskatzen duen baliozkotze-logika baztertuko du. Dagokion erlazionatutako entitateetarako sarbidea izan behar duzu, adibidez **Proiektua**. Sarbide hori duen norbaitek eslei dezake **Proiektuaren arduraduna** rola.

SISTEMA erabiltzailearen testuinguruak balioztatzeak saihesten ditu segurtasun-funtzio proiektuaren onarpenaren administratzaileak egiten dituen modu berean.
