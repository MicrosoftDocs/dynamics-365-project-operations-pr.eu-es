---
title: Denboraren saltzailearen fakturaren lerroak
description: Artikulu honek saltzaileen faktura lerroak nola erregistratu azaltzen du azpikontratistek jartzen dituzten denbora-kostuengatik.
author: rumant
ms.date: 03/15/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 7f28af3ad76d456dddcfd8e85d968cecb773f8fc
ms.sourcegitcommit: b2224d1f3c0bd4925d647e6ca3960db81a209521
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/11/2022
ms.locfileid: "9261997"
---
# <a name="vendor-invoice-lines-for-time"></a>Denboraren saltzailearen fakturaren lerroak

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Saltzaileen faktura bat Microsoft-en Dynamics 365 Project Operations denborarako saltzaileen faktura lerroak izan ditzake. Proiektu-kudeatzaileek saltzaileen faktura-lerroak erabil ditzakete denborarako, proiektuetan azpikontratistaren denboraren kostuak erregistratzeko.

Denboraren saltzaileen faktura-lerroek denborarako azpikontratazio-lerro bati erreferentzia egin dezakete edo ez. Denboraren fakturazio-lerro batek azpikontratu bati erreferentzia egiten badio, proiektu-zuzendariek hornitzaileen faktura-lerroak fakturatzen ari den denbora parekatu eta egiaztatu ahal izango dute, azpikontratistek erregistratutako eta proiektuko arduradunek proiektuan onartutako denborarekin.

Ondorengo taulak denborari buruzko hornitzaileen faktura-lerroetako eremuei buruzko informazioa eskaintzen du.

| Eremua | Deskribapenak | Inpaktu funtzionala |
| --- | --- | --- |
| Eman izena | Saltzaileen faktura-lerroaren izena, identifikazioan laguntzeko. | Izen hau saltzaileen faktura-lerroetan oinarritutako bilaketa guztietan lehen zutabe gisa agertuko da. |
| Deskribapenak | Saltzaileak fakturatzen dituen zerbitzuen deskribapen laburra hornitzailearen faktura lerroan. | Batere ez |
| Azpikontratua | Zerbitzuak hasiera batean agindutako azpikontratua. | Saltzaileen fakturarako azpikontratu bat hautatzen denean, saltzaileen fakturako lerro guztiek hautapen hori heredatuko dute. Saltzaileen faktura batek ezin du izan azpikontratu desberdinak aipatzen dituzten hornitzaileen faktura lerroak. |
| Azpikontratazio lerroa | Zerbitzuak agindutako azpikontratazio lerroa. Hauta daitezkeen azpikontratazio-lerroen zerrenda hautatutako azpikontratuko lerroetara mugatzen da. | Saltzaileen faktura-lerro batean azpikontratazio-lerro bat hautatzen denean denborarako, balio lehenetsiak **Proiektua**, **·**, eta **Erreserba daitekeen baliabidea** eremuak azpikontratuaren lerroan dagozkion eremuetatik sartzen dira. Hautatutako azpikontratazio lerroak balioak baditu **Proiektua**, **·**, eta **Erreserbatu daiteke** eremuetan, hornitzaileen faktura-lerroko dagozkien eremuen balioak ezin dira balio horietatik desberdinak izan. |
| Transakzioaren data | Saltzaileen faktura-lerroaren benetako kostua proiektuan erregistratuko den data. | Batere ez |
| Transakzio-klasea | Balio lehenetsia **Denbora** da. | Balioa **Denbora** saltzaileen faktura lerroa azpikontratistaren denboraren fakturaren zenbatekoa erregistratzeko erabiltzen ari dela adierazten du. |
| Project | Fakturatzen ari diren zerbitzuak erabili diren proiektuaren izena. | Eremu hau beharrezkoa da eta ezin da hutsik utzi. |
| Zeregina | Fakturatzen ari diren zerbitzuak erabili ziren proiektuaren zereginaren izena. Eremu hau proiektu bat hautatzen bada soilik dago erabilgarri. Proiektuko zeregina hautatzea aukerakoa da. | Eremu hau hutsik geratzen bada, proiektuaren kudeatzaileak hornitzaileen faktura-lerroa proiektuko edozein zereginetan azpikontratistaren baliabideek erregistratzen duten denborarekin pareka dezake. Saltzaileen faktura-lerroak ez badu azpikontratazio-lerrorik aipatzen, eta eremu hau hutsik geratzen bada, saltzaileen faktura-lerroak sortzen duen kostu erreala ez da fakturatu gabeko salmenta errealekin lotuko. Kasu honetan, zereginetan oinarritutako fakturazioa konfiguratzen bada, baliteke kostuak azken bezeroari ezin izango zaizkio fakturatu. |
| Funtzioa | Denbora fakturatzen ari diren azpikontratazio baliabideen eginkizuna. | Eremu honek hornitzaileen fakturan denbora fakturatzen duten azpikontratazio baliabideek betetzen duten rola zehazten du. |
| Baliabide erreserbagarria | Ordua fakturatzen ari den azpikontratistaren izena. Erreserba daitekeen baliabide bat hautatzea aukerakoa da. | Eremu hau hutsik geratzen bada, proiektu-kudeatzaileak hornitzailearen faktura-lerroa saltzailearen faktura-lerroko edozein baliabidek erregistratzen duen denborarekin pareka dezake. |
| Kantitatea | Sartu saltzaileak fakturatzen dituen ordu kopurua faktura lerroan. |Batere ez |
| Salmenta-unitatea | Balio lehenetsia da **Denbora-unitate taldea** eta ezin da aldatu. | Batere ez |
| Unitatea | Balio lehenetsia ordu-unitatearen oinarrizko ordu-unitatea da. Balio hori alda dezakezu denbora-unitate taldeko edozein unitatetan erosteko, hala nola egunean edo astean. | -ren konbinazioa **Rola** eta **Unitatea** balioak balio lehenetsi edo kalkulatu gisa erabiliko dira **Unitatearen prezioa** saltzaileen faktura lerroko eremua. |
| Unitateko prezioa | Unitateko prezio lehenetsiak ren konbinazioa erabiltzen du **Rola** eta **Unitatea** saltzaileen faktura-lerroaren transakzio-datari dagozkion proiektuko prezioen zerrendako balioak. | Dagokion proiektuaren prezio-zerrendaren prezioa saltzaileen faktura-lerroko unitatetik desberdina den unitate batean ezartzen bada, sistemak unitate-bihurketa erabiltzen du unitate bakoitzeko prezioa kalkulatzeko. |
| Guztizko partziala | Irakurtzeko soilik den eremu hau honela kalkulatzen da *Kantitatea*&times;*Unitatearen prezioa*, bietan balioak sartzen badira **Kantitatea** eremua eta **Unitatearen prezioa** eremua. Eremu horietako bat edo biak hutsik badaude, eremu honetan balio bat sar dezakezu. | Batere ez |
| Salmenten zerga | Idatzi salmenta-zergaren zenbatekoa. | Batere ez |
| Kopuru osoa | Saltzaileen faktura-lerroaren guztizko zenbatekoa, zergak barne. Eremu hau honela kalkulatzen da *Azpitotala* + *Salmenta zerga*. | Batere ez |

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
