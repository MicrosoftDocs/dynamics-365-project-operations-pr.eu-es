---
title: Enpresen arteko gastuak
description: Erakunde bateko pertsona juridiko batek lan egiten duen langileak erakunde bereko beste pertsona juridiko baterako lana egin dezake. Egoera horretan, enpresen arteko gastuen eginbidea erabil dezakezu langilearen gastuak lana egin duen pertsona juridikoari esleitzeko.
author: ShylaThompson
manager: AnnBe
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvParameters
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 0967f23e4e1f8e0431c55d4d54554e7e90e2451c
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071187"
---
# <a name="intercompany-expenses"></a>Enpresen arteko gastuak

[!include [banner](../includes/banner.md)]

Erakunde bateko pertsona juridiko batek lan egiten duen langileak erakunde bereko beste pertsona juridiko baterako lana egin dezake. Egoera horretan, enpresen arteko gastuen eginbidea erabil dezakezu langilearen gastuak lana egin duen pertsona juridikoari esleitzeko. Langilea enplegatzen duen pertsona juridikoari mailegu-pertsona deitzen zaio. Langileak gastuak egiten dituen pertsona juridikoari mailegu-pertsona deitzen zaio. 

Langile batek beste pertsona juridiko batentzat egiten duen lanaren gastuak sortu eta aurkeztu ahal izango ditu aurretik, maileguan dagoen pertsona juridikoan, **Gastuak kudeatzeko parametroak** orria, hautatu **Onartu enpresen arteko gastu lerroak** aukera. 

## <a name="tax-posting-for-intercompany-expenses"></a>Enpresen arteko gastuen zerga argitaratzea

[!include [banner](../includes/banner.md)]

Mailegu (iturburu) pertsona juridikoarekin lotura duten zerga taldeak erabili behar badituzu zure gastuen txostenean maileguarekin (helmuga) duen pertsona juridikoarekin ordez, hau konfiguratu beharko duzu liburu nagusiko salmenten gaineko zerga konfiguratuta. Liburu nagusiaren parametroa denean, **Enpresen arteko zergak argitaratzeko pertsona juridikoa** ezarrita dago **Iturria** eta **Salmenten gaineko zergaren gaineko zerga arauak aplikatzea** ezarrita dago **Ez** , mailegu-entitate juridikoaren zerga-konbinazioa erabiliko da. Parametro bera ezarrita dagoenean **Helmuga** , zorpetutako entitate juridikoaren zerga-konbinazioa erabiliko da. Estatu Batuetako pertsona juridikoetarako, parametroa ezarrita dagoenean **Iturria** , **Kobratu beharreko salmenten gaineko zerga** eremua berrian konfiguratu behar da **Liburuak argitaratzeko taldeak** orrialdea. Kontabilitate motorrak eremu honetako informazioa erabiliko du zergekin lotutako kontabilitate sarrera egiteko.   
Jokabidea koherentea da proiektuarekin edo proiekturik gabe argitaratutako gastu lerroetan.  
