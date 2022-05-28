---
title: Azpikontratatutako osagaien denbora, gastuak eta materialaren erabilera erregistratzea
description: Gai honek Microsoft-ek azpikontratatutako osagaietatik proiektuetan erregistratutako denbora, gastu eta materialaren erabileraren jarraipena nola egiten duen azaltzen du Dynamics 365 Project Operations.
author: rumant
ms.date: 12/03/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 5a31b4a1092cc4829cbfc789e8b8e30030b2826b
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8599209"
---
# <a name="recording-time-expenses-and-material-usage-on-projects-for-subcontracted-components"></a>Azpikontratatutako osagaien proiektuetan denbora, gastuak eta materialaren erabilera erregistratzea

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Gai honek Microsoft-ek azpikontratatutako osagaietatik proiektuetan erregistratutako denbora, gastu eta materialaren erabileraren jarraipena nola egiten duen azaltzen du Dynamics 365 Project Operations.

## <a name="costing-for-subcontractor-time-on-projects"></a>Proiektuetan azpikontratistaren denboraren kostua
Proiektuen Eragiketetan, lan-kontratuko langileek proiektuetan denbora graba dezakete langileen antzera. Proiektuetan edo/eta proiektuko zereginetan denbora sartzerakoan, kontratu-langile batek azpikontratu eta azpikontratu lerro zehatz bat hauta dezake.

Lan-kontratuko langileek aurkeztutako denbora onartzen denean, proiektuaren kostua erregistratzen da lan-kontratuko langile-baliabide horretarako ezarritako kostu unitarioaren tasa erabiliz.**Rolen prezioak** azpikontratuko erosketa prezioen zerrendaren atala.

## <a name="costing-for-subcontracted-expenses-on-projects"></a>Proiektuetan azpikontratatutako gastuen kostua
Proiektuetan sortutako gastuak sartzerakoan, azpikontratazioa eta azpikontratazio lerroa hauta ditzakezu gastuen sarreran. 

Gastuen idazpen hau aurkeztu eta onartzen denean, gastu-kostua proiektuan erregistratzen da transakzio-kategoria horretarako ezartzen den kostu unitarioaren arabera.**Kategorien prezioak** azpikontratuko erosketa prezioen zerrendaren atala.

## <a name="costing-for-subcontracted-materials-on-projects"></a>Proiektuetan azpikontratatutako materialen kostuak
Proiektuetan materialaren erabilera sartzerakoan, materialaren erabileraren erregistroan azpikontratu eta azpikontratu lerro bat hauta ditzakezu. Materialaren erabileraren erregistroa aurkeztu eta onartzen denean, materialaren kostua proiektuan erregistratzen da produktu horretarako ezartzen den unitateko kostuaren arabera.**Prezio zerrendako elementuak** azpikontratuaren prezioen zerrendaren atala.

Materialaren erabilera proiektuetan idazteko produktuetarako ere erregistra daiteke. Material-erabilera mota hau azpikontratazio eta azpikontratazio lerro batekin ere lotu daiteke. Idazteko produktuen materialaren erabilera erregistratzean, idazteko produktuaren unitateko kostua sartu behar duzu. 


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
