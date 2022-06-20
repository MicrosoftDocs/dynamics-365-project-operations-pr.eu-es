---
title: Kudeatu proiektu-eskaintzetako hainbat bezero - arina
description: Artikulu honek proiektua finantzatuko duten hainbat bezerorekin kotizazioetan nola lan egin erakusten du. (Sales)
author: rumant
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 337619e8d8081cdebd73f9336fa9fa99885a0ab2
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8921057"
---
# <a name="manage-multiple-customers-on-project-quotes---lite"></a>Kudeatu proiektu-eskaintzetako hainbat bezero - arina

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proiektuaren aurrekontuek proposamena akordioa finantzatuko duten bezero anitzekin lotzen duten agertokia onartzen dute. Eskaintzaren **Laburpena** fitxak akordioaren bezero nagusia identifikatzen duen **Bezero potentziala** eremua du. Akordiorako beste bezero batzuk konfigura daitezke **Bezeroak** proiektuaren aurrekontuaren fitxa.

Aurrekontuaren bezero guztiak **Bezeroak** proiektuaren aurrekontuaren fitxa lehenetsitako lerroen bezero gisa, aurrekonturako sortutako proiektuetan oinarritutako aurrekontu lerro **berrietan**. Lehendik dauden proiektuetan oinarritutako aurrekontu lerroek ez dituzte ondoren sortutako aurrekontu bezeroen erregistro berriak jasotzen.

Produktuetan oinarritutako aurrekontu lerroak automatikoki lotzen dira bezeroaren lehen bezeroarekin **Bezero potentziala** eremuan **Laburpena** aurrekontuaren fitxa.

Aurrekontuaren bezeroak eta aurrekontuen linea bezeroak gehitu, eguneratu edo ezabatu daitezke aurrekontua irabazi aurretik.

## <a name="concept-of-a-primary-customer"></a>Lehen bezero baten kontzeptua

Bezero potentzialaren proiektuaren laburpen fitxan dagoen bezeroa aurrekontuaren bezero nagusia da. Aurrekontuan bezero nagusia zerrendatik bezero nagusia ezabatzen saiatzen zarenean, akats bat ikusiko duzu aurrekontuan bezero nagusiaren erregistroa ezin dela ezabatu.

Bezero nagusia ez da aurrekontuko bezeroen zerrendatik eguneratu behar. Hala ere, bezero nagusian eragina izan dezakezu bezero potentziala aldatuz **Laburpena** aurrekontuaren fitxa. Eremu hau eguneratu denean **Aipuaren laburpena**, hautatu berri den bezero potentziala aurrekontuaren bezero berri gisa gehitzen da **Lehen Hezkuntza** bandera ezarri. Bezero potentzial zaharra aurrekontuan bezero izango da.

## <a name="create-update-or-delete-a-quote-customer-record"></a>Sortu, Eguneratu edo Ezabatu aurrekontuaren bezeroaren erregistroa

Aurrekontuaren bezero bat sortu, eguneratu edo ezabatu daiteke **Aipatu bezeroak** fitxan **Aurrekontua** orrialdea. Hurrengo taulan zerrendatzen diren eremuak proiektu-eskaintza bateko aurrekontuaren bezeroaren erregistroaren eremuak agertzen dira.

| **Eremua** | **Kokalekua** | **Azalpena** | **Downstream eragina** |
| --- | --- | --- | --- |
| Account | Sarean editagarria batean **Aipatu bezeroak** fitxa, inprimaki **Nagusia** eta aurrekontuaren bezeroarentzako **azkar sortzeko** inprimakia. | Kontu aktibo guztien zerrendak. Eremu hau blokeatuta dago erregistroa sortu ondoren. Eguneratu nahi baduzu, ezabatu erregistroa eta sortu berriro. Benetako datuak grabatu badituzu edo aurrekontuaren bezeroaren erregistroa bezero nagusia bada, ezin izango duzu erregistroa ezabatu. | Eskaintzaren bezeroak eskaintzaren lerroko bezeroen gainean kopiatzen dira, eskaintzaren lerro bat sortzen denean. Eskaintzaren bezeroak ere proiektuaren kontratuko bezeroei kopiatzen zaizkie eskaintza bat irabazten denean. |
| Fakturazioko zatitzearen ehunekoa | Sarean editagarria batean **Aipatu bezeroak** fitxa, inprimaki **Nagusia** eta aurrekontuaren bezeroarentzako **azkar sortzeko** inprimakia. | Adierazi aurrekontu honen bezeroari egotziko zaion fakturatu gabeko salmenta transakzio bakoitzaren ehunekoa. | Aurrekontu lerro berrietara eta kontratupeko bezeroei kopiatuta. |
| Fakturaziorako kontaktuaren izena | Sarean editagarria batean **Aipatu bezeroak** fitxa, inprimaki **Nagusia** eta aurrekontuaren bezeroarentzako **azkar sortzeko** inprimakia. | Testu-eremua da eta bezero honen Fakturako harremanetarako pertsona identifikatzeko erabili behar da. Horiek erlazionatutako kontu erregistroan lehenetsita daude | Eskaintza irabazten dutenean proiektuaren kontratuko bezeroei kopiatuta eta, aldi berean, Kontratuaren fakturaren izena bezero honentzat sortzen den Fakturaren eremua. |
| Fakturaziorako izena | Sarean editagarria batean **Aipatu bezeroak** fitxa, inprimaki **Nagusia** eta aurrekontuaren bezeroarentzako **azkar sortzeko** inprimakia. | Testu-eremua da bezero honen fakturako harremanetarako pertsona identifikatzeko erabili behar da. | Aurrekontua irabazten dutenean proiektuaren kontratuko bezeroei kopiatuta eta, aldi berean, **Kontratuaren fakturaren izena** bezero honentzat sortzen den fakturaren eremua. |
| Ordainketa-baldintzak | Sarean editagarria batean **Aipatu bezeroak** fitxa, inprimaki **Nagusia** eta aurrekontuaren bezeroarentzako **azkar sortzeko** inprimakia. | Hau aukera multzo da erlazionatutako kontu erregistroan lehenetsitako balioak dituena. | Aurrekontua irabazten dutenean proiektuaren kontratuko bezeroei kopiatuta eta, aldi berean, **Kontratuaren fakturaren izena** bezero honentzat sortzen den fakturaren eremua, |
| Biribiltzen da | Sarean editagarria batean **Aipatu bezeroak** fitxa, inprimaki **Nagusia** eta aurrekontuaren bezeroarentzako **azkar sortzeko** inprimakia. | Bezero hau akordio honetako biribiltze lehenetsia den ala ez adierazten du. | Eskaintza bat irabazten denean, proiektuaren kontratuko bezeroan kopiatuta. |
| Ez gainditzeko muga | Sarean editagarria batean **Aipatu bezeroak** fitxa, inprimaki **Nagusia** eta aurrekontuaren bezeroarentzako **azkar sortzeko** inprimakia. | Konpromiso honengatik bezero honi fakturatuko zaion zenbateko orokorraren muga edo muga negoziatua dagoen adierazten du | Eskaintza bat irabazten denean, proiektuaren kontratuko bezeroan kopiatuta. |

## <a name="editing-billing-split-percentages"></a>Fakturazioko zatitzearen ehunekoa editatzea

Fakturazio zatitutako ehunekoak editatu ditzakezu lineako sareta editatzeko esperientzia erabiliz. Fakturazio zatitutako ehunekoak % 100 guztira ez direnean, errore bat gertatuko da. Fakturazio zatitutako ehunekoak eguneratu ondoren, freskatu orria errorea ezabatzeko.

Aukeratzen ere saia zaitezke **Banatu uniformeki** eskaintzaren bezeroen azpisarean. Ekintza honek fakturazio zatiak banatzen dizkie aurrekontu bezero guztiei. Biribiltze faktore bat badago, hori biribiltze bezeroari gehituko zaio. Aurrekontuaren bezeroetako bat beti biribildutako bezero gisa etiketatuta dago. Horrek esan nahi du aurrekontuaren bezeroaren erregistroak hau duela **Biribilketa** bandera ezarri da **Bai**. Normalean, aurrekontuaren bezero nagusia da hau, baina hori alda daiteke.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
