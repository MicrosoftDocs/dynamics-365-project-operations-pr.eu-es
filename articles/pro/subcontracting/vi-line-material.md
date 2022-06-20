---
title: Produktuen saltzailearen fakturaren lerroak
description: Artikulu honetan, produktuetarako hornitzaileen fakturen lerroak nola erregistratu eta hornitzaileen produktuen erosketak erregistratzeko eremuak nola erabili azaltzen da.
author: rumant
ms.date: 03/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 206dd36a1a1e7141678da27d76a99561ac89044b
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8931361"
---
# <a name="vendor-invoice-lines-for-products"></a>Produktuen saltzailearen fakturaren lerroak

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Microsoften Dynamics 365 Project Operations hornitzaile-faktura batek produktuetarako hornitzailearen faktura-lerroak izan ditzake (materialak ere deituak). Proiektu-kudeatzaileek hornitzaileen faktura-lerroak erabil ditzakete produktuetarako, proiektuetan erositako produktuen kostuak erregistratzeko.

Produktuetarako hornitzaileen fakturazio-lineek materialetarako azpikontratu-linea bati erreferentzia egin diezaiokete edo ez. Produktuetarako hornitzaile-faktura-linea batek azpikontratu bati egiten badio erreferentzia, proiektu-kudeatzaileek bat egin eta egiaztatu ahal izango dituzte hornitzailearen faktura-lerroak fakturatzen dituen produktuak eta proiektu-kudeatzaileek erregistratu eta onartutako produktuak erostearekin.

Hurrengo taulan, produktuetarako hornitzaileen fakturen arloei buruzko informazioa ematen da.

| Eremua | Deskribapenak | Inpaktu funtzionala |
| --- | --- | --- |
| Eman izena | Saltzaileen faktura-lerroaren izena, identifikazioan laguntzeko. | Izen hau saltzaileen faktura-lerroetan oinarritutako bilaketa guztietan lehen zutabe gisa agertuko da. |
| Deskribapenak | Hornitzailea hornitzailearen faktura-lerroan fakturatzen ari den produktuen deskribapen laburra. | Batere ez |
| Azpikontratua | Produktuak hasiera batean ordenatu ziren azpikontratua. | Saltzaileen fakturarako azpikontratu bat hautatzen denean, saltzaileen fakturako lerro guztiek hautapen hori heredatuko dute. Saltzaile-faktura batek ezin du izan azpikontratu desberdinak aipatzen dituzten hornitzaile-faktura-lerroak. |
| Azpikontrato-lerroa | Produktuak ordenatzeko azpikontratu-lerroa. Hauta daitezkeen azpikontratazio-lerroen zerrenda hautatutako azpikontratuko lerroetara mugatzen da. | Produktuetarako hornitzailearen faktura-lerro batean azpikontratu-linea bat aukeratzen denean, azpikontrato-lineako eremuetatik **Proiektu**, Tarea **eta** Produktu **arloetarako** aurrez zehaztutako balioak sartzen dira. Hautatutako azpikontratu-lerroak Proiektu **,** Tarea **eta** Produktu **arloetako** balioak baditu, hornitzailearen faktura-lerroko eremuetako balioak ezin dira balore horietatik ezberdinak izan. |
| Transakzioaren data | Saltzaileen faktura-lerroaren benetako kostua proiektuan erregistratuko den data. | Batere ez|
| Transakzio-klasea | Produktuak fakturatzen direnean, eremu hori Materialean **ezarri behar** da. | Balio **materialaren** arabera, hornitzailearen faktura-lerroa erositako materialen fakturaren zenbatekoa erregistratzeko erabiltzen ari da. |
| Project | Fakturatzen diren produktuak erabili ziren proiektuaren izena. | Eremu hau beharrezkoa da eta ezin da hutsik utzi. |
| Zeregina | Fakturatzen diren produktuak erabili ziren proiektu-lanaren izena. Eremu hau proiektu bat hautatzen bada soilik dago erabilgarri. Proiektuko zeregina hautatzea aukerakoa da. | Arlo hori zuri uzten bada, proiektu-kudeatzaileak bat egin dezake hornitzailearen faktura-lerroarekin eta proiektuaren edozein zereginetan erabiltzen den erositako produktuarekin. Saltzaileen faktura-lerroak ez badu azpikontratazio-lerrorik aipatzen, eta eremu hau hutsik geratzen bada, hornitzaile-faktura-lerroak sortzen duen kostu erreala ez da fakturatu gabeko salmenta-errealekin lotuko. Kasu horretan, zereginetan oinarritutako fakturazioa konfiguratzen bada, kostuak ezin izango zaizkio azken bezeroari fakturatu. |
| Hautatu produktua | Aukeratu fakturatzen ari den produktua katalogoko produktu bat edo idazkera-produktu bat den. | Aurrez zehaztutako balioa azpikontrato-lerrotik sartzen da azpikontrato-lerro bat aukeratzen denean. |
| Produktu | Aukeratu katalogoko produktua. Produktua idazkera-produktua bada, sartu produktuaren izena. | Eremu hau lehendik dauden produktuen erosketa-prezio aurredeterminatuak sartzeko erabiltzen da. |
| Kantitatea | Sartu hornitzailea fakturatzen ari den material kopurua faktura-lerro honetan. | Batere ez |
| Salmenta-unitatea | Fakturatzen ari den zenbatekoa adierazten duen unitateko unitate-taldea hautatu. | Batere ez |
| Unitatea | Balio lehenetsia hautatzen den unitate-taldearen oinarrizko unitatea da. Balio hori alda dezakezu hautatutako unitateen taldeko edozein unitatetan ordaintzeko. | Produktu- eta **unitate-balioen** **konbinazioa aldez aurretik zehaztutako edo kalkulatutako** **balio gisa erabiliko da, hornitzailearen faktura-lerroan.** |
| Unitateko prezioa | Aurrez zehaztutako unitate-prezioan, produktu-balioen **eta** proiektuaren prezioen **zerrendaren unitatearen** konbinazioa erabiltzen da, hornitzailearen faktura-lerroaren transakzio-datan aplikatzen dena. | Batere ez |
| Guztizko partziala | Irakurtzeko soilik den eremu hau honela kalkulatzen da *Kantitatea*&times;*Unitatearen prezioa*, bietan balioak sartzen badira **Kantitatea** eremua eta **Unitatearen prezioa** eremua. Eremu horietako bat edo biak hutsik badaude, eremu honetan balio bat sar dezakezu. | Batere ez |
| Salmenten zerga | Idatzi salmenta-zergaren zenbatekoa. | Batere ez |
| Zenbateko osoa | Saltzaileen faktura-lerroaren guztizko zenbatekoa, zergak barne. Eremu hau honela kalkulatzen da *Azpitotala* + *Salmenta zerga*. | Batere ez |

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
