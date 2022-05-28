---
title: Gastuak kudeatzeko parametroak
description: Ondorengo parametroek Gastuen kudeaketan jokabidea kontrolatzen dute.
author: KimANelson
ms.date: 01/12/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: TrvParameters
audience: Application User
ms.reviewer: johnmichalak
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2017-06-30
ms.dyn365.ops.version: July 2017 update
ms.openlocfilehash: 3a8cdce2552b4d1bafe2cb0796d7b82c231584ea
ms.sourcegitcommit: 2c2a5a11d446adec2f21030ab77a053d7e2da28e
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/04/2022
ms.locfileid: "8685685"
---
# <a name="expense-management-parameters"></a>Gastuak kudeatzeko parametroak


Ondorengo parametroek Gastuen kudeaketan jokabide orokorra kontrolatzen dute.

### <a name="general"></a>Orokorra

| **Eremua**                                                | **Deskribapena**                                                 |
|----------------------------------------------------------|---------------------------------------------------------------------|
| **Kilometrajearen tasa estandarra**                             | Idatzi kilometrajearen gastuen itzulketa-tasa. Tasa gasturako sartutako kilometrajearekin biderkatzen da bidaiaren gastuagatik itzultzen den zenbatekoa kalkulatzeko.                       |
|**Ordaindutako gastu pertsonalak**                             | Aukeratu nor arduratuko den pertsonal gisa sailkatutako kreditu txartelaren transakzio zenbatekoak ordaintzeaz.                                                                                                     |
|**Bistaratu gastuen txosten osoa zulatzean**               | Aukeratu aukera hau gastu-txostenaren gastu guztiak erakusteko, jatorrizko dokumentuaren xehetasunak gastu-txostena argitaratu zenean sortu zen bonu zehatz baterako ikusten direnean.              |
|**Bidaia aldez aurretik baimentzea derrigorrezkoa da**                 | Aukeratu aukera hau, langile batek gastuen txostena aurkeztu aurretik bidaia eskaera aurkeztu eta onartu behar dela eskatzeko.                                                                    |
|**Baimendu banaketak editatzea argitaratu aurretik**            | Aukeratu gastu-txosten baten banaketak argitaratu aurretik editatu daitezkeen ala ez.                                                                                                                 |
|**Gastuak kudeatzeko politikak ebaluatzea**                     | Aukeratu gastuak noiz ebaluatuko diren jakiteko gastu-politika bat urratu den ala ez jakiteko. Gastuak arau-hausteen arabera ebaluatu daitezke, gastu sarrera sartu eta gordetzen denean edo gastua onarpenerako aurkezten denean. Behar diren ordainagirien politika arauak gastu lerroa gordetzen denean ebaluatuko dira.                   |
|**Onartu enpresen arteko gastu lerroak**                         | Aukeratu beste pertsona juridiko batzuen gastuen sarrera baimentzeko gastuen txostenean.                                                                                                          |
|**Baimendu kreditu txartelaren gastuen truke-tasa editatzea** | Aukeratu aukera hau erabiltzaileak inportatutako kreditu txartelaren gastuen truke tasa editatzeko.                                                                        |
|**Bistaratzeko maila anitzeko hierarkia eremuak**                  | Aukeratu zein onarpen-eremu erakutsiko diren lan-fluxua esleitzeko mota hierarkia gisa ezarrita dagoenean eta hierarkia hautapena onarpen hierarkia, gastu maila anitzeko onarpena erabiltzeko ezarrita dago. Lan-fluxu baterako maila anitzeko onarpen hierarkia erabiltzen denean, hautatutako eremuak Gastuen txostenean erakutsiko dira eta editatu egin daitezke. |
|**Idatzi langilearen kreditu txartelaren zenbakia (2017ko uztailaren eguneratzea)**     | Aukeratu 15 edo 16 karaktereko zenbakia sar daitekeen eta gorde **Txartelaren IDa** eremuan **Kreditu-txartelak** langile baten orrialdea.                                                                          |

### <a name="financial"></a>Finantza-jarduerak

| **Eremua**                                                            | **Azalpena**     |
|----------------------------------------------------------------------|------------------------------------|
|**Liburu nagusiaren egunkariaren izena**                                         | Aukeratu onartutako gastuen txostenak argitaratzen diren liburuaren egunkariaren izena.            |
|**Gaitu gastuen zerga berreskuratzea**                                  | Aukeratu aukera hau gastuen gaineko zerga berreskuratzeko gaitutako gastuetarako. Aukera hau ezin da hautatu AEBetako salmenten gaineko zerga eta erabilera zergen arauak gaituta badaude.      |
|**Bidali eskudirutan aurrerakinak berehala**                                     | Aukeratu aukera hau ordaindutako eta transferentzia prozesua amaitutakoan onartutako dirua aurreratzeko. Aukera hau hautatuta ez badago, Ordaindu eta transferitu prozesuak argitaratu gabeko aldizkari orokorra sortzen du. |
|**Kontabilitate data zuzena argitaratzean**                             | Aukeratu aukera hau gastuak kontabilizatzen diren kontabilitate data eguneratzeko, uneko epea itxita edo itxita badago. Kontabilitate data hurrengo aldi irekian ezarriko da.   |
|**Onartu transakzioen multzokatzea ordainketa-metodoan zehaztutako konpentsazio-kontuan oinarrituta**      | Aukeratu aukera hau gastu-txosten baten gastu-eragiketak laburbiltzeko, gastuen ordainketa-metodoan zehaztutako konpentsazio-kontuan oinarrituta.   
|**Zergak barne**                                                   | Aukeratu aukera hau lehenespenez gastuaren zenbatekoan salmenten gaineko zerga sartzeko.             |
|**Bidaia eskaerak ixteko kargak askatu**            | Aukeratu aukera hau onartutako bidaia eskaera bat ixten denean kargatutako fondoak askatzeko.                                                                                   |
|**Baimendu bidaia-eskaerak aurrekontuaren gainditzean bidaltzea aurrekontuen erregistroa eta proiektuaren aurrekontua** | Aukeratu aukera hau langileek bidaiarako eskaerak onar ditzaten baimentzeko, nahiz eta aurrekontuen erregistroan ezarritako baimendutako aurrekontua edo proiektu baterako baimendutako aurrekontua gainditu.            |
|**Baimendu gastuen txostena aurrekontuaren gainditzean bidaltzea aurrekontuen erregistroa eta proiektuaren aurrekontua**    | Aukeratu aukera hau langileek gastuen erregistroak onar ditzaten baimentzeko, nahiz eta aurrekontuen erregistroan ezarritako baimendutako aurrekontua edo proiektu baterako baimendutako aurrekontua gainditu.                |
|**Baimendu gastuen txostena aurrekontuaren gainditzean onartzea aurrekontuen erregistroan soilik**                | Aukeratu aukera hau onarleek aurrekontuen erregistroan ezarritako baimendutako aurrekontua gainditzen duten gastuen txostenak onar ditzaten.                                                                       |

### <a name="per-diem"></a>Eguneko dieta

| **Eremua**                             | **Deskribapena**             |
|---------------------------------------|--------------------------------------------------------------------------------------|
|**Dietarako gutxieneko orduak**           | Idatzi langile batek egunean lan egin behar duen gutxieneko ordu kopurua, bidaiari lotutako gastuengatik dietak jasotzeko eskubidea izateko.  Balio hau lehenetsitako balio gisa erabiltzen da Gutxieneko orduak eguneko tasa-mailetarako eremua.                                                                                      |
|**Otorduen ehunekoa**                          | Idatzi eguneko dietaren ehuneko lehenetsia bidaiari lotutako gastuaren lehenengo eta azken egunetan erabiltzen den otorduetarako **Kalkulatu otorduen murrizketa arabera** eremua bietan ezarrita dago **Eguneko otordu mota** edo **Eguneko otordu kopurua**. Lehenengo eta azken egunetako lanaldia lanegun estandarra baino laburragoa izan daiteke. Hori dela eta, egun horietako dietaren zenbatekoa zenbateko arruntarekin alderatuta egon liteke. Portzentajea ezarrita badago 0 (zero), lehenengo eta azken egunetako kenkariak 0,00 izango dira. |
|**Hotelaren ehunekoa**                        | Idatzi eguneko dietaren ehuneko lehenetsia bidaiari lotutako gastuaren lehenengo eta azken egunetan erabiltzen den hoteletan. Lehenengo eta azken egunetako lanaldia lanegun estandarra baino laburragoa izan daiteke. Hori dela eta, egun horietako dietaren zenbatekoa zenbateko arruntarekin alderatuta egon liteke. Portzentajea ezarrita badago 0 (zero), lehenengo eta azken egunetako kenkariak 0,00 izango dira.                                              |
|**Beste ehuneko bat**                        | Idatzi eguneko dietaren ehuneko lehenetsia bidaiari lotutako gastuaren lehenengo eta azken egunetan erabiltzen den askotariko gastuetan. Lehenengo eta azken egunetako lanaldia lanegun estandarra baino laburragoa izan daiteke. Hori dela eta, egun horietako dietaren zenbatekoa zenbateko arruntarekin alderatuta egon liteke. Portzentajea ezarrita badago 0 (zero), lehenengo eta azken egunetako kenkariak 0,00 izango dira.                                                                                                     |
|**Gosarian portzentajea murriztea** | Idatzi eguneko dietak gosarian murrizten duen kopurua. Adibidez, langile batek gosari osagarria jasotzen badu, eguneko zenbatekoa ehuneko 10 murriztu nahiko zenuke.                               |
|**Bazkarian portzentajea murriztea**    | Idatzi eguneko dietak bazkarian murrizten duen kopurua. Adibidez, langile batek bazkari osagarria jasotzen badu, eguneko zenbatekoa ehuneko 15 murriztu nahiko zenuke.                                       |
|**Afarian portzentajea murriztea**   | Idatzi eguneko dietak afarian murrizten duen kopurua. Adibidez, langile batek afari osagarria jasotzen badu, eguneko zenbatekoa ehuneko 25 murriztu nahiko zenuke.                                     |
|**Kalkulatu otorduen murrizketa arabera**         | Hautatu sistemak eguneko janari murrizketa nola kalkulatu behar duen, murrizketa bidaia bakoitzeko edo eguneko otordu motaren araberakoa den edo egunean onartzen den otordu kopuruaren arabera hautatuta.|
|**Eguneko biribiltzea**                  | Aukeratu eguneko gastuetarako erabiltzen den biribiltze mota. Biribiltze normala hautatzen baduzu, 0,50 zenbatekoa duen eguneroko gastua 1,00era biribiltzen da eta 0,50 baino txikiagoa den eguneroko gastua 0,00ra biribiltzen da.                                                                                              |
|**Eguneko kalkulua**         | Aukeratu eguneko zenbatekoa egun naturalean edo 24 orduko epean oinarritzen den.       |

### <a name="fax-cover-pages"></a>Faxen azalak

| **Eremua**                      | **Deskribapena**            |
|--------------------------------|-----------------------------------------------------------------------------|
| **Instrukzioak**                   | Idatzi langileek jarraitu beharreko argibideak gastu-txostenarekin erlazionatutako ordainagiriak bidaltzeko erabiltzen den fax baten azal orria sortzen dutenean. Sakatu **Itzulpenak** botoia, erabiltzailearen hizkuntzan oinarrituta erakutsiko den hizkuntza zehatzeko testua sartzeko. |
|**Erabiltzaile IDa (barra kodearen informazioa)** | Aukeratu aukera hau langilearen identifikatzaile bakarra faxaren azalean erabiltzen den barra kodean gordetzeko.                 |
|**Barra kodea**                      | Aukeratu faxaren azalean erabiltzen den barra kodea. 39 eta 128 barra-kodeak onartzen dira Gastuen kudeaketan.               |

### <a name="anti-corruption"></a>Ustelkeriaren aurkakoa

|                 <strong>Eremua</strong>                 |                                                                                                                                                                                            <strong>Azalpena</strong>                                                                                                                                                                                             |
|--------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|  <strong>Erakutsi ustelkeriaren aurkako agiria</strong>  | Aukeratu aukera hau gastuaren txostena sortzen denean ustelkeriaren aurkako testua erakusteko. Gastu-kategoria zehatzak gaitu daitezke, ustelkeriaren aurkako egiaztagiria gastu-txostenean hautatzea eskatuko dutenak. Adibidez, gobernuko ofizialen gastuekin lotutako opari kategoria batek langileak baieztatu beharko du gastuak gobernuko funtzionarioekin zerikusia duen enpresaren politika betetzen duela baieztatzea. |
| <strong>Ustelkeriaren aurkako mezua bidaltzailearentzat</strong> |                                                                                             Idatzi langileari gastu txosten berria sortzerakoan erakutsiko zaion testua. Sakatu <strong>Itzulpenak</strong> botoia, erabiltzailearen hizkuntzan oinarrituta erakutsiko den hizkuntza zehatzeko testua sartzeko.                                                                                             |
| <strong>Ustelkeriaren aurkako mezua onartzailearentzat</strong>  |                                                                                             Idatzi langileari gastu txosten berria sortzerakoan erakutsiko zaion testua. Sakatu <strong>Itzulpenak</strong> botoia, erabiltzailearen hizkuntzan oinarrituta erakutsiko den hizkuntza zehatzeko testua sartzeko.                                                                                             |



[!INCLUDE[footer-include](../includes/footer-banner.md)]