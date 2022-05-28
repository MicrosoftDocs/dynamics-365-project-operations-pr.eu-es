---
title: Saltzaileen faktura lerroak denborarako
description: Gai honek azpikontratistek jartzen dituzten denbora-kostuen saltzaileen faktura lerroak nola erregistratu azaltzen du.
author: rumant
ms.date: 03/15/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: ac598dff7b0b4a29ac0397a31130ada3b197fe44
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8597185"
---
# <a name="vendor-invoice-lines-for-time"></a>Saltzaileen faktura lerroak denborarako

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Saltzaileen faktura bat Microsoft-en Dynamics 365 Project Operations denborarako saltzaileen faktura lerroak izan ditzake. Proiektu-kudeatzaileek saltzaileen faktura-lerroak erabil ditzakete denborarako, proiektuetan azpikontratistaren denboraren kostuak erregistratzeko.

Denboraren saltzaileen faktura-lerroek denborarako azpikontratazio-lerro bati erreferentzia egin dezakete edo ez. Denboraren saltzaileen faktura-lerro batek azpikontratu bati erreferentzia egiten badio, proiektu-zuzendariek saltzaileen faktura-lerroak fakturatzen ari den denbora parekatu eta egiaztatu ahal izango dute, azpikontratistek erregistratutako eta proiektuko arduradunek proiektuan onartutako denborarekin.

Ondorengo taulak denborari buruzko hornitzaileen faktura-lerroetako eremuei buruzko informazioa eskaintzen du.

| Eremua | Deskribapenak | Inpaktu funtzionala |
| --- | --- | --- |
| Eman izena | Saltzaileen faktura-lerroaren izena, identifikazioan laguntzeko. | Izen hau saltzaileen faktura-lerroetan oinarritutako bilaketa guztietan lehen zutabe gisa agertuko da. |
| Deskribapenak | Saltzaileak fakturatzen dituen zerbitzuen deskribapen laburra hornitzaileen faktura lerroan. | Batere ez |
| Azpikontratua | Zerbitzuak hasiera batean agindutako azpikontratua. | Saltzaileen fakturarako azpikontratu bat hautatzen denean, saltzaileen fakturako lerro guztiek hautapen hori heredatuko dute. Saltzaile-faktura batek ezin du izan azpikontratu desberdinak aipatzen dituzten hornitzaile-faktura-lerroak. |
| Azpikontratazio lerroa | Zerbitzuak agindutako azpikontratazio lerroa. Hauta daitezkeen azpikontratazio-lerroen zerrenda hautatutako azpikontratuko lerroetara mugatzen da. | Saltzaileen faktura-lerro batean azpikontratazio-lerro bat hautatzen denean denborarako, balio lehenetsiak **Proiektua**, **·**, eta **Erreserba daitekeen baliabidea** eremuak azpikontratuaren lerroan dagozkion eremuetatik sartzen dira. Hautatutako azpikontratazio-lerroak balioak baditu **Proiektua**, **·**, eta **Erreserbatu daiteke** eremuetan, hornitzaileen faktura-lerroko dagozkien eremuen balioak ezin dira balio horietatik desberdina izan. |
| Transakzioaren data | Saltzaileen faktura-lerroaren benetako kostua proiektuan erregistratuko den data. | Batere ez |
| Transakzio-klasea | Balio lehenetsia **Denbora** da. | Balioa **Denbora** saltzaileen faktura-lerroa azpikontratistaren denboraren faktura-kopurua erregistratzeko erabiltzen ari dela adierazten du. |
| Project | Fakturatzen ari diren zerbitzuak erabili diren proiektuaren izena. | Eremu hau beharrezkoa da eta ezin da hutsik utzi. |
| Zeregina | Fakturatzen ari diren zerbitzuak erabili diren proiektuaren atazaren izena. Eremu hau proiektu bat hautatzen bada soilik dago erabilgarri. Proiektuko ataza hautatzea aukerakoa da. | Eremu hau hutsik geratzen bada, proiektuaren kudeatzaileak hornitzaileen faktura-lerroa proiektuko edozein zereginetan azpikontratistaren baliabideek erregistratzen duten denborarekin pareka dezake. Saltzaileen faktura-lerroak ez badu azpikontratazio-lerrorik aipatzen, eta eremu hau hutsik geratzen bada, hornitzaile-faktura-lerroak sortzen duen kostu erreala ez da fakturatu gabeko salmenta-errealekin lotuko. Kasu honetan, zereginetan oinarritutako fakturazioa konfiguratzen bada, baliteke kostuak ezin izango zaizkiola azken bezeroari fakturatu. |
| Funtzioa | Denbora fakturatzen ari diren azpikontratazio baliabideen eginkizuna. | Eremu honek hornitzaileen fakturan denbora fakturatzen duten azpikontratazio baliabideek betetzen duten rola zehazten du. |
| Baliabide erreserbagarria | Denbora fakturatzen ari den azpikontrataren izena. Erreserba daitekeen baliabide bat hautatzea aukerakoa da. | Eremu hau hutsik geratzen bada, proiektu-kudeatzaileak hornitzailearen faktura-lerroa hornitzailearen faktura-lerroko edozein baliabidek erregistratzen duen denborarekin pareka dezake. |
| Kantitatea | Sartu saltzaileak fakturatzen ari den ordu kopurua faktura lerroan. |Batere ez |
| Salmenta-unitatea | Balio lehenetsia da **Denbora-unitate taldea** eta ezin da aldatu. | Batere ez |
| Unitatea | Balio lehenetsia ordu-unitatearen oinarrizko ordu-unitatea da. Balio hori alda dezakezu denbora-unitate taldeko edozein unitatetan erosteko, hala nola egunean edo astean. | -ren konbinazioa **Rola** eta **Unitatea** balioak balio lehenetsi edo kalkulatu gisa erabiliko dira **Unitatearen prezioa** saltzaileen faktura lerroko eremua. |
| Unitateko prezioa | Unitateko prezio lehenetsiak ren konbinazioa erabiltzen du **Rola** eta **Unitatea** saltzaileen faktura-lerroaren transakzio-datari dagozkion proiektuko prezioen zerrendako balioak. | Dagokion proiektuaren prezio-zerrendaren prezioa saltzaileen faktura lerroko unitatetik desberdina den unitate batean ezartzen bada, sistemak unitate-bihurketa erabiltzen du unitate bakoitzeko prezioa kalkulatzeko. |
| Guztizko partziala | Irakurtzeko soilik den eremu hau honela kalkulatzen da *Kantitatea*&times;*Unitatearen prezioa*, bietan balioak sartzen badira **Kantitatea** eremua eta **Unitatearen prezioa** eremua. Eremu horietako bat edo biak hutsik badaude, eremu honetan balio bat sar dezakezu. | Batere ez |
| Salmenten zerga | Idatzi salmenta-zergaren zenbatekoa. | Batere ez |
| Kopuru osoa | Saltzaileen faktura-lerroaren guztizko zenbatekoa, zergak barne. Eremu hau honela kalkulatzen da *Azpitotala* + *Salmenta zerga*. | Batere ez |

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
