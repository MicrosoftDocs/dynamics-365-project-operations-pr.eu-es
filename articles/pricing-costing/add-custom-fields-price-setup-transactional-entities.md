---
title: Gehitu beharrezko eremu pertsonalizatuak prezioen konfigurazioan eta entitate transakzionaletan
description: Artikulu honetan, erakundeei eta formulario eta ikuspegiei beharrezkoak diren eremu pertsonalizatuen erreferentziak nola gehitu buruzko informazioa ematen da.
author: rumant
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: johnmichalak
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: a984dc9e04857e101fa012734fd822440899aced
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8926025"
---
# <a name="add-required-custom-fields-to-price-setup-and-transactional-entities"></a>Gehitu beharrezko eremu pertsonalizatuak prezioen konfigurazioan eta entitate transakzionaletan

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Artikulu honetan, prezio-dimentsio gisa erabiliko diren eremu eta erakunde pertsonalizatuak sortzeko [artikuluko prozedurak osatu dituela suposatzen da](create-custom-fields-entities-pricing-dimensions.md). Prozedura horiek bete ez badituzu, joan atzera eta osatu eta, ondoren, itzuli artikulu honetara. 

Artikulu honetan, prozedurek beharrezkoak diren eremu pertsonalizatuen erreferentziak entitateei eta erabiltzailearen interfazeari (UI) elementuei, hala nola inprimakiak eta ikuspegiak, nola gehitu erakutsiko dizute.

## <a name="add-custom-pricing-dimension-fields"></a>Gehitu prezioen dimentsio-eremu pertsonalizatuak 
Eremu eta entitate pertsonalizatuak sortu ondoren, hurrengo urratsa da prezioen konfigurazioa eta transakzio-entitateak entitate pertsonalizatuak edo aukera-multzoak ezagutzea, erreferentzia-eremuak sortuz. Zure prezioen dimentsioen zerrendak aukera-multzo dimentsioak edo entitatearen neurriak edo biak biltzen dituen ala ez kontuan hartuta, jarraitu **Aukera-multzoetan oinarritutako prezioen dimentsioak** edo **Entitatean oinarritutako prezioen dimentsioak** ataletan soilik dauden urratsak, edo biak, hurrenez hurren.

### <a name="option-set-based-custom-pricing-dimensions"></a>Aukera-multzoetan oinarritutako prezioen dimentsioak
Prezioen dimentsio pertsonalizatu bat aukera-multzoan oinarritutakoan, gehitu eremu gisa funtsezko entitateei. Hurrengo prozeduran, **Baliabideen lanaren kokalekua** eta **Baliabideen lan ordutegia** aukerak aukeramultzoan oinarritutako prezioen dimentsio gisa erabiltzen dira. Lehenik eta behin, prezio-erakundeei eremu gisa gehitu behar zaizkie, **Funtzio-prezioa** eta **Funtzioaren prezioen gainprezioa**.

1. Proiektuaren eragiketetan, hautatu **Ezarpenak** > **Soluzioak** eta sakatu bi aldiz **\<your organization name>prezio-dimentsioa**. 
2. Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Entitateak> Funtzio-prezioa**.
3. Zabaldu **Funtzio-prezioa** entitatea eta hautatu **Eremuak**.
4. Hautatu **Berria** eremuan eremu berria sortzeko **Baliabideen lanaren kokalekua** izenekoa eta hautatu **Aukera-multzoa** eremu mota gisa. 
5. Hautatu **Erabili lehendik dagoen aukera-multzoa** aukera, hautatu **Baliabideen lanaren kokalekua** aukera-multzoa, eta hautatu **Gorde** aukeran.
6. Errepikatu 1-5 urratsak eremu hau **Funtzio-prezioaren gainprezioa** entitatera gehitzeko. 
7. Errepikatu 1-5 urratsak **Baliabideen lana** aukera-multzorako.

> [!IMPORTANT]
> Eremua entitate batean baino gehiagotan gehitzen duzunean, erabili eremu-izen bera entitate guztietan. 

> ![Baliabideen lanaren kokapena gehitzea Funtzio-prezioari.](media/RWL-Field.png)

Proiektu baten salmenta eta zenbatespen faseetan, **lokalean** eta **gunean** burutu behar den lan ahaleginaren kalkuluak, **Ohiko orduak** eta **Ordutegi gehigarria** ataletan, eskaintza/proiektuaren balioa kalkulatzeko erabiltzen dira. **Baliabideen lanaren kokalekua** eta **Baliabideen lana** eremuak **eskaintza lerroaren xehetasuna**, **Kontratuaren lerroaren xehetasuna**, **Proiektuko taldekidea**, eta **Estimazio lerroa** estimazio entitateei gehituko zaizkie.

1. Proiektuaren eragiketetan, hautatu **Ezarpenak** > **Soluzioak** eta, ondoren, sakatu bi aldiz **\<your organization name>prezio-dimentsioa**. 
2. Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Entitateak> Eskaintza lerroaren xehetasuna**.
3. Zabaldu **Eskaintza lerroaren xehetasuna** entitatea eta hautatu **Eremuak**.
4. Hautatu **Berria** eremuan eremu berria sortzeko **Baliabideen lanaren kokalekua** izenekoa eta hautatu eremu mota, **Aukera-multzoa**. 
5. Aukeratu **Erabili lehendik dagoen aukera-multzoa** eta **Baliabideen lanaren kokalekua** aukerak eta hautatu **Gorde** aukeran.
6. Errepikatu 1-5 urratsak eremu hau **Proiektuaren kontratuaren lerroaren xehetasuna**, **Proiektuko taldekidea**, eta **Estimazio lerroa** entitateei gehitzeko.
7. Errepikatu 1-6 urratsak **Baliabideen lana** aukera-multzorako. 

> ![Baliabideen lanaren kokapena gehitzea estimazio lerroari.](media/RWL-Default-Value.png)

Entrega eta fakturaziorako, amaitutako lana zehaztasunez preziatu behar da **lokalean** edo **gunean** egin den zehazteko, eta **ohiko orduetan** edo **aparteko orduetan** egin den hautatzeko proiektuaren benetako datuetan. **Baliabideen lanaren kokalekua** eta **Baliabideen lana** eremuak **sarrera-ordua**, **benetakoa**, **faktura lerroaren xehetasuna**, eta **kutxako liburuaren lerroa** entitateetan gehitu behar dira.

1. Hautatu **Ezarpenak** > **Soluzioak** eta, ondoren, sakatu bi aldiz **\<your organization name>prezio-dimentsioa**.
2. Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Entitateak> Sarrera-ordua**.
3. Zabaldu **Eskaintza lerroaren xehetasuna** entitatea eta gero hautatu **Eremuak**.
4. Hautatu **Berria** eremuan eremu berria sortzeko **Baliabideen lanaren kokalekua** izenekoa eta hautatu **Aukera-multzoa** eremu mota gisa. 
5. Hautatu **Erabili lehendik dagoen aukera-multzoa** aukera, hautatu **Baliabideen lanaren kokalekua** aukera-multzoa, eta hautatu **Gorde** aukeran.
6. Errepikatu 1-5 urratsak eremua **Benetakoa**, **Faktura lerroaren xehetasuna**, eta **Kutxako liburuaren lerroa** entitateetan gehitzeko.
7. Errepikatu 1-6 urratsak **Baliabideen lana** aukera-multzorako. 

> ![Baliabideen lanaren kokapena gehitzea denbora-sarreran.](media/RWL-time-entry.png)

Aukera-multzoan oinarritutako neurri pertsonalizatuetarako beharrezkoak diren eskema aldaketak osatzen ditu.

## <a name="entity-based-custom-pricing-dimensions"></a>Entitate-multzoetan oinarritutako prezioen dimentsioak

Prezioen dimentsio pertsonalizatua entitate bat denean, dimentsio-entitatearen eta entitate-gakoen artean 1:N harremanak gehituko dituzu. Goiko titulu estandarraren adibidea erabiliz, zentzuzkoa da langile bakoitzari titulu estandarra esleitzea espero izatea. Ondorioz, 1:N harremana beharko duzu titulu estandarretik baliabide erreserbagarrira, edo N:1 erlazioa baliabide erreserbagarritik titulu estandarrera sortu bada.

1. Proiektuaren eragiketetan, hautatu **Ezarpenak** > **Soluzioak** eta, ondoren, sakatu bi aldiz **\<your organization name>prezio-dimentsioa**. 
2. Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Entitateak> Titulu estandarra**.
3. Zabaldu **Titulu estandarra** entitatea eta hautatu **1:N harremanak**.
4. Hautatu **Berria** aukeran 1:N harreman berria sortzeko, **Titulu estandarretik baliabideak erreserbagarrira** izena duena. Sartu beharrezko informazioa eta, ondoren, hautatu **Gorde** aukeran.

> ![Titulu estandarra gehitzea baliabide erreserbagarrietan erreferentzia-eremu gisa.](media/ST-BR.png)

Titulu estandarra prezio-erakundeei ere gehitu beharko zaie, hala nola **Funtzioaren prezioa** eta **Funtzioaren prezioaren gainprezioa**. Hau ere: **Titulu estandarra** eta **Funtzioaren prezioa** entitateen eta **Titulu estandarra** eta **Funtzioaren prezioen gainprezioa** entitateen artean 1:N harremanak erabiliz osatzen da.

1. Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Entitateak> Titulu estandarra**.
2. Zabaldu **Titulu estandarra** entitatea eta hautatu **1:N harremanak**.
3. Hautatu **Berria** aukeran 1:N harreman berria sortzeko, **Titulu estandarretik funtzioaren preziora** izena duena. Sartu beharrezko informazioa eta, ondoren, hautatu **Gorde** aukeran.
4. 1-4 urratsak errepikatu **Titulu estandarra** eta **Funtzioaren prezioaren gainprezioa** entitateen artean 1:N harremanak sortzeko.

Proiektuaren salmenta- eta estimazio-faseetan, eskaintza/proiektua preziatzeko, titulu estandar bakoitzeko lanaren ahaleginaren kalkuluak behar dira. Honek esan nahi du entitate horietako bakoitzeko 1:N harremanak behar direla: 

- **Eskaintzaren lerroaren xehetasunak**
- **Proiektu-kontratuaren lerroko xehetasunak**
- **Proiektu-taldeko kidea**
- **Aurreikuspenaren lerroa**

5. Errepikatu 1-5 urratsak **Titulu estandarra** entitatetik **Eskaintzaren lerroaren xehetasuna**, **Proiektuaren kontratuaren lerroaren xehetasuna**, **Proiektuko taldekidea**, eta **Aurreikuspenaren lerroa** entitateetara 1:N harremanak sortzeko.

> ![Titulu estandarra gehitzea aurreikuspenaren lerroa erreferentzia-eremu gisa.](media/ST-Estimate-Line.png)

  Entrega- eta fakturazio-faseetan, titulu estandar bakoitzak osatutako lanak proiektuaren benetakoa atalean zehaztasunez preziatu behar dira. Horrek esan nahi du 1: N harremanak izan behar direla **Titulu estandarra** entitatetik **Denbora-sarrera**, **Benetakoa**, **Faktura lerroaren xehetasuna**, eta **Kutxako liburuaren lerroa entitateak** entitateetara.

6. Errepikatu 1-6 urratsak 1: N harremanak sortzeko **Titulu estandarra** entitatetik **Denbora-sarrera**, **Benetakoa**, **Faktura lerroaren xehetasuna**, eta- **Kutxako liburuaren lerroa entitateak** entitateetara.

> ![Titulu estandarra gehitzea denbora-sarrera erreferentzia-eremu gisa.](media/ST-Mapping.png)

### <a name="set-up-dimension-value-defaulting-using-the-mappings-features-of-the-platform"></a>Konfiguratu lehenetsitako dimentsioaren balioa plataformako esleitze-ezaugarriak erabiliz
Denbora-sarrera entitaterako, lagungarria izango litzateke sistemak lehenespenez denbora-sarrera entitatearen izena sarrera erregistratzen ari den baliabide erreserbagarritik hartzea. Jarraitu urrats hauei 1:N erlazioan eremuko mapak gehitzeko **Erreserbatzeko baliabidea** entitatetik **Denbora-sarrera** entitatera.

1. Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Entitateak> Titulu estandarra**.
2. Zabaldu **Titulu estandarra** entitatea eta hautatu **1:N harremanak**.
3. Egin klik bikoitza **Denbora-sarrerarako baliabide erreserbagarria** entitatean. **Harremana** orrian, hautatu **Erabili eremu-esleipenak** atalean. 
4. Hautatu **Berria** aukeran eremu-esleipen berria sortzeko **Titulu estandarra** eremuaren, **Baliabide erresebagarria** entitatekoaren eta **Titulu estandarra** erreferentzia-eremuaren artean, **Denbora-sarrera** entitatekoa. 

> ![Konfiguratu eremu-esleipenak, baliabide erreserbagarriak denbora-sarrerara izenburu estandarra lehenetsi ahal izateko.](media/ST-Mapping2.png)

Entitateetan oinarritutako neurri pertsonalizatuetarako beharrezkoak diren eskema aldaketak osatzen ditu.

##  <a name="add-custom-fields-to-forms-views-and-business-rules"></a>Gehitu eremu pertsonalizatuak inprimaki, ikuspegi eta negozioaren arauera.

Beharrezko eskema-aldaketa guztiak egin ondoren, hurrengo urratsa da erabiltzaileare-interfazeko eremuak ikusgai jartzea eremuak inprimakietan eta ikuspegietan gehituz.

1. Inprimakia edo ikuspegia ireki. Eskuineko nabigazio-panelean, hautatu eremua eta arrastatu inprimakiaren mihisera. 
2. Ikuspegia editatzen ari bazara, erabili eskuineko nabigazio-panela, hautatu **Gehitu eremuak** atalean, eta **Eremuen zerrenda** elkarrizketa-koadroan hautatu behar dituzun eremuak eta hautatu **Ados** aukeran.

Hurrengo taulak erabiltzeko prest dauden inprimakien eta ikuspegien zerrenda zabala eskaintzen du, entitateen arabera, eta eremu berriekin eguneratu beharko da. Entitate horien pertsonalizazioetan ikuspegi edo inprimaki gehigarririk balduzu, gehitu eremu berriak horietan ere.

| Entity        | Eremu berria behar dituen inprimakiak   |Eremu berria behar dituen ikuspegiak      |
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

Eremu pertsonalizatuak negozioaren arauetan ere gehitu behar dira zehaztutakoaren arabera. Berezko adibide bat negozioaren araudirako **Denbora-sarreraren editagarritasuna egoeraren arabera** entitatea da. Arau honek definitzen du zer eremu blokeatu behar diren, denbora-sarrerak aldatzen ez den egoera duenean, hala nola **Onartutakoa** egoera. Gehitu eremuak negozioaren arau honetara, eremuak editatzeko blokeatuta gera daitezen, denbora-sarrera **Zirriborroa** edo **Itzulia** ez den beste egoera batean dagoenean.


[!INCLUDE[footer-include](../includes/footer-banner.md)]