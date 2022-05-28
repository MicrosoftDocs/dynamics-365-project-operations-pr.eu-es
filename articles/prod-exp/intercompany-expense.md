---
title: Enpresen arteko gastuak
description: Gai honetan enpresen arteko gastuak langilearen gastuak lana burutu den entitate juridikoari esleitzeko moduari buruzko informazioa ematen da.
author: suvaidya
ms.date: 07/08/2021
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: TrvParameters
audience: Application User
ms.reviewer: johnmichalak
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 6788a590879bd839ebb9dedc45895dc047cc9f15
ms.sourcegitcommit: 2c2a5a11d446adec2f21030ab77a053d7e2da28e
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/04/2022
ms.locfileid: "8684214"
---
# <a name="intercompany-expenses"></a>Enpresen arteko gastuak

Erakunde bateko pertsona juridiko batek lan egiten duen langileak erakunde bereko beste pertsona juridiko baterako lana egin dezake. Enpresen arteko gastuak langilearen gastuak lana burutu den entitate juridikoari esleitzeko erabil dezakezu. Langilea enplegatzen duen pertsona juridikoari mailegu-pertsona deitzen zaio. Langileak gastuak egiten dituen pertsona juridikoari mailegu-pertsona deitzen zaio. 

Langile batek enpresen arteko gastuak sortu eta bidali aurretik, enpresen arteko gastuen lerroak gaitu behar dituzu. Pertsona juridiko mailegatzailean **Gastuak kudeatzeko parametroak** orrialdea, hautatu **Onartu enpresen arteko gastu lerroak**. 

## <a name="tax-posting-for-intercompany-expenses"></a>Enpresen arteko gastuen zerga argitaratzea

[!include [banner](../includes/banner.md)]

Mailegu (iturburu) erakunde juridikoarekin lotutako mailegu (destino) entitate juridikoarekin lotutako zerga taldeak erabili aurretik, zure gastuaren txostenean, funtzionalitatea gaitu behar duzu liburu nagusien salmenten gaineko zergaren konfigurazioan. **Enpresen arteko zergak argitaratzeko pertsona juridikoa** parametroa ezarrita dagoenean **Iturria** eta **Salmenten gaineko zergaren gaineko zerga arauak aplikatzea** ezarrita dago **Ez**, mailegu-entitate juridikoaren zerga-konbinazioa erabiltzen da. Parametro bera ezarrita dagoenean **Helmuga**, zorpetutako entitate juridikoaren zerga-konbinazioa erabiliko da. Estatu Batuetako pertsona juridikoetarako, parametroa ezarrita dagoenean **Iturria**, **Kobratu beharreko salmenten gaineko zerga** eremua berrian konfiguratu behar da **Liburuak argitaratzeko taldeak** orrialdea. Kontabilitate motorrak eremu honetako informazioa erabiliko du zergekin lotutako kontabilitate sarrera egiteko.   
Jokabidea koherentea da proiektuarekin edo proiekturik gabe argitaratutako gastu lerroetan.  

## <a name="new-expense-expression-builder"></a>Gastu adierazpenen eraikitzaile berria

Gastu adierazpenen eraikitzaile berriak proiektuak erabiltzen dituzten enpresen arteko gastu eszenatokiekin arazoak jorratzen ditu. Ezaugarri honi esker, enpresen arteko gastua sortzen duzunean, gastu-politika gastu-lerroan hautatutako proiektuaren aurka behar bezala balioztatzen dela eta gastuen txostena ongi bidal daitekeela ziurtatzen da.

Gastuen adierazpenen eraikitzailearen funtzioak funtziona dezan, aktibatuta egon behar da. Gainera, proiektuaren IDa duen gastu politika ezarri beharko litzateke.

Gastuaren lerroan proiektuaren IDa balioztatzen duten politikak konfiguratu badituzu, politika horiek erretiratu egin beharko dira. Eginbidea aktibatu eta gidalerroak berriro konfigura ditzakezu.

Eginbide hau aktibatzeko, jarraitu ondorengo urratsak.

1. Joan **Laneko areak** \> **Eginbideen kudeaketa** atalera.
2. Zerrendan, hautatu **Gastu adierazpenen eraikitzaile berriak proiektuak erabiltzen dituzten enpresen arteko gastu eszenatokiekin arazoak jorratzen ditu**. Ondoren hautatu **Gaitu orain**.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
