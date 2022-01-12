---
title: Azpikontratatutako osagaien denbora, gastuak eta materialaren erabilera erregistratzea
description: Gai honek Microsoft-ek azpikontratatutako osagaietatik proiektuetan erregistratutako denbora, gastu eta materialaren erabileraren jarraipena nola egiten duen azaltzen du Dynamics 365 Project Operations.
author: rumant
ms.date: 12/03/2021
ms.topic: article
ms.reviewer: tonyafehr
ms.author: rumant
ms.openlocfilehash: 04c78dd48367c3720b8f5ad5d924ed106da6a128
ms.sourcegitcommit: 45893132bd8bfaf944ee0ac855484684dd1ee945
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/09/2021
ms.locfileid: "7902982"
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
Proiektuetan materialaren erabilera sartzean, materialaren erabileraren erregistroan azpikontratu eta azpikontratazio lerro bat hauta ditzakezu. Materialaren erabileraren erregistroa aurkeztu eta onartzen denean, materialaren kostua proiektuan erregistratzen da produktu horretarako ezartzen den unitateko kostuaren arabera.**Prezio zerrendako elementuak** azpikontratuaren prezioen zerrendaren atala.

Materialaren erabilera proiektuetan idazteko produktuetarako ere erregistra daiteke. Material-erabilera mota hau azpikontratazio eta azpikontratazio lerro batekin ere lotu daiteke. Idazteko produktuen materialaren erabilera erregistratzean, idazteko produktuaren unitateko kostua sartu behar duzu. 


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
