---
title: Segurtasuna eta onarpenak
description: Artikulu honek onarpenekin lan egiteko segurtasun-konfigurazioari buruzko informazioa eskaintzen du Microsoft Dynamics 365 Project Operations.
author: stsporen
ms.date: 08/29/2022
ms.topic: conceptual
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 88186485dff43c3011095b267640151948b4d77c
ms.sourcegitcommit: 0d11377bf3ac74c80afbd2013775fcc9869f926a
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/10/2022
ms.locfileid: "9841908"
---
# <a name="security-and-approvals"></a>Segurtasuna eta onarpenak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Microsoft Dynamics 365 Project Operations bi segurtasun-rol erabiltzen ditu denbora, gastu eta material-sarrerak onartzeko:

- Proiektuaren onartzailea
- Proiektuaren onartzailearen administratzailea

## <a name="project-approver"></a>Proiektuaren onartzailea

Izan behar duzu **Proiektuaren onespena** segurtasun-funtzio proiektuaren denbora, gastua eta materialaren sarrerak onartzeko. Dagokion entitateetarako sarbidea ere izan behar duzu, adibidez **Proiektua**. Sarbide hori duen norbaitek eslei dezake **Proiektuaren arduraduna** rola. Gainera, proiektuko taldekidea izan behar duzu eta onartzaile gisa markatuta egon behar duzu.

Proiektuak ez diren sarrerak onartzeko, bidaltzailearen kudeatzailea izan behar duzu.

## <a name="project-approver-admin"></a>Proiektuaren onartzailearen administratzailea

> [!NOTE]
> [Onarpen multzoak](approval-sets.md) eginbidea gaituta egon behar da Project Approver Admin funtzioa erabili ahal izateko.

**Proiektuaren onartzailea administratzailea** segurtasun-funtzio-ek erabiltzaileei politikak saihesteko aukera ematen die eta proiektu guztietan sarrerak onartzeko aukera ematen du. Rol hau esleitzeak taldekide izatea eta onartzaile gisa markatzea eskatzen duen baliozkotze-logika baztertuko du. Dagokion tauletarako sarbidea izan behar duzu, adibidez **Proiektua**, esleitutako segurtasun-rolen bidez.

SISTEMA erabiltzailearen testuinguruak baliozkotzeak saihesten ditu segurtasun-funtzio Proiektuaren onartzaileen administratzaileak egiten duen moduan.
