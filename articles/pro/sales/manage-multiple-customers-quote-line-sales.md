---
title: Kudeatu proiektuetan oinarritutako eskaintzaren lerroetako hainbat bezero - arina
description: Gai honek proiektuak oinarritutako eskaintza-lerroetan bezero anitz kudeatzeko moduari buruzko informazioa azaltzen du.
author: rumant
ms.date: 10/06/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: fbd0c17de3de8dc4cd84860851fb5837b86586cd
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8927773"
---
# <a name="manage-multiple-customers-on-project-based-quote-lines---lite"></a>Kudeatu proiektuetan oinarritutako eskaintzaren lerroetako hainbat bezero - arina

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proiektuetan oinarritutako aurrekontu lerroek aurrekontu lerro bakoitzak ordaintzen duten bezeroen zerrenda duten eszenatokiak onartzen ditu. Proiektuan oinarritutako aurrekontuaren lerroan dagoen bezeroen zerrenda aurrekontuko bezeroen zerrenda bezalakoa izan daiteke. Bezeroen zerrenda ere desberdina izan dadin alda dezakezu. Proiektuaren eskaintza irabazten denean, proiektuan oinarritutako aurrekontu lerroan bezeroen zerrenda dagokion proiektuan oinarritutako kontratu lerroan kopiatzen da behin-behineko proiektu-kontratua sortzeko. Proiektuan oinarritutako aurrekontuaren bezeroak proiektuaren kontratuan kopiatzen dira.

Proiektuaren azken kontratua fakturatzen duzunean, proiektuan oinarritutako kontratuaren lineako bezeroen zerrendak lehentasuna du proiektuaren kontratuko zerrendan. Proiektuaren kontratuko bezeroen zerrenda proiektuaren kontratu lerro berriak lehenesteko soilik erabiltzen da.

Aurrekontuaren bezero guztiak **Bezeroak** proiektuaren aurrekontuaren fitxa lehenetsitako lerroen bezero gisa, proiektuaren aurrekonturako sortutako proiektuetan oinarritutako aurrekontu lerro berrietan. Lehendik dauden proiektuetan oinarritutako aurrekontu lerroek ez dituzte ondoren sortutako aurrekontu bezeroen erregistro berriak jasotzen.

## <a name="create-update-or-delete-a-quote-line-customer-record"></a>Sortu, eguneratu edo ezabatu aurrekontu-lerroaren bezeroaren erregistroa

Aurrekontuaren bezeroa sor dezakezu, eguneratu edo ezabatu **Aipatu lineako bezeroak** fitxan **Proiektuetan oinarritutako aurrekontu lerroa** orrialdea. Proiektuan oinarritutako aurrekontu lerroan bezero berri bat gehitzen duzunean, bezeroa aurrekontu orokorrera gehitzen da aurrekontu bezero gisa, fakturazio portzentaje lehenetsia % 0ko aurrekontu orokorraren gainean. Aurrekontu orokorraren fakturazio zatitutako portzentajea aurrekontu lerro berrietara eta proiektuaren kontratu bateratura kopiatzen da. Hala ere, kontratuagatik fakturatzen duzunean, aurrekontu lerro mailan fakturazio zatitutako ehunekoa erabiltzen da, ez fakturazio zatitutako ehunekoa kontratu maila orokorrean. 

Hurrengo taulan proiektuan oinarritutako aurrekontu lerro bateko aurrekontu lerroaren bezeroaren erregistroaren eremuak agertzen dira.

| Eremua | Kokapena | Azalpena eta argibideak | Downstream eragina |
| --- | --- | --- | --- |
| **Kontua** | Sarean editagarria batean **Aipatu lineako bezeroak** fitxa, inprimaki nagusiak eta aurrekontu lerroaren bezeroarentzako azkar sortzeko inprimakia. | Kontu aktibo guztien zerrendak. Eremu hau blokeatuta dago erregistroa sortu ondoren. Eremua eguneratu behar baduzu, ezabatu eta birsortu erregistroa. Benetako datuak grabatu badituzu, ezin duzu erregistroa ezabatu. | Gehitu beharreko kontu zerrenda nagusitik kontu bat hautatzen duzunean, eskaintza-lerroaren bezeroa eskaintzaren bezero gisa ere gehitzen da gordetzen duzunean. Aurrekontuaren lineako bezeroak proiektuaren kontratuko lineako bezeroei kopiatzen zaizkie aurrekontua irabazten denean. |
| **Fakturazioko zatitzearen ehunekoa** | Sarean editagarria batean **Aipatu lineako bezeroak** fitxa, inprimaki nagusiak eta aurrekontu lerroaren bezeroarentzako azkar sortzeko inprimakia. | Aurrekontu lerro honen bezeroari egotziko zaion fakturatu gabeko salmenta transakzio bakoitzaren ehunekoa adierazten du. | Proiektu-kontratuaren lerroaren bezeroen gainean kopiatuta. |
| **Ez gainditzeko muga** | Sarean editagarria batean **Aipatu lineako bezeroak** fitxa, inprimaki nagusiak eta aurrekontu lerroaren bezeroarentzako azkar sortzeko inprimakia. | Eskaintzadun lerro honengatik bezero honi fakturatuko zaion zenbateko orokorraren muga edo muga negoziatua dagoen adierazten du. | Eskaintza bat irabazten denean, proiektuaren kontratuaren lerroko bezeroen gainean kopiatuta. |
| **Biribiltzen da** | Sarean editagarria batean **Aipatu lineako bezeroak** fitxa, inprimaki nagusiak eta aurrekontu lerroaren bezeroarentzako azkar sortzeko inprimakia. | Proiektuan oinarritutako aurrekontu lerro honetako bezero biribilketa lehenetsia den ala ez adierazten du. | Eskaintza bat irabazten denean, proiektuaren kontratuko bezeroen gainean kopiatuta. |

## <a name="edit-billing-split-percentages"></a>Editatu fakturazioko zatitzearen ehunekoa

Fakturazio zatitutako ehunekoak linean edita ditzakezu. Fakturazio zatitutako ehunekoak % 100 guztira ez direnean, errore bat gertatzen da. Fakturazio zatitutako ehunekoak editatu ondoren, freskatu aurrekontuaren lerroaren orria errorea ezabatzeko.

Erabili aurrekontu lerroaren bezeroen azpisailean modu uniformean banatu ekintza aurrekontu lerro bezero guztiei fakturazio zatiak banatzeko. Biribiltze faktore bat badago, hori biribiltze bezeroari gehituko zaio. Aurrekontu lerroetako bezeroetako bat beti biribildutako bezero gisa etiketatuta dago, hau da, aurrekontu lerroaren bezeroaren erregistroak biribiltze bandera ezarrita du **Bai**. 


[!INCLUDE[footer-include](../../includes/footer-banner.md)]