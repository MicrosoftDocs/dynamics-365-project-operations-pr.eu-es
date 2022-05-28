---
title: Kudeatu hainbat bezero proiektuaren kontratuetan - arina
description: Gai honek proiektuan oinarritutako proiektuaren kontratuan bezero kudeatzeari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 10/27/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 015e407b1b9e464edec1e57ce6b5132f21f5ae6d
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8593045"
---
# <a name="manage-multiple-customers-on-project-contracts---lite"></a>Kudeatu hainbat bezero proiektuaren kontratuetan - arina

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Dynamics 365 Project Operations-eko proiektuen kontratuek ituneko akordioak akordio bat finantzatzen duten bezero anitzek hartzen duten eszenatokia onartzen dute. **Laburpena** fitxan **Proiektuaren kontratua** orrialdeak **Bezeroa** eremua. Eremu honek akordioaren bezero nagusia identifikatzen du. Akordiorako beste bezero batzuk konfigura daitezke **Bezeroak** fitxategiaren fitxa **Proiektuaren kontratua** orrialdea.

Kontratatutako bezero guztiak proiektuaren kontratuaren fitxa, kontratuaren lineako bezero gisa, proiektuan oinarritutako kontraturako sortutako kontratu lerro berrietan. Lehendik dauden proiektuetan oinarritutako kontratu lerroek ez dituzte kontratu bezero berriak oinordetzen erregistro berriak sortu ahala.

Produktuetan oinarritutako kontratu lineak automatikoki lotzen dira lehen bezeroarekin.

Kontratuaren bezeroak eta kontratuen lineako bezeroak gehitu, eguneratu edo ezabatu daitezke kontratua irabazi aurretik.

## <a name="primary-customer"></a>Bezero nagusia

Zerrendan agertzen den bezeroa **Laburpena** proiektuaren kontratuaren fitxa bezero potentziala kontratuko bezero nagusia baita. Bezero nagusia kontratuan bezeroen zerrendatik ezabatzen saiatzen zarenean, errore-mezu bat jasoko duzu kontratuko bezeroaren erregistro nagusia ezin dela ezabatu.

Ezin da bezero nagusia kontratuko bezeroen zerrendatik eguneratu. Horren ordez, aldatu bezero potentziala **Laburpena** kontratuaren fitxa. Eremu hau eguneratu denean **Kontratuaren laburpena** orrialdean, bezero berria kontratu bezero berri gisa gehitzen da **Lehen Hezkuntza** bandera ezarri. Aurreko bezero nagusia kontratuan bezero izango da.

## <a name="create-update-or-delete-a-contract-customer-record"></a>Sortu, eguneratu edo ezabatu kontratuko bezeroaren erregistroa

Kontratuaren bezero bat sortu, eguneratu edo ezabatu daiteke **Bezeroak** fitxan **Proiektuaren kontratua** orrialdea. Ondorengo taulako eremuak proiektuaren kontratuaren bezeroaren kontratuko erregistroan daude eta kontuan izan behar dira kontratuarekin lanean ari zarenean.

| Eremua | Kokapena | Deskribapena | Downstream eragina |
| --- | --- | --- | --- |
| **Kontua** | Sareta edita daiteke **Kontratuaren bezeroak** fitxa eta **Nagusia** eta **Sortu bizkor** kontratuaren bezeroarentzako inprimakiak. | Kontu aktibo guztien zerrendak. Eremu hau blokeatuta dago erregistroa sortu ondoren. Kontua eguneratzeko, ezabatu erregistroa eta sortu erregistroa. Benetako datuak grabatu badituzu edo kontratuaren bezeroaren erregistroa bezero nagusia bada, ezin duzu erregistroa ezabatu. | Kontratuetako bezeroak kontratu-lerro bezero gisa kopiatzen dira kontratu-linea sortzen denean. |
| **Fakturazioko zatitzearen ehunekoa** | Sareta edita daiteke **Kontratuaren bezeroak** fitxa eta **Nagusia** eta **Sortu bizkor** kontratuaren bezeroarentzako inprimakiak. | Kontratu lineako bezero honi egotziko zaion fakturatu gabeko salmenta transakzio bakoitzaren ehunekoa adierazten du. | Kontratatutako linea berrietara kopiatzea eta proiektuaren kontratu lerro berrietako bezeroei proiektatzea. |
| **Fakturaziorako kontaktuaren izena** | Sareta edita daiteke **Kontratuaren bezeroak** fitxa eta **Nagusia** eta **Sortu bizkor** kontratuaren bezeroarentzako inprimakiak. | Testu-eremua da bezero honen fakturako harremanetarako pertsona identifikatzeko erabili behar da. Eremu hau erlazionatutako kontu erregistroan lehenetsita dago. | Fitxategira kopiatuta **Kontratuaren fakturaren izena** bezero honentzat sortzen den fakturaren eremua. |
| **Fakturaziorako izena** | Sareta edita daiteke **Kontratuaren bezeroak** fitxa eta **Nagusia** eta **Sortu bizkor** kontratuaren bezeroarentzako inprimakiak | Testu-eremua da bezero honen fakturako harremanetarako pertsona identifikatzeko erabili behar da. Eremu hau erlazionatutako kontu erregistroan lehenetsita dago. | Fitxategira kopiatuta **Kontratuaren fakturaren izena** bezero honentzat sortzen den fakturaren eremua. |
| **Ordainketa-baldintzak** | Sareta edita daiteke **Kontratuaren bezeroak** fitxa eta **Nagusia** eta **Sortu bizkor** kontratuaren bezeroarentzako inprimakiak. | Balio lehenetsia rlazionatutako kontu erregistroan lehenetsita dago. | Fitxategira kopiatuta **Kontratuaren fakturaren izena** bezero honentzat sortzen den fakturaren eremua. |
| **Biribiltzen da** | Sareta edita daiteke **Kontratuaren bezeroak** fitxa eta **Nagusia** eta **Sortu bizkor** kontratuaren bezeroarentzako inprimakiak. | Bezero hau akordio honetako biribiltze lehenetsia den ala ez adierazten du. Proiektuaren kontratuan bezero borobildu bakarra egon daiteke. | Kopuruaren kostua eta fakturatu gabeko salmentak zatitzean biribiltze-aldea eragiten dutenean, desberdintasun hori bezero honi mapatzen dion benetakoari aplikatuko zaio. |
| **Ez gainditzeko muga** | Sareta edita daiteke **Kontratuaren bezeroak** fitxa eta **Nagusia** eta **Sortu bizkor** kontratuaren bezeroarentzako inprimakiak | Bezero honi konpromisoagatik fakturatuko zaion zenbateko osoari negoziatutako muga edo muga dagoen adierazten du. | **Ez gainditzeko muga** kontratuan bezero mailan ezarritakoa ebaluatuko da **Fakturatutako salmenten benetako datuak** kontratu honen bezeroari erreferentzia egiten diotenak. |

## <a name="edit-billing-split-percentages"></a>Editatu fakturazioko zatitzearen ehunekoa

Fakturazio zatitutako ehunekoak saretan editatzeko esperientzia. Fakturazio zatitutako ehunekoak ehuneko 100 guztira ez direnean, errore bat jasoko da. Fakturazio zatien ehunekoak editatu ondoren, freskatu orria errorea baztertzeko.

Aukeratu ere egin dezakezu **Banatu uniformeki** **Kontratuaren bezeroak** azpisarean fakturazio banaketak kontratuko bezero guztiei modu uniformean banatzeko. Biribiltze faktorerik badago, biribiltze bezeroari gehituko zaio. Kontratuko bezeroetako bat beti bezala etiketatuta dago **biribiltzea** bezeroak, horrek esan nahi du kontratuaren bezeroaren erregistroak biribiltze bandera ezarrita duela **Bai**. Normalean, hau da kontratuko bezero nagusia, baina alda daiteke ere.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]