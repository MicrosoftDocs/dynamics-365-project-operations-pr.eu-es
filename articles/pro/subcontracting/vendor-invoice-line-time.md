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

Microsoft Dynamics 365 Project Operations-eko saltzailearen fakturak saltzaileen faktura-lerroak izan ditzakete denborarako. Proiektuen kudeatzaileek denboraren saltzaileen faktura lerroak erabil ditzakete proiektuen azpikontratuen denboraren kostuak erregistratzeko.

Denboraren saltzaileen faktura-lerroek denboraren azpikontratazio-lerro bati erreferentzia egin dezakete edo ez. Denboraren saltzaileen faktura-lerro batek azpikontratu bati erreferentzia egiten badio, proiektu-kudeatzaileek saltzaileen faktura-lerroak fakturatzen ari diren produktuak parekatu eta egiaztatu ahal izango dituzte, azpikontratatzaileek erregistratu eta proiektuko arduradunek proiektuan onartutako gastuekin.

Ondorengo taulan fitxategien eremuei buruzko informazioa ematen da denboraren saltzailearen faktura-lerroan.

| Eremua | Deskribapenak | Inpaktu funtzionala |
| --- | --- | --- |
| Eman izena | Identifikazioan laguntzeko saltzailearen faktura-lerroaren izena. | Izena saltzailearen faktura-lerroetan oinarritutako bilaketa guztietan lehen zutabe gisa erakutsiko da. |
| Deskribapenak | Saltzaileak saltzailearen faktura-lerroan fakturatzen dituen zerbitzuen deskribapen laburra. | Batere ez |
| Azpikontratua | Zerbitzuak hasiera batean agindutako azpikontratua. | Saltzaileen fakturarako azpikontratu bat hautatzen denean, saltzaileen fakturako lerro guztiek hautapen hori heredatuko dute. Saltzaileen faktura batek ezin du izan azpikontratu desberdinak aipatzen dituzten hornitzaileen faktura lerroak. |
| Azpikontratuaren lerroa | Zerbitzuak eskatuta azpikontratuaren lerroa. Hauta daitezkeen azpikontratuaren lerroen zerrenda hautatutako azpikontratuaren lerroetara mugatzen da. | Hornitzaileen faktura lerro batean azpikontratuaren lerro bat hautatzen denean denborarako, balio lehenetsiak **Proiektua**, **funtzioa**, eta **baliabide erreserbagarria** eremuak azpikontratuaren lerroan dagozkion eremuetatik sartzen dira. Hautatutako azpikontratuaren lerroak balioak baditu **Proiektua**, **funtzioa**, eta **erreserbagarria** eremuetan, hornitzaileen faktura-lerroko dagozkien eremuen balioak ezin dira balio horietatik desberdina izan. |
| Transakzioaren data | Saltzaileen faktura-lerroaren benetako kostua proiektuan erregistratuko den data. | Batere ez |
| Transakzio-klasea | Balio lehenetsia **Denbora** da. | **Denbora** balioak saltzaileen faktura-lerroa azpikontratatzailearen denboraren zenbatekoa erregistratzeko erabiltzen ari dela adierazten du. |
| Project | Fakturatutako zerbitzuak erabili diren proiektuaren izena. | Eremua beharrezkoa da eta ezin da hutsik utzi. |
| Zeregina | Fakturatutako zerbitzuak erabili diren proiektuaren zereginaren izena. Eremu hau proiektu bat hautatzen bada soilik dago erabilgarri. Proiektuko zeregina hautatzea aukerakoa da. | Eremu hau hutsik geratzen bada, proiektuaren kudeatzaileak hornitzaileen faktura-lerroa proiektuko edozein zereginetan azpikontratatzaileak erregistratutako baliabideak denborarekin lotu dezake. Saltzaileen faktura-lerroak ez badu azpikontratuaren lerrorik aipatzen, eta eremu hau hutsik geratzen bada, saltzaileen faktura-lerroak sortzen duen kostu erreala ez da fakturatu gabeko salmenta errealekin lotuko. Kasu honetan, zereginetan oinarritutako fakturazioa konfiguratzen bada, baliteke kostuak azken bezeroari ezin izango zaizkio fakturatu. |
| Funtzioa | Denbora fakturatzen ari diren azpikontratatutako baliabideen eginkizuna. | Eremu honek hornitzaileen fakturan denbora fakturatzen duten azpikontratazio baliabideek betetzen duten rola zehazten du. |
| Baliabide erreserbagarria | Denbora fakturatzen ari diren azpikontratatzailearen izena. Baliabide erreserbagarria hautatzea aukerakoa da. | Eremu hau hutsik geratzen bada, proiektuaren kudeatzaileak hornitzaileen faktura-lerroa saltzaileari dagokion saltzaile-lerroko baliabideekin denborarekin lotu dezake. |
| Kantitatea | Saltzaileak saltzailearen faktura-lerroan fakturatzen duen ordu kopurua. |Batere ez |
| Salmenta-unitatea | Lehenetsitako balioa **Denboraren salmenta-unitatea** da, aldatu ezin dena. | Batere ez |
| Unitatea | Eremu honek denbora-unitateko oinarrizko ordu-unitatea da lehenespenez. Balio hau alda dezakezu Denbora unitate taldeko edozein unitate erosteko, hala nola eguna edo astea. | **Funtzioa** eta **Unitatea** balioen konbinazioa lehenetsitako moduan edo balio konputatu gisa erabiliko da saltzailearen faktura-lerroko **Unitatearen prezioa** eremuan. |
| Unitateko prezioa | Unitatearen prezio lehenetsiak erabiltzen ditu saltzailearen faktura-lerroko transakzioaren datan aplikatu daitekeen **Funtzioa** eta **Unitatea** balioak proiektuaren prezio-zerrendatik. | Aplikagarria den proiektuaren prezioen zerrendak saltzailearen faktura-lerroaren unitatea ez den beste unitate batean konfiguratuta dagoenean, sistemak unitate bihurketa erabiltzen du prezio unitarioa kalkulatzeko. |
| Guztizko partziala | Irakurtzeko soilik den eremua *Kopurua* &times; *Unitatearen prezioa* gisa kalkulatzen da, **Kopurua** eremua eta **Unitatearen prezioa** eremuetan balioak sartzen badira. Eremu bat edo biak hutsik badaude, balio bat sar dezakezu eremu horretan. | Batere ez |
| Salmenten zerga | Idatzi salmenta-zergaren zenbatekoa. | Batere ez |
| Zenbatekoa guztira | Saltzailearen faktura-lerroaren guztizko kantitatea barne hartutako zergak. Eremu honetan kalkulatuta dago *Azpitotala* + *Salmenten zerga*. | Batere ez |

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
