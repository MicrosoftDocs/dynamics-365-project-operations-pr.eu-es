---
title: Benetakoak
description: Gai honek benetako datuen antolaketari buruzko informazioa ematen du.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/06/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 44c6e85f-5b21-4e24-999c-15a2f065d977
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8291e0eb8531e8e9690368675f333c44b6e92e48
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748927"
---
# <a name="actuals"></a>Benetakoak

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Oraingoak proiektu batean burutu den lan kopurua da. Proiektuaren errealitateak jatorrizko dokumentuetara aurki daitezke. Jatorri-dokumentu horiek denbora, gastua eta kutxako liburuko idazpen eta fakturak ere barne hartzen dituzte.

![Proiektuen errealitateak nola zuzentzen diren iturri dokumentuetara](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a>Bidali denbora-sarrera

PSAn, denboraren eta materialen kontratu-lerro batera mapatutako proiektu baterako denbora-sarrera bat bidaltzen denean, bi aldizkari-lerro sortzen dira. Lerro bat kostua da, eta bestea, berriz, fakturatu gabeko salmentetarako. Prezio finkoa kontratu-lerro batera mapatutako proiektu baterako denbora-sarrera bat bidaltzen denean, bi kutxako liburuaren lerroa sortzen da kostuetarako bakarrik. 

Prezio lehenetsiak sartzeko logika kutxako liburuaren lerroan dago. Aldi bateko sarrera-eremuko balio guztiak kutxako liburuaren lerroan kopiatzen dira. Eremu hauetan daude transakzioaren data, proiektua esleitu duen kontratuaren lerroa eta dibisaren emaitza prezioen zerrenda egokian. 

Prezio lehenetsiei eragiten dieten eremuak, adibidez **Funtzioa** eta **Organo Unitatea**, lehenetsitako kutxako liburuaren linean linean sartu behar izatea. Denboraren sarreran eremu pertsonalizatu bat gehitzen baduzu eta eremuaren balioa aktualitatera hedatu nahi baduzu, sortu eremua Aktualitateko entitatean eta erabili eremuko mapak eremua kopiatzeko garaian benetako sarrerara.

## <a name="submitting-an-expense-entry"></a>Gastu sarrera aurkeztuz

PSAn, gastu eta materialen kontratu-lerro batera mapatutako proiektu baterako denbora-sarrera bat bidaltzen denean, bi aldizkari-lerro sortzen dira. Lerro bat kostua da, eta bestea, berriz, fakturatu gabeko salmentetarako. Gastua kontratu-lerro batera esleitutako proiektu baterako denbora-sarrera bat bidaltzen denean, bi kutxako liburuaren lerroa sortzen da kostuetarako bakarrik.

Gastuen prezio lehenetsiak sartzeko logika, hautatutako gastu kategorian oinarritzen da **Sarrera gastua** orria. Transakzioaren data, proiektua esleitu duen kontratuaren lerroa eta dibisaren emaitza prezio-zerrenda egokia zehazteko erabiltzen dira. Hala ere, prezioarengatik, erabiltzaileak sartu duen zenbatekoa lehenetsitako gastu aldizkariaren lineetan kostua eta salmentak lehenetsiko dira.

PSAren gaur egungo bertsioan, gastu sarreretan unitate bakoitzeko prezioen lehenetsitako kategorien sarrera ez dago erabilgarri.

## <a name="using-journals-to-record-costs"></a>Aldizkariak erabiltzea kostuak erregistratzeko

PSAn, aldizkariek kostua edo diru-sarrerak erregistratzen dizkizute material, kuota, denbora, gastu edo zerga transakzio klaseetan. Aldizkari batek goiburua, lerroak eta a ditu **Berretsia** ekintza. Hona hemen aldizkari bat erabil dezakezuen eszenatoki batzuk:

- Proiektu batean benetako kostuak eta salmentak erregistratu behar dituzu.
- Transakzioen egitateak beste sistema batetik PSAra eraman behar dituzu.
- Beste sistema batean gertatu diren kostuak erregistratu behar dituzu, hala nola kontratazioan edo azpikontratazioan.

## <a name="recording-actuals-based-on-project-events"></a>Proiektuen gertaeretan oinarritutako errealitateak grabatu

Psak proiektu batean zehar gertatzen diren transakzio-ekonomiko guztiak erregistratzen ditu. Transakzio hauek honela erregistratzen dira: **unekoak**. Hurrengo tauletan, sortzen diren errealitate mota desberdinak daude, proiektuaren denbora eta materialak, prezio finkoa edo barne proiektua den ala ez, edo aurrez aurreko fasean dagoen ala ez, edo barne-proiektua den.

**Baliabidea proiektuaren kontratazio unitateko antolakuntza unitate bera da**

<table>
<thead>
<tr>
<th rowspan="3">Gertaera</th>
<th colspan="4">Proiektu fakultagarria edo saldu</th>
<th rowspan="3">Proiektua presazko etapan</th>
<th rowspan="3">Barne proiektua</th>
</tr>
<tr>
<th colspan="2">Denbora eta materialak</th>
<th colspan="2">Prezio finkoa</th>
</tr>
<tr>
<th>Benetakoak</th>
<th>Transakzio-moneta</th>
<th>Prezio finkoa</th>
<th>Transakzio-dibisa</th>
</tr>
</thead>
<tbody>
<tr>
<td>Denbora-sarrera bat sortu da.</td>
<td colspan="6">Ez dago jarduerarik Aktiboen entitatean</td>
</tr>
<tr>
<td>Denbora-sarrera bat bidali da.</td>
<td colspan="6">Ez dago jarduerarik Aktiboen entitatean</td>
</tr>
<tr>
<td rowspan="2">Ordua onartzen da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</td>
<td>Benetako kostua</td>
<td>Kontratatzailearen unitatearen dibisa</td>
<td rowspan="2">Benetako kostua</td>
<td rowspan="2">Kontratatzailearen unitatearen dibisa
<td rowspan="2">Benetako kostua</td>
<td rowspan="2">Benetako kostua</td>
</tr>
<tr>
<td>Fakturatu gabeko salmenten benetako zenbatekoa - Kargagarria</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
<tr>
<td rowspan="3">Ordua onartzen da eta ez da igoerarik fakturazio orduetan onartzen da.</td>
<td>Benetako kostua</td>
<td>Kontratatzailearen unitatearen dibisa</td>
<td rowspan="3">Benetako kostua</td>
<td rowspan="3">Kontratatzailearen unitatearen dibisa</td>
<td rowspan="3">Benetako kostua</td>
<td rowspan="3">Benetako kostua</td>
</tr>
<tr>
<td>Fakturatu gabeko salmenten benetako kopurua - Kargagarria kantitate berri baterako</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
<tr>
<td>Fakturatu gabeko salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
<tr>
<td rowspan="2">Faktura berresten da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</td>
<td>Fakturatu gabeko salmenten itzulera</td>
<td>Proiektu-kontratuaren dibisa</td>
<td rowspan="2">Mugarriko salmenta fakturatuak</td>
<td rowspan="2">Proiektu-kontratuaren dibisa</td>
<td rowspan="2">Ez da aplikagarria</td>
<td rowspan="2">Ez da aplikagarria</td>
</tr>
<tr>
<td>Fakturatutako salmentak</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
<tr>
<td rowspan="3">Faktura berresten da eta ez jeitsierarik fakturazio orduetan onartzen da.</td>
<td>Fakturatu gabeko salmenten itzulera</td>
<td>Proiektu-kontratuaren dibisa</td>
<td rowspan="3">Ez da aplikagarria</td>
<td rowspan="3">Ez da aplikagarria</td>
<td rowspan="3">Ez da aplikagarria</td>
<td rowspan="3">Ez da aplikagarria</td>
</tr>
<tr>
<td>Fakturatutako salmenten benetako kopurua - Kargagarria kantitate berri baterako</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
<tr>
<td>Fakturatutako salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
<tr>
<td rowspan="2">Faktura zuzentzen da kargatu beharreko kantitatea handitzeko.</td>
<td>Fakturatutako salmenten itzulera</td>
<td>Proiektu-kontratuaren dibisa</td>
<td rowspan="5">
<ul>
<li>Mugarriko salmenta itzulera</li>
<li>Mugarri-egoera aldatu da <strong>Fakturatutakoa</strong> egoeratik <strong>Faktura egiteko prest</strong> egoerara</li>
</ul>
</td>
<td rowspan="5">Proiektu-kontratuaren dibisa</td>
<td rowspan="5">Ez da aplikagarria</td>
<td rowspan="5">Ez da aplikagarria</td>
</tr>
<tr>
<td>Fakturatutako salmentak</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
<tr>
<td rowspan="3">Faktura zuzentzen da kargatu beharreko kantitatea gutxitzeko.</td>
<td>Fakturatutako salmenten itzulera</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
<tr>
<td>Fakturatutako salmenten benetako kopurua: kantitate berri baterako</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
<tr>
<td>Fakturatu gabeko salmenten benetako kopurua: kargagarria ezberdintasunerako</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
</tbody>
</table>

**Baliabidea proiektuaren kontratazio unitateko antolakuntza ez da unitate bera da**

<table>
<thead>
<tr>
<th rowspan="3">Gertaera</th>
<th colspan="4">Proiektu fakultagarria edo saldu</th>
<th rowspan="3">Proiektua presazko etapan</th>
<th rowspan="3">Barne proiektua</th>
</tr>
<tr>
<th colspan="2">Denbora eta materialak</th>
<th colspan="2">Prezio finkoa</th>
</tr>
<tr>
<th>Benetakoak</th>
<th>Transakzio-moneta</th>
<th>Prezio finkoa</th>
<th>Transakzio-dibisa</th>
</tr>
</thead>
<tbody>
<tr>
<td>Denbora-sarrera bat sortu da.</td>
<td colspan="6">Ez dago jarduerarik Aktiboen entitatean</td>
</tr>
<tr>
<td>Denbora-sarrera bat bidali da.</td>
<td colspan="6">Ez dago jarduerarik Aktiboen entitatean</td>
</tr>
<tr>
<td rowspan="4">Ordua onartzen da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</td>
<td>Benetako kostua</td>
<td>Kontratatzailearen unitatearen dibisa</td>
<td rowspan="4">Benetako kostua</td>
<td rowspan="4">Kontratatzailearen unitatearen dibisa</td>
<td rowspan="4">Benetako kostua</td>
<td rowspan="4">Benetako kostua</td>
</tr>
<tr>
<td>Fakturatu gabeko salmenten benetako zenbatekoa - Kargagarria</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
<tr>
<td>Baliabidearen unitate-kostua</td>
<td>Baliabidearen unitate-dibisa</td>
</tr>
<tr>
<td>Erakunde arteko salmentak</td>
<td>Kontratatzailearen unitatearen dibisa</td>
</tr>
<tr>
<td rowspan="5">Ordua onartzen da eta ez da igoerarik fakturazio orduetan onartzen da.</td>
<td>Benetako kostua</td>
<td>Kontratatzailearen unitatearen dibisa</td>
<td rowspan="5">Benetako kostua</td>
<td rowspan="5">Kontratatzailearen unitatearen dibisa</td>
<td rowspan="5">Benetako kostua</td>
<td rowspan="5">Benetako kostua</td>
</tr>
<tr>
<td>Baliabidearen unitate-kostua</td>
<td>Baliabidearen unitate-dibisa</td>
</tr>
<tr>
<td>Erakunde arteko salmentak</td>
<td>Kontratatzailearen unitatearen dibisa</td>
</tr>
<tr>
<td>Fakturatu gabeko salmenten benetako kopurua - Kargagarria kantitate berri baterako</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
<tr>
<td>Fakturatu gabeko salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
<tr>
<td rowspan="2">Faktura berresten da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</td>
<td>Fakturatu gabeko salmenten itzulera</td>
<td>Proiektu-kontratuaren dibisa</td>
<td rowspan="2">Mugarriko salmenta fakturatuak</td>
<td rowspan="2">Proiektu-kontratuaren dibisa</td>
<td rowspan="2">Ez da aplikagarria</td>
<td rowspan="2">Ez da aplikagarria</td>
</tr>
<tr>
<td>Fakturatutako salmentak</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
<tr>
<td rowspan="3">Faktura berresten da eta ez jeitsierarik fakturazio orduetan onartzen da.</td>
<td>Fakturatu gabeko salmenten itzulera</td>
<td>Proiektu-kontratuaren dibisa</td>
<td rowspan="3">Ez da aplikagarria</td>
<td rowspan="3">Ez da aplikagarria</td>
<td rowspan="3">Ez da aplikagarria</td>
<td rowspan="3">Ez da aplikagarria</td>
</tr>
<tr>
<td>Fakturatutako salmenten benetako kopurua - Kargagarria kantitate berri baterako</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
<tr>
<td>Fakturatutako salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
<tr>
<td rowspan="2">Faktura zuzentzen da kargatu beharreko kantitatea handitzeko.</td>
<td>Fakturatutako salmenten itzulera</td>
<td>Proiektu-kontratuaren dibisa</td>
<td rowspan="5">
<ul>
<li>Mugarriko salmenta itzulera</li>
<li>Mugarri-egoera aldatu da <strong>Fakturatutakoa</strong> egoeratik <strong>Faktura egiteko prest</strong> egoerara</li>
</ul>
</td>
<td rowspan="5">Proiektu-kontratuaren dibisa</td>
<td rowspan="5">Ez da aplikagarria</td>
<td rowspan="5">Ez da aplikagarria</td>
</tr>
<tr>
<td>Fakturatutako salmentak</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
<tr>
<td rowspan="3">Faktura zuzentzen da kargatu beharreko kantitatea gutxitzeko.</td>
<td>Fakturatutako salmenten itzulera</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
<tr>
<td>Fakturatutako salmenten benetako kopurua: kantitate berri baterako</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
<tr>
<td>Fakturatu gabeko salmenten benetako kopurua: kargagarria ezberdintasunerako</td>
<td>Proiektu-kontratuaren dibisa</td>
</tr>
</tbody>
</table>
