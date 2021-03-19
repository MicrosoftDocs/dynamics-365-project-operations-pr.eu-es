---
title: Erabili Transakzioen kategoria prezio-dimentsio gisa
description: Gai honek Transakzioen kategoria eremua prezio-dimentsio gisa erabiltzeari buruzko informazioa eskaintzen du.
author: rumant
manager: tfehr
ms.date: 11/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: c84d3aaf7cd7577dcd15311f225c82b538586445
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274578"
---
# <a name="use-transaction-category-as-a-pricing-dimension"></a>Erabili Transakzioen kategoria prezio-dimentsio gisa


_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_


Gai honek **Transakzioen kategoria** eremua prezio-dimentsio gisa erabiltzeko modua azaltzen du. 

## <a name="prerequisites"></a>Aurrebaldintzak
Gai honetako prozedurak amaitu aurretik, prezioen dimentsio irtenbide berri bat izan behar duzu zure erakundearentzat. Oraindik sortu ez baduzu, ikusi [Sortu eremu eta entitate pertsonalizatuak prezioen dimentsio gisa](create-custom-fields-entities-pricing-dimensions.md).

## <a name="add-the-transaction-category-field-to-forms-and-views"></a>Gehitu Transakzioen kategoria eremua inprimakietan eta ikuspegietan
**Transakzioen kategoria** eremua prezioen dimentsioaren irtenbidean ikusgai egiteko, eremua entitate gisa forma eta ikuspegi guztietara gehitu behar duzu.

Hurrengo taulan kutxaz kanpoko forma eta ikuspegi guztiak zerrendatzen dira, entitatearen arabera. Eremu berria gehitu beharko duzu pertsonalizatutako entitateetako inprimaki edo ikuspegi osagarrietara.

|  Entity        | Inprimakiak     |Ikuspegiak        |
| ------------------------------|---------------------------------|----------------------------------|
|  Funtzioaren prezioa| Informazioa |- Baliabide-kategorien prezio aktiboak<br> - Baliabide-kategorien prezioekin erlazionatuta |
|  Funtzio-prezioaren gainprezioa| Informazioa|- Funtzio-prezioaren gainprezio aktiboa<br>- Funtzio-prezioaren gainprezioarekin erlazionatuta |
|  Eskaintzaren lerroaren xehetasunak|- Proiektuari buruzko informazioa<br>- Sorrera bizkorreko proiektua| - Eskaintzaren lerroaren xehetasun aktiboak<br>- Konbinatutako eskaintzaren lerroen xehetasunak<br>- Eskaintzaren lerroen xehetasunekin erlazionatuta |
|  Proiektu-kontratuaren lerroko xehetasunak|- Proiektuari buruzko informazioa<br>- Sorrera bizkorreko proiektua|- Kontratuaren lerroaren xehetasun konbinatuak<br>- Kontratuaren lerroaren xehetasun aktiboak<br>- Kontratuaren lerroen xehetasunekin erlazionatuta |
|  Proiektuaren zeregina|- Informazioa<br>- Inprimaki berria| &nbsp; |
|  Proiektu-taldeko kidea|- Informazioa<br>- Inprimaki berria|- Proiektu-taldeko kide aktiboak<br>- Proiektuaren taldeko kideak<br>- Proiektu-taldeko kideekin erlazionatuta |
|  Denbora-sarrera|- Informazioa<br>- Sortu denbora-sarrera|- Nire denbora-sarrerak, dataren arabera<br>- Aste honetako nire denbora-sarrerak<br>- Onartu beharreko denbora-sarrerak|
|  Kutxako liburuaren lerroa|- Informazioa<br>- Sorrera bizkorra|- Kutxako liburuaren lerro aktiboak<br>- Kutxako liburuaren lerroekin erlazionatuta|
|  Fakturaren lerroaren xehetasunak|- Informazioa<br>- Sorrera bizkorra|- Fakturaren lerroen xehetasun aktiboak<br>- Kobra daitezkeen fakturen transakzioak<br>- Doako fakturen transakzioak<br>- Fakturaren lerroen xehetasunekin erlazionatuta <br>- Kobra ezin daitezkeen fakturaren transakzioak|
|  Unekoa"|- Informazioa<br>- Benetako datu aktiboak| Benetako datuekin erlazionatuta |

## <a name="set-up-the-transaction-category-field-as-a-pricing-dimension"></a>Konfiguratu Transakzioen kategoria eremua prezio-dimentsio gisa

1. Joan **Ezarpenak** > **Parametroak** atalera. 
2. **Parametroak** orrialdean, **Zenbatekoan oinarritutako prezio-dimentsioak** fitxan, egiaztatu agertzen den saretak **Prezio-dimentsioak** entitateko erregistroak erakusten dituela.
3. Gehitu **Transakzioen kategoria** zerrenda honetara eta ezarri **Kostuari aplikagarria** eta **Salmentari aplikagarria** eremuak **Bai** gisa.
4. **Dimentsio mota** eremuan, hautatu **Zenbatekoan oinarrituta** eta, ondoren, hautatu **Transakzioen kategoria** aukerarekin erlazionatutako kostu eta salmentetarako lehentasuna.


[!INCLUDE[footer-include](../includes/footer-banner.md)]