---
title: Mugarrien saltzailearen fakturaren lerroak
description: Artikulu honetan, azpikontratu batean mugarrietarako hornitzailearen faktura-lerroak nola sortu azaltzen da.
author: rumant
ms.date: 03/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 212d68c32e712ac2349d1670f9e799bcc5144148
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8931315"
---
# <a name="vendor-invoice-lines-for-milestones"></a>Mugarrien saltzailearen fakturaren lerroak

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Microsoften Dynamics 365 Project Operations hornitzailearen faktura batek hornitzailearen faktura-lineak izan ditzake, azpikontrato-linea batean definitzen diren mugarrietarako. Proiektu-kudeatzaileek hornitzailearen faktura-lineak erabil ditzakete mugarrietarako, proiekturako eskuratzen diren zerbitzu edo produktuetan gertatzen diren mugarrietan oinarritutako kostu gisa eskuratzen diren zerbitzuen kostuak erregistratzeko.

Hornitzaileen fakturazio-lineek beti aipatu behar dute prezio finkoko fakturazio-metodoa duen azpikontratu-linea bat. Hornitzailearen fakturazio-lerro batek azpikontratu-linea bati egiten dion erreferentzia egiten duenean, proiektu-kudeatzaileek azpikontratu-lerro horri erreferentzia egiten dioten denbora-, gastu- edo material-kostuak bat egin eta egiaztatu ahal izango dituzte, hornitzailea fakturatzen ari den mugarriarekin.

Hurrengo taulan, hornitzailearen faktura-lerroen eremuei buruzko informazioa ematen da mugarrietarako.

| Eremua | Deskribapenak | Inpaktu funtzionala |
| --- | --- | --- |
| Eman izena | Saltzaileen faktura-lerroaren izena, identifikazioan laguntzeko. | Izen hau saltzaileen faktura-lerroetan oinarritutako bilaketa guztietan lehen zutabe gisa agertuko da. |
| Deskribapenak | Hornitzailea hornitzailearen faktura-lerroan fakturatzen ari den zerbitzuen deskribapen laburra. | Batere ez |
| Azpikontratua | Zerbitzuak hasiera batean agindutako azpikontratua. | Saltzaileen fakturarako azpikontratu bat hautatzen denean, saltzaileen fakturako lerro guztiek hautapen hori heredatuko dute. Saltzaile-faktura batek ezin du izan azpikontratu desberdinak aipatzen dituzten hornitzaile-faktura-lerroak. |
| Azpikontrato-lerroa | Zerbitzuak agindutako azpikontratazio lerroa. Hauta daitezkeen azpikontratazio-lerroen zerrenda hautatutako azpikontratuko lerroetara mugatzen da. | Hornitzailearen faktura-lerro batean azpikontratu-linea bat aukeratzen denean, **Rol** eta **Transakzio kategoriako** eremuak eta produktuarekin lotutako eremuak garrantzirik gabekoak dira eta ez daude eskuragarri. Unitateen **kantitatea**, **unitatea** eta **taldea** ere ez dira garrantzitsuak mugarrietan oinarritutako hornitzaileen fakturen lerroetarako. |
| Transakzioaren data | Saltzaileen faktura-lerroaren benetako kostua proiektuan erregistratuko den data. | Batere ez |
| Transakzio-klasea | **Aukeratu** Hornitzaile-faktura bat erregistratzeko, azpikontrato-lerro batean definitu zen mugarri oso baterako. | Batere ez |
| Mugarria | Fakturatzeko **listo gisa** markatuta dagoen azpikontratu-lerroan zehaztutako mugarria hautatu. | Listo estatuak fakturatzeko **duen azpikontratazio-linearen** mugarriak hornitzailearen faktura-lerro batean aukera daitezke. |
| Project | Fakturatzen ari diren zerbitzuak erabili diren proiektuaren izena. | Eremu hau beharrezkoa da eta ezin da hutsik utzi. |
| Zeregina | Fakturatzen ari diren zerbitzuak erabili diren proiektuaren atazaren izena. Eremu hau proiektu bat hautatzen bada soilik dago erabilgarri. Proiektuko zeregina hautatzea aukerakoa da. | Arlo hori zuri uzten bada, proiektuaren zuzendariak bat egin dezake hornitzailearen faktura-lerroarekin eta proiektuaren edozein zereginetan erregistratzen den azpikontratu-lerroko transakzio-motarekin. Saltzaileen faktura-lerroak ez badu azpikontratazio-lerrorik aipatzen, eta eremu hau hutsik geratzen bada, hornitzaile-faktura-lerroak sortzen duen kostu erreala ez da fakturatu gabeko salmenta-errealekin lotuko. Kasu honetan, zereginetan oinarritutako fakturazioa konfiguratzen bada, baliteke kostuak ezin izango zaizkiola azken bezeroari fakturatu. |
| Mugarriaren zenbatekoa | Zehaztutako mugarriaren balioa sartu fakturatzeko prest dagoen azpikontratu-lerroan. | Batere ez |
| Salmenten zerga | Idatzi salmenta-zergaren zenbatekoa. | Batere ez |
| Zenbateko osoa | Saltzaileen faktura-lerroaren guztizko zenbatekoa, zergak barne. Eremu hori salmenten gaineko *zergaren* + *mugarriaren zenbateko* gisa kalkulatzen da. | Batere ez |

> [!NOTE]
> Azpikontrato-linearen mugarri bati erreferentzia egiten dion hornitzaile-faktura-lerro bat sortzen denean, azpikontratoaren mugarriaren egoera sortutako **hornitzailearen fakturari** eguneratzen zaio. Gero, hornitzailearen faktura hori baieztatzen denean, azpikontratazio-linearen mugarriaren egoera berretsitako **hornitzailearen fakturara** eguneratzen da.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
