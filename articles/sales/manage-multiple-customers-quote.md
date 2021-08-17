---
title: Kudeatu hainbat bezero proiektuaren eskaintza batean
description: Gai honek proiektua finantzatuko duten hainbat bezeroekin aurrekontuak lantzeari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: eef3e8754cdfdb810ffd5283976445edbb126b51e20d5b51d603d2ba9e2c02c9
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6991966"
---
# <a name="manage-multiple-customers-on-a-project-quote"></a>Kudeatu hainbat bezero proiektuaren eskaintza batean

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Proiektuaren aurrekontuek proposamena akordioa finantzatuko duten bezero anitzekin lotzen duten agertokia onartzen dute. Eskaintzaren **Laburpena** fitxak akordioaren bezero nagusia identifikatzen duen **Bezero potentziala** eremua du. Akordiorako beste bezero batzuk konfigura daitezke **Bezeroak** proiektuaren aurrekontuaren fitxa.

Aurrekontuaren bezero guztiak **Bezeroak** proiektuaren aurrekontuaren fitxa lehenetsitako lerroen bezero gisa, aurrekonturako sortutako proiektuetan oinarritutako aurrekontu lerro **berrietan**. Lehendik dauden proiektuetan oinarritutako aurrekontu lerroek ez dituzte ondoren sortutako aurrekontu bezeroen erregistro berriak jasotzen.

Aurrekontuaren bezeroak eta aurrekontuen linea bezeroak gehitu, eguneratu edo ezabatu daitezke aurrekontua irabazi aurretik. Aurrekontuaren baliozko bezeroa bezero titular gisa eratu behar da enpresa titularrean edo pertsona juridikoan **Bezeroak** orrialdea. Pertsona juridikoak **Proiektuen kudeaketa eta kontabilitatea** modulua Dynamics 365 Project Operations eta enpresa gisa egiten dira eskuragarri Project Operations-en **Proiektuen salmenta eta Entrega** moduluetan.

## <a name="concept-of-a-primary-customer"></a>Lehen bezero baten kontzeptua

Bezero potentzialaren proiektuaren **Laburpena** fitxan dagoen bezeroa aurrekontuaren bezero nagusia da. Aurrekontuan bezero nagusia zerrendatik bezero nagusia ezabatzen saiatzen zarenean, akats bat jasoko duzu aurrekontuan bezero nagusiaren erregistroa ezin dela ezabatu.

Bezero nagusia ez da aurrekontuko bezeroen zerrendatik eguneratu behar. Hala ere, bezero nagusian eragina izan dezakezu bezero potentziala aldatuz **Laburpena** aurrekontuaren fitxa. Eremu hau eguneratu denean **Aipuaren laburpena**, hautatu berri den bezero potentziala aurrekontuaren bezero berri gisa gehitzen da **Lehen Hezkuntza** bandera ezarri. Bezero potentzial zaharra aurrekontuan bezero izango da.

## <a name="create-update-or-delete-a-quote-customer-record"></a>Sortu, Eguneratu edo Ezabatu aurrekontuaren bezeroaren erregistroa

Aurrekontuaren bezero bat sortu, eguneratu edo ezabatu daiteke **Aipatu bezeroak** fitxan **Aurrekontua** orrialdea. Hurrengo taulan zerrendatzen diren eremuak proiektu-eskaintza bateko aurrekontuaren bezeroaren erregistroaren eremuak agertzen dira.

| **Eremua** | **Kokalekua** | **Azalpena** | **Downstream eragina** |
| --- | --- | --- | --- |
| Account | Sarean editagarria batean **Aipatu bezeroak** fitxa, inprimaki **Nagusia** eta aurrekontuaren bezeroarentzako **azkar sortzeko** inprimakia. | Kontu aktibo guztien zerrendak. Eremu hau blokeatuta dago erregistroa sortu ondoren. Eguneratu nahi baduzu, ezabatu erregistroa eta sortu berriro. Benetako datuak grabatu badituzu edo aurrekontuaren bezeroaren erregistroa bezero nagusia bada, erregistroa ezabatzeko baimena izango duzu. | Eskaintzaren bezeroak eskaintzaren lerroko bezeroen gainean kopiatzen dira, eskaintzaren lerro bat sortzen denean. Eskaintzaren bezeroak ere proiektuaren kontratuko bezeroei kopiatzen zaizkie eskaintza bat irabazten denean. |
| Fakturazioko zatitzearen ehunekoa | Sarean editagarria batean **Aipatu bezeroak** fitxa, inprimaki **Nagusia** eta aurrekontuaren bezeroarentzako **azkar sortzeko** inprimakia. | Adierazi aurrekontu honen bezeroari egotziko zaion fakturatu gabeko salmenta transakzio bakoitzaren ehunekoa. | Sortutako eskaintzaren lerro berrietara eta kontratupeko bezeroei kopiatuta. |
| Fakturaziorako kontaktuaren izena | Sarean editagarria batean **Aipatu bezeroak** fitxa, inprimaki **Nagusia** eta aurrekontuaren bezeroarentzako **azkar sortzeko** inprimakia. | Testu-eremua da eta bezero honen Fakturako harremanetarako pertsona identifikatzeko erabili behar da. Horiek erlazionatutako kontu erregistroan lehenetsita daude | Eskaintza irabazten dutenean proiektuaren kontratuko bezeroei kopiatuta eta, aldi berean, Kontratuaren fakturaren izena bezero honentzat sortzen den Fakturaren eremua. |
| Fakturaziorako izena | Sarean editagarria batean **Aipatu bezeroak** fitxa, inprimaki **Nagusia** eta aurrekontuaren bezeroarentzako **azkar sortzeko** inprimakia. | Testu-eremua da bezero honen fakturako harremanetarako pertsona identifikatzeko erabili behar da. | Aurrekontua irabazten dutenean proiektuaren kontratuko bezeroei kopiatuta eta, aldi berean, **Kontratuaren fakturaren izena** bezero honentzat sortzen den fakturaren eremua. |
| Ordainketa-baldintzak | Sarean editagarria batean **Aipatu bezeroak** fitxa, inprimaki **Nagusia** eta aurrekontuaren bezeroarentzako **azkar sortzeko** inprimakia. | Hau aukera multzo da erlazionatutako kontu erregistroan lehenetsitako balioak dituena. | Aurrekontua irabazten dutenean proiektuaren kontratuko bezeroei kopiatuta eta, aldi berean, **Kontratuaren fakturaren izena** bezero honentzat sortzen den fakturaren eremua. |
| Biribiltzen da | Sarean editagarria batean **Aipatu bezeroak** fitxa, inprimaki **Nagusia** eta aurrekontuaren bezeroarentzako **azkar sortzeko** inprimakia. | Bezero hau akordio honetako biribiltze lehenetsia den ala ez adierazten du. | Eskaintza bat irabazten denean, proiektuaren kontratuko bezeroan kopiatuta. |
| Jabetzadun enpresa | Sarean editagarria batean **Aipatu bezeroak** fitxa, inprimaki **Nagusia** eta aurrekontuaren bezeroarentzako **azkar sortzeko** inprimakia. | Bezero honen pertsona juridikoa **Proiektuen kudeaketa eta kontabilitatea** modulua. Eremu hau irakurtzeko soilik da eta aurrekontuaren enpresa titularra da. Hemen gehitu beharreko bezeroen zerrenda **Kontua** eremua dagoeneko zerrendara iragazita dago jabeko enpresan **Proiektuen kudeaketa eta kontabilitatea** proiektuaren eragiketen modulua. | Enpresa titularra pertsona juridikoaren kontzeptuarekin bat dator **Proiektuen kudeaketa eta kontabilitatea** proiektuaren eragiketen modulua. Proiektu honetatik sortzen diren kostu eta diru-sarrera guztiak enpresa jabearen liburu nagusian kontabilizatzen dira. |
| Ez gainditzeko muga | Sarean editagarria batean **Aipatu bezeroak** fitxa, inprimaki **Nagusia** eta aurrekontuaren bezeroarentzako **azkar sortzeko** inprimakia. | Konpromiso honengatik bezero honi fakturatuko zaion zenbateko orokorraren muga edo muga negoziatua dagoen adierazten du. | Eskaintza bat irabazten denean, proiektuaren kontratuko bezeroan kopiatuta. |

## <a name="editing-billing-split-percentages"></a>Fakturazioko zatitzearen ehunekoa editatzea

Fakturazio zatitutako ehunekoak editatu ditzakezu lineako sareta editatzeko esperientzia erabiliz. Fakturazio zatitutako ehunekoak % 100 guztira ez direnean, errore bat gertatuko da. Fakturazio zatitutako ehunekoak eguneratu ondoren, freskatu orria errorea ezabatzeko.

Aukeratzen ere saia zaitezke **Banatu uniformeki** eskaintzaren bezeroen azpisarean. Ekintza honek fakturazio zatiak banatzen dizkie aurrekontu bezero guztiei. Biribiltze faktore bat badago, hori biribiltze bezeroari gehituko zaio. Aurrekontuaren bezeroetako bat beti biribildutako bezero gisa etiketatuta dago. Horrek esan nahi du aurrekontuaren bezeroaren erregistroak hau duela **Biribilketa** bandera ezarri da **Bai**. Normalean, aurrekontuaren bezero nagusia da hau, baina hori alda daiteke.


[!INCLUDE[footer-include](../includes/footer-banner.md)]