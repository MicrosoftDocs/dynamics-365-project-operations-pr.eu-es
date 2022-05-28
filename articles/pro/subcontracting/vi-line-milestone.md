---
title: Mugarrietarako saltzaileen faktura-lerroak
description: Gai honek azpikontratu bateko mugarrietarako hornitzaileen faktura-lerroak nola sortu azaltzen du.
author: rumant
ms.date: 03/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 4fa11e2a4f459016b3ce141b03fe97e55c9a2759
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8590607"
---
# <a name="vendor-invoice-lines-for-milestones"></a>Mugarrietarako saltzaileen faktura-lerroak

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Saltzaileen faktura bat Microsoft-en Dynamics 365 Project Operations saltzaileen faktura-lerroak izan ditzake azpikontratu-lerro batean definitutako mugarrietarako. Proiektu-kudeatzaileek saltzaileen faktura-lerroak erabil ditzakete mugarrietarako kontratatzen diren zerbitzuen kostuak proiekturako kontratatzen diren zerbitzu edo produktuetan sortzen diren mugarrietan oinarritutako kostu gisa erregistratzeko.

Mugarrien saltzaileen faktura-lerroek beti egin behar dute erreferentzia prezio finkoko fakturazio-metodoa duen azpikontratazio-lerroa. Mugarrien saltzaileen faktura-lerro batek azpikontratu-lerro bati erreferentzia egiten dionean, proiektu-kudeatzaileek azpikontratu-lerro horri erreferentzia egiten dioten denbora, gastu edo materialen azpiko kostuak saltzaileak fakturatzen ari den mugarriarekin lotu eta egiaztatu ahal izango dituzte.

Hurrengo taulak hornitzaileen faktura-lerroetako eremuei buruzko informazioa eskaintzen du mugarrietarako.

| Eremua | Deskribapenak | Inpaktu funtzionala |
| --- | --- | --- |
| Eman izena | Saltzaileen faktura-lerroaren izena, identifikazioan laguntzeko. | Izen hau saltzaileen faktura-lerroetan oinarritutako bilaketa guztietan lehen zutabe gisa agertuko da. |
| Deskribapenak | Saltzaileak fakturatzen dituen zerbitzuen deskribapen laburra hornitzailearen faktura lerroan. | Batere ez |
| Azpikontratua | Zerbitzuak hasiera batean agindutako azpikontratua. | Saltzaileen fakturarako azpikontratu bat hautatzen denean, saltzaileen fakturako lerro guztiek hautapen hori heredatuko dute. Saltzaile-faktura batek ezin du izan azpikontratu desberdinak aipatzen dituzten hornitzaile-faktura-lerroak. |
| Azpikontratazio lerroa | Zerbitzuak agindutako azpikontratazio lerroa. Hauta daitezkeen azpikontratazio-lerroen zerrenda hautatutako azpikontratuko lerroetara mugatzen da. | Mugarrietarako saltzaileen faktura-lerro batean azpikontratazio-lerro bat hautatzen denean, **Rola** eta **Transakzio kategoria** eremuak eta produktuekin erlazionatutako eremuak ez dira garrantzirik eta ez daude eskuragarri. The **Kantitatea**, **·**, eta **Unitate taldea** eremuak ere ez dira garrantzitsuak mugarrietan oinarritutako hornitzaileen faktura-lerroetarako. |
| Transakzioaren data | Saltzaileen faktura-lerroaren benetako kostua proiektuan erregistratuko den data. | Batere ez |
| Transakzio-klasea | Hautatu **Mugarria** Azpikontratazio-lerro batean definitu zen amaitutako mugarri baten saltzaile-faktura erregistratzeko. | Batere ez |
| Mugarria | Hautatu gisa markatuta dagoen erlazionatutako azpikontratuaren lerroan definitzen den mugarria **Fakturatzeko prest**. | Egoera duten azpikontratazio-lerroaren mugarriak **Fakturatzeko prest** saltzaileen faktura-lerro batean hauta daiteke. |
| Project | Fakturatzen ari diren zerbitzuak erabili diren proiektuaren izena. | Eremu hau beharrezkoa da eta ezin da hutsik utzi. |
| Zeregina | Fakturatzen ari diren zerbitzuak erabili diren proiektuaren atazaren izena. Eremu hau proiektu bat hautatzen bada soilik dago erabilgarri. Proiektuko ataza hautatzea aukerakoa da. | Eremu hau hutsik geratzen bada, proiektuaren kudeatzaileak hornitzaileen faktura-lerroa proiektuko edozein zereginetan erregistratutako erlazionatutako azpikontratu-lerroko transakzio-klasearekin lo dezake. Saltzaileen faktura-lerroak ez badu azpikontratazio-lerrorik aipatzen, eta eremu hau hutsik geratzen bada, hornitzaile-faktura-lerroak sortzen duen kostu erreala ez da fakturatu gabeko salmenta-errealekin lotuko. Kasu honetan, zereginetan oinarritutako fakturazioa konfiguratzen bada, baliteke kostuak ezin izango zaizkiola azken bezeroari fakturatu. |
| Mugarriaren zenbatekoa | Sartu fakturatzeko prest dagoen azpikontratuaren lerroan definitutako mugarriaren balioa. | Batere ez |
| Salmenten zerga | Idatzi salmenta-zergaren zenbatekoa. | Batere ez |
| Kopuru osoa | Saltzaileen faktura-lerroaren guztizko zenbatekoa, zergak barne. Eremu hau honela kalkulatzen da *Mugarri kopurua* + *Salmenta zerga*. | Batere ez |

> [!NOTE]
> Azpikontratu-lerroaren mugarri bati erreferentzia egiten dion hornitzaileen faktura-lerroa sortzen denean, azpikontratuaren mugarriaren egoera eguneratzen da.**Saltzaileen faktura sortu da**. Ondoren, saltzaileen faktura hori berresten denean, azpikontratuaren lerroaren mugarriaren egoera eguneratzen da **Saltzaileen faktura berretsi da**.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
