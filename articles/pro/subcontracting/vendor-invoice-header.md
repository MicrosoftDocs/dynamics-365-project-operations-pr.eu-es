---
title: Saltzaileen fakturen goiburuaren xehetasunak
description: Artikulu honek saltzaileen fakturaren goiburuan ematen den funtzionaltasuna azaltzen du Microsoft Dynamics 365 Project Operations-en.
author: rumant
ms.date: 03/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: d575ebe44e45411e1009c64e9b575777b741322f
ms.sourcegitcommit: b2224d1f3c0bd4925d647e6ca3960db81a209521
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/11/2022
ms.locfileid: "9261638"
---
# <a name="header-details-for-vendor-invoices"></a>Saltzaileen fakturen goiburuaren xehetasunak

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Artikulu honek saltzaileen fakturaren goiburuan ematen den funtzionaltasuna azaltzen du Microsoft Dynamics 365 Project Operations-en.

Proiektu kudeatzaile batek proiektuak planifikatu eta exekutatzen dituen heinean, azpikontratistak kontratatu eta produktuak eta zerbitzuak saltzaileei eros ditzakete. Proiektu baten exekuzioan zehar, kostuak saltzaileekin azpikontratetan eskuratzen diren zerbitzu, material eta gastu kategorietatik sortzen dira. Saltzaileek proiektuei fakturatzen dizkiete kostu horiek saltzaileen fakturak sortuz.

Ondorengo taulan fitxategien eremuei buruzko informazioa ematen da Project Operations-eko saltzaileen fakturaren goiburuan.

| Eremua | Deskribapenak | Inpaktu funtzionala |
| --- | --- | --- |
| Eman izena | Saltzailearen fakturaren izena. | Saltzailearen fakturaren goitibeherako zerrenda guztietan, saltzailearen fakturaren izena lehen zutabean azaltzen da saltzailearen kontratua identifikatzen laguntzeko. Lehenespenez, saltzaileen faktura bat azpikontratu batetik sortzen denean, **Izena** Saltzaileen fakturaren eremua azpikontratuaren izenak gehi uneko datak osatzen duen balio batean ezartzen da. |
| Deskribapenak | Saltzaileen fakturan fakturatzen ari diren zerbitzuen eta produktuen deskribapen laburra. | Batere ez |
| Saltzailea | Produktuak eta zerbitzuak fakturatzen ari den enpresaren izena. Enpresak **Saltzailea** edo **Hornitzailea** motako erlazioa duen kontuaren erregistro bat izan behar du. | <p>Aukeratutako saltzailearen arabera, balio lehenetsiak automatikoki sartzen dira eremu hauetarako:</p><ul><li>Moneta</li><li>Prezio-zerrendak</li><li>Ordainketa-baldintzak</li><li>Ordainketa-helbidea</li></ul> |
| Azpikontratua | Saltzaileen fakturaren azpikontratuaren erreferentzia. | <p>Aukeratutako azpikontratuaren arabera, balio lehenetsiak automatikoki sartzen dira eremu hauetarako:</p><ul><li>Moneta</li><li>Prezio-zerrendak</li><li>Ordainketa-baldintzak</li><li>Ordainketa-helbidea</li></ul><p>Saltzaileen fakturaren goiburuan hautatzen den azpikontratua lehenespenez saltzaileen faktura lerroetan sartzen da eta ezin da bertan aldatu.</p> |
| Fakturaren data | Saltzaileen faktura berresten denean sortuko diren kostu errealen data. | Fakturaren data erosketa prezioen zerrenda zuzena hautatzeko erabiltzen da, erlazionatutako saltzaileari atxikitako prezioen zerrendetatik edo proiektuaren parametroetatik. |
| Egoeraren arrazoia | Saltzailearen fakturaren egoera. | <p>Egoerak zehazten du non dagoen saltzailearen faktura negozio prozesuan eta ea editatu daitekeen. Eskuragarri dauden balio batzuk:</p><ul><li>**Zirriborroa** – Saltzailearen faktura editatu daiteke.</li><li>**Baieztatuta** – Saltzaileen faktura egiaztatu eta berretsi da. Egoeran horretan dauden Saltzailearen fakturak ezin dira editatu edo ezabatu.</li><li>**Prozesuan** – Saltzaileen faktura berrikusten ari da. Egoeran horretan dauden Saltzailearen fakturak editatu daitezke, baina ezin dira ezabatu.</li><li>**Bertan behera utzita** – Saltzaileen faktura baliogabetu egin da. Egoeran horretan dauden Saltzailearen fakturak ezin dira editatu edo ezabatu.</li></ul> |
| Moneta | Saltzaileak saltzailearen fakturako produktu eta zerbitzuengatik fakturatzen duen moneta. | Azpikontratu bati erreferentzia egiten dion saltzaile-faktura batean, azpikontratuaren moneta sartzen da lehenespenez saltzaile-fakturaren dibisa gisa. Azpikontraturik aipatzen ez duen saltzaile-faktura batean, balio lehenetsia saltzaileen kontuaren erregistrotik sartzen da eta alda daiteke. Saltzaileen faktura gorde ondoren, dirua ezin da editatu. |
| Kontratazio-unitatea | Saltzailearengandik zerbitzuak eta/edo produktuak jasotzeaz arduratzen den enpresaren dibisioa. | Batere ez |
| Ordainketa-baldintzak | Ematen diren saltzaileen fakturen ordainketa baldintzak. Lehenetsitako balioa automatikoki sartzen da saltzailearen kontuaren erregistrotik. | Azpikontratazioaren ordainketa baldintzak azpikontratu honekin erlazionatutako saltzaileen faktura guztietan kopiatzen dira. Ordainketa-baldintzak egunera daitezke saltzailearen fakturak egoera badu **Zirriborroa**. |
| Ordainketa-helbidea | Ordainketak bidali behar zaizkion saltzailearen helbidea. Lehenetsitako balioa automatikoki sartzen da saltzailearen kontuaren erregistrotik. | Azpikontratako ordainketa helbidea azpikontratu honetarako sortzen diren saltzaile faktura guztietara ordaindutako helbide gisa kopiatzen da. Ordainketa-helbideak egunera daitezke saltzailearen fakturak egoera badu **Zirriborroa**. |
| Guztizko partziala | Saltzailearen faktura batek lerroak ez baditu, sartu fakturaren azpitotala zergak baino lehen. Saltzailearen fakturak lerroak baditu, eremu hau soilik irakurtzen da. Kasu horretan, erakusten den zenbatekoa saltzailearen fakturako lerro guztietako azpitotala da. | Batere ez |
| Zergak guztira | Azpikontratu batek lerroak ez baditu, sartu guztizko zergak azpikontratuan. Saltzailearen fakturak lerroak baditu, eremu hau soilik irakurtzen da. Kasu horretan, erakusten den zenbatekoa saltzailearen fakturako lerro guztietako zerga kopuruen batura da. | Batere ez |
| Zenbatekoa guztira | Kalkulatutako eremu honek zergak sartu ondoren saltzailearen fakturaren zenbateko osoa erakusten du. | Batere ez |

> [!NOTE]
> Saltzaile-faktura bateko eremu hauek ezin dira aldatu saltzaile-faktura gorde ondoren: **Saltzailea**, **Azpikontratazioa**, **Moneta**, **Kontratazio-unitatea**, eta **Ordainketa baldintzak**. Saltzaile-faktura batean eremu hauetan aldaketaren bat behar izanez gero, saltzaile-faktura ezabatu eta hornitzaile-faktura berri bat sortu behar duzu.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
