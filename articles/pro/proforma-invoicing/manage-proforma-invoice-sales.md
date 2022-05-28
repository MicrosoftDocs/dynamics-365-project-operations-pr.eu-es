---
title: Kudeatu proformako proiektuaren faktura
description: Gai honek proforma proiektuan oinarritutako fakturak horiekin lan egiteko moduari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 04/05/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 359f17fb5510b13de97d2349dcbc91d11b48e0f9
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8582603"
---
# <a name="manage-a-proforma-project-invoice"></a>Kudeatu proformako proiektuaren faktura 

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Dynamics 365 Project Operations-en, proforma fakturak Dynamics 365 Sales-en fakturen luzapen gisa eraikitzen dira. Hala ere, fakturazio prozesuan desberdintasun ugari daude salmenten eta proiektuen eragiketen artean fakturazioari dagokionez. Adibidez, ezin da fakturarik sortu **Fakturen zerrenda** orrialdea Project Operations atalean, baina posible da Salmentan egitea. Desberdintasun eta luzapen horiek salmenta-eskaera baten faktura tipikoa ez den proiektuen fakturazio-prozesuei laguntzeko daude.

> [!IMPORTANT]
> Desberdintasunak direla eta, ez erabili fakturak Salmentetan eta Project Operations-en modu aldakorrean.

## <a name="invoice-header"></a>Faktura goiburua

Informazio hau Proforma fakturaren goiburuan dago eskuragarri Project Operations-en.

| Eremua | Kokapena | Deskribapena | Downstream eragina |
| --- | --- | --- | --- |
| **Fakturaren IDa** | **Laburpena** fitxa | Normalean automatikoki sortuko IDa da proformako faktura sortzen denean. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Eremu hau proformako faktura bakoitzerako erreferentzia gisa erabiltzen da. |
| **Izena** | **Laburpena** fitxa | Ezarri proiektuaren kontratuaren izena lehenespenez. Eremu hau erabiltzaileak editatu dezake. | &nbsp;  |
| **Moneta** | **Laburpena** fitxa | Ezarri proiektuaren kontratuaren moneta lehenespenez. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |&nbsp; |
| **Prezio-zerrenda** | **Laburpena** fitxa | Ezarri proiektuaren kontratuaren prezio-zerrenda lehenespenez. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Abagunea** | **Laburpena** fitxa | Lotutako aukeraren erreferentzia. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp;  |
| **Kontratua** | **Laburpena** fitxa | Lotutako proiektuaren kontratuari egindako erreferentzia. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Bezeroa** | **Laburpena** fitxa | Lotutako proiektuaren kontratuari egindako erreferentzia. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |&nbsp;  |
| **Azalpena** | **Laburpena** fitxa | Faktura deskribatzen duen testu eremua. Eremu hau erabiltzaileak editatu dezake. | &nbsp; |
| **Kobratu** eta erlazionatutako eremuak | **Laburpena fitxa** | Lehenespenak proiektuaren kontratuko bezeroarengandik ezartzen dira. Eremu hau erabiltzaileak editatu dezake.  | &nbsp; |
| **Egoera** | **Laburpena** fitxa | Aukera hauek ezartzen ditu: **Aktiboa**, **Itxita**, **Ordainduta** eta **Bertan behera utzi da**, eta erabiltzaileak editatu dezake. | Proiektuaren eragiketetarako egoera onartezinak daude **Itxita** eta **Bertan behera utzi da**. </br> Egoera ezarrita dago **Aktiboa** faktura sortzen denean. </br>Egoera ezarri behar da **Ordainduta** soilik faktura baieztatu ondoren. |
| **Proiektuaren fakturaren egoera** | **Laburpena** fitxa | Aukera hauek ezartzen ditu: **Zirriborroa**, **Berrikusten** eta **Berretsita**, eta erabiltzaileak editatu dezake. | Bietan **Zirriborroa** eta **Berrikusten** egoerak, faktura editatu daiteke. Faktura ezin da editatu baieztatu ondoren. |
| **Zenbateko xehatua** | **Laburpena** fitxa | Faktura-lerro guztietako zenbatekoen batura aurrerakinak eta kenkariak egin ondoren. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Eremu hau azken zenbatekoa kalkulatzeko erabiltzen da. |
| **Deskontua (%)** | **Laburpena** fitxa | Eremu hau edita daiteke deskontu ehunekoa sartzeko. Eremu hau ez dago Project Operations funtzionaltasunarekin onartuta. | Onartzen ez den eremua da. |
| **Deskontuaren zenbatekoa** | **Laburpena** fitxa | Eremu hau edita daiteke deskontuaren zenbatekoa sartzeko. Eremu hau ez dago Project Operations funtzionaltasunarekin onartuta. | Onartzen ez den eremua da. |
| **Pleit gabeko zenbatekoa** | **Laburpena fitxa** | Deskontuen ondorengo fakturaren zenbateko osoa aplikatu da. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Eremu hau azken zenbatekoa kalkulatzeko erabiltzen da. |
| **Pleitaren zenbatekoa** | **Laburpena** fitxa | Eremu hau edita daiteke pleitaren zenbatekoa sartzeko. Eremu hau ez dago Project Operations funtzionaltasunarekin onartuta. | Onartzen ez den eremua da. |
| **Zergak guztira** | **Laburpena** fitxa | Fakturan faktura lerro guztietako zerga osoa. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Bat ere ez. |
| **Zenbatekoa guztira** | **Laburpena** fitxa | Deskontuen eta zergen ondorengo zenbatekoaren batura. | Batuketa bezeroak ordaindu behar duen zenbatekoa da. |
## <a name="project-based-invoice-lines"></a>Proiektuetan oinarritutako fakturaren lerroak

Project Operations-en, beti dago faktura lerro bat proiektuaren kontratu lerro bakoitzeko. Faktura lerroa benetakoak ez badira ere sortzen da. Informazio hau Proforma fakturaren lerroan dago eskuragarri.

| Eremua | Kokapena | Deskribapena | Downstream eragina |
| --- | --- | --- | --- |
| **Fakturaren IDa** | **Orokorra** fitxa | Fakturaren IDaren erreferentzia. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Fakturaren ID esteka fakturaren goiburura itzultzeko erabil daiteke. |
| **Izena** | **Orokorra** fitxa | Faktura-lerroaren izena lehenespenez kontratu-lerroaren izenetik ezarrita dago. Eremu hau erabiltzaileak editatu dezake. | &nbsp; |
| **Project** | **Orokorra** fitxa | Proiektua lotutako proiektuaren kontratu lerroan. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Proiektuaren esteka proiektuan nabigatzeko erabil daiteke. |
| **Fakturazio-metodoa** | **Orokorra** fitxa | Fakturazio-metodoa lotutako proiektuaren kontratu lerroan. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Kontratuaren lerroko zenbatekoa** | **Orokorra** fitxa | Lotutako proiektu-kontratuko kontratuaren zenbatekoa. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Data honetara arte fakturatutakoa** | **Orokorra** fitxa | Faktura horren faktura-lerroaren xehetasun guztien zenbatekoen batura. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Zenbatekoa** | **Orokorra** fitxa | Faktura horren faktura kargagarriaren lerroaren xehetasun guztien zenbatekoen batura. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Eremu hau fakturaren goiburuko azken zenbatekoa kalkulatzeko erabiltzen da. |
| **Zerga** | **Orokorra** fitxa | Faktura horren faktura-lerroaren xehetasun guztien zerga-zenbatekoen batura. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Eremu hau fakturaren goiburuko azken zerga-zenbatekoa kalkulatzeko erabiltzen da. |
| **Zenbateko hedatua** | **Orokorra** fitxa | Faktura horren fakturako lerro kargagarrien xehetasun guztien guztizko zenbatekoen batura (**Zerga + Zenbatekoak**). Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Eremu hau fakturaren goiburuko azken zenbatekoa kalkulatzeko erabiltzen da. |


## <a name="invoice-line-details"></a>Fakturaren lerroaren xehetasunak

Proiektuaren faktura bateko faktura lerro bakoitzak faktura lerroaren xehetasunak biltzen ditu. Lerroaren xehetasun horiek fakturazio-lerroak aipatzen duen kontratu-lerroarekin lotutako fakturazio gabeko salmenten faktoreekin eta mugarriekin lotuta daude. Transakzio horiek guztiak markatuta daude **Fakturatzeko prest**.

**Denbora eta faktura materiala** lerroan, fakturaren lerroaren xehetasunak multzokatzen dira **Kargagarria**, **Ez da ordaindu behar** eta **Osagarria** **Faktura-lerroa** orrialdean. **Faktura-linea kargagarria** xehetasunak fakturaren lerroaren guztirako gehitzen dira. **Osagarria** eta **Kobratu gabeko Egileak** ez gehitu faktura-lerroaren guztirako.

**Prezio finkoaren faktura** lerroan, fakturaren lerroaren xehetasunak honela markatuta dauden mugarrietatik sortzen dira **Fakturatzeko prest** lotutako kontratu lerroan. Fakturaren lerroaren xehetasuna mugarri batetik sortu ondoren, mugarriaren fakturazio egoera eguneratu egingo da **Bezeroaren faktura sortu da**.

### <a name="edit-invoice-line-details"></a>Editatu fakturaren lerroen xehetasunak

Ondorengo eremuak fakturazio-lerroaren xehetasunetan daude eskuragarri, fakturatu gabeko salmenten benetako babesarekin:

| Eremua | Deskribapena | Downstream eragina |
| --- | --- | --- |
| **Fakturaren lerroa** | **Fakturaren lerroaren IDa** eremuari erreferentzia. Irakurtzeko soilik eremua, blokeatuta editatzeko. | Esteka fakturaren goiburura itzultzeko erabil daiteke. |
| **Azalpena** | Fakturaren lerroko xehetasunaren azalpena. Ezarri lehenetsita **Barne iruzkinak** eremuan **Denbora-sarrera** eta **Deskribapena** eremua **Gastuen sarrera** aukeran. Eremua erabiltzaileak editatu dezake.| &nbsp; |
| **Kanpoko azalpena** | Fakturaren lerroko xehetasunaren azalpena. Ezarri lehenetsita **Kanpo iruzkinak** eremuan **Denbora-sarrera** eta **Deskribapena** eremua **Gastuen sarrera** aukeran. Eremua erabiltzaileak editatu dezake. | Deskribapen hau bezeroari bidaliko zaion faktura inprimatuan zer egon behar duen zehazteko erabil daiteke. Project Operations-en, proforma fakturak ez ditu faktura guztiak inprimatzeko ezarpenak konfiguratzeko beharrezko funtzionalitate guztiak. |
| **Hasiera-data** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Eremu hau jatorrizko iturri batek babesten ez duen faktura lerroaren xehetasun berri batean editatu daiteke. |
| **Project** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Ezarri lehenespenez lotutako kontratuaren lerroko proiektuan. |
| **Zeregina** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Eremua jatorrizko iturri batek babesten ez duen faktura lerroaren xehetasun berri batean editatu daiteke. Goitibeherako zerrendan erlazionatutako proiektuaren kontratu lerroarekin lotutako zeregin guztiak agertzen dira.  |
| **Transakzio-kategoria** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Eremua jatorrizko iturri batek babesten ez duen faktura lerroaren xehetasun berri batean editatu daiteke. |
| **Funtzioa** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Eremua jatorrizko iturri batek babesten ez duen faktura lerroaren xehetasun berri batean edita daiteke. |
| **Baliabide erreserbagarria** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Eremua jatorrizko iturri batek babesten ez duen faktura lerroaren xehetasun berri batean editatu daiteke. |
| **Baliabide-unitatea** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Eremua jatorrizko iturri batek babesten ez duen faktura lerroaren xehetasun berri batean edita daiteke. |
| **Kopurua** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Eremua jatorrizko iturri batek babesten ez duen faktura lerroaren xehetasun berri batean edita daiteke. |
| **Unitate-antolaketa** | Fakturazio lerroaren xehetasunetarako, hau beti ezarrita dago eta ezin da editatu. Gastuei dagokienez, lehenespenez ezartzen da jatorrizko gastutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Lehenespenez ezarri **Denbora** benetako batek babesten ez duen faktura-lerroaren xehetasun berri batean. |
| **Unitatea** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Eremua jatorrizko iturri batek babesten ez duen faktura lerroaren xehetasun berri batean edita daiteke |
| **Prezioa** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Eremua jatorrizko iturri batek babesten ez duen faktura lerroaren xehetasun berri batean edita daiteke. Balorerik sartzen ez bada, lehenespenez ezartzen da **Gorde**. |
| **Moneta** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Ezartzen da lehenespenez fakturaren goiburutik fakturaren xehetasun berri bat sortzen denean babesik gabe.  Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |
| **Zenbatekoa** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Honela kalkulatuta **Kopurua \* Prezioa** fakturaren xehetasun berri bat sortzen denean babesik izan gabe. Ondoren kalkulatzen da **Gorde**. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |
| **Zerga** | Ezarri lehenetsitako iturburutik. Eremua erabiltzaileak editatu dezake | Erabiltzaileak editatu dezake eremua faktura lerroaren xehetasun berri bat sortzerakoan babesik izan gabe. |
| **Zenbateko hedatua** | Kalkulatutako eremua, honela kalkulatuta **Zenbatekoa + Zerga**. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Fakturazio mota** | Ezarri lehenetsitako iturburutik. Eremua erabiltzaileak editatu dezake. | Aukeratzen **Kargagarria** lerroa faktura-lerroaren guztizkoari gehitzen dio. **Osagarria** eta **Ez da ordaindu behar** faktura-lerroaren guztitik kanpo utziko du. |
| **Hautatu produktua** | Ezarri lehenespenez iturburuko benetako datuetatik, irakurtzeko soilik da eremu hau. | Fakturazio-lerroaren xehetasun berri bat sortzen duzunean babesik izan gabe, eremu hau edita daiteke. |
| **Produktu** | Ezarri lehenespenez iturburuko benetako datuetatik, irakurtzeko soilik da eremu hau. | Fakturazio lerroaren xehetasun berri bat babeskopiarik gabe sortzen duzunean, eremu hau edita daiteke **Aukeratu produktua** eremua ezarrita dago **Lehendik dagoen produktua**. |
| **Produktuaren izena** | Ezarri lehenespenez iturburuko benetako datuetatik, irakurtzeko soilik da eremu hau. | Faktura-lerroaren xehetasun berri batean, produktuaren IDa katalogoan hautatuta dagoenean, eremu hau produktuaren izenarekin ezartzen da. Produktuan idazteko, eremuan izena idazteko ezarri da. |
| **Katalogotik kanpoko deskribapena** | Ezarri lehenespenez iturburuko benetako datuetatik, eremua irakurtzeko soilik da. | Fakturaren lerroaren xehetasun berri bat sortzen duzunean babesik izan gabe, produktuaren deskribapenean idatz dezakezu. |
| **Transakzio mota** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Lehenespenez ezarri **Fakturatutako salmentak** eta blokeatuta berria sortzean **Faktura lerroaren xehetasuna** benetako babesik gabe.  |
| **Transakzio-klasea** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Ezarri lehenespenez erabiltzaileak fitxategi bat sortzea aukeratzen duenaren arabera **Denbora**, **Gastua**, **Materiala** edo **Kuota** fakturaren lerroaren xehetasunak berria sortu bitartean **Faktura lerroaren xehetasuna** benetako babesik gabe. Blokeatuta ez editatzeko. |

Ondorengo eremuak fakturazio-lerroaren xehetasunetan daude eskuragarri, mugarri batekin:

| Eremua | Deskribapena | Downstream eragina |
| --- | --- | --- |
| **Fakturaren lerroa** | **Fakturaren lerroaren IDa** eremuari erreferentzia. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | Esteka fakturaren goiburura itzultzeko erabil daiteke. |
| **Azalpena** | Fakturaren lerroko xehetasunaren azalpena. Ezarri lehenespenez iturburu mugarriaren deskribapenetik. | &nbsp; |
|**Kanpoko azalpena** | Jatorrizko mugarriaren deskribapenetik lehenespenez ezartzen den faktura-lerroaren deskribapena. | Eremu hau bezeroari bidaliko zaion faktura inprimatuan zer egon behar duen zehazteko erabil daiteke. Project Operations-en, proforma fakturak ez ditu faktura guztiak inprimatzeko ezarpenak konfiguratzeko beharrezko funtzionalitate guztiak. |
| **Hasiera-data** | Ezarri lehenetsita **Mugarria** data iturriaren mugarrian. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Project** | Ezarri lehenetsitako iturburuaren mugarritik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Zeregina** | Ezarri lehenetsitako iturburuaren mugarritik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Transakzio-kategoria** | Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Funtzioa** | Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Baliabide erreserbagarria** | Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Baliabide-unitatea** | Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Unitate-antolaketa** | Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Unitatea** | Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Prezioa** | Ezarri lehenespenez iturburu mugarriaren zenbatekotik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Moneta** | Ezarri lehenetsitako iturburuaren mugarritik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |&nbsp; |
| **Zenbatekoa** | Ezarri lehenespenez iturburu mugarriaren zenbatekotik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Zerga** | Ezarri lehenespenez iturburu mugarriaren zerga-zenbatekotik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Zenbateko hedatua** | Ezarri lehenespenez iturburu mugarriaren zenbateko hedatutik. Eremua erabiltzaileak editatu dezake | &nbsp; |
| **Fakturazio mota** | Beti lehenetsita beti bezala **Kargagarria**. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Transakzio mota** | Ezarri lehenetsitako iturburuaren mugarritik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |
| **Transakzio-klasea** | Ezarri lehenetsitako iturburuaren mugarritik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | &nbsp; |

### <a name="create-new-invoice-line-details"></a>Sortu fakturaren lerroaren xehetasunak

Denbora eta material fakturazio lerroetan, faktura lerroaren xehetasun berriak sor ditzakezu. Faktura-lerroaren xehetasun horiek ez dituzte benetako baten babesik. Denbora eta material faktura lerro baten faktura lerroan hauta dezakezu **Berria** fakturazio lerroaren xehetasun berria sortzeko, kontratu lerroan sartzen diren transakzio klaseetarako.

## <a name="refresh-invoice-transactions"></a>Freskatu fakturaren transakzioak

Faktura sortu ondoren sartu diren datuak badituzu, faktura horiek sar ditzakezu fakturan.

1. **Fakturazio-zorroaren ikuspegia** eremuan, markatu datuak **Fakturatzeko prest**.   
2. Ireki proforma faktura zirriborroa eta, **Ekintzak** zintan, sakatu **Freskatu faktura lineako transakzioak**.

  Honek fakturazio-lerroaren xehetasunak sortzen ditu iraganeko data gisa eta gisa markatuta dagoen edozein **Fakturatzeko prest**; baina ez dago fakturan sartuta.

## <a name="product-based-invoice-lines"></a>Produktuetan oinarritutako fakturaren lerroak

Project Operations-etan, fakturazio lerroak sor ditzakezu edozein proiekturi aplikatzen ez zaizkien produktuetarako edo proiektu guztietarako proiektuetan oinarritutako faktura lerroekin batera. Faktura-lerro hauek produktuan oinarritutako kontratu-lerro gisa sortzen dira eta fakturatzeko prest daudela markatu ondoren, produktuan oinarritutako faktura-lerro gisa gehitzen dira.

Produktuan oinarritutako faktura lerroak gehitu ondoren, ezin dira aldatu. Hala ere, proforma fakturaren zirriborroan ezaba daitezke.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
