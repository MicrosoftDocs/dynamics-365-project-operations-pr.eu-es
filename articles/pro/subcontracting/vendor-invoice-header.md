---
title: Saltzaileen fakturen goiburuko xehetasunak
description: Gai honek Microsoft-en hornitzaileen fakturaren goiburuan ematen den funtzionaltasuna azaltzen du Dynamics 365 Project Operations.
author: rumant
ms.date: 03/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 17be106d5486358ff0bbf011af3da26a4c85a274
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8575565"
---
# <a name="header-details-for-vendor-invoices"></a>Saltzaileen fakturen goiburuko xehetasunak

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Gai honek Microsoft-en hornitzaileen fakturaren goiburuan ematen den funtzionaltasuna azaltzen du Dynamics 365 Project Operations.

Proiektu-kudeatzaileek proiektuak planifikatzen eta exekutatzen dituzten heinean, baliteke azpikontratistak kontratatzea eta saltzaileei produktuak eta zerbitzuak erostea. Proiektu baten exekuzioan zehar, kostuak saltzaileekin azpikontratetan eskuratzen diren zerbitzu, material eta gastu kategorietatik sortzen dira. Saltzaileek proiektuei fakturatzen dizkiete kostu horiek saltzaileen fakturak sortuz.

Hurrengo taulak saltzaileen fakturen goiburuetako eremuei buruzko informazioa eskaintzen du Project Operations-en.

| Eremua | Deskribapenak | Inpaktu funtzionala |
| --- | --- | --- |
| Eman izena | Saltzailearen fakturaren izena. | Saltzaileen fakturen goitibeherako zerrendetan, hornitzailearen fakturaren izena lehen zutabean agertzen da, hornitzailearen faktura identifikatzen laguntzeko. Lehenespenez, saltzaileen faktura bat azpikontratu batetik sortzen denean, **Izena** Saltzaileen fakturaren eremua azpikontratuaren izenak gehi uneko datak osatzen duen balio batean ezartzen da. |
| Deskribapenak | Saltzaileen fakturan fakturatzen ari diren zerbitzu eta produktuen deskribapen laburra. | Batere ez |
| Saltzailea | Produktu eta zerbitzuen fakturazioa egiten duen enpresaren izena. Enpresa honek harreman mota bat duen kontu-erregistro bat izan behar du **Saltzailea** edo **Hornitzailea**. | <p>Hautatzen den hornitzailearen arabera, balio lehenetsiak automatikoki sartzen dira eremu hauetan:</p><ul><li>Moneta</li><li>Prezio-zerrendak</li><li>Ordainketa-baldintzak</li><li>Ordainketa helbidea</li></ul> |
| Azpikontratua | Saltzaileen fakturaren azpikontratuaren erreferentzia. | <p>Hautatzen den azpikontratuaren arabera, balio lehenetsiak automatikoki sartzen dira eremu hauetan:</p><ul><li>Moneta</li><li>Prezio-zerrendak</li><li>Ordainketa-baldintzak</li><li>Ordainketa helbidea</li></ul><p>Saltzaileen fakturaren goiburuan hautatzen den azpikontratua lehenespenez saltzaileen faktura-lerroetan sartzen da eta ezin da bertan aldatu.</p> |
| Fakturaren data | Saltzaileen faktura berresten denean sortuko diren kostu errealen data. | Fakturaren data ere erosketa-prezio-zerrenda zuzena hautatzeko erabiltzen da erlazionatutako saltzaileari atxikitako prezio-zerrendetatik edo proiektuaren parametroetatik. |
| Egoeraren arrazoia | Saltzaileen fakturaren egoera. | <p>Egoerak zehazten du saltzaileen faktura negozio-prozesuan non dagoen eta editatu daitekeen ala ez. Hona hemen erabilgarri dauden balioetako batzuk:</p><ul><li>**Zirriborroa** – Saltzaileen faktura editatu daiteke.</li><li>**Baieztatuta** – Saltzaileen faktura egiaztatu eta berretsi da. Egoera honetan dauden saltzaileen fakturak ezin dira editatu edo ezabatu.</li><li>**Prozesuan** – Saltzaileen faktura berrikusten ari da. Egoera honetan dauden saltzaileen fakturak edita daitezke, baina ezin dira ezabatu.</li><li>**Bertan behera utzita** – Saltzaileen faktura baliogabetu egin da. Egoera honetan dauden saltzaileen fakturak ezin dira editatu edo ezabatu.</li></ul> |
| Moneta | Saltzaileak fakturatzen duen produktu eta zerbitzuetarako fakturatzen duen moneta. | Azpikontratu bati erreferentzia egiten dion saltzaile-faktura batean, azpikontratuaren moneta sartzen da lehenespenez saltzaile-fakturaren dibisa gisa. Azpikontraturik aipatzen ez duen saltzaile-faktura batean, balio lehenetsia saltzaileen kontuaren erregistrotik sartzen da eta alda daiteke. Saltzaileen faktura gorde ondoren, ezingo da dirua editatu. |
| Kontratazio-unitatea | Saltzailearengandik zerbitzuak eta/edo produktuak jasotzeaz arduratzen den enpresaren dibisioa. | Batere ez |
| Ordainketa-baldintzak | Igortzen diren saltzaileen fakturetan ordaintzeko baldintzak. Lehenetsitako balioa automatikoki sartzen da saltzailearen kontuaren erregistrotik. | Azpikontratu bateko ordainketa-baldintzak azpikontratuarekin zerikusia duten saltzaileen faktura guztietan kopiatzen dira. Ordainketa baldintzak egunera daitezke saltzaileen fakturak egoera badu **Zirriborroa**. |
| Ordainketa helbidea | Ordainketak bidali behar zaizkion saltzailearen helbidea. Lehenetsitako balioa automatikoki sartzen da saltzailearen kontuaren erregistrotik. | Azpikontratu bateko ordainketa-helbidea ordainketa-helbide gisa kopiatzen da azpikontratu horretarako sortzen diren saltzaile-faktura guztietan. Ordainketa helbidea eguneratu daiteke saltzaileen fakturak egoera badu **Zirriborroa**. |
| Guztizko partziala | Saltzaileen fakturak lerrorik ez badu, idatzi fakturaren azpi-totala zergak baino lehen. Saltzaileen fakturak lerroak baditu, eremu hau irakurtzeko soilik da. Kasu honetan, erakusten den zenbatekoa saltzaileen fakturako lerro guztietako azpi-totalaren zenbatekoa da. | Batere ez |
| Zerga osoa | Saltzaileen fakturak lerrorik ez badu, idatzi azpikontratuaren gaineko zergak guztira. Saltzaileen fakturak lerroak baditu, eremu hau irakurtzeko soilik da. Kasu honetan, erakusten den zenbatekoa saltzaile-fakturako lerro guztietako zerga-kopuruen batura da. | Batere ez |
| Kopuru osoa | Kalkulatutako eremu honek saltzaileen fakturaren guztizko zenbatekoa erakusten du zergak sartu ondoren. | Batere ez |

> [!NOTE]
> Saltzaile-faktura bateko eremu hauek ezin dira aldatu saltzaile-faktura gorde ondoren: **Saltzailea**, **·**, **·**, **-unitatea**, eta **Ordainketa baldintzak**. Saltzaile-faktura batean eremu hauetan aldaketaren bat behar izanez gero, saltzaile-faktura ezabatu eta hornitzaile-faktura berri bat sortu behar duzu.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
