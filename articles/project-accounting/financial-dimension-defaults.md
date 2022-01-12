---
title: Finantza-dimentsio lehenetsiak
description: Gai honek dimentsio finantzarioaren lehenespenak konfiguratzeko moduari buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 12/14/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 8c1eb71d13ca7fc59118d15fef7ac914577b3b0e
ms.sourcegitcommit: fe5610464fdb5be756aa6a6a5b3c9a991dea0ed8
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/15/2021
ms.locfileid: "7922923"
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

## <a name="apply-financial-dimensions-for-project-time-entries"></a>Aplikatu finantza-dimentsioak proiektuaren denbora sarreretarako
Proiektuaren denbora-sarreretarako finantza-dimentsioak aplikatzeko, kontuan izan dimentsio-balio lehenetsia hurrengo ordenan oinarritzen dela:

1. Baliabidea
2. Project
3. Finantzaketa iturria

Adibidez, baliabide batean dimentsio lehenetsia zehazten bada, proiektuan zehaztutako lehenetsi baten gainean aplikatuko da. Era berean, proiektuaren dimentsio lehenetsi bat aplikatuko da finantzaketa iturrian zehaztutako lehenetsiaren gainean.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
