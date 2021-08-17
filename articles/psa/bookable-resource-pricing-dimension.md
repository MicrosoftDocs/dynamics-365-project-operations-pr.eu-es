---
title: Erabili baliabide erreserbagarriak prezio-dimentsio gisa
description: Gai honek baliabide erreserbagarriak prezio-dimentsio gisa erabiltzeari buruzko informazioa eskaintzen du.
author: Rumant
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: c551673708ae2d965979136e92326be98252304a601964c1fbc52a329c592712
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6988951"
---
# <a name="use-bookable-resource-as-a-pricing-dimension"></a>Erabili baliabide erreserbagarriak prezio-dimentsio gisa

[!include [banner](../includes/psa-now-project-operations.md)]

Gai honek baliabide erreserbagarriak prezio-dimentsio gisa erabiltzeari buruzko informazioa eskaintzen du. Hasi aurretik, prezio-dimentsioaren soluzioa sortu ez baduzu, bat sortu beharko duzu. Prezioen dimentsioko irtenbidea baduzu, orduan aldaketak egin ditzakezu soluzio horretan. Zure erakunderako prezio-dimentsio soluzio berririk sortu ez baduzu, jarraitu [Sortu eremu eta entitate pertsonalizatuak](create-custom-fields-entities.md) gaian azaldutako prozedurei.

## <a name="add-bookable-resource-to-forms-and-views"></a>Gehitu baliabide erreserbagarriak inprimakietan eta ikuspegietan
Eremuak prezio-dimentsioaren soluzioko IU-an ikusgai jartzeko, entitatearen inprimaki eta ikuspegi guztiak ikusi beharko dituzu eta eremu horiek Project Service-eko entitate horien inprimakietan eta ikuspegietan gehitu beharko dituzu.
Hurrengo taula erabiltzeko prest dauden inprimakien eta ikuspegien zerrenda zabala da, entitateen arabera zerrendatuta, eta eguneratu beharko da. Entitate horien pertsonalizazioetan ikuspegi edo inprimaki gehigarririk baldin badago, gehitu eremu berriak horietan ere.
Ireki soluzio-arakatzailea prezio-dimentsioaren soluzioa lortzeko eta, ondoren, egin klik **Argitaratu pertsonalizazio guztiak** atalean.


|   Entitatea        | Inprimakiak   |Ikuspegiak        |
| ------------------------------|---------------------------------|----------------------------------|
|  Funtzioaren prezioa|• Informazioa |• Baliabide-kategorien prezio aktiboak<br> • Baliabide-kategorien prezioekin erlazionatutako ikuspegia|
|  Funtzio-prezioaren gainprezioa|• Informazioa|• Funtzio-prezioaren gainprezio aktiboa<br>• Funtzio-prezioaren gainprezioarekin erlazionatutako ikuspegia|
|  Eskaintzaren lerroaren xehetasunak|• Proiektuari buruzko informazioa<br>• Sorrera bizkorreko proiektua|• Eskaintzaren lerroaren xehetasun aktiboak<br>• Konbinatutako eskaintzaren lerroen xehetasunak<br>• Eskaintzaren lerroen xehetasunekin erlazionatutako ikuspegia|
|  Proiektu-kontratuaren lerroaren xehetasunak|• Proiektuari buruzko informazioa<br>• Sorrera bizkorreko proiektua|• Kontratuaren lerroaren xehetasun konbinatuak<br>• Kontratuaren lerroaren xehetasun aktiboak<br>• Kontratuaren lerroen xehetasunekin erlazionatutako ikuspegia|
|  Proiektuaren zeregina|• Informazioa<br>• Inprimaki berria||
|  Proiektu-taldeko kidea|• Informazioa<br>• Inprimaki berria|• Proiektu-taldeko kide aktiboak<br>• Proiektu-taldeko kideak<br>• Proiektu-taldeko kideekin erlazionatutako ikuspegia|
|  Denbora-sarrera|• Informazioa<br>• Sortu denbora-sarrera|• Nire denbora-sarrerak dataren arabera<br>• Aste honetako nire denbora-sarrerak<br>• Onartu beharreko denbora-sarrerak|
|  Kutxako liburuaren lerroa|• Informazioa<br>• Sorrera bizkorra|• Kutxako liburuaren lerro aktiboak<br>• Kutxako liburuaren lerroekin erlazionatutako ikuspegia|
|  Fakturaren lerroaren xehetasunak|• Informazioa<br>• Sorrera bizkorra|• Fakturaren lerroen xehetasun aktiboak<br>• Kobra daitezkeen fakturen transakzioak<br>• Doako fakturen transakzioak<br>• Fakturaren lerroen xehetasunekin erlazionatutako ikuspegia<br>• Kobra ezin daitezkeen fakturaren transakzioak|
|  Benetakoa|• Informazioa<br>• Benetako datu aktiboak|• Benetako datuen ikuspegia|

## <a name="set-up-bookable-resource-as-a-pricing-dimension"></a>Konfiguratu baliabide erreserbagarriak prezio-dimentsio gisa

1. Web interfazean, joan **Project Service** > **Ezarpenak** > **Parametroak** atalera. **Parametroak** orrialdean, **Zenbatekoan oinarritutako prezio-dimentsioak** fitxan, ohartu fitxan agertzen den saretak prezio-dimentsioak entitateko erregistroak erakusten dituela. 
2. Gehitu **Baliabide erreserbagarriak** prezio-dimentsioen zerrenda honetara **msdyn_bookableresource** gisa. 
3. Adierazi baliabide erreserbagarriak prezio-dimentsio gisa funtzionatzen duen testuingurua eta ezarri **Kostuari aplikagarria** eta **Salmentari aplikagarria** balioak.
4. **Neurriaren mota** eremuan, hautatu **Zenbatekoan oinarrituta** aukera. 
5. Aukeratu baliabide erreserbagarriaren kostua eta salmenta lehentasuna. Normalean prezio-dimentsio gisa sartuta dagoenean, baliabide erreserbagarriek dute lehentasun handiena, beraz, hori **1** aukeran jartzeak (edo **0** aukeran, lehentasuna nola zenbatzen duzunaren arabera) portaera hori ziurtatuko luke.

## <a name="set-up-pricing-dimension-field-names"></a>Konfiguratu prezio-dimentsio aktiboen eremuak

Prezioen dimentsioaren eremuaren izena denean **Funtzioaren prezioa** taula bere eremuaren izenaren desberdina da prezioen lehenetsiak funtzionatu behar duen beste edozein entitateren kasuan, prezioen dimentsioaren erregistroa izen desberdinen berri izan behar da.    
Baliabide erresbagarrietarako, **Proiektuko taldekideak** entitateak beste izen bat du (**msdyn_bookableresourceid**) **Funtzioaren prezioa** entitatearekin konparatuta (**msdyn_bookableresource**). Prezioen dimentsioaren erregistroa **msydn_bookableresource** baliabiderako horretaz jabetu behar da. 
1. Horretarako, egin klik bikoitza errenkadan **Prezioen neurriak** saretan dimentsio orria irekitzeko **msdyn_bookableresource** baliabidekoa.
2. Dimentsioaren orrian, **Erlazionatutakoa** fitxan, egin klik **Prezioen dimentsioaren eremu-izenak** aukeran.

 ![Prezio-dimentsioaren eremu-izenak fitxa.](media/PD-fieldname.png)

4. Elkartzen den ikuspegian, egin klik **Gehitu prezioen dimentsioaren eremu berria** aukeran.

 ![Gehitu prezio-dimentsio eremu berriak.](media/Add-NewPD-fieldname.png)


Honek irekitzen du **Prezioen dimentsioaren eremu berriaren izena** orrialdea **msdyn_bookableresource** baliabiderako. 

5. Gehitu **msdyn_projectteam** **Erakundearen izena** eremuan eta **msdyn_bookableresourceid** **Eremuaren izena** eremuan. Erregistroa gorde

 ![Prezio-dimentsioaren eremu-izena.](media/PD-fieldname-Added.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]