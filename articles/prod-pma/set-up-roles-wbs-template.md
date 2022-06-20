---
title: Konfiguratu funtzioak zereginen xehetasunen egituraren txantiloietan
description: Artikulu honek Lanaren banaketa-egituraren txantiloietan rolaren informazioa konfiguratzeari buruzko informazioa eskaintzen du.
author: Yowelle
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: johnmichalak
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 8721c5e5798c2b80c6f3eb65cef118d1ade5e680
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8920781"
---
# <a name="set-up-roles-on-work-breakdown-structure-templates"></a>Konfiguratu funtzioak zereginen xehetasunen egituraren txantiloietan

[!include [banner](../includes/banner.md)]

Proiektu-arduradunek zereginen xehetasunen egituraren (WBS) txantiloiak konfigura ditzakete, proiektu berrietarako WBS bat sortzen dutenean aplika ditzaketenak. Proiektuen kudeatzaileek rolak gehi ditzakete txantiloia sortzen dutenean. Erabili prozedura hau WBS txantiloiari rol bat esleitzeko.

1. Aukeratu **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Proiektuak** > **Zereginen xehetasunen egituraren txantiloiak**.
2. Aukeratu **Xehetasunak** hautatutako WBS txantiloia lortzeko.
3. Hautatu zeregin bat zerrendan, eta gero **Rola** eremuan, hautatu zereginari esleitzeko funtzioa.

## <a name="work-with-a-wbs"></a>Egin lan WBS

Sortu egin dezakezu WBS berria edo kopiatu WBS inprimakia existitzen den WBS txantiloia. Proiektu kudeatzaile batek baliabideak erraz kudea ditzake WBSko zeregin berriei rolak esleituz. Rolak ordezka daitezke baliabide bat eskuratu ondoren edo zereginean lan egiteko baieztatutako baliabide bat identifikatu ondoren. Malgutasun honi esker, proiektuen kudeatzaileek zeregin hauek bete ditzakegu:

- Identifikatu WBS lan paketeetarako beharrezkoak diren baliabide kopurua.
- Balioztatu proiektuaren kostuak.
- Aurretiazko aurrekontua zehaztu.
- Jardueraren iraupena kalkulatu, rol eta baliabideetan oinarrituta.
- Proiektuak kudeatzeko zenbait plan garatu, eskuragarri dagoen proiektuaren informazioan oinarrituta.

Aukera osagarriak gehitu dira WBSn, baliabideen funtzionalitatea hobeto erabiltzeko.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Aukera</th>
<th>Deskribapenak</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Baliabide-esleipenak</td>
<td>Ikusi esleitutako baliabideak, datak, ordu kopurua eta erreserba mota WBSn zereginetarako.</td>
</tr>
<tr class="even">
<td>Auto sortu taldea</td>
<td>Gehitu automatikoki aurreikusitako baliabideak ataza batekin lotutako rolak erabiliz. Finantzak automatikoki iradokitzen ditu planifikatutako baliabideak, roletan oinarritutako irizpide anitzeko erabakien analisia erabiliz. WBS batean zereginak egiteko rolak eta ahalegina (orduak) ezarri ondoren, eta egitura askatu ondoren, hautatu <strong>Auto taldea sortu</strong>. Aurreikusitako beharrezko baliabide kopurua gehitzen zaio WBSri eta <strong>Proiektuen eta taldeen programazioa</strong> fitxa.</td>
</tr>
<tr class="odd">
<td>Baliabidea (goitibehera zerrenda)</td>
<td>Gainean <strong>Baliabideen esleipena abiarazi</strong> orrialdean, hard-book edo soft-book baliabideak hauta ditzakezu, zehaztutako iraupenaren arabera. Ikuspegiaren ezarpenak doitu ditzakezu baliabideen jardueren iraupena ikusi eta ezartzeko. Lan pakete mailan baliabideak hauta eta esleitu ditzakezu aukera hauek erabiliz:
<ul>
<li><strong>Onartu</strong> - Egiaztatu zeregin bati esleitutako baliabidearen aldaketak.</li>
<li><strong>Ezeztatu</strong> - Ezeztatu zeregin bati esleitutako baliabidearen aldaketak.</li>
<li><strong>Esleitu automatikoki</strong> - Bat datorren eginkizuna duen langile baliabide erabilgarri bat automatikoki hautatzen da eta hautatutako ataza esleitzen zaio.</li>
</ul></td>
</tr>
</tbody>
</table>

1. Gainean **Proiektu guztiak** orria, hautatu **XYZ berritzea 2. fasea** proiektua.
2. Aukeratu **Plana** > **Jarduerak** > **Zereginen xehetasunen egitura**.
3. Aukeratu **Berria** WBSari maila bateko jarduera hauek gehitzeko:

    - Hasi
    - Antolaketa
    - Exekutatzen
    - Monitorizatu eta kontrola
    - Itxi

4. Ezarri datak eta ahalegina (orduak), hurrengo ilustrazioan agertzen den moduan.

    [![Datak eta ahalegina zehaztea.](./media/projectresourcing10.jpg)](./media/projectresourcing10.jpg)

5. Aukeratu **Hasi** ataza lerroa, eta gero, **Rola** eremua, hautatu **Proiektu zuzendari nagusia**.
6. Hautatu **Argitaratu**.
7. Lerro berean, **Baliabidea** eremua, hautatu **Daniel Goldschmidt** eta, ondoren, hautatu **Onartu**.
8. Aukeratu **Plangintza** ataza lerroa, eta gero, **Rola** eremua, hautatu **Enpresa analista**.
9. Aukeratu **Argitaratu** eta, ondoren, hautatu **Auto taldea sortu**.
10. Agertzen den mezuaren koadroa, hautatu **Bai**.
11. **Baliabidea** eremua, egiaztatu balioa dela **Enpresa analista 1**.
12. Hurrengorako **Enpresa analista 1** baliabidea, ireki bilaketa eta hautatu **Abiarazi baliabideen esleipenak**. Ondoren, hautatu langilea zereginerako.
13. Aukeratu **Soft esleitzeko** &gt; **Edukiera osoa**.

    > [!NOTE] 
    > Ez duzu ohartarazten zehaztutako baliabidea 2 dela, baliabide kopurua 1 izaten jarraitzen duelako.

14. Gainean **Lanen matxuren egitura** orrialdean, baliozkotu baliabideen esleipena WBSn eta hautatu **Gorde**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]