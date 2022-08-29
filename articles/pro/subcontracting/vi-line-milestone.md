---
title: Mugarrien saltzailearen fakturaren lerroak
description: Artikulu honek azpikontratu bateko mugarrietarako hornitzaileen faktura-lerroak nola sortu azaltzen du.
author: rumant
ms.date: 03/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: f066c2ac7377a989a92a9ae2e9a732d3c979a0db
ms.sourcegitcommit: b2224d1f3c0bd4925d647e6ca3960db81a209521
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/11/2022
ms.locfileid: "9260980"
---
# <a name="vendor-invoice-lines-for-milestones"></a>Mugarrien saltzailearen fakturaren lerroak

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Saltzaileen faktura bat Microsoft-en Dynamics 365 Project Operations saltzaileen faktura-lerroak izan ditzake azpikontratu-lerro batean definitutako mugarrietarako. Proiektu-kudeatzaileek saltzaileen faktura-lerroak erabil ditzakete mugarrietarako kontratatzen diren zerbitzuen kostuak proiekturako kontratatzen diren zerbitzu edo produktuetan sortzen diren mugarrietan oinarritutako kostu gisa erregistratzeko.

Mugarrietarako saltzaileen faktura-lerroek beti egin behar dute erreferentzia prezio finkoko fakturazio-metodoa duen azpikontratazio-lerroa. Mugarrien saltzaileen faktura-lerro batek azpikontratu-lerro bati erreferentzia egiten dionean, proiektu-kudeatzaileek azpikontratazio-lerro horri erreferentzia egiten dioten denbora, gastu edo materialen azpiko kostuak saltzaileak fakturatzen ari den mugarriarekin lotu eta egiaztatu ahal izango dituzte.

Hurrengo taulak hornitzaileen faktura-lerroetako eremuei buruzko informazioa eskaintzen du mugarrietarako.

| Eremua | Deskribapenak | Inpaktu funtzionala |
| --- | --- | --- |
| Eman izena | Saltzaileen faktura-lerroaren izena, identifikazioan laguntzeko. | Izen hau saltzaileen faktura-lerroetan oinarritutako bilaketa guztietan lehen zutabe gisa agertuko da. |
| Deskribapenak | Saltzaileak fakturatzen dituen zerbitzuen deskribapen laburra hornitzailearen faktura lerroan. | Batere ez |
| Azpikontratua | Zerbitzuak hasiera batean agindutako azpikontratua. | Saltzaileen fakturarako azpikontratu bat hautatzen denean, saltzaileen fakturako lerro guztiek hautapen hori heredatuko dute. Saltzaileen faktura batek ezin du izan azpikontratu desberdinak aipatzen dituzten hornitzaileen faktura lerroak. |
| Azpikontratazio lerroa | Zerbitzuak agindutako azpikontratazio lerroa. Hauta daitezkeen azpikontratazio-lerroen zerrenda hautatutako azpikontratuko lerroetara mugatzen da. | Mugarrietarako saltzaileen faktura-lerro batean azpikontratazio-lerro bat hautatzen denean, **Rola** eta **Transakzio kategoria** eremuak eta produktuekin erlazionatutako eremuak ez dira garrantzirik eta ez daude eskuragarri. The **Kantitatea**, **·**, eta **Unitate taldea** eremuak ere ez dira garrantzitsuak mugarrietan oinarritutako hornitzaileen faktura-lerroetarako. |
| Transakzioaren data | Saltzaileen faktura-lerroaren benetako kostua proiektuan erregistratuko den data. | Batere ez |
| Transakzio-klasea | Hautatu **Mugarria** Azpikontratazio-lerro batean definitu zen amaitutako mugarri baten saltzaile-faktura erregistratzeko. | Batere ez |
| Mugarria | Hautatu gisa markatuta dagoen azpikontratazio-lerroan definitzen den mugarria **Fakturatzeko prest**. | Egoera duten azpikontratazio lerroaren mugarriak **Fakturatzeko prest** saltzaileen faktura lerro batean hauta daiteke. |
| Project | Fakturatzen ari diren zerbitzuak erabili diren proiektuaren izena. | Eremu hau beharrezkoa da eta ezin da hutsik utzi. |
| Zeregina | Fakturatzen ari diren zerbitzuak erabili ziren proiektuaren zereginaren izena. Eremu hau proiektu bat hautatzen bada soilik dago erabilgarri. Proiektuko zeregina hautatzea aukerakoa da. | Eremu hau hutsik geratzen bada, proiektuaren kudeatzaileak hornitzaileen faktura-lerroa proiektuko edozein zereginetan erregistratutako erlazionatutako azpikontratu-lerroko transakzio-klasearekin lo dezake. Saltzaileen faktura-lerroak ez badu azpikontratazio-lerrorik aipatzen, eta eremu hau hutsik geratzen bada, saltzaileen faktura-lerroak sortzen duen kostu erreala ez da fakturatu gabeko salmenta errealekin lotuko. Kasu honetan, zereginetan oinarritutako fakturazioa konfiguratzen bada, baliteke kostuak azken bezeroari ezin izango zaizkio fakturatu. |
| Mugarriaren zenbatekoa | Sartu fakturatzeko prest dagoen azpikontratuaren lerroan definitutako mugarriaren balioa. | Batere ez |
| Salmenten zerga | Idatzi salmenta-zergaren zenbatekoa. | Batere ez |
| Kopuru osoa | Saltzaileen faktura-lerroaren guztizko zenbatekoa, zergak barne. Eremu hau honela kalkulatzen da *Mugarri kopurua* + *Salmenta zerga*. | Batere ez |

> [!NOTE]
> Azpikontratazioaren mugarri bati erreferentzia egiten dion hornitzaileen faktura-lerroa sortzen denean, azpikontratuaren mugarriaren egoera eguneratzen da.**Saltzaileen faktura sortu da**. Ondoren, saltzaileen faktura hori berresten denean, azpikontratuaren lerroaren mugarriaren egoera eguneratzen da **Saltzaileen faktura berretsi da**.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
