---
title: Kudeatu proiektuetan oinarritutako kontratuaren lerroetako hainbat bezero - arina
description: Gai honek proiektuan oinarritutako kontratuaren lerroetako hainbat bezero kudeatzeari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/27/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f28e7d1363647621f7bd23504aa6d4ea3fc95fc9
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181579"
---
# <a name="manage-multiple-customers-on-project-based-contract-lines---lite"></a>Kudeatu proiektuetan oinarritutako kontratuaren lerroetako hainbat bezero - arina

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proiektuetan oinarritutako kontratu lerroek ordainketaz arduratzen diren bezeroen zerrenda barne har dezakete. Proiektuetan oinarritutako kontratuaren lineako bezeroen zerrenda kontratuaren bezeroen zerrenda bera izan daiteke, baina hori ez da beharrezkoa. Proiektuaren aurrekontua irabazten denean eta proiektuaren kontratua sortzen denean, aurrekontuaren lerroan agertzen den bezeroen zerrenda dagokion kontratu lerroan kopiatzen da. Aurrekontuaren bezeroak kontratuan kopiatzen dira.

Proiektuaren kontratua fakturatzen denean, proiektuan oinarritutako kontratu linearen bezeroen zerrendak lehentasuna du kontratuko bezeroen zerrendaren gainetik. Proiektuaren kontratuko bezeroen zerrenda kontratu lerro berriak lehenesteko soilik erabiltzen da.

Kontratatutako bezero guztiak **Bezeroak** proiektuaren kontratuaren fitxa, kontratuaren lineako bezero gisa, proiektuaren kontraturako sortutako kontratu lerro berrietan. Lehendik dauden kontratu lerroek ez dituzte ondoren sortutako kontratu bezeroen erregistro berriak oinordetuko.

## <a name="create-update-or-delete-a-contract-line-customer-record"></a>Sortu, eguneratu edo ezabatu kontratuaren lineako bezeroaren erregistroa

Kontratu-lerroaren bezero bat sortu, eguneratu edo ezaba dezakezu Kontratu-lerroen bezeroak fitxan, proiektuan oinarritutako kontratu-lerroaren orrian. Proiektuan oinarritutako kontratu lerroan bezero berri bat gehitzen denean, kontratu orokorrean ere gehitzen dira kontratuko bezero gisa, fakturazio ehuneko lehenetsiaren ehuneko zeroarekin. Kontratu orokorreko fakturazio zatiaren portzentajea kontratu lerro berrietara eta proiektuaren azken kontratura kopiatzen da. Hala ere, kontratuaren fakturazioan, fakturazio zatitutako ehunekoa erabiltzen da kontratu lerro mailan eta ez fakturazio zatitutako ehunekoa kontratu maila orokorrean.

Jarraian, eremuko eremuak daude **Kontratua** proiektuan oinarritutako kontratu lerro baten bezeroaren erregistroa, harekin lanean ari zaren bitartean kontuan hartzeko:

| Eremua | Kokapena | Deskribapena | Downstream eragina |
| --- | --- | --- | --- |
| **Kontua** | Sareta editagarria **Kontratuaren bezeroak** fitxa eta **Nagusia** eta **Sortu bizkor** kontratuaren bezeroarentzako inprimakiak. | Kontu aktibo guztiak. Eremu hau blokeatuta dago erregistroa sortu ondoren. Eremua eguneratzeko, ezabatu erregistroa eta sortu erregistro berria. Benetako datuak grabatu badituzu, ezin duzu erregistroa ezabatu. Hala ere, fakturazio zatitutako ehunekoa zero gisa marka dezakezu kontu horretarako. Erregistroa zero gisa markatzen denean, bezero honi egotzitako edo banatutako etorkizuneko kostuen eta diru-sarreren faktoreek eragina izango dute. | Gehitu eta gordetzeko kontu zerrenda nagusitik kontu bat hautatzen duzunean, kontratuko linea bezeroa ere kontratu bezero gisa gehitzen da. Kontratu-lineako bezeroak fakturak sortzen direnean erabiltzen dira. |
| **Fakturazioko zatitzearen ehunekoa** | Sareta editagarria **Kontratuaren bezeroak** fitxa eta **Nagusia** eta **Sortu bizkor** kontratuaren bezeroarentzako inprimakiak. | Eremu honek kontratu lineako bezero honi egotziko zaion fakturatu gabeko salmenta transakzio bakoitzaren ehunekoa adierazten du. | Kontratu-lineako bezeroak eta fakturazio zatitutako ehunekoak erabiltzen dira egiazkoak onartu ondoren faktura sortzen denean eta faktura sortzen denean. |
| **Ez gainditzeko muga** | Sareta editagarria **Kontratuaren bezeroak** fitxa eta **Nagusia** eta **Sortu bizkor** kontratuaren bezeroarentzako inprimakiak. | Bezero honi kontratu lerroagatik fakturatuko zaion zenbateko osoari negoziatutako muga edo muga dagoen adierazten du. | Kontratu-lerroaren bezeroarentzako ez gainditzeko muga erabiltzen da egiazkoak sortu eta fakturak sortzen direnean. |
| **Biribiltzen da** | Sareta editagarria **Kontratuaren bezeroak** fitxa eta **Nagusia** eta **Sortu bizkor** kontratuaren lerroaren bezeroarentzako inprimakiak. | Eremu honek proiektuan oinarritutako kontratu lerro honetako bezero biribilketa lehenetsia den adierazten du. | Fakturazio zatitutako ehunekoaren arabera benetako bat sortzen duzunean, desberdintasun biribil batzuk egon daitezke. Bezero honi kasu honetan biribiltzeko aldeak egotzi zaizkio. |

## <a name="edit-billing-split-percentages"></a>Editatu fakturazioko zatitzearen ehunekoa

Fakturazio zatitutako ehunekoak saretan editatu daitezke. Fakturazio zatitutako ehunekoak ehuneko 100 guztira ez direnean, errore bat gertatuko da. Fakturazio zatien ehunekoak editatu ondoren, freskatu orria errorea ezabatzeko.

Aukeratu ere egin dezakezu **Banatu uniformeki** kontratu-lerroan bezeroen azpisarean. Ekintza honek fakturazio banaketak banatzen dizkie kontratu lineako bezero guztiei. Biribiltze faktorerik badago, biribiltze bezeroari gehituko zaio. Kontratu lineako bezero bat beti bezala etiketatuta dago **Biribilketa** bezeroarekin **Biribilketa** bandera ezarri da **Bai**.
