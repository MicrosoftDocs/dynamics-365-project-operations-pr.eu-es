---
title: Kudeatu proiektuetan oinarritutako fakturaren proforma
description: Gai honek proforma proiektuan oinarritutako fakturak kudeatu eta horiekin lan egiteko moduari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 04/05/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: cba74c14f6d039dce0650f25ee04cbe35ec8f668b774cdaaa3bbf1aab99cb44d
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6989311"
---
# <a name="manage-a-proforma-project-based-invoice"></a>Kudeatu proiektuetan oinarritutako fakturaren proforma

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Dynamics 365 Project Operations-en, proforma fakturak Dynamics 365 Sales-en fakturen luzapen gisa eraikitzen dira. Hala ere, fakturazio prozesuan desberdintasun ugari daude salmenten eta proiektuen eragiketen artean fakturazioari dagokionez. Adibidez, ezin da fakturarik sortu **Fakturen zerrenda** orrialdea Project Operations atalean, baina posible da Salmentan egitea. Desberdintasun eta luzapen horiek salmenta-eskaera baten faktura tipikoa ez den proiektuen fakturazio-prozesuei laguntzeko daude.

> [!IMPORTANT]
> Desberdintasunak direla eta, ez erabili fakturak Salmentetan eta Project Operations-en modu aldakorrean.

## <a name="invoice-header"></a>Faktura goiburua

Informazio hau Proforma fakturaren goiburuan dago eskuragarri Project Operations-en.

| Eremua | Kokapena | Deskribapenak |
| --- | --- | --- | 
| **Fakturaren IDa** | **Laburpena** fitxa | Normalean automatikoki sortuko IDa da proformako faktura sortzen denean. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. Eremu hau proformako faktura bakoitzerako erreferentzia gisa erabiltzen da. |
| **Izena** | **Laburpena** fitxa | Ezarri proiektuaren kontratuaren izena lehenespenez. Eremu hau edita dezake. | 
| **Moneta** | **Laburpena** fitxa | Ezarri proiektuaren kontratuaren moneta lehenespenez. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |
| **Prezio-zerrenda** | **Laburpena** fitxa | Ezarri proiektuaren kontratuaren prezio-zerrenda lehenespenez. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Abagunea** | **Laburpena** fitxa | Lotutako aukeraren erreferentzia. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Kontratua** | **Laburpena** fitxa | Lotutako proiektuaren kontratuari egindako erreferentzia. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Bezeroa** | **Laburpena** fitxa | Lotutako proiektuaren kontratuari egindako erreferentzia. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |
| **Azalpena** | **Laburpena** fitxa | Faktura deskribatzen duen testu eremua. Eremu hau edita dezake. | 
| **Kobratu** eta erlazionatutako eremuak | **Laburpena fitxa** | Lehenespenak proiektuaren kontratuko bezeroarengandik ezartzen dira. Eremu hau edita dezake.  | 
| **Egoera** | **Laburpena** fitxa | Aukera hauek ezartzen ditu: **Aktiboa**, **Itxita**, **Ordainduta** eta **Bertan behera utzi da**, eta editatu egin daiteke. Proiektuaren eragiketetarako egoera onartezinak daude **Itxita** eta **Bertan behera utzi da**. </br> Egoera ezarrita dago **Aktiboa** faktura sortzen denean. </br>Egoera ezarri behar da **Ordainduta** soilik faktura baieztatu ondoren.  | 
| **Proiektuaren fakturaren egoera** | **Laburpena** fitxa | Aukera hauek ezartzen ditu: **Zirriborroa**, **Berrikuspenean** eta **Baieztatuta**, eta editatu egin daiteke. Bietan **Zirriborroa** eta **Berrikusten** egoerak, faktura editatu daiteke. Faktura ezin da editatu baieztatu ondoren. | 
| **Zenbateko xehatua** | **Laburpena** fitxa | Faktura-lerro guztietako zenbatekoen batura aurrerakinak eta kenkariak egin ondoren. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua.  Eremu hau azken zenbatekoa kalkulatzeko erabiltzen da. | 
| **Deskontua (%)** | **Laburpena** fitxa | Eremu hau edita daiteke deskontu ehunekoa sartzeko. Eremu hau ez dago Project Operations funtzionaltasunarekin onartuta. Onartzen ez den eremua da.|  
| **Deskontuaren zenbatekoa** | **Laburpena** fitxa | Eremu hau edita daiteke deskontuaren zenbatekoa sartzeko. Eremu hau ez dago Project Operations funtzionaltasunarekin onartuta. Onartzen ez den eremua da. |  
| **Pleit gabeko zenbatekoa** | **Laburpena fitxa** | Deskontuen ondorengo fakturaren zenbateko osoa aplikatu da. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. Eremu hau azken zenbatekoa kalkulatzeko erabiltzen da.  | 
| **Pleitaren zenbatekoa** | **Laburpena** fitxa | Eremu hau edita daiteke pleitaren zenbatekoa sartzeko. Eremu hau ez dago Project Operations funtzionaltasunarekin onartuta. Onartzen ez den eremua da. |
| **Zergak guztira** | **Laburpena** fitxa | Fakturan faktura lerro guztietako zerga osoa. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Zenbatekoa guztira** | **Laburpena** fitxa | Deskontuen eta zergen ondorengo zenbatekoaren batura. Batuketa bezeroak ordaindu behar duen zenbatekoa da. | 

## <a name="project-based-invoice-lines"></a>Proiektuetan oinarritutako fakturaren lerroak

Project Operations-en, beti dago faktura lerro bat proiektuaren kontratu lerro bakoitzeko. Faktura lerroa benetakoak ez badira ere sortzen da. Informazio hau Proforma fakturaren lerroan dago eskuragarri.

| Eremua | Kokapena | Deskribapenak | 
| --- | --- | --- |
| **Fakturaren IDa** | **Orokorra** fitxa | Fakturaren IDaren erreferentzia. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. Fakturaren ID esteka fakturaren goiburura itzultzeko erabil daiteke. | 
| **Izena** | **Orokorra** fitxa | Faktura-lerroaren izena lehenespenez kontratu-lerroaren izenetik ezarrita dago. Eremu hau edita dezake. |
| **Project** | **Orokorra** fitxa | Proiektua lotutako proiektuaren kontratu lerroan. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. Proiektuaren esteka proiektuan nabigatzeko erabil daiteke. | 
| **Fakturazio-metodoa** | **Orokorra** fitxa | Fakturazio-metodoa lotutako proiektuaren kontratu lerroan. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |
| **Kontratuaren lerroko zenbatekoa** | **Orokorra** fitxa | Lotutako proiektu-kontratuko kontratuaren zenbatekoa. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Data honetara arte fakturatutakoa** | **Orokorra** fitxa | Faktura horren faktura-lerroaren xehetasun guztien zenbatekoen batura. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Zenbatekoa** | **Orokorra** fitxa | Faktura horren faktura kargagarriaren lerroaren xehetasun guztien zenbatekoen batura. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. Eremu hau fakturaren goiburuko azken zenbatekoa kalkulatzeko erabiltzen da. | 
| **Zerga** | **Orokorra** fitxa | Faktura horren faktura-lerroaren xehetasun guztien zerga-zenbatekoen batura. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. Eremu hau fakturaren goiburuko azken zerga-zenbatekoa kalkulatzeko erabiltzen da. | 
| **Zenbateko hedatua** | **Orokorra** fitxa | Faktura horren fakturako lerro kargagarrien xehetasun guztien guztizko zenbatekoen batura (**Zerga + Zenbatekoak**). Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. Eremu hau fakturaren goiburuko azken zenbatekoa kalkulatzeko erabiltzen da. |

## <a name="invoice-line-details"></a>Fakturaren lerroaren xehetasunak

Proiektuaren faktura bateko faktura lerro bakoitzak faktura lerroaren xehetasunak biltzen ditu. Lerroaren xehetasun horiek fakturazio-lerroak aipatzen duen kontratu-lerroarekin lotutako fakturazio gabeko salmenten faktoreekin eta mugarriekin lotuta daude. Transakzio horiek guztiak markatuta daude **Fakturatzeko prest**.

**Denbora eta faktura materiala** lerroan, fakturaren lerroaren xehetasunak multzokatzen dira **Kargagarria**, **Ez da ordaindu behar** eta **Osagarria** **Faktura-lerroa** orrialdean. **Faktura-linea kargagarria** xehetasunak fakturaren lerroaren guztirako gehitzen dira. **Osagarria** eta **Kobratu gabeko egileak** ez gehitu faktura-lerroaren guztirako.

**Prezio finkoaren faktura** lerroan, fakturaren lerroaren xehetasunak honela markatuta dauden mugarrietatik sortzen dira **Fakturatzeko prest** lotutako kontratu lerroan. Fakturaren lerroaren xehetasuna mugarri batetik sortu ondoren, mugarriaren fakturazio egoera eguneratu egingo da **Bezeroaren faktura sortu da**.

### <a name="edit-invoice-line-details"></a>Editatu fakturaren lerroen xehetasunak

Ondorengo eremuak fakturazio-lerroaren xehetasunetan daude eskuragarri, fakturatu gabeko salmenten benetako babesarekin.

| Eremua | Deskribapenak |
| --- | --- | 
| **Fakturaren lerroa** | **Fakturaren lerroaren IDa** eremuari erreferentzia. Eremu hau irakurtzeko soilik dago eta editatzeko blokeatuta dago. Esteka fakturaren goiburura itzultzeko erabil daiteke. | 
| **Azalpena** | Fakturaren lerroko xehetasunaren azalpena. Ezarri lehenetsita **Barne iruzkinak** eremuan **Denbora-sarrera** eta **Deskribapena** eremua **Gastuen sarrera** aukeran. Eremua edita dezake.| 
| **Kanpoko azalpena** | Fakturaren lerroko xehetasunaren azalpena. Ezarri lehenetsita **Kanpo iruzkinak** eremuan **Denbora-sarrera** eta **Deskribapena** eremua **Gastuen sarrera** aukeran. Eremua edita dezake. Deskribapen hau bezeroari bidaliko zaion faktura inprimatuan zer egon behar duen zehazteko erabil daiteke. Project Operations-en, proforma fakturak ez ditu faktura guztiak inprimatzeko ezarpenak konfiguratzeko beharrezko funtzionalitate guztiak. | 
| **Hasiera-data** | Irakurtzeko soilik den eremua da jatorrizko iturritik lehenespenez ezartzen dena. |
| **Project** | Irakurtzeko soilik den eremua da, lehenespenez ezarrita dagoen iturburutik proiektuari lotutako kontratu-lerroan. |  
| **Ataza** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |
| **Transakzio-kategoria** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Funtzioa** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |  
| **Baliabide erreserbagarria** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Baliabideen enpresa** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Baliabide-unitatea** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Kantitatea** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |  
| **Unitate-antolaketa** | Fakturazio lerroaren xehetasunetarako, hau beti ezarrita dago eta ezin da editatu. Gastuei dagokienez, lehenespenez ezartzen da jatorrizko gastutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Unitatea** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |  
| **Prezioa** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |
| **Moneta** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Kopurua** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Zergak** | Ezarri lehenetsitako iturburutik. Eremua edita dezake.| 
| **Zenbateko hedatua** | Kalkulatutako eremua, honela kalkulatuta **Zenbatekoa + Zerga**. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Fakturazio mota** | Ezarri lehenetsitako iturburutik. Eremua edita dezake. Aukeratzen **Kargagarria** lerroa faktura-lerroaren guztizkoari gehitzen dio. **Osagarria** eta **Ez da ordaindu behar** faktura-lerroaren guztitik kanpo utziko du.| 
| **Hautatu produktua** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |
| **Produktu** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Produktuaren izena** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |  
| **Katalogotik kanpoko deskribapena** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |
| **Transakzio mota** | Irakurtzeko soilik den eremua da jatorrizko iturritik lehenespenez ezartzen dena **Fakturatutako salmentak**. |  
| **Transakzio-klasea** | Ezarri lehenetsitako iturburutik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 

Ondorengo eremuak fakturazio-lerroaren xehetasunetan daude eskuragarri, mugarri batekin.

| Eremua | Deskribapenak |
| --- | --- | 
| **Fakturaren lerroa** | **Fakturaren lerroaren IDa** eremuari erreferentzia. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. Esteka fakturaren goiburura itzultzeko erabil daiteke.  | 
| **Azalpena** | Fakturaren lerroko xehetasunaren azalpena. Ezarri lehenespenez iturburu mugarriaren deskribapenetik. | 
|**Kanpoko azalpena** | Jatorrizko mugarriaren deskribapenetik lehenespenez ezartzen den faktura-lerroaren deskribapena. Eremu hau bezeroari bidaliko zaion faktura inprimatuan zer egon behar duen zehazteko erabil daiteke. Project Operations-en, proforma fakturak ez ditu faktura guztiak inprimatzeko ezarpenak konfiguratzeko beharrezko funtzionalitate guztiak. | 
| **Hasiera-data** | Ezarri lehenetsita **Mugarria** data iturriaren mugarrian. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Project** | Ezarri lehenetsitako iturburuaren mugarritik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |
| **Zeregina** | Ezarri lehenetsitako iturburuaren mugarritik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Transakzio-kategoria** | Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |
| **Funtzioa** | Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Baliabide erreserbagarria** | Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Baliabide-unitatea** | Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Unitate-antolaketa** | Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Unitatea** | Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Prezioa** | Ezarri lehenespenez iturburu mugarriaren zenbatekotik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |
| **Moneta** | Ezarri lehenetsitako iturburuaren mugarritik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |
| **Zenbatekoa** | Ezarri lehenespenez iturburu mugarriaren zenbatekotik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Zerga** | Ezarri lehenespenez iturburu mugarriaren zerga-zenbatekotik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |
| **Zenbateko hedatua** | Ezarri lehenespenez iturburu mugarriaren zenbateko hedatutik. Eremua edita dezake. | 
| **Fakturazio mota** | Beti lehenetsita beti bezala **Kargagarria**. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. |
| **Transakzio mota** | Ezarri lehenetsitako iturburuaren mugarritik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 
| **Transakzio-klasea** | Ezarri lehenetsitako iturburuaren mugarritik. Editatzetik blokeatuta dagoen irakurtzeko soilik den eremua. | 

## <a name="refresh-invoice-transactions"></a>Freskatu fakturaren transakzioak

Faktura sortu ondoren sartu diren datuak badituzu, faktura horiek sar ditzakezu fakturan.

1. **Fakturazio-zorroaren ikuspegia** eremuan, markatu datuak **Fakturatzeko prest**.   
2. Ireki proforma faktura zirriborroa eta, **Ekintzak** zinta, hautatu **Freskatu faktura lineako transakzioak**.

  Fakturen lerroaren xehetasunak iraganean datatutako eta gisa markatutako benetako edozeinetarako sortzen dira **Fakturatzeko prest**, baina ez dago fakturan sartuta.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
