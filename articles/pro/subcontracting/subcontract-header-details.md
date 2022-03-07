---
title: Azpikontratuen goiburuaren xehetasunak
description: Gai honek Project Operations azpikontratatutako goiburuan emandako funtzionalitatea azaltzen du.
author: rumant
ms.date: 09/14/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ee863d31b45e7de962488fe804202ddfe580eb04
ms.sourcegitcommit: 083e3d219cd5126eecb74debb1b70b361680b1f6
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/18/2021
ms.locfileid: "7501311"
---
# <a name="header-details-for-subcontracts"></a>Azpikontratuen goiburuaren xehetasunak

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Gai honek Dynamics 365 Project Operations azpikontratatutako goiburuan emandako funtzionalitatea azaltzen du.

Proiektu kudeatzaile batek proiektuak planifikatu eta exekutatzen dituen heinean, azpikontratistak kontratatu eta produktuak eta zerbitzuak saltzaileei eros ditzakete. Proiektu kudeatzaile batek produktuak edo zerbitzuak erosi behar dituenean, azpikontrata sor dezakete Project Operations.

Azpikontrata sortzeko, jarraitu urrats hauek.

1. Nabigazio panelean, hautatu **Azpikontratak**, eta **Azpikontrata** orrialdea, hautatu **Berria**.
2. Sartu beharrezko informazioa eta, ondoren, hautatu **Gorde** aukeran.

    Hurrengo taulan **Azpikontratatu goiburua** orriko eremuei buruzko informazioa ematen da.

    | Eremua | Deskribapenak |Inpaktu funtzionala |
    |---|------|---| 
    | Izena | Azpikontratuaren izena. | Azpikontrata goitibeherako zerrenda guztietan, azpikontratuaren izena lehen zutabean azaltzen da azpikontratua identifikatzen laguntzeko. | 
    | Deskribapenak | Azpikontratuan erosten ari diren zerbitzuen eta produktuen deskribapen laburra. | Batere ez |
    | Saltzailea | Produktuak eta zerbitzuak erosten ari den enpresaren izena. Erregistroaren kontuak **Saltzailea** edo **Hornitzailea** motako erlazioa du. | Aukeratutako saltzailearen arabera, balio lehenetsiak automatikoki sartzen dira eremu hauetarako:<br/> **• Moneta** </br> **• Prezio-zerrendak** </br> **• Ordainketa-baldintzak**</br> **• Ordainketa-helbidea**</br> **• Fakturazio-helbidea**</br> **• Fakturaziorako izena** </br>**• Saltzailearen kontuaren kudeatzailea**|
    | Azpikontratuaren data | Azpikontratua sortzen den eguna. | Azpikontratazio data erosketa prezioen zerrenda zuzena hautatzeko erabiltzen da, erlazionatutako saltzaileari atxikitako prezioen zerrendetatik edo proiektuaren parametroetatik. |
    | Egoeraren arrazoia | Azpikontratuaren egoera. | Egoerak zehazten du non dagoen azpikontratua negozio prozesuan eta ea editatu daitekeen. <br/>Balioak honakoak dira:<br>•**Zirriborroa**: Azpikontratua editatu daiteke. **Zirriborroa** egoera duten azpikontratuak soilik editatu ditzakezu.<br/>•**Baieztatuta**: Saltzailearekin negoziatzea amaitu da eta azpikontratua entregatzeko onartzen da. <br/>•**Itxita**: Azpikontrataren entrega amaitu da.<br/>•**Bertan behera utzita**: Azpikontratua bertan behera utzi da eta ez da aurreikusten entrega.  | 
    | Moneta | Produktuak eta zerbitzuak erosten diren moneta. Lehenetsitako balioa automatikoki saltzailearen kontutik sartzen da, baina alda daiteke. | Azpikontratazioaren moneta erosketa prezioen zerrenda hautatzeko erabiltzen da, erlazionatutako saltzaileari atxikitako prezioen zerrendetatik edo proiektuaren parametroetatik. Beste moneta bateko prezio zerrendak ezin dira azpikontratarekin lotu. Saltzaileen baliabideek azpikontrata honetatik entregatzen dituzten denbora, gastuak eta materialen kostua moneta honetan erregistratzen dira proiektuan. Azpikontratazio erregistroa gorde ondoren, azpikontratako moneta ezin da aldatu.|
    | Kontratatzailea | Saltzailearekin erosketa kontratua edo azpikontratua egiten ari den enpresaren banaketa. | Batere ez |
    | Ordainketa-baldintzak | Azpikontratu honetan ematen diren saltzaileen fakturen ordainketa baldintzak. Lehenetsitako balioa automatikoki sartzen da saltzailearen kontuaren erregistrotik. | Azpikontratazioaren ordainketa baldintzak azpikontratu honekin erlazionatutako saltzaileen faktura guztietan kopiatzen dira. Ordainketa-baldintzak egunera daitezke azpikontratak egoera badu **Zirriborroa**. | 
    | Ordainketa-helbidea | Ordainketak bidali behar zaizkion saltzailearen helbidea. Lehenetsitako balioa automatikoki sartzen da saltzailearen kontuaren erregistrotik. | Azpikontratako ordainketa helbidea azpikontratu honetarako sortzen diren saltzaile faktura guztietara ordaindutako helbide gisa kopiatzen da. Ordainketa-helbideak egunera daitezke azpikontratak egoera badu **Zirriborroa**.|
    | Fakturaziorako izena | Faktura bidaliko duen saltzailearen enpresako pertsonaren edo zatiketaren izena. Lehenetsitako balioa automatikoki sartzen da saltzailearen kontuaren erregistrotik. | Azpikontratazioaren **Fakturatu izen honi** balioa azpikontratu honekin erlazionatutako saltzaileen faktura guztietan kopiatzen da. Eremu hau egunera daiteke azpikontratak egoera badu **Zirriborroa**.|
    | Fakturaziorako helbidea | Saltzailearen fakturetan erabiltzen den helbidea. Lehenetsitako balioa automatikoki sartzen da saltzailearen kontuaren erregistrotik. | Helbide hau azpikontratu honetarako sortzen diren saltzaileen fakturetako "fakturatik" helbidea da. |
    | Guztizko partziala | Azpikontrata batek lerroak ez baditu, sartu ordena azpitotala zergak baino lehen. Azpikontratazioak lerroak baditu, eremu hau soilik irakurtzen da. Erakusten den zenbatekoa azpikontratako lerro guztietako azpitotala da. | Batere ez |
    | Zergak, guztira | Azpikontrata batek lerroak ez baditu, sartu azpikontrata honen guztizko zergak. Azpikontratazioak lerroak baditu, eremu hau soilik irakurtzen da. Erakusten den zenbatekoa azpikontratako lerro guztietako zergen batura da. | Batere ez |
    | Zenbatekoa guztira | Kalkulatutako eremu honek zergak sartu ondoren azpikontrataren zenbateko osoa erakusten du. | Batere ez |
    | Berretsitako data | Azpikontratua berretsi zeneko data. | Batere ez |
    | Eskatzailea | Lehenespenez, eremu hau azpikontratua sortzen duen erabiltzailearen izena da. Hala ere, azpikontratuaren sortzaileak balioa alda dezake azpikontratua sortzen ari den pertsona adierazteko. | Batere ez |
    | Saltzailearen kontuaren kudeatzailea | Saltzailearen kontuaren lehen kontaktuaren izena. Lehenetsitako balioa automatikoki sartzen da saltzailearen kontuaren erregistrotik. Azpikontrataren saltzailearen kontu kudeatzaile gisa beste kontaktu bat hauta dezakezu. | Prezioen negoziazioen ondorioz azpikontratetan aldaketak egiten direnean posta elektroniko bidezko alertak konfigura ditzakezu. |
