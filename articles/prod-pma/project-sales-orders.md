---
title: Proiektuen denbora eta material proiektuen salmenta aginduak
description: Gai honetan proiektuetan oinarritutako salmenta aginduak nola sortu azaltzen da denbora eta proiektu materialetarako.
author: Yowelle
manager: AnnBe
ms.date: 04/05/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2019-04-05
ms.dyn365.ops.version: AX 10.0.2
ms.openlocfilehash: 3653a6869dab323be88f1fd0f9fd0f2cb35c456f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071021"
---
# <a name="project-sales-orders-for-time-and-material-projects"></a>Proiektuen denbora eta material proiektuen salmenta aginduak

[!include[banner](../includes/banner.md)]

Gai honetan proiektu baten salmenta eskaera nola sortu azaltzen da. Salmenta aginduak motako proiektuetarako bakarrik sor daitezke **denbora eta materiala**.

Denbora eta material proiektu batek proiektuaren kontratuan finantzaketa iturri ugari baditu, gaitu behar duzu **Baimendu diru iturri anitz dituzten proiektuen salmenta aginduak** parametroa **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea. 

> [!NOTE]
> - Finantzaketa iturri anitz dituzten proiektuen salmenta eskaerei buruzko laguntza eskuragarri dago 10.0.2 aplikazioaren bertsio berritik hasita.
> - Finantzaketa iturri anitz dituzten proiektuen salmenta aginduen laguntza gaitzeko parametroa kenduko da 2020ko apirileko bertsio uhinean, eta ondoren funtzionaltasuna beti gaituko da.

Proiektuetan oinarritutako salmenta aginduak bi modutan sor ditzakezu:

- Joan proiektura bertara. Ekintza panelean, hautatu **Kudeatu > Elementuen zereginak > Salmenta agindua**. Proiektuaren informazioa proiektuaren salmenta eskaera lehenetsiko da. Proiektuaren kontratuak finantzaketa iturri bat baino gehiago baditu, finantzaketa iturria hautatu beharko duzu bezeroa salmenta eskaerarako ezartzeko. Proiektua finantzatzeko iturri bakarra baldin badago, bezeroa automatikoki konfiguratuko da.
- Joan **Salmenta eskaera guztiak** zerrendaren orria eta salmenta eskaera berria sortu. Salmenta eskaeraren proiektua hautatu beharko duzu. Proiektua hautatu ondoren, bezeroa finantziazio iturritik ezarriko da edo finantzaketa iturria hautatu beharko duzu proiektuaren kontratuak finantzazio iturri anitz baditu.
