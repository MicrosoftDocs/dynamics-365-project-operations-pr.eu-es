---
title: Proiektuaren eskaintak aztertzea
description: Gai honek proiektuaren eskaintzak aztertzeari buruzko informazioa ematen du.
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: acb3f1a2020cfd59f60f828e9092bd7ccde00077
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012436"
---
# <a name="analysis-of-project-quotes"></a>Proiektuaren eskaintak aztertzea

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Dynamics 365 Project Service Automation-ek errentagarritasuna balioesteko proiektuaren eskaintzak aztertzen ditu. Eskaintza bezeroaren itxaropenekin nola lotzen den aztertzen da, entrega-data edo bukaera-data eta aurrekontuei buruzkoak.

## <a name="profitability-analysis"></a>Errentagarritasun-analisia

Project Service Automation-ek errentagarritasuna aztertzen du marjina gordina eta doitutako marjina gordina erabiliz.

- Marjina gordina formula hau erabiliz kalkulatzen da:

  `
    (Sum of estimated chargeable sales value – Sum of estimated chargeable costs) x 100
  `
- Doitutako marjina gordina formula hau erabiliz kalkulatzen da:

  `
    (Sum of estimated chargeable sales value – Sum of all estimated costs) x 100
  `

Marjina gordinaren eta doitutako marjina gordinaren balioak marjina zabalan desberdinak badira, eskaintzako lanaren zatirik handiena kargagabea delako.

## <a name="analysis-of-customer-expectations"></a>Bezeroak espero duenaren analisia

Eskaintzak aztertu eta diagramak sor ditzakezu bezeroen itxaropenen arabera, antolaketari eta aurrekontuei dagokienez, eremu hauek lortzeko balioak sartzen badituzu:

- **Eskatutako entrega-data** eremua eskaintzaren goiburuan.
- **Bezeroaren aurrekontua** eremua eskaintzaren lerro bakoitzeko (proiektuan oinarritutako lerroetarako eta produktuetan oinarritutako lerroetarako).

Antolaketaren inguruko bezeroen itxaropenen analisia eskaintzaren lerroaren azken dataren eskaintza aldez aurretik eskatutako entrega-datarekin alderatuz egiten da eskaintzaren lerro guztietan.

Bezeroaren aurrekontuen itxaropenaren analisia bezeroaren aurrekontuaren guztizko zenbatekoa eskaintzaren lerroarekin konparatuz egiten da.


[!INCLUDE[footer-include](../includes/footer-banner.md)]