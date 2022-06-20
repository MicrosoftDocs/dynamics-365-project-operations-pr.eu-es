---
title: Saltzaileen fakturen goiburuaren xehetasunak
description: Artikulu honetan Microsoft ko hornitzailearen fakturaren buruan ematen den funtzionaltasuna azaltzen da Dynamics 365 Project Operations.
author: rumant
ms.date: 03/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 95f84f2d2a357abbd8d507705412a0434b44f658
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8929843"
---
# <a name="header-details-for-vendor-invoices"></a>Saltzaileen fakturen goiburuaren xehetasunak

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Artikulu honetan Microsoft ko hornitzailearen fakturaren buruan ematen den funtzionaltasuna azaltzen da Dynamics 365 Project Operations.

Proiektu-kudeatzaileek proiektuak planifikatzen eta gauzatzen dituzten heinean, azpikontratistak erabil ditzakete eta hornitzaileen produktuak eta zerbitzuak eros ditzakete. Proiektu bat gauzatzen den bitartean, hornitzaileekin azpikontratuetan eskuratzen diren zerbitzu, material eta gastu-kategorien kostuak egiten dira. Hornitzaileek kostu horiek proiektuei fakturatzen dizkiete, hornitzaileen fakturak sortuz.

Hurrengo taulan, proiektu-eragiketen hornitzaileen fakturen arloei buruzko informazioa ematen da.

| Eremua | Deskribapenak | Inpaktu funtzionala |
| --- | --- | --- |
| Eman izena | Hornitzailearen fakturaren izena. | Hornitzaileen fakturen zerrenda zabalgarri guztietan, hornitzailearen fakturaren izena lehen zutabean agertzen da, hornitzailearen faktura identifikatzen laguntzeko. Aurrez zehaztuta, azpikontratu batetik hornitzaile-faktura bat sortzen denean, hornitzailearen fakturaren izenaren **eremua** azpikontratuaren izena eta egungo data izango dituen balio batean ezartzen da. |
| Deskribapenak | Hornitzailearen fakturan fakturatzen diren zerbitzu eta produktuen deskribapen laburra. | Batere ez |
| Saltzailea | Produktu eta zerbitzuengatik fakturatzen ari den enpresaren izena. Enpresa horrek saltzailearen edo **hornitzailearen zerrenda duen kontu-erregistroa** **izan behar du**. | <p>Hautatutako hornitzailearen arabera, aurrez zehaztutako balioak automatikoki sartzen dira honako eremu hauetan:</p><ul><li>Moneta</li><li>Prezio-zerrendak</li><li>Ordainketa-baldintzak</li><li>Ordainketa-helbidea</li></ul> |
| Azpikontratua | Hornitzailearen fakturarako azpikontratuari buruzko erreferentzia. | <p>Hautatutako azpikontratuaren arabera, aurrez zehaztutako balioak automatikoki sartzen dira honako eremu hauetan:</p><ul><li>Moneta</li><li>Prezio-zerrendak</li><li>Ordainketa-baldintzak</li><li>Ordainketa-helbidea</li></ul><p>Hornitzailearen fakturan aukeratutako azpikontratua hornitzailearen faktura-lerroetan sartzen da, aldez aurretik zehaztuta, eta ezin da bertan aldatu.</p> |
| Fakturaren data | Hornitzailearen faktura konfirmatzen denean sortuko diren benetako kostuen data. | Fakturaren data erosketa-prezio zuzenen zerrenda aukeratzeko ere erabiltzen da, dela lotutako hornitzaileari erantsitako prezio-zerrendetakoa, dela proiektuaren parametroetakoa. |
| Egoeraren arrazoia | Hornitzailearen fakturaren egoera. | <p>Estatuak zehazten du hornitzailearen faktura non dagoen negozio-prozesuan eta ea editatu daitekeen. Hauek dira eskuragarri dauden balioetako batzuk:</p><ul><li>**Zirriborroa** : hornitzailearen faktura editatu daiteke.</li><li>**Baieztatuta: hornitzailearen** faktura egiaztatu eta berretsi egin zen. Hornitzaileen fakturak ezin dira editatu, ezta ezabatu ere.</li><li>**Prozesuan** : hornitzailearen faktura berrikusten ari dira. Hornitzaileen fakturak egoera honetan editatu daitezke, baina ezin dira ezabatu.</li><li>**Bertan behera:** hornitzailearen faktura baliogabetu egin zen. Hornitzaileen fakturak ezin dira editatu, ezta ezabatu ere.</li></ul> |
| Moneta | Hornitzailea hornitzailearen fakturan produktuak eta zerbitzuak fakturatzen ari den txanpona. | Azpikontratu bati erreferentzia egiten dion hornitzaile-faktura batean, azpikontratuko dinasa aurrez zehaztuz sartzen da, hornitzailearen fakturaren txanpon gisa. Azpikontratu bati erreferentziarik egiten ez dion hornitzaile-faktura batean, aurrez zehaztutako balioa hornitzaile-kontuaren erregistroan sartzen da eta alda daiteke. Hornitzailearen faktura bat gorde ondoren, txanpona ezin da argitaratu. |
| Kontratazio-unitatea | Hornitzailearen zerbitzuak eta / edo produktuak jasotzeaz arduratzen den enpresaren banaketa. | Batere ez |
| Ordainketa-baldintzak | Jaulkitzen diren hornitzaileen fakturen ordainketa-baldintzak. Lehenetsitako balioa automatikoki sartzen da saltzailearen kontuaren erregistrotik. | Azpikontratu bat ordaintzeko baldintzak azpikontratuarekin lotutako hornitzaileen faktura guztietan kopiatzen dira. Ordainketa-baldintzak eguneratu egin daitezke hornitzailearen fakturak egoera borratzailea **badu**. |
| Ordainketa-helbidea | Ordainketak bidali behar zaizkion saltzailearen helbidea. Lehenetsitako balioa automatikoki sartzen da saltzailearen kontuaren erregistrotik. | Azpikontratu baten ordainketa-helbidea azpikontratu horretarako sortzen diren hornitzaileen faktura guztien ordainketa-helbide gisa kopiatzen da. Ordainketa-helbidea eguneratu egin daiteke hornitzailearen fakturak estatu borratzailea **badu**. |
| Guztizko partziala | Hornitzailearen fakturak lerrorik ez badu, sartu fakturaren azpitotala zergen aurretik. Hornitzailearen fakturak lerroak baditu, alor hau irakurketa hutsa da. Kasu horretan, erakusten den zenbatekoa hornitzailearen fakturaren linea guztien zenbateko subtotala da. | Batere ez |
| Zerga osoa | Hornitzailearen fakturak lerrorik ez badu, sartu azpikontratuaren gaineko zerga guztiak. Hornitzailearen fakturak lerroak baditu, alor hau irakurketa hutsa da. Kasu honetan, hornitzailearen fakturan lerro guztietako zerga-kopuruen batura erakusten da. | Batere ez |
| Zenbateko osoa | Kalkulatutako eremu horrek hornitzailearen fakturaren zenbateko osoa erakusten du, zergak sartu ondoren. | Batere ez |

> [!NOTE]
> Hornitzailearen faktura baten eremu hauek ezin dira aldatu hornitzailearen faktura gorde ondoren: Hornitzailea, Azpikontratua, Dirua, Kontratazio Unitatea **eta** Ordainketa **Baldintzak.** **·** **·** **·** Hornitzaile-faktura batean arlo horietan aldaketaren bat behar bada, hornitzailearen faktura ezabatu eta hornitzailearen faktura berri bat sortu behar da.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
