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

Saltzaileen faktura bat Microsoft Dynamics 365 Project Operations saltzaileen faktura-lerroak izan ditzake azpikontratu-lerro batean definitutako mugarrietarako. Proiektu-kudeatzaileek hornitzaileen faktura-lerroak erabil ditzakete mugarrietarako kontratatzen diren zerbitzuen kostuak proiekturako kontratatzen diren zerbitzu edo produktuetan sortzen diren mugarrietan oinarritutako kostu gisa erregistratzeko.

Mugarrietarako saltzaileen faktura-lerroek beti egin behar dute erreferentzia prezio finkoko fakturazio-metodoa duen azpikontratazio-lerroa. Mugarrien saltzaileen faktura-lerro batek azpikontratuaren lerro bati erreferentzia egiten badio, proiektu-kudeatzaileek saltzaileen denboraren azpiko kostuak, gastuak edo materialak bat etorriko eta egiaztatuko ditu azpikontratuaren lerroari erreferentzia egiten diotenak saltzaileak fakturatzen duen mugarrian.

Ondorengo taulan fitxategien eremuei buruzko informazioa ematen da mugarrien saltzailearen faktura-lerroan.

| Eremua | Deskribapenak | Inpaktu funtzionala |
| --- | --- | --- |
| Eman izena | Identifikazioan laguntzeko saltzailearen faktura-lerroaren izena. | Izena saltzailearen faktura-lerroetan oinarritutako bilaketa guztietan lehen zutabe gisa erakutsiko da. |
| Deskribapenak | Saltzaileak saltzailearen faktura-lerroan fakturatzen dituen zerbitzuen deskribapen laburra. | Batere ez |
| Azpikontratua | Zerbitzuak hasiera batean agindutako azpikontratua. | Saltzaileen fakturarako azpikontratu bat hautatzen denean, saltzaileen fakturako lerro guztiek hautapen hori heredatuko dute. Saltzaileen faktura batek ezin du izan azpikontratu desberdinak aipatzen dituzten hornitzaileen faktura lerroak. |
| Azpikontratuaren lerroa | Zerbitzuak eskatuta azpikontratuaren lerroa. Hauta daitezkeen azpikontratuaren lerroen zerrenda hautatutako azpikontratuaren lerroetara mugatzen da. | Mugarrietarako saltzaileen faktura-lerro batean azpikontratazio-lerro bat hautatzen denean, **Rola** eta **Transakzio kategoria** eremuak eta produktuekin erlazionatutako eremuak ez dira garrantzirik eta ez daude eskuragarri. **Kantitatea**, **Unitatea**, eta **Unitate taldea** eremuak ere ez dira garrantzitsuak mugarrietan oinarritutako hornitzaileen faktura-lerroetarako. |
| Transakzioaren data | Saltzaileen faktura-lerroaren benetako kostua proiektuan erregistratuko den data. | Batere ez |
| Transakzio-klasea | Hautatu **Mugarria** Azpikontratazio-lerro batean definitu zen amaitutako mugarri baten saltzaile-faktura erregistratzeko. | Batere ez |
| Mugarria | Hautatu gisa markatuta dagoen azpikontratazio-lerroan definitzen den mugarria **Fakturatzeko prest**. | Azpikontratatuaren lerroaren mugarri bat **fakturatzeko prest** egoeran dagoena hautatu daitek saltzailearen faktura-lerroan. |
| Project | Fakturatutako zerbitzuak erabili diren proiektuaren izena. | Eremua beharrezkoa da eta ezin da hutsik utzi. |
| Zeregina | Fakturatutako zerbitzuak erabili diren proiektuaren zereginaren izena. Eremu hau proiektu bat hautatzen bada soilik dago erabilgarri. Proiektuko zeregina hautatzea aukerakoa da. | Eremu hau hutsik geratzen bada, proiektuaren kudeatzaileak hornitzaileen faktura-lerroa proiektuko edozein zereginetan erlazionatutako azpikontratuaren erroaren transakzio motaren erregistratutako baliabideak denborarekin lotu dezake. Saltzaileen faktura-lerroak ez badu azpikontratuaren lerrorik aipatzen, eta eremu hau hutsik geratzen bada, saltzaileen faktura-lerroak sortzen duen kostu erreala ez da fakturatu gabeko salmenta errealekin lotuko. Kasu honetan, zereginetan oinarritutako fakturazioa konfiguratzen bada, baliteke kostuak azken bezeroari ezin izango zaizkio fakturatu. |
| Mugarriaren zenbatekoa | Sartu gisa markatuta dagoen azpikontratazio-lerroan definitzen den mugarriaren balioa Fakturatzeko prest. | Batere ez |
| Salmenten zerga | Idatzi salmenta-zergaren zenbatekoa. | Batere ez |
| Zenbatekoa guztira | Saltzailearen faktura-lerroaren guztizko kantitatea barne hartutako zergak. *Mugarri kopurua* + *Salmenta zergak*. gisa kalkulatzen da eremua. | Batere ez |

> [!NOTE]
> Azpikontratu-lerroaren mugarri bati erreferentzia egiten dion hornitzaileen faktura-lerroa sortzen denean, azpikontratuaren mugarriaren egoera eguneratzen da **Saltzaileen faktura sortu da**. Ondoren, saltzaileen faktura hori berresten denean, azpikontratuaren lerroaren mugarriaren egoera eguneratzen da **Saltzaileen faktura berretsi da**.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
