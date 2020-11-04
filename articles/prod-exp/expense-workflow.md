---
title: Gastuen kudeaketaren lan-fluxua
description: Gai honek lan fluxuaren sistema nola erabil dezakezun azaltzen du Microsoft Dynamics 365 Finance, Gastuen kudeaketan gastuen txostenak berrikusteko prozesua ezartzeko.
author: ShylaThompson
manager: AnnBe
ms.date: 09/13/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: WorkflowtableListPageRnr
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 5207be92cb58d8ab2658096b3e0f3fc81d73d91e
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071191"
---
# <a name="expense-management-workflow"></a>Gastuen kudeaketaren lan-fluxua

[!include [banner](../includes/banner.md)]

Fluxuaren sistema erabil dezakezu, Gastuen kudeaketan gastuen txostenak berrikusteko prozesua ezartzeko. Gastu txostenak nork onartzen dituen zehazteko irizpide hauek erabiltzen dituen lan fluxua konfigura dezakezu:

- Langilearen berri emateko hierarkia eta aurrez definitutako onarpen mugak
- Behin-behineko onartzaileak eta behin betiko onartzailea onartzen dituen maila anitzeko onespena
- Finantza dimentsioak eta proiektuaren erantzukizuna
- Erabiltzaile edo erabiltzaile talde jakin batzuei esleitzea

Lan-fluxuen onarpenak sor daitezke gastuen txostenak, bidaia-eskaerak, dirua aurreratzeko eta balio erantsiaren gaineko zergaren (BEZ) berreskurapenetarako.

**Adibidez**

Hurrengo prozesua gastu-txosten baten kudeaketa-fluxuaren adibidea da.

1. Langile batek gastuen txostena sortu eta gordetzen du.
2. Langilearen gastuen txostena bidaltzen du onartzeko. Onartzailea lan-fluxua konfiguratu zenean definitutako arauetan oinarrituta identifikatzen da.
3. Onartzaileak gastuen txostena onartzeko prest dagoela jakinarazten dio. Onartzaileak gastuen txostena aztertzen du eta baldintza hauek betetzen direla egiaztatzen du:

    - Gastuek ez dute inolako gastu politikarik urratzen. Gastu batek politika bat urratzen badu, onartzaileak egiaztatzen du gastuen txostenak baliozko negozio justifikazioa duela.
    - Ordainagiri elektronikoak gastuen txostenari eransten zaizkio.

4. Onesleak gastuen txostena onartzen du.
5. Gastuen txostena Kobratu beharreko kontuen koordinatzaileari esleitzen zaio argitaratzeagatik.
6. Urrats hauetako bat gertatzen da, argitaratze automatikoa konfiguratuta dagoen ala ez kontuan hartuta:

    - Bidalketa automatikoa konfiguratzen bada, gastuen txostena ordaintzeko prozesatuko da eta gastuen txostenaren egoera eguneratuko da.
    - Bidalketa automatikoa konfiguratuta ez badago, ordaindu beharreko Kontuen koordinatzaileak egiaztatzen du jatorrizko ordainagiri guztiak aurkeztu direla eta ordainagiriak gastuen txosteneko gastuekin bat datozela. Gastu txostenean sartutako zerga kode guztiak zuzenak direla ere egiaztatu behar da.

Baldintza horiek egiaztatu ondoren, gastuen txostena argitaratuko da.

Gastuen txostena argitaratu ondoren, gastuen txostena ordaintzeko baimena ematen da eta langileari itzulketa egiten zaio.
