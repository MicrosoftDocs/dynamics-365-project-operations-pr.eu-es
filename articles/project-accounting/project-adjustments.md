---
title: Proiektuaren doikuntzak
description: Artikulu honek proiektuaren doikuntzari buruzko informazioa eskaintzen du.
author: ryansandness
ms.date: 11/09/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ryansandness
ms.openlocfilehash: 52a262adce2bb624bc088e50858e25824f845e5c
ms.sourcegitcommit: bb03ac64e01112c93bb24035a51653a0a88cd5fc
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/18/2022
ms.locfileid: "9788359"
---
# <a name="project-adjustments"></a>Proiektuaren doikuntzak

_**Honi aplikatzen zaio:** Izakinen edo ekoizpenean oinarritutako egoeretarako Project Operations_

## <a name="adjustments-overview"></a>Doikuntzen ikuspegi orokorra

Microsoft Dynamics 365 Project Operations konfigura dezakezu erabiltzaileek argitaratutako transakzioetan aldaketak egin ditzaten. Proiektuaren transakzioak banan-banan doi ditzakezu edo aldi berean transakzio anitz hauta ditzakezu proiektuko transakzio guztien zerrenda batean. Proiektuaren doikuntzak erabiltzen dira, adibidez, fakturagarria den egoera masiboki eguneratzeko, konfigurazio-aldaketa baten ondoren kostua berriro kalkulatzeko edo finantzaketa-iturriak eguneratzeko.

Erabiltzaileek proiektuaren doikuntza funtzionalitatera hainbat modutara atzi dezakete:

-  **Egokitu transakzioak** orria erabiliz, **Proiektuen kudeaketa eta kontabilitatea** \> **Konfiguraziotik atzi daitekeen**.
- By using the **Adjustment** button on the **Posted project transactions** page that can be accessed from **Project Management and accounting** \> **Transactions**.
- Proiektu baten testuinguruan **Argitaratutako proiektuaren transakzioak** orriko **Doikuntza** botoia erabiliz. Orri honetara **Proiektuen kudeaketa eta kontabilitatea** \> **Proiektu guztiak** tik atzi daiteke.

To allow for adjustments you must enable one or more transaction statuses from **Project Management and accounting** \> **Project Management and accounting paramaters** on the **General** tab under the section **Allow adjustment of transaction status**. Transakzio-egoeren adibideak dira argitaratutako transakzioak, fakturatutako transakzioak edo ezabatutako transakzioak.  **Ez** n ezarrita dagoen edozein transakzio-egoerak egoera horretako transakzioak izango ditu, doikuntza-prozesuan doikuntzarako hautagarri gisa agertuko ez direnak.

 **Sortu beti doikuntza-transakzioa**  izeneko konfigurazio-aukera eskuragarri dago une honetan Proiektuen kudeaketa eta kontabilitate parametroetan. Aukera hau desgaitu dezakezu jatorrizko transakzioa eguneratzeko, agertokien azpimultzo batean transakzio berriak sortu beharrean. Parametro hau 2023ko martxoaren 1erako zaharkituta geratuko dela iragarri da. 2023ko martxoaren 1etik aurrera, sistemak aukera gaituta egongo balitz bezala jokatuko du beti.

## <a name="adjustments-process-flow"></a>Egokitzapen prozesuaren fluxua

Hurrengo urratsek doikuntzak prozesatzeko ohiko fluxua erakusten dute.

1. Ireki **Proiektuaren doikuntzak** orrialdea.
2. Hautatu **Hautatu** doikuntzarako espero diren irizpideak betetzen dituzten transakzioak bilatzeko.
3. Transakzioen zerrendan, hautatu transakzio guztiak edo transakzioen azpimultzo bat doitzeko.
4. Hautatu **Egokitu** eta aldatu lerroko atributuak. Bestela, transakzioen sarreran balioak eskuz zehaztu badira, sistemaren balio lehenetsiak sartzea hauta dezakezu.
5. Transakzioen zerrenda itzultzen da, eta kontrol-marka bat agertzen da **Egokitzapenaren zain** zutabean, aldaketak non egin diren adierazteko. Zain dauden aldaketak dituzten doikuntzak orriaren beheko erdian agertzen dira. Bertan, aurreko orrian erakutsitakoaz gain, aldaketa zehatzak egin ditzakezu.
6. Hautatu **Argitaratu** doikuntza-transakzioak argitaratzeko.

Konfigurazioaren arabera, normalean transakzio berriak sortzen dira doikuntzarako.

- Jatorrizko transakzioaren **Fakturaren egoera** eremua **Egokitua** gisa ezarrita dago.
- Berraztertzeko transakzio bat sortzen da jatorrizko transakzioa alderantzikatzeko, eta **Egoera** eremua **Egokitua** gisa ezartzen da.
- Egokitzapen prozesuan egindako aldaketak dituen transakzio berri bat sortzen da.

### <a name="selecting-multiple-posted-project-transactions-at-a-time-for-adjustments-and-credit-notes"></a>Aldi berean argitaratutako hainbat proiektu-transakzio hautatzea doikuntzak eta kreditu-oharrak egiteko

10.0.30 bertsioan sartu zen eginbide berri batek aldi berean doitzeko hainbat transakzio hautatzea ahalbidetzen du **Argitaratutako proiektuaren transakzioak** orritik.

Ezaugarri hau erabili aurretik, zure sisteman gaituta egon behar da. Administratzaileek **Eginbideak kudeatzeko** laneko eremua erabil dezakete funtzioaren egoera egiaztatzeko eta behar izanez gero gaitzeko.  **Eginbideen kudeaketa** laneko eremuan, bilatu eta hautatu **Hautatu anitz argitaratutako proiektu-transakzioak doikuntzak eta kreditu-oharrak**, eta gero hautatu **Gaitu orain**.

Ezaugarri honek funtzio gako hauek gaitzen ditu:

- Proiektu baten barruan argitaratutako transakzio-orritik atzi daiteke lehendik dagoen **Doikuntza** botoia erabiliz.
- Errenkada anitzeko aukeraketa kontrola gaitzen du **Argitaratutako proiektuaren transakzioak** orrian. Zerrenda-orrian iragazkiak aplika ditzakezu eta zure erregistroak hauta ditzakezu doikuntzak hasi aurretik.
-  **Doikuntza** botoia desgaitzen du transakzio bakarren bat doitu ezin bada edo kreditu-oharrak eta aldizkariak batera hautatzen badituzu banan-banan beharrean.
- Errenkada anitzeko aukeraketa kontrola gehituta, zintako **Konprometitutako kostua** esteka ez da desgaitzen errenkada bat baino gehiago hautatzen badira.
- Abisu-mezu hau gehitzen du: "Egokitzatzeko (hautatutako zenbakia) erregistro baino gehiago hautatu dituzu. Baliteke ekintza honekin aurrera egiteak denbora pixka bat behar izatea. Ziur ekintza honekin jarraitu nahi duzula?"

Ezaugarri honek 2. urratsa ere kentzen du artikulu honetan lehenago deskribatu zen prozesu-fluxutik. Hori dela eta, **Egokitu transakzioak** orrialdea ireki baino lehen hautatutako transakzio guztiak doitzeko transakzioen zerrendan sartuko dira. Ez duzu  **Hautatu** botoia erabili behar haiek bilatzeko.

> [!NOTE] 
> Eginbide hau desgaituta badago ere, hala ere, hainbat erregistro hauta ditzakezu doitzeko. Hala ere, erregistro bakarra *hautatuta geratuko da*, eta **Hautatu transakzioak** elkarrizketa-koadroa agertuko da hau hautatu eta berehala. doikuntza irekiak.

## <a name="adjustment-transaction-statuses-that-can-be-enabled-or-disabled-for-adjustments"></a>Doikuntzak egiteko gaitu edo desgaitu daitezkeen doikuntza-transakzio-egoerak

The following statuses can be enabled or disabled on the **General** tab of the **Project management and accounting parameters** page:

- Argitaratuta
- Faktura-proposamena
- Fakturatuta
- Aurreikusita
- Ezabatuta
- Hasierako balantzea (ordua)

## <a name="adjustment-parameters"></a>Doikuntza-parametroak

These parameters are listed on the **Project management and accounting parameters** page on the **General** tab under the **Adjustment** group and will modify behavior for how adjustments are processed. 

| Parametroaren izena | Deskribapenak |
|----------------|-------------
| Sortu beti doikuntza-transakzioa | Parametro hau gaituta badago, doikuntza-prozesuak beti sortuko du atzera-eragiketa berri bat eta doitutako transakzio berria finantza- edo txosten-eragin bat dagoenean. Parametroa desgaituta badago, doikuntza-prozesuak jatorrizko transakzioa eguneratuko du atzerakada eta transakzio berria sortu beharrean, transakzio testua eguneratzeko adibidez. |
| Automatikoki eguneratzea eremua | Parametro hau gaituta badago, sistemak kostu-prezioa eta salmenta-prezioa berriro kalkulatuko ditu. |
| Erabili doikuntza data proiektu berri gisa | Parametro hau transakzioak etorkizuneko aldi fiskal batera eramateko erabiltzen da sistemak funtzio hau onartzen zuen aurretik. Ez dugu gomendatzen hura erabiltzea, transakzioaren negozio-data aldatzen duelako eta etorkizuneko bertsio batean zaharkituta geratuko delako. |
| Onartu jarduera itxiak | Normalean, transakzioak ezin dira sortu itxitako jardueretarako. Parametro hau gaituta badago, portaera hori gainidatziko da. Beraz, doikuntzak sor daitezke jarduera itxietarako. |
