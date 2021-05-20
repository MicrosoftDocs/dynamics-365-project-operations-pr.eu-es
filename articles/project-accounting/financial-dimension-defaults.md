---
title: Finantza-dimentsio lehenetsiak
description: Gai honek dimentsio finantzarioaren lehenespenak konfiguratzeko moduari buruzko informazioa eskaintzen du.
author: sigitac
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 0a76447bb1a81a7157fccc0cd58eddd1eb5995de
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/27/2021
ms.locfileid: "5950114"
---
# <a name="financial-dimension-defaults"></a>Finantza-dimentsio lehenetsiak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Dynamics 365 Project Operations-ek erabiltzen du [Finantza-dimentsioak](/dynamics365/finance/general-ledger/financial-dimensions) esparrua Dynamics 365 Finance proiektu gehigarrien eta liburu nagusien transakzioen inguruko informazio osagarria eskaintzeko.

Finantza dimentsio lehenetsiak bezero, proiektuaren finantzaketa iturri, mugarri, proiektu kontratu lerro edo proiektu batean ezar daitezke.

## <a name="define-default-financial-dimensions-for-a-customer"></a>Definitu bezeroarentzako lehenetsitako finantza dimentsioak

Bezeroen dimentsio lehenetsiak Finantzan zehazten dira. Osatu urrats hauek dimentsioaren balio lehenetsiak ezartzeko.

1. Joan **Kobratu beharreko kontuak** > **Bezeroak** > **Bezero guztiak**.
2. **Bezeroak** orrialdean, **Finantza dimentsioak** fitxa, ezarri bezero zehatzentzako finantza dimentsioaren balioak.

## <a name="define-default-financial-dimensions-for-project-contracts"></a>Definitu proiektu-kontratuen lehenetsitako finantza dimentsioak

Proiektuen kontratuak urtean sortu eta mantentzen dira Common Data Service (CDS). Proiektuen kontratuen kontabilitate atributuak **Proiektuen kudeaketa eta kontabilitatea** modulua Finantzetan.

### <a name="set-financial-dimensions-for-a-project-funding-source"></a>Ezarri proiektuaren finantzaketa iturriaren dimentsio ekonomikoak

1. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuak** > **Proiektu-kontratuak**.
2. Hautatu eguneratu nahi duzun erregistroa eta **Proiektuaren kontratua** fitxa, hautatu **Erakutsi lehenetsitako kontabilitatea**.
3. Zabaldu **Lotutako informazioa** eta hautatu **Finantzaketa iturriak** fitxa.
4. Ezarri finantza-dimentsio lehenetsiak. Kontuan izan finantza dimentsioak bezeroaren kontutik lehenetsita daudela.

### <a name="set-financial-dimensions-for-a-project-contract-line"></a>Ezarri proiektuaren kontratuaren lerroaren dimentsio ekonomikoak

1. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuak** > **Proiektu-kontratuak**.
2. Hautatu eguneratu nahi duzun erregistroa eta **Proiektuaren kontratua** fitxa, hautatu **Erakutsi lehenetsitako kontabilitatea**.
3. Zabaldu **Lotutako informazioa** eta hautatu **Kontratuaren lerroak** fitxa.
4. Ezarri finantza-dimentsio lehenetsiak. Finantza dimentsioaren lehenespenak aplikagarriak dira eta prezio finkoaren (mugarria) kontratu lerroekin bakarrik erabil daitezke.

Lehenespen horiek erlazionatutako proiektuaren kontuko transakzioetan eta faktura lerroetan erabiltzen dira.

## <a name="define-default-financial-dimensions-for-projects"></a>Definitu proiektuen lehenetsitako finantza dimentsioak

Proiektuak CDS-n sortu eta mantentzen dira. Proiektuen kontabilitate atributuak **Proiektuen kudeaketa eta kontabilitatea** modulua Finantzetan.

1. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuak** > **Proiektu guztiak**.
2. Hautatu eguneratu nahi duzun erregistroa eta **Proiektua** fitxa, hautatu **Erakutsi lehenetsitako kontabilitatea**.
3. Zabaldu **Lotutako informazioa** eta hautatu **Konfiguratu** fitxa.
4. Ezarri finantza-dimentsio lehenetsiak. Kontuan izan finantza dimentsioak bezeroaren kontutik lehenetsita daudela. Proiektua proiektu kontratuko bezero anitzekin kontratu lerro batekin lotzen bada, bezero nagusia lehenetsitako finantza dimentsioetarako erabiltzen da.

Proiektuaren lehenetsitako finantza dimentsioak egunkariaren lerroaren lehenespenak ezartzeko erabiltzen dira denbora, gastu eta kuoten transakzioetarako **Project Operations Integration Journal** eta lotutako proiektuen faktura-lerroetan.


[!INCLUDE[footer-include](../includes/footer-banner.md)]