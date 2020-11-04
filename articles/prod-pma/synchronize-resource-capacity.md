---
title: Sinkronizatu baliabideen gaitasuna
description: Gai honetan baliabidearen ahalmena egutegiekin eta proiektuekin sinkronizatzeko moduari buruzko informazioa eskaintzen da.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 006ebbfea42572f17663fab324a20a10321b78f0
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071014"
---
# <a name="synchronize-resource-capacity"></a>Sinkronizatu baliabideen gaitasuna

[!include [banner](../includes/banner.md)]

Baliabideak sinkronizatzeko prozesuei esker, egutegiaren eta oinarrizko egutegiaren informazioa proiektuaren baliabideen programazioan sartzen da. Egutegia aldatzen bada, prozesuek beharrezko eguneratzeak egiten dituzte proiektuaren baliabideen programazioan. Prozesuek errendimendua hobetzen ere laguntzen dute, egutegiaren baliabideen informazioa aldez aurretik sinkronizatuta dagoelako. Hori dela eta, baliabideak antolatzeko informazioaren eguneratzeak azkarrago gertatzen dira. Prozesuak multzo gisa antolatzea gomendatzen dizugu, aldi berean ordez. Bestela, norbaitek informazioa azkeneko aldiz sinkronizatu zeneko egun biak barne ahazteko arriskua dago. Data inklusiboak erabiltzen ez badira, hutsuneak gerta daitezke data sinkronizatzean.

![Egutegiaren sinkronizazioa](./media/projectresourcing04-1024x471.jpg)

## <a name="synchronize-resource-capacity-roll-ups"></a>Sinkronizatu baliabide-gaitasuna bateratzea

Sinkronizazio prozesua baliabideen egutegiko informazio guztia sinkronizatzeko diseinatuta dago. Informazio honek proiektuaren Baliabideen egutegiaren edukiera taulan egindako aldaketen inguruko oinarrizko egutegiko informazioa biltzen du. Proiektuan baliabide berriak gehitzen badira, sinkronizazioak eguneratutako egutegiko informazioa eskuragarri dagoela bermatzen laguntzen du. Sinkronizazio hau edozein unetan egin daiteke.

Gomendatzen dizugu erabiltzea sorta gisa. Aukerak eskuragarri daude edukiera erreserbak sinkronizatzean.

1. Aukeratu **Proiektuen kudeaketa eta kontabilitatea** &gt; **Aldizkakoa** &gt; **Edukiera sinkronizatzea** &gt; **Sinkronizatu baliabideen ahalmenak**.
2. Ezarri aukerak ondoko taulan bistaratzen dira.

    | Aukera      | Deskribapenak |
    |-------------|-------------|
    | Garai kodea | Aukeran hautatu Liburu nagusiaren data tarte kodea, baliabideen edukiera biltzeko sinkronizazio prozesuaren hasiera eta amaiera datak ezartzeko. |
    | Hasiera-data  | Idatzi baliabideen edukiera biltzeko prozesuen sinkronizazio prozesuaren hasiera data. |
    | Amaiera-data    | Idatzi baliabideen edukiera biltzeko prozesuen sinkronizazio prozesuaren amaiera data. |

[![Sinkronizazio-prozesua](./media/projectresourcing09.jpg)](./media/projectresourcing09.jpg)
