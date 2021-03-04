---
title: Kudeatu bezerogaiak
description: Gai honek proiektuetan oinarritutako bezerogaiei buruzko informazioa ematen du.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 16f5dbb283eee12cf10ca7145ea9e17c5ef8923e
ms.sourcegitcommit: 869bde007805ef255f61b03937e4a44aeef61df9
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/12/2020
ms.locfileid: "4513819"
---
# <a name="manage-leads"></a>Kudeatu bezerogaiak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Proiektuetan oinarritutako bezeroak Project Operations-etan kudeatu eta kualifikatu daitezke. Lead-en kudeaketa-prozesuak laneko oinarritutako lead-ak sortzea eta lead horiek sailkatzea ditu barne. 

## <a name="project-sales-leads"></a>Proiektuetako salmenta-bezerogaiak

**Salmentak** atalean, ezkerreko nabigazio panelean, ireki **Bezerogaiak** zerrenda orria sistemako berunezko erregistro guztien zerrenda ikusteko. Erakutsitako eramangarrien zerrenda laneko oinarritutako eta beste sorkuntza mota batzuk sor daitezke, Dynamics 365 Sales edo Dynamics 365 Field Service aplikazioak.

Iragazitako ikuspegia sor dezakezu proiektuan oinarritutako eramangarriak soilik ikusteko, iragazkia sortuz **Mota** balioan. Adibidez, lanean oinarritutako bezeroak soilik erakustea hauta dezakezu.

## <a name="create-a-new-lead-for-a-project-based-deal"></a>Sortu berri bat proiektuan oinarritutako akordio baterako

Proiektuetan oinarritutako liderra kualifikatzen denean, aukera eta kontua sortzen dira. Proiektuetan oinarritutako aukera da Aukera fasean salmentak bilatzeko jardueren abiapuntua. Proiektuetan oinarritutako aukerek proiektuaren lana saltzeko beharrezkoak diren gaitasun bakarrak dituzte. Gaitasun horien artean daude:

- Denbora eta materiala eta Prezio finkoko fakturazio-metodoak
- Proiektuetan sortutako giza baliabideen, gastuen eta materialaren prezioen zerrenda eraginkorra

Bezerogai kualifikatuak aukera automatikoki sor dezan, ezarri **Mota** atributua **Lanean oinarrituta** bezerogaia sortzen duzunean. Beste mota bat aukeratzen baduzu, liderrak ez du proiektuan oinarritutako aukerarik sortuko kualifikatua denean. Proiektuan oinarritutako aukera sortzen ez bada, proiektuaren berariazko gaitasunak ez dira eskuragarri egongo downstream salmenta prozesuetan.

Ondorengo taulan, lider baten eremuko informazio garrantzitsua eta eremu horien ondorioak dituzten ondorioak daude.
 
| **Eremua** | **Kokalekua** | **Azalpena** | **Downstream eragina** |
| --- | --- | --- | --- |
| Gaia | Fitxa orokorra | Testu-eremu honek akordioaren deskribapen laburra izan behar du. | Bezerogaiaren gaia lehenetsita egongo da Abagunearen gai gisa, eta Eskaintzaren izena eta Proiektuaren kontratua. |
| Mota | Fitxa orokorra | Aukera multzo eremu honek aukera hauek ditu:</br>- Lanean oinarrituta (Project Operations instalatuta dagoenean soilik eskuragarri)</br>- Elementuetan oinarrituta (Project Operations eta Sales instalatuta badituzu soilik)</br>- Zerbitzua mantentze lanetan oinarrituta (Field Service instalatuta dagoenean eskuragarri) | Eremu honen balioa ezarrita dagoenean **Lanean oinarrituta** markagailuan, liderra proiektuan oinarritutako aukera sortzeko gaituta dago. Proiektuan abagunea behar da akordio honetarako salmenta prozesuan proiektuaren berariazko luzapen eta funtzionalitate guztiak ahalbidetzeko. |
| Izena | Fitxa orokorra | Bezero potentzialaren kontaktuaren izena | Bezerogaia gailua denean, kontu, kontaktu eta abagune bat sortzen dira. Kontaktuaren izena da hemen ezartzen den balioa. |
| Abizenak | Fitxa orokorra | Bezero potentzialaren kontaktuaren abizena | Bezerogaia gailua denean, kontu, kontaktu eta abagune bat sortzen dira. Hemen balioa ezarritako kontaktuaren abizena. |
| Enpresa | Fitxa orokorra | Bezero potentzialaren enpresaren izena | Bezerogaia gailua denean, kontu, kontaktu eta abagune bat sortzen dira. Hemen ezarritako balioa sortutako kontaktuaren abizena. |
| Moneta | Xehetasunen fitxa | Bezero potentzialaren moneta | Bezerogaia gailua denean, kontu, kontaktu eta abagune bat sortzen dira. Hemen sortutako kontaktuaren moneta ezartzen da. |

## <a name="qualify-a-new-project-based-lead"></a>Kualifikatu proiektuan oinarritutako berri bat

Bezerogaiek **Mota** balioa ezarri da **Lanean oinarrituta** proiektuetan oinarritutako bezerogai deritze. Proiektuetan oinarritutako liderra kualifikatzen denean, hau sortzen da:

- Erabiltzen duen kontua **Enpresa** eremua markagailutik.
- Kontuarekin erlazionatutako kontaktu erregistroa **Izena** eta **Abizena** eremuak bezerogaian.
- Proiektuan oinarritutako aukera **Mota** eremua ezarrita dago **Lanetan oinarrituta**.

Sailkapen abantailen inguruko informazio zehatzagoa lortzeko, ikusi [Liderrak sailkatu edo bihurtu](https://docs.microsoft.com/dynamics365/sales-enterprise/qualify-lead-convert-opportunity-sales).

## <a name="lead-qualification-and-legal-entity-information"></a>Bezerogaiaren kalifikazio eta pertsona juridikoen informazioa 

Proiektuaren eragiketak inplementazio modua erabiliz, Proiektuaren eragiketak baliabideetan / stockean oinarritutako eszenatokietarako, bezero eta aukera bakoitzak edukitzea beharrezkoa izango da **Enpresa titularra** zelai multzoa. Jabe den enpresa zure erakundeko pertsona juridikoa da, proiektua entregatzeko jabea. Bezero bakoitzak edo harreman mota duen bezeroak eduki behar du **Enpresa titularra** bezero honekin kontratatu eta negoziatzen duen pertsona juridikoari ezarritako balioa. Bezeroa pertsona juridiko bakarrean egon daiteke.

Lider bat kualifikatuta dagoenean, sortutako bezero eta aukera erregistroek izango dute **Enpresa titularra** eremua uneko erabiltzailearen baliabide erreserbagarrien erregistroaren konpainian ezarri da.

Uneko erabiltzailearen baliabide erreserbagarrien erregistroa hutsik badago, orduan **Enpresa titularra** erabiltzailearen erregistroan dagoen eremuko balioa bezeroaren eta aukera erregistroen lehenespen gisa erabiltzen da.

## <a name="business-process-flow-for-project-based-deals"></a>Negozio-prozesuaren fluxu proiektuetan oinarritutako akordioetarako

Ondorengo negozio-prozesuen fluxuak onartzen dira proiektuetan oinarritutako Project Operations-en:

- Bezerogaitik abagunerako negozio-prozesua
- Abagune-salmenten prozesua

Bezerogaitik abagunerako negozio-prozesuak fase hauek onartzen ditu:

| Fasearen izena | Esleitutako entitatea | Funtzioa |
| --- | --- | --- |
| Gaitu | Bezerogaia | Gaitu bezerogaia kontu, kontaktu eta abagune bat sortzeko. |
| Garatu | Abagunea | Garatu aukera inplikatutako lanari, funtsezko eragileei eta lehiari buruzko informazio gehiago gehitzeko. |
| Proposatu | Abagunea | Garatu proposamena eta lortu barne ebaluazio taldearen onespena. |
| Itxi | Abagunea | Irabazi abagunea mahuka ixteko. |


[!INCLUDE[footer-include](../includes/footer-banner.md)]