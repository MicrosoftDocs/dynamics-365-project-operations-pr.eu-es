---
title: Saltzailearen fakturaren lerroak gastu-kategorien arabera
description: Artikulu honek saltzaileen faktura-lerroak nola erregistratu azaltzen du gastu-kategorietarako.
author: rumant
ms.date: 03/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 2c3cd2fab87af1cbfccd81e543f2cea0278978f6
ms.sourcegitcommit: b2224d1f3c0bd4925d647e6ca3960db81a209521
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/11/2022
ms.locfileid: "9261657"
---
# <a name="vendor-invoice-lines-for-expense-categories"></a>Saltzailearen fakturaren lerroak gastu-kategorien arabera

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Microsoft Dynamics 365 Project Operations-eko saltzailearen fakturak saltzaileen faktura-lerroak izan ditzakete gastu kategorietarako. Proiektu-kudeatzaileek saltzaileen faktura-lerroak erabil ditzakete gastu-kategorietarako, kontratatzen diren zerbitzuen kostuak gastu-kategoria gisa erregistratzeko.

Gastu-kategorien saltzaileen faktura-lerroek gastu-kategorien azpikontratazio-lerro bati erreferentzia egin dezakete edo ez. Gastu-kategorien saltzaileen faktura-lerro batek azpikontratu bati erreferentzia egiten badio, proiektu-kudeatzaileek saltzaileen faktura-lerroak fakturatzen ari diren gastuak parekatu eta egiaztatu ahal izango dituzte, gastu-kategoria horietan erregistratu eta proiektuko arduradunek proiektuan onartutako gastuekin.

Ondorengo taulan fitxategien eremuei buruzko informazioa ematen da gastuen kategorien saltzailearen faktura-lerroan.

| Eremua | Deskribapenak | Inpaktu funtzionala |
| --- | --- | --- |
| Eman izena | Identifikazioan laguntzeko saltzailearen faktura-lerroaren izena. | Izena saltzailearen faktura-lerroetan oinarritutako bilaketa guztietan lehen zutabe gisa erakutsiko da. |
| Deskribapenak | Saltzaileak saltzailearen faktura-lerroan fakturatzen dituen zerbitzuen deskribapen laburra. | Batere ez |
| Azpikontratua | Zerbitzuak hasiera batean agindutako azpikontratua. | Saltzaileen fakturarako azpikontratu bat hautatzen denean, saltzaileen fakturako lerro guztiek hautapen hori heredatuko dute. Saltzaileen faktura batek ezin du izan azpikontratu desberdinak aipatzen dituzten hornitzaileen faktura lerroak. |
| Azpikontratuaren lerroa | Zerbitzuak eskatuta azpikontratuaren lerroa. Hauta daitezkeen azpikontratuaren lerroen zerrenda hautatutako azpikontratuaren lerroetara mugatzen da. | Hornitzaileen faktura lerro batean azpikontratuaren lerro bat hautatzen denean gastu kategorietarako, balio lehenetsiak **Proiektua**, **Zeregin**, eta **Transakzio kategoria** eremuak azpikontratuaren lerroan dagozkion eremuetatik sartzen dira. Hautatutako azpikontratuaren lerroak balioak baditu **Proiektua**, **Proiektuaren zeregina**, eta **Transakzio kategoria** eremuetan, hornitzaileen faktura-lerroko dagozkien eremuen balioak ezin dira balio horietatik desberdina izan. |
| Transakzioaren data | Saltzaileen faktura-lerroaren benetako kostua proiektuan erregistratuko den data. |Batere ez |
| Transakzio-klasea | Hautatu **Gastua** gastu-kategoria baten saltzailearen faktura erregistratzeko. | **Gastua** balioak saltzaileen faktura-lerroa gastu-kategoria gisa kontratatu ziren zerbitzuen fakturaren zenbatekoa erregistratzeko erabiltzen ari dela adierazten du. |
| Project | Fakturatutako zerbitzuak erabili diren proiektuaren izena. | Eremua beharrezkoa da eta ezin da hutsik utzi. |
| Zeregina | Fakturatutako zerbitzuak erabili diren proiektuaren zereginaren izena. Eremu hau proiektu bat hautatzen bada soilik dago erabilgarri. Proiektuko zeregina hautatzea aukerakoa da. | Eremu hau hutsik geratzen bada, proiektuaren kudeatzaileak hornitzaileen faktura-lerroa proiektuko edozein zereginetan erregistratzen diren gastuekin lo dezake. Saltzaileen faktura-lerroak ez badu azpikontratuaren lerrorik aipatzen, eta eremu hau hutsik geratzen bada, saltzaileen faktura-lerroak sortzen duen kostu erreala ez da fakturatu gabeko salmenta errealekin lotuko. Kasu honetan, zereginetan oinarritutako fakturazioa konfiguratzen bada, baliteke kostuak azken bezeroari ezin izango zaizkio fakturatu. |
| Transakzio-kategoria | Fakturatzen ari den transakzio-kategoria. Hautatutako transakzio kategoriarako dagokion gastu-kategoria sortu behar da. | **Transakzioaren kategoria** eta **Unitatea** balioen konbinazioa lehenetsitako moduan edo balio konputatu gisa erabiliko da saltzailearen faktura-lerroko **Unitatearen prezioa** eremuan. |
| Kantitatea | Sartu saltzaileak fakturatzen ari den kopurua faktura lerroan. |Batere ez|
| Salmenta-unitatea | Balio lehenetsia sartzen da hautatutako transakzioaren kategoriaren unitate-taldean oinarrituta. | Batere ez |
| Unitatea | Balio lehenetsia da hautatuta unitate-taldearen oinarrizko unitatea. Balio hau alda dezakezu unitate taldeko edozein unitate erosteko. | **Transakzioaren kategoria** eta **Unitatea** balioen konbinazioa lehenetsitako moduan edo balio konputatu gisa erabiliko da saltzailearen faktura-lerroko **Unitatearen prezioa** eremuan. |
| Unitateko prezioa | Unitatearen prezio lehenetsiak erabiltzen ditu saltzailearen faktura-lerroko transakzioaren datan aplikatu daitekeen **Transakzioaren kategoria** eta **Unitatea** balioak proiektuaren prezio-zerrendatik. | Aplikagarria den proiektuaren prezioen zerrendak saltzailearen faktura-lerroaren unitatea ez den beste unitate batean konfiguratuta dagoenean, sistemak unitate bihurketa erabiltzen du prezio unitarioa kalkulatzeko. |
| Guztizko partziala | Irakurtzeko soilik den eremua *Kopurua* &times; *Unitatearen prezioa* gisa kalkulatzen da, **Kopurua** eremua eta **Unitatearen prezioa** eremuetan balioak sartzen badira. Eremu bat edo biak hutsik badaude, balio bat sar dezakezu eremu horretan.| Batere ez |
| Salmenten zerga | Idatzi salmenta-zergaren zenbatekoa. | Batere ez |
| Zenbatekoa guztira | Saltzailearen faktura-lerroaren guztizko kantitatea barne hartutako zergak. Eremu honetan kalkulatuta dago *Azpitotala* + *Salmenten zerga*. | Batere ez |

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
