---
title: Kudeatu proiektuetan oinarritutako kontratuaren lerroetako hainbat bezero
description: Artikulu honek hainbat bezero dituzten kontratu-lerroekin eta kontratuekin lan egiteari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 10/22/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 0e0652d4b9cdb0489d4f191ef0f3b251e39262f5
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8914847"
---
# <a name="manage-multiple-customers-on-project-based-contract-lines"></a>Kudeatu proiektuetan oinarritutako kontratuaren lerroetako hainbat bezero

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Proiektuetan oinarritutako kontratu lerroek ordainketaz arduratzen diren bezeroen zerrenda barne har dezakete. Proiektuetan oinarritutako kontratuaren lineako bezeroen zerrenda kontratuaren bezeroen zerrenda bera izan daiteke, baina hori ez da beharrezkoa. Proiektuaren aurrekontua irabazten denean eta proiektuaren kontratua sortzen denean, aurrekontuaren lerroan agertzen den bezeroen zerrenda dagokion kontratu lerroan kopiatzen da. Aurrekontuaren bezeroak kontratuan kopiatzen dira.

Proiektuaren kontratua fakturatzen denean, proiektuan oinarritutako kontratu linearen bezeroen zerrendak lehentasuna du kontratuko bezeroen zerrendaren gainetik. Proiektuaren kontratuko bezeroen zerrenda kontratu lerro berriak lehenesteko soilik erabiltzen da.

Kontratatutako bezero guztiak **Bezeroak** proiektuaren kontratuaren fitxa, kontratuaren lineako bezero gisa, proiektuaren kontraturako sortutako kontratu lerro berrietan. Lehendik dauden kontratu lerroek ez dituzte ondoren sortutako kontratu bezeroen erregistro berriak oinordetuko.

## <a name="create-update-or-delete-a-contract-line-customer-record"></a>Sortu, eguneratu edo ezabatu kontratuaren lineako bezeroaren erregistroa

Kontratu-lerroaren bezero bat sortu, eguneratu edo ezaba dezakezu **Kontratu-lerroen bezeroak** fitxan, **Proiektuan oinarritutako kontratu-lerroa** orrian. Proiektuan oinarritutako kontratu lerroan bezero berri bat gehitzen denean, kontratu orokorrean ere gehitzen dira kontratuko bezero gisa, fakturazio ehuneko lehenetsiaren ehuneko zeroarekin. Kontratu orokorreko fakturazio zatiaren portzentajea kontratu lerro berrietara eta proiektuaren azken kontratura kopiatzen da. Hala ere, kontratuaren fakturazioan, fakturazio zatitutako ehunekoa erabiltzen da kontratu lerro mailan eta ez fakturazio zatitutako ehunekoa kontratu maila orokorrean. 

Jarraian, eremuko eremuak daude Kontratua proiektuan oinarritutako kontratu lerro baten bezeroaren erregistroa, harekin lanean ari zaren bitartean kontuan hartzeko:

| Eremua | Kokapena | Deskribapena | Downstream eragina |
| --- | --- | --- | --- |
| Account | Sareta editagarria **Kontratuaren lerroaren bezeroak** fitxa eta Nagusia eta Sortu bizkor kontratuaren lerroaren bezeroarentzako inprimakiak | Kontu aktibo guztiak. Eremu hau blokeatuta dago erregistroa sortu ondoren. Eremua eguneratzeko, ezabatu erregistroa eta sortu erregistro berria. Benetako datuak grabatu badituzu, ezin duzu erregistroa ezabatu. Hala ere, fakturazio zatitutako ehunekoa zero gisa marka dezakezu kontu horretarako. Erregistroa zero gisa markatzen denean, bezero honi egotzitako edo banatutako etorkizuneko kostuen eta diru-sarreren faktoreek eragina izango dute. | Gehitu eta gordetzeko kontu zerrenda nagusitik kontu bat hautatzen duzunean, kontratuko linea bezeroa ere kontratu bezero gisa gehitzen da. Kontratu-lineako bezeroak fakturak sortzen direnean erabiltzen dira. |
| Fakturazioko zatitzearen ehunekoa | Sareta editagarria **Kontratuaren lerroaren bezeroak** fitxa eta Nagusia eta Sortu bizkor kontratuaren lerroaren bezeroarentzako inprimakiak | Eremu honek kontratu lineako bezero honi egotziko zaion fakturatu gabeko salmenta transakzio bakoitzaren ehunekoa adierazten du. | Kontratu-lineako bezeroak eta fakturazio zatitutako ehunekoak erabiltzen dira egiazkoak onartu ondoren faktura sortzen denean eta faktura sortzen denean. |
| Ez gainditzeko muga | Sareta editagarria **Kontratuaren lerroaren bezeroak** fitxa eta Nagusia eta Sortu bizkor kontratuaren lerroaren bezeroarentzako inprimakiak | Bezero honi kontratu lerroagatik fakturatuko zaion zenbateko osoari negoziatutako muga edo muga dagoen adierazten du. | Kontratu-lerroaren bezeroarentzako ez gainditzeko muga erabiltzen da egiazkoak sortu eta fakturak sortzen direnean. |
| Jabetzadun enpresa | Sareta editagarria **Eskaintzaren lerroaren bezeroak** fitxa eta Nagusia eta Sortu bizkor eskaintzaren lerroaren bezeroarentzako inprimakiak | Bezero hau konfiguratuta dagoen pertsona juridikoa. Eremu hau irakurtzeko soilik da eta aurrekontuaren enpresa titularra da. Hemen gehitu beharreko bezeroen zerrenda **Kontua** eremua jabea den enpresa honetatik zerrendara iragazita dago. | Jabe den enpresa baten kontzeptua pertsona juridiko baten kontzeptuarekin bat dator. Proiektu honetatik sortutako kostu eta diru-sarrera guztiak enpresa jabearen liburu nagusian kontabilizatzen dira. |
| Biribiltzen da | Sareta editagarria **Kontratuaren lerroaren bezeroak** fitxa eta Nagusia eta Sortu bizkor kontratuaren lerroaren bezeroarentzako inprimakiak | Eremu honek proiektuan oinarritutako kontratu lerro honetako bezero biribilketa lehenetsia den adierazten du. | Fakturazio zatitutako ehunekoaren arabera benetako bat sortzen duzunean, desberdintasun biribil batzuk egon daitezke. Bezero honi kasu honetan biribiltzeko aldeak egotzi zaizkio. |

## <a name="edit-billing-split-percentages"></a>Editatu fakturazioko zatitzearen ehunekoa

Fakturazio zatitutako ehunekoak saretan editatu daitezke. Fakturazio zatitutako ehunekoak ehuneko 100 guztira ez direnean, errore bat gertatuko da. Fakturazio zatien ehunekoak editatu ondoren, freskatu orria errorea ezabatzeko.

Aukeratzen ere saia zaitezke **Banatu uniformeki** kontratu-lerroan bezeroen azpisarean. Ekintza honek fakturazio banaketak banatzen dizkie kontratu lineako bezero guztiei. Biribiltze faktorerik badago, biribiltze bezeroari gehituko zaio. Kontratu lineako bezero bat beti bezala etiketatuta dago **Biribilketa** bezeroarekin **Biribilketa** bandera ezarri da **Bai**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]