---
title: Produktuen saltzailearen fakturaren lerroak
description: Artikulu honek produktuen saltzaileen faktura-lerroak nola erregistratu eta eremu desberdinak nola erabili saltzaileen produktuen erosketak erregistratzeko azaltzen du.
author: rumant
ms.date: 03/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: d38a447c576c095a7bbe2f5ed84342a88bf69a9b
ms.sourcegitcommit: b2224d1f3c0bd4925d647e6ca3960db81a209521
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/11/2022
ms.locfileid: "9261543"
---
# <a name="vendor-invoice-lines-for-products"></a>Produktuen saltzailearen fakturaren lerroak

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Saltzaileen faktura bat Microsoft-en Dynamics 365 Project Operations produktuen saltzaileen faktura-lerroak izan ditzake (materialak ere deitzen zaie). Proiektuen kudeatzaileek produktuen saltzaileen faktura lerroak erabil ditzakete proiektuetan erositako produktuen kostuak erregistratzeko.

Produktuen hornitzaileen faktura-lerroek materialetarako azpikontratazio-lerroa erreferentzia izan dezakete edo ez. Produktuen saltzaileen faktura-lerro batek azpikontratu bati erreferentzia egiten badio, proiektu-zuzendariek saltzaileen faktura-lerroak fakturatzen ari diren produktuak parekatu eta egiaztatu ahal izango dituzte proiektu-kudeatzaileek erregistratu eta onartutako erositako produktuen erabilerarekin.

Hurrengo taulak produktuen hornitzaileen faktura-lerroetako eremuei buruzko informazioa eskaintzen du.

| Eremua | Deskribapenak | Inpaktu funtzionala |
| --- | --- | --- |
| Eman izena | Saltzaileen faktura-lerroaren izena, identifikazioan laguntzeko. | Izen hau saltzaileen faktura-lerroetan oinarritutako bilaketa guztietan lehen zutabe gisa agertuko da. |
| Deskribapenak | Saltzaileak fakturatzen dituen produktuen deskribapen laburra hornitzailearen faktura lerroan. | Batere ez |
| Azpikontratua | Hasiera batean produktuak eskatu ziren azpikontratua. | Saltzaileen fakturarako azpikontratu bat hautatzen denean, saltzaileen fakturako lerro guztiek hautapen hori heredatuko dute. Saltzaileen faktura batek ezin du izan azpikontratu desberdinak aipatzen dituzten hornitzaileen faktura lerroak. |
| Azpikontratazio lerroa | Produktuak eskatu ziren azpikontratazio-lerroa. Hauta daitezkeen azpikontratazio-lerroen zerrenda hautatutako azpikontratuko lerroetara mugatzen da. | Produktuen saltzaileen faktura lerro batean azpikontratazio-lerro bat hautatzen denean, balio lehenetsiak **Proiektua**, **·**, eta **Produktua** eremuak azpikontratuaren lerroan dagozkion eremuetatik sartzen dira. Hautatutako azpikontratazio lerroak balioak baditu **Proiektua**, **·**, eta **Produktua** eremuetan, hornitzaileen faktura-lerroko dagozkien eremuen balioak ezin dira balio horietatik desberdina izan. |
| Transakzioaren data | Saltzaileen faktura-lerroaren benetako kostua proiektuan erregistratuko den data. | Batere ez|
| Transakzio-klasea | Produktuak fakturatzen direnean, eremu hau ezarri behar da **Materiala**. | Balioa **Materiala** saltzaileen faktura-lerroa erositako materialen fakturaren zenbatekoa erregistratzeko erabiltzen ari dela adierazten du. |
| Project | Fakturatzen ari diren produktuak erabili diren proiektuaren izena. | Eremu hau beharrezkoa da eta ezin da hutsik utzi. |
| Zeregina | Fakturatzen ari diren produktuak erabili diren proiektuaren atazaren izena. Eremu hau proiektu bat hautatzen bada soilik dago erabilgarri. Proiektuko zeregina hautatzea aukerakoa da. | Eremu hau hutsik geratzen bada, proiektuaren kudeatzaileak saltzailearen faktura-lerroa proiektuko edozein zereginetan erabiltzen den erositako produktuarekin lo dezake. Saltzaileen faktura-lerroak ez badu azpikontratazio-lerrorik aipatzen, eta eremu hau hutsik geratzen bada, saltzaileen faktura-lerroak sortzen duen kostu erreala ez da fakturatu gabeko salmenta errealekin lotuko. Kasu honetan, zereginetan oinarritutako fakturazioa konfiguratzen bada, kostuak ezin izango zaizkio azken bezeroari fakturatu. |
| Hautatu produktua | Hautatu fakturatzen ari den produktua katalogoko lehendik dagoen produktua edo idatzizko produktua den. | Balio lehenetsia azpikontratazio lerrotik sartzen da azpikontratazio lerro bat hautatzen denean. |
| Produktu | Hautatu produktua katalogotik. Produktua idazteko produktua bada, idatzi produktuaren izena. | Eremu hau lehendik dauden produktuen erosketa prezio lehenetsiak sartzeko erabiltzen da. |
| Kantitatea | Sartu faktura-lerro honetan saltzaileak fakturatzen duen material-kantitatea. | Batere ez |
| Salmenta-unitatea | Hautatu fakturatzen den kantitatea adierazten den unitateko unitate-taldea. | Batere ez |
| Unitatea | Balio lehenetsia hautatzen den unitate-taldearen oinarrizko unitatea da. Balio hori alda dezakezu hautatutako unitate-taldeko edozein unitatetan ordaintzeko. | -ren konbinazioa **Produktua** eta **Unitatea** balioak balio lehenetsi edo kalkulatu gisa erabiliko dira **Unitatearen prezioa** saltzaileen faktura lerroko eremua. |
| Unitateko prezioa | Unitateko prezio lehenetsiak ren konbinazioa erabiltzen du **Produktua** eta **Unitatea** saltzaileen faktura-lerroaren transakzio-datari dagozkion proiektuko prezioen zerrendako balioak. | Batere ez |
| Guztizko partziala | Irakurtzeko soilik den eremu hau honela kalkulatzen da *Kantitatea*&times;*Unitatearen prezioa*, bietan balioak sartzen badira **Kantitatea** eremua eta **Unitatearen prezioa** eremua. Eremu horietako bat edo biak hutsik badaude, eremu honetan balio bat sar dezakezu. | Batere ez |
| Salmenten zerga | Idatzi salmenta-zergaren zenbatekoa. | Batere ez |
| Kopuru osoa | Saltzaileen faktura-lerroaren guztizko zenbatekoa, zergak barne. Eremu hau honela kalkulatzen da *Azpitotala* + *Salmenta zerga*. | Batere ez |

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
