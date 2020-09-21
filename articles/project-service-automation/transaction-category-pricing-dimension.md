---
title: Erabili transakzioen kategoria prezio-dimentsio gisa
description: Gai honek transakzioen kategoria prezio-dimentsio gisa erabiltzeari buruzko informazioa eskaintzen du.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/19/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: 64b81ca7-e2db-4e4a-a202-aae0eb235ffd
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: a36e0578b8d77a0ed1ea61134453aa064771760f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748935"
---
# <a name="use-transaction-category-as-a-pricing-dimension"></a>Erabili transakzioen kategoria prezio-dimentsio gisa
Gai honek transakzioen kategoria prezio-dimentsio gisa erabiltzeko moduari buruzko informazioa eskaintzen du. Hasi aurretik, prezio-dimentsioaren soluzioa sortu ez baduzu, bat sortu beharko duzu. Prezioen dimentsioko irtenbidea baduzu, orduan aldaketak egin ditzakezu soluzio horretan. Zure erakunderako prezio-dimentsio soluzio berririk sortu ez baduzu, jarraitu [Sortu eremu eta entitate pertsonalizatuak](create-custom-fields-entities.md) gaian azaldutako prozedurei.

## <a name="add-transaction-category-to-forms-and-views"></a>Gehitu transakzioen kategoria inprimakietan eta ikuspegietan
Trantsakzio-kategoria prezio-dimentsioaren soluzioko IU-an ikusgai jartzeko, entitatearen inprimaki eta ikuspegi guztiak ikusi beharko dituzu eta eremu horiek entitate horien inprimakietan eta ikuspegietan gehitu beharko dituzu.
Hurrengo taula erabiltzeko prest dauden inprimakien eta ikuspegien zerrenda zabala da, entitateen arabera zerrendatua, eta eremu berriekin eguneratu beharko da. Entitate horien pertsonalizazioetan ikuspegi edo inprimaki gehigarririk baldin badago, gehitu eremu berriak horietan ere.

|  Entitatea        | Inprimakiak     |Ikuspegiak        |
| ------------------------------|---------------------------------|----------------------------------|
|  Funtzioaren prezioa|• Informazioa |• Baliabide-kategorien prezio aktiboak<br> • Baliabide-kategorien prezioekin erlazionatutako ikuspegia|
|  Funtzio-prezioaren gainprezioa|• Informazioa|• Funtzio-prezioaren gainprezio aktiboa<br>• Funtzio-prezioaren gainprezioarekin erlazionatutako ikuspegia|
|  Eskaintzaren lerroaren xehetasunak|• Proiektuari buruzko informazioa<br>• Sorrera bizkorreko proiektua|• Eskaintzaren lerroaren xehetasun aktiboak<br>• Konbinatutako eskaintzaren lerroen xehetasunak<br>• Eskaintzaren lerroen xehetasunekin erlazionatutako ikuspegia|
|  Proiektu-kontratuaren lerroaren xehetasunak|• Proiektuari buruzko informazioa<br>• Sorrera bizkorreko proiektua|• Kontratuaren lerroaren xehetasun konbinatuak<br>• Kontratuaren lerroaren xehetasun aktiboak<br>• Kontratuaren lerroen xehetasunekin erlazionatutako ikuspegia|
|  Proiektu-taldeko kidea|• Informazioa<br>• Inprimaki berria|• Proiektu-taldeko kide aktiboak<br>• Proiektu-taldeko kideak<br>• Proiektu-taldeko kideekin erlazionatutako ikuspegia|
|  Denbora-sarrera|• Informazioa<br>• Sortu denbora-sarrera|• Nire denbora-sarrerak dataren arabera<br>• Aste honetako nire denbora-sarrerak<br>• Onartu beharreko denbora-sarrerak|
|  Kutxako liburuaren lerroa|• Informazioa<br>• Sorrera bizkorra|• Kutxako liburuaren lerro aktiboak<br>• Kutxako liburuaren lerroekin erlazionatutako ikuspegia|
|  Fakturaren lerroaren xehetasunak|• Informazioa<br>• Sorrera bizkorra|• Fakturaren lerroen xehetasun aktiboak<br>• Kobra daitezkeen fakturen transakzioak<br>• Doako fakturen transakzioak<br>• Fakturaren lerroen xehetasunekin erlazionatutako ikuspegia<br>• Kobra ezin daitezkeen fakturaren transakzioak|
|  Benetakoa|• Informazioa<br>• Benetako datu aktiboak|• Benetako datuen ikuspegia|

## <a name="set-up-transaction-category-as-a-pricing-dimension"></a>Konfiguratu transakzioen kategoria prezio-dimentsio gisa

1. Web interfazean, joan **Project Service** > **Ezarpenak** > **Parametroak** atalera. 
2. **Parametroak** orrialdean, **Zenbatekoan oinarritutako prezio-dimentsioak** fitxan, ohartu fitxan agertzen den saretak **Prezio-dimentsioak** entitateko erregistroak erakusten dituela.
3. Gehitu **Transakzioen kategoria** zerrenda honetara eta ezarri **Kostuari aplikagarria** eta **Salmentari aplikagarria** eremuak **Bai** gisa.
4. **Dimentsio mota** eremuan, hautatu **Zenbatekoan oinarrituta** eta, ondoren, hautatu **Transakzioen kategoria** aukerarekin erlazionatutako kostu eta salmentetarako lehentasuna.
