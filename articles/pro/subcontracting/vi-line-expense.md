---
title: Saltzailearen fakturaren lerroak gastu-kategorien arabera
description: Artikulu honek saltzaileen faktura-lerroak nola erregistratu azaltzen du gastu-kategorietarako.
author: rumant
ms.date: 03/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 3ffad20b53344221ead9b6850ecdc1efd48d5b13
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8925844"
---
# <a name="vendor-invoice-lines-for-expense-categories"></a>Saltzailearen fakturaren lerroak gastu-kategorien arabera

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Saltzaileen faktura bat Microsoft-en Dynamics 365 Project Operations saltzaileen faktura-lerroak izan ditzakete gastu kategorietarako. Proiektu-kudeatzaileek saltzaileen faktura-lerroak erabil ditzakete gastu-kategorietarako, kontratatzen diren zerbitzuen kostuak gastu-kategoria gisa erregistratzeko.

Gastu-kategorien saltzaileen faktura-lerroek gastu-kategorietarako azpikontratazio-lerro bati erreferentzia egin dezakete edo ez. Gastu-kategorien saltzaileen faktura-lerro batek azpikontratu bati erreferentzia egiten badio, proiektu-kudeatzaileek saltzaileen faktura-lerroak fakturatzen ari diren gastuak parekatu eta egiaztatu ahal izango dituzte, gastu-kategoria horietan erregistratu eta proiektuko arduradunek proiektuan onartutako gastuekin.

Hurrengo taulak gastu-kategorien saltzaileen faktura-lerroetako eremuei buruzko informazioa eskaintzen du.

| Eremua | Deskribapenak | Inpaktu funtzionala |
| --- | --- | --- |
| Eman izena | Saltzaileen faktura-lerroaren izena, identifikazioan laguntzeko. | Izen hau saltzaileen faktura-lerroetan oinarritutako bilaketa guztietan lehen zutabe gisa agertuko da. |
| Deskribapenak | Saltzaileak fakturatzen dituen zerbitzuen deskribapen laburra hornitzaileen faktura lerroan. | Batere ez |
| Azpikontratua | Zerbitzuak hasiera batean agindutako azpikontratua. | Saltzaileen fakturarako azpikontratu bat hautatzen denean, saltzaileen fakturako lerro guztiek hautapen hori heredatuko dute. Saltzaile-faktura batek ezin du izan azpikontratu desberdinak aipatzen dituzten hornitzaile-faktura-lerroak. |
| Azpikontratazio lerroa | Zerbitzuak agindutako azpikontratazio lerroa. Hauta daitezkeen azpikontratazio-lerroen zerrenda hautatutako azpikontratuko lerroetara mugatzen da. | Hornitzaileen faktura-lerro batean azpikontratu-lerro bat hautatzen denean gastu-kategorietarako, balio lehenetsiak **Proiektua**, **·**, eta **Transakzio kategoria** eremuak azpikontratuaren lerroan dagozkion eremuetatik sartzen dira. Hautatutako azpikontratazio-lerroak balioak baditu **Proiektua**, **zeregina**, eta **Transakzio kategoria** eremuetan, hornitzaileen faktura-lerroko dagozkien eremuen balioak ezin dira balio horietatik desberdina izan. |
| Transakzioaren data | Saltzaileen faktura-lerroaren benetako kostua proiektuan erregistratuko den data. |Batere ez |
| Transakzio-klasea | Hautatu **Gastua** gastu-kategoria baten saltzaile-faktura erregistratzeko. | Balioa **Gastua** saltzaileen faktura-lerroa gastu-kategoria gisa kontratatu ziren zerbitzuen fakturaren zenbatekoa erregistratzeko erabiltzen ari dela adierazten du. |
| Project | Fakturatzen ari diren zerbitzuak erabili diren proiektuaren izena. | Eremu hau beharrezkoa da eta ezin da hutsik utzi. |
| Zeregina | Fakturatzen ari diren zerbitzuak erabili diren proiektuaren atazaren izena. Eremu hau proiektu bat hautatzen bada soilik dago erabilgarri. Proiektuko zeregina hautatzea aukerakoa da. | Eremu hau hutsik geratzen bada, proiektuaren kudeatzaileak hornitzailearen faktura-lerroa proiektuko edozein zereginetan erregistratzen diren gastuekin lo dezake. Saltzaileen faktura-lerroak ez badu azpikontratazio-lerrorik aipatzen, eta eremu hau hutsik geratzen bada, hornitzaile-faktura-lerroak sortzen duen kostu erreala ez da fakturatu gabeko salmenta-errealekin lotuko. Kasu honetan, zereginetan oinarritutako fakturazioa konfiguratzen bada, baliteke kostuak ezin izango zaizkiola azken bezeroari fakturatu. |
| Transakzio-kategoria | Fakturatzen ari den transakzio-kategoria. Hautatutako transakzio kategoriarako dagokion gastu-kategoria sortu behar da. | -ren konbinazioa **Transakzio kategoria** eta **Unitatea** balioak balio lehenetsi edo kalkulatu gisa erabiliko dira **Unitatearen prezioa** saltzaileen faktura lerroko eremua. |
| Kantitatea | Sartu saltzaileak fakturatzen ari den kopurua faktura lerroan. |Batere ez|
| Salmenta-unitatea | Aukeratutako transakzio-kategoriaren unitate-taldearen araberako balio lehenetsia sartzen da. | Batere ez |
| Unitatea | Balio lehenetsia hautatzen den unitate-taldearen oinarrizko unitatea da. Balio hori alda dezakezu unitate-taldeko edozein unitatetan erosteko. | -ren konbinazioa **Transakzio kategoria** eta **Unitatea** balioak balio lehenetsi edo kalkulatu gisa erabiliko dira **Unitatearen prezioa** saltzaileen faktura lerroko eremua. |
| Unitateko prezioa | Unitateko prezio lehenetsiak ren konbinazioa erabiltzen du **Transakzio kategoria** eta **Unitatea** saltzaileen faktura-lerroaren transakzio-datari dagozkion proiektuko prezioen zerrendako balioak. | Dagokion proiektuaren prezio-zerrendaren prezioa saltzaileen faktura lerroko unitatetik desberdina den unitate batean ezartzen bada, sistemak unitate-bihurketa erabiltzen du unitate bakoitzeko prezioa kalkulatzeko. |
| Guztizko partziala | Irakurtzeko soilik den eremu hau honela kalkulatzen da *Kantitatea*&times;*Unitatearen prezioa*, bietan balioak sartzen badira **Kantitatea** eremua eta **Unitatearen prezioa** eremua. Eremu horietako bat edo biak hutsik badaude, eremu honetan balio bat sar dezakezu.| Batere ez |
| Salmenten zerga | Idatzi salmenta-zergaren zenbatekoa. | Batere ez |
| Kopuru osoa | Saltzaileen faktura-lerroaren guztizko zenbatekoa, zergak barne. Eremu hau honela kalkulatzen da *Azpitotala* + *Salmenta zerga*. | Batere ez |

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
