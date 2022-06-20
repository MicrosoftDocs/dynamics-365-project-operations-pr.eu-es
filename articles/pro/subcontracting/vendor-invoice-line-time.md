---
title: Denboraren saltzailearen fakturaren lerroak
description: Artikulu honetan, hornitzailearen faktura-lerroak nola erregistratu azaltzen da, azpikontratistek inbertitzen dituzten denbora-kostuetarako.
author: rumant
ms.date: 03/15/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 0b81d2884580e9054457906627c1f9101f435524
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8927516"
---
# <a name="vendor-invoice-lines-for-time"></a>Denboraren saltzailearen fakturaren lerroak

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Microsoften Dynamics 365 Project Operations hornitzailearen faktura batek hornitzailearen faktura-lerroak izan ditzake denboraren arabera. Proiektu-kudeatzaileek hornitzailearen faktura-lerroak erabili ahal izango dituzte denboran zehar azpikontratistaren denbora-kostuak proiektuetan erregistratzeko.

Hornitzailearen faktura-lerroek, denborarako, azpikontrato-linea bati erreferentzia egin diezaiokete edo ez. Hornitzailearen faktura-lerro batek denborarako azpikontratu bati egiten badio erreferentzia, proiektu-kudeatzaileek berdindu eta egiaztatu ahal izango dute hornitzailearen faktura-lerroak fakturatzen duen denbora, azpikontratistek erregistratutako eta proiektu-kudeatzaileek proiektuan onartutako denboraren aurka.

Hurrengo taulan, hornitzailearen faktura-lerroen eremuei buruzko informazioa ematen da.

| Eremua | Deskribapenak | Inpaktu funtzionala |
| --- | --- | --- |
| Eman izena | Saltzaileen faktura-lerroaren izena, identifikazioan laguntzeko. | Izen hau saltzaileen faktura-lerroetan oinarritutako bilaketa guztietan lehen zutabe gisa agertuko da. |
| Deskribapenak | Saltzaileak fakturatzen dituen zerbitzuen deskribapen laburra hornitzaileen faktura lerroan. | Batere ez |
| Azpikontratua | Zerbitzuak hasiera batean agindutako azpikontratua. | Saltzaileen fakturarako azpikontratu bat hautatzen denean, saltzaileen fakturako lerro guztiek hautapen hori heredatuko dute. Saltzaile-faktura batek ezin du izan azpikontratu desberdinak aipatzen dituzten hornitzaile-faktura-lerroak. |
| Azpikontrato-lerroa | Zerbitzuak agindutako azpikontratazio lerroa. Hauta daitezkeen azpikontratazio-lerroen zerrenda hautatutako azpikontratuko lerroetara mugatzen da. | Hornitzailearen faktura-lerro batean azpikontratu-linea bat aukeratzen denean, Proiektu **·**, Rol **eta** Erreserbagarri baliabide-eremuetarako **aurrez** zehaztutako balioak azpikontrato-lineako eremuetatik sartzen dira. Hautatutako azpikontratu-lerroak Proiektu **,** Rol **eta** Erreserbagarriko **arloetako** balioak baditu, hornitzailearen faktura-lerroko eremuetako balioak ezin dira balore horietatik ezberdinak izan. |
| Transakzioaren data | Saltzaileen faktura-lerroaren benetako kostua proiektuan erregistratuko den data. | Batere ez |
| Transakzio-klasea | Balio lehenetsia **Denbora** da. | Denbora **balioaren** arabera, hornitzailearen faktura-lerroa azpikontratistaren denboraren fakturaren zenbatekoa erregistratzeko erabiltzen ari da. |
| Project | Fakturatzen ari diren zerbitzuak erabili diren proiektuaren izena. | Eremu hau beharrezkoa da eta ezin da hutsik utzi. |
| Zeregina | Fakturatzen ari diren zerbitzuak erabili diren proiektuaren atazaren izena. Eremu hau proiektu bat hautatzen bada soilik dago erabilgarri. Proiektuko zeregina hautatzea aukerakoa da. | Arlo hori zuri uzten bada, proiektu-kudeatzaileak bat egin dezake hornitzailearen faktura-lerroarekin, azpikontratistaren baliabideek proiektuaren edozein zereginetan erregistratzen duten denborarekin. Saltzaileen faktura-lerroak ez badu azpikontratazio-lerrorik aipatzen, eta eremu hau hutsik geratzen bada, hornitzaile-faktura-lerroak sortzen duen kostu erreala ez da fakturatu gabeko salmenta-errealekin lotuko. Kasu honetan, zereginetan oinarritutako fakturazioa konfiguratzen bada, baliteke kostuak ezin izango zaizkiola azken bezeroari fakturatu. |
| Funtzioa | Denbora fakturatzen ari diren azpikontratatutako baliabideen zeregina. | Arlo horretan, hornitzailearen fakturan fakturatzen den azpikontratoaren baliabideek egiten duten rola zehazten da. |
| Baliabide erreserbagarria | Denbora fakturatzen ari den azpikontratistaren izena. Baliabide erreserbagarri bat hautatzea aukerakoa da. | Arlo hori zuri uzten bada, proiektu-kudeatzaileak hornitzailearen faktura-lerroa hornitzailearen faktura-lerroan hornitzailearen faktura-lerroan hornitzailearen edozein baliabide erregistratzen duen denborarekin bat egin dezake. |
| Kantitatea | Sartu hornitzailea faktura-lerroan fakturatzen ari den denbora-kopurua. |Batere ez |
| Salmenta-unitatea | Aurrez zehaztutako balioa denbora-unitateen **taldea da** eta ezin da aldatu. | Batere ez |
| Unitatea | Aurrez zehaztutako balioa ordu-unitateen taldearen ordu-unitatea da. Balio hori alda dezakezu denbora-unitateko edozein unitatetan erosteko, hala nola egun edo astean. | rol- eta **unitate-balioen** **konbinazioa aldez aurretik zehaztutako edo kalkulatutako balio gisa erabiliko da, hornitzailearen faktura-lerroan, unitateko prezioaren** eremurako **.** |
| Unitateko prezioa | Aurrez zehaztutako unitate-prezioan, hornitzailearen faktura-lerroaren **transakzio-datan aplikatzen den proiektuaren prezioen zerrendaren rol** - eta **unitate-balioen** konbinazioa erabiltzen da. | Dagokion proiektuaren prezio-zerrendaren prezioa saltzaileen faktura lerroko unitatetik desberdina den unitate batean ezartzen bada, sistemak unitate-bihurketa erabiltzen du unitate bakoitzeko prezioa kalkulatzeko. |
| Guztizko partziala | Irakurtzeko soilik den eremu hau honela kalkulatzen da *Kantitatea*&times;*Unitatearen prezioa*, bietan balioak sartzen badira **Kantitatea** eremua eta **Unitatearen prezioa** eremua. Eremu horietako bat edo biak hutsik badaude, eremu honetan balio bat sar dezakezu. | Batere ez |
| Salmenten zerga | Idatzi salmenta-zergaren zenbatekoa. | Batere ez |
| Zenbateko osoa | Saltzaileen faktura-lerroaren guztizko zenbatekoa, zergak barne. Eremu hau honela kalkulatzen da *Azpitotala* + *Salmenta zerga*. | Batere ez |

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
