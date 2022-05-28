---
title: Kudeatu hainbat bezero proiektuaren kontratuetan
description: Gai honek proiektuan oinarritutako proiektuaren kontratuan hainbat bezero kudeatzeari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 11/18/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: bf8b0d313b2b07924d730fe8923b05559bbcc244
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8591297"
---
# <a name="manage-multiple-customers-on-project-contracts"></a>Kudeatu hainbat bezero proiektuaren kontratuetan

Gai honek proiektuan oinarritutako proiektuaren kontratuan hainbat bezero kudeatzeari buruzko informazioa eskaintzen du. Proiektuaren kontratua erabil dezakezu kontratua finantzatzeko bezero anitzentzako itunpeko akordioa behar denean. **Proiektuaren kontratua** orrialdean, **Laburpena** fitxan akordio baterako bezero nagusiari buruzko informazioa dago. Akordioan parte hartzen duten beste bezero batzuk gehitu daitezke **Bezeroak** fitxa.

Kontratatutako bezero guztiak **Bezeroak** proiektuaren kontratuaren fitxa, kontratuaren lineako bezero gisa, proiektuaren kontraturako sortutako proiektuetan oinarritutako kontratu lerro berrietan. Lehendik dauden edozein proiektutan oinarritutako kontratu lerroek ez dituzte kontratu bezeroak geroago sortutakoak.

Kontratuaren eta kontratuaren lerro bezeroak gehitu, eguneratu edo ezabatu daitezke kontratua irabazi aurretik. Proiektuaren kontratuko bezero batek bezero gisa eratu behar du enpresa titular edo pertsona juridikoan **Bezeroak** orrialdea. Pertsona juridikoak **Proiektuen kudeaketa eta kontabilitatea** modulua Dynamics 365 Project Operations eta enpresa gisa eskuragarri daude **Proiektuen salmenta** eta **Entrega** proiektuaren eragiketen moduluak.

## <a name="primary-customers"></a>Bezero nagusiak

Balizko bezeroa **Laburpena** proiektuaren kontratuaren fitxa bezero potentziala kontratuko bezero nagusia baita. Ez duzu eguneratu bezero nagusia kontratuko bezeroaren zerrendatik. Bezero nagusia kontratuan bezeroen zerrendatik ezabatzen saiatzen zarenean, errore bat jasoko duzu kontratuko bezeroaren erregistro nagusia ezin dela ezabatu. Edo, aldatu bezeroa **Balizko bezeroa** eremuan proiektuaren kontratuaren **Laburpena** fitxan. Eremu hau eguneratu denean, hautatu den bezero berriak kontratuaren bezero gisa gehitzen da **Nagusia** **Bai** gisa ezarrita. Aurreko bezero nagusia kontratuan dagoen bezeroa da oraindik, hala ere, jada ez dira bezero nagusiak.

## <a name="create-update-or-delete-a-contract-customer-record"></a>Sortu, eguneratu edo ezabatu kontratuko bezeroaren erregistroa

Kontratuaren bezero bat sortu, eguneratu edo ezabatu daiteke **Kontratuaren bezeroak** fitxan **Kontratua** orrialdea. Eremu hauek proiektuaren kontratuaren kontratuaren bezeroaren erregistroan sartzen dira.

| **Eremua** | **Kokalekua** | **Azalpena** | 
| --- | --- | --- | 
| Account | Sareta editagarria **Kontratuaren bezeroak** fitxa eta nagusia eta sortu bizkor orriak kontratuaren bezeroarentzako. | Kontu aktibo guztien zerrendak. Eremu hau blokeatuta dago erregistroa sortu ondoren. Erregistroa eguneratzeko, ezabatu erregistroa eta berriro sortu erregistroa. Benetako datuak grabatu badituzu edo kontratuaren bezeroaren erregistroa bezero nagusia bada, ezin duzu erregistroa ezabatu. Kontratuaren lerroa sortzen denean, kontratuaren bezeroak kontratuaren lerroko bezero gisa kopiatuta daude. |
| Fakturazioko zatitzearen ehunekoa | Sareta editagarria **Kontratuaren bezeroak** fitxa eta nagusia eta sortu bizkor orriak kontratuaren bezeroarentzako. | Kontratu lineako bezero honi egotziko zaion fakturatu gabeko salmenta transakzio bakoitzaren ehunekoa adierazten du. Proiektuen kontratu lerro berriak sortzen direnean, fakturazio zatiaren portzentajea sortutako kontratu lerro berriei eta kontratu lerro bezeroei proiektatzen zaie. |
| Fakturaziorako kontaktuaren izena | Sareta editagarria **Kontratuaren bezeroak** fitxa eta nagusia eta sortu bizkor orriak kontratuaren bezeroarentzako. | Testu-eremu hau fakturarekin harremanetan jartzeko bezeroa identifikatzeko erabili behar da. Balio lehenetsia rlazionatutako kontu erregistroan lehenetsita dago. Kontaktuaren izena **Kontratuaren fakturaren izena** bezero honentzat sortzen den fakturaren eremua. |
| Fakturaziorako izena | Sareta editagarria **Kontratuaren bezeroak** fitxa eta nagusia eta sortu bizkor orriak kontratuaren bezeroarentzako. | Erabili testu-eremu hau fakturarekin harremanetan jartzeko bezeroa identifikatzeko. Balio lehenetsia rlazionatutako kontu erregistroan lehenetsita dago. Izena **Kontratuaren fakturaren izena** eremuan kopiatzen da bezero honentzat sortzen den fakturaren eremua. |
| Ordainketa-baldintzak | Sareta editagarria **Kontratuaren bezeroak** fitxa eta nagusia eta sortu bizkor orriak kontratuaren bezeroarentzako. | Balio lehenetsia rlazionatutako kontu erregistroan lehenetsita dago. Aldiak **Kontratuaren fakturaren izena** eremuaren gainean kopiatzen dira bezero honentzat sortzen den fakturaren eremua. |
| Jabetzadun enpresa | Sareta editagarria **Proiektuaren kontratuaren bezeroak** fitxa eta nagusia eta sortu bizkor orriak proiektuaren kontratuaren bezeroarentzako. | Bezeroan bezeroaren egoitza juridikoa **Proiektuen kudeaketa eta kontabilitatea** modulua. Eremu hau irakurtzeko soilik da eta proiektuaren kontratuaren enpresa titularra da.</br>Hemen gehitu beharreko bezeroen zerrenda **Kontua** eremua dagoeneko zerrendara iragazita dago jabeko enpresan **Proiektuen kudeaketa eta kontabilitatea** proiektuaren eragiketen modulua. Enpresa titularra pertsona juridikoaren berdina da **Proiektuen kudeaketa eta kontabilitatea** Project Operations-en modulua. Proiektu honetatik sortutako kostu eta diru-sarrera guztiak enpresa jabearen liburu nagusian kontabilizatzen dira. |
| Biribiltzen da | Sareta editagarria **Kontratuaren bezeroak** fitxa eta nagusia eta sortu bizkor orriak kontratuaren bezeroarentzako. | Bezeroa akordiorako biribiltzeko bezero lehenetsia den adierazten du. Proiektuaren kontratuan bezero borobildu bakarra egon daiteke. Kopuruaren kostua eta fakturatu gabeko salmentak zatitzean biribiltze-aldea eragiten dutenean, desberdintasun hori bezero honi mapatzen dion benetakoari aplikatuko zaio. |
| Ez gainditzeko muga | Sareta editagarria **Kontratuaren bezeroak** fitxa eta nagusia eta sortu bizkor orriak kontratuaren bezeroarentzako. | Bezero honi konpromisoagatik fakturatuko zaion zenbateko osoari negoziatutako muga edo muga dagoen adierazten du. Ez gainditzeko muga kontratuan bezero mailan ezarritakoa ebaluatuko da fakturatutako salmenten benetako datuak kontratu honen bezeroari erreferentzia egiten diotenak. |

## <a name="edit-billing-split-percentages"></a>Editatu fakturazioko zatitzearen ehunekoa

Fakturazio zatitutako ehunekotan edita ditzakezu sareta editatuta. Fakturazio zatitutako ehunekoak ehuneko 100 guztira ez direnean, errore bat gertatuko da. Fakturazio zatien ehunekoak editatu ondoren, **Proiektuaren kontratua** orria errorea ezabatzeko.

Aukeratu ere egin dezakezu **Banatu uniformeki** proiektuaren kontratu-bezeroen azpisarean. Fakturazioaren zatitzeak berdin banatzen dira proiektuaren kontratuko bezero guztien artean. Biribiltze faktorerik badago, faktorea biribiltze bezeroari gehituko zaio. Kontratuko bezeroetako batek beti du **Biribilketa** bandera ezarri da **Bai**. Bezero hori bezero biribila da. Normalean, biribiltzeko bezeroa ere kontratuko bezero nagusia da, baina hori ez da beharrezkoa.


[!INCLUDE[footer-include](../includes/footer-banner.md)]