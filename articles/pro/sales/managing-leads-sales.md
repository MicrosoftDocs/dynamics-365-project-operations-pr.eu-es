---
title: Kudeatu bezerogaiak (Pro)
description: Gai honek proiektuetan oinarritutako bezerogaiei buruzko informazioa ematen du (pro).
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 005e36811643b0b1e98a686792cf39125ae97949
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896311"
---
# <a name="manage-leads-pro"></a>Kudeatu bezerogaiak (Pro)

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proiektuetan oinarritutako bezeroak Project Operations-etan kudeatu eta kualifikatu daitezke. Lead-en kudeaketa-prozesuak laneko oinarritutako lead-ak sortzea eta lead horiek sailkatzea ditu barne. 

## <a name="list-of-project-sales-leads"></a>Proiektuetako salmenta-bezerogaien zerrenda

**Salmentak** atalean, ezkerreko nabigazio panelean, ireki **Bezerogaiak** zerrenda orria sistemako berunezko erregistro guztien zerrenda ikusteko. Erakutsitako eramangarrien zerrenda laneko oinarritutako eta beste sorkuntza mota batzuk sor daitezke, Dynamics 365 Sales edo Dynamics 365 Field Service aplikazioak.

Iragazitako ikuspegia sor dezakezu proiektuan oinarritutako eramangarriak soilik ikusteko, iragazkia sortuz **Mota** balioan. Adibidez, lanean oinarritutako bezeroak soilik erakustea hauta dezakezu.

## <a name="creating-a-new-lead-for-a-project-based-deal"></a>Bezerogai berri bat sortzea proiektuan oinarritutako akordio baterako

Proiektuetan oinarritutako liderra kualifikatzen denean, aukera eta kontua sortzen dira. Proiektuetan oinarritutako aukera da Aukera fasean salmentak bilatzeko jardueren abiapuntua. Proiektuetan oinarritutako aukerek proiektuaren lana saltzeko beharrezkoak diren gaitasun bakarrak dituzte. Gaitasun horien artean daude:

- Denbora eta materiala eta Prezio finkoko fakturazio-metodoak
- Proiektuetan sortutako giza baliabideen, gastuen eta materialaren prezioen zerrenda eraginkorra.

Bezerogai kualifikatuak aukera automatikoki sor dezan, ezarri **Mota** atributua **Lanean oinarrituta** bezerogaia sortzen duzunean. Beste mota bat aukeratzen baduzu, liderrak ez du proiektuan oinarritutako aukerarik sortuko kualifikatua denean. Proiektuan oinarritutako aukera sortzen ez bada, proiektuaren berariazko gaitasunak ez dira eskuragarri egongo downstream salmenta prozesuetan.

Ondorengo taulan, lider baten eremuko informazio garrantzitsua eta eremu horien ondorioak dituzten ondorioak daude.

| **Eremua** | **Kokalekua** | **Garrantzia, xedea eta orientazioa** | **Downstream eragina** |
| --- | --- | --- | --- |
| Gaia | Fitxa orokorra | Testu-eremu honek akordioaren deskribapen laburra izan behar du. | Bezerogaiaren gaia lehenetsita egongo da Abagunearen gai gisa, eta eskaintzaren izena eta Proiektuaren kontratua. |
| Mota | Fitxa orokorra | Aukera multzo eremu honek aukera hauek ditu:</br>- Lanean oinarrituta (Project Operations instalatuta dagoenean soilik eskuragarri)</br>- Elementuetan oinarrituta (Project Operations eta Sales instalatuta badituzu soilik)</br>- Zerbitzua mantentze lanetan oinarrituta (Field Service instalatuta dagoenean eskuragarri) | Eremu honen balioa ezarrita dagoenean **Lanean oinarrituta** markagailuan, liderra proiektuan oinarritutako aukera sortzeko gaituta dago. Proiektuan abagunea behar da akordio honetarako salmenta prozesuan proiektuaren berariazko luzapen eta funtzionalitate guztiak ahalbidetzeko. |
| Izena | Fitxa orokorra | Bezero potentzialaren kontaktuaren izena | Bezerogaia gailua denean, kontu, kontaktu eta abagune bat sortzen dira. Kontaktuaren izena da hemen ezartzen den balioa. |
| Abizenak | Fitxa orokorra | Bezero potentzialaren kontaktuaren abizena | Bezerogaia gailua denean, kontu, kontaktu eta abagune bat sortzen dira. Hemen balioa ezarritako kontaktuaren abizena. |
| Enpresa | Fitxa orokorra | Bezero potentzialaren enpresaren izena | Bezerogaia gailua denean, kontu, kontaktu eta abagune bat sortzen dira. Hemen sortutako kontaktuaren abizena ezartzen da. |
| Moneta | Xehetasunen fitxa | Bezero potentzialaren moneta | Bezerogaia gailua denean, kontu, kontaktu eta abagune bat sortzen dira. Hemen sortutako kontaktuaren moneta ezartzen da. |

## <a name="qualify-a-new-project-based-lead"></a>Kualifikatu proiektuan oinarritutako berri bat

Bezerogaiek **Mota** balioa ezarri da **Lanean oinarrituta** proiektuetan oinarritutako bezerogai deritze. Proiektuetan oinarritutako liderra kualifikatzen denean, hau sortzen da:

- Erabiltzen duen kontua **Enpresa** eremua markagailutik.
- Kontuarekin erlazionatutako kontaktu erregistroa **Izena** eta **Abizena** eremuak bezerogaian.
- Proiektuan oinarritutako aukera **Mota** eremua ezarrita dago &quot;**Lanetan oinarrituta**.

Sailkapen abantailen inguruko informazio zehatzagoa lortzeko, ikusi [Liderrak sailkatu edo bihurtu](https://docs.microsoft.com/dynamics365/sales-enterprise/qualify-lead-convert-opportunity-sales).

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
