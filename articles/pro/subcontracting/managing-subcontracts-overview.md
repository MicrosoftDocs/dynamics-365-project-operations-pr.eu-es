---
title: Azpikontratuen kudeaketa Project Operations-en
description: Gai honek amaierako azpikontrata kudeatzeko prozesuaren ikuspegi orokorra eskaintzen du Microsoft Dynamics 365 Project Operations-en.
author: rumant
ms.date: 08/02/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 6ffceb0886fdc841ea01a099243cf4eeb43e5374a18414576f3639a3e50857fd
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6994216"
---
# <a name="subcontract-management-in-project-operations"></a>Azpikontratuen kudeaketa Project Operations-en

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

azpikontratazioa Microsoft Dynamics 365 Project Operations onartzen du honako negozio-prozesuaren fluxu.

![Azpikontratazio prozesuaren fluxua](../media/SubcontractingProcessFlow.png)

Hona hemen azpikontratazio prozesuaren urratsez urrats deskribapena.

1. Proiektuaren kudeatzaileak azpikontrata sortzen du saltzaile batekin. Berez, saltzailearen erregistroari atxikitako prezioen zerrendak azpikontratatzeko erabiltzen dira. Saltzailearen kontuak **Saltzailea** edo **Hornitzailea** motako erlazioa du.
2. Proiektuaren zuzendariak erosketa guztiak azpikontratako lineako elementu gisa sailka ditzake. Azpikontratazio lineak denbora, gastu edo produktuetarako izan daitezke. Azpikontratazio lerro bakoitzean hautatzen den transakzio klaseak zehazten du zertarako den linea.
3. Saltzailearen kontu kudeatzaileak eta proiektuaren kudeatzaileak azpikontrataren bidez errepika dezakete. Prezioa doi dezakezu azpikontratuan esleitu diren erosketaren prezio-zerrendetan.
4. Prozesuaren une honetan edo geroago, azpikontratazio lerroa denbora bada, saltzailearen kontu kudeatzaileak azpikontratazio lerro bakoitzarekin kontaktuak lotzen ditu. Elkarte honek informazioa ematen dio azpikontratuan lanean ari den proiektuaren zuzendariari. Kontaktu bat azpikontratazio lerro batekin lotzen denean, sistemak automatikoki erreserbatzeko baliabide bat sortzen du kontaktuarekin, erreserbatzeko baliabide bat existitzen ez bada.
5. Azpikontratazio lerro bakoitzeko fakturazio metodoa izan daiteke **Prezio finkoa** edo **Denbora eta materiala**. Prezio finkoaren azpikontratazio lerroetan, mugarrietan oinarritutako fakturen egutegia konfigura dezakezu.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
