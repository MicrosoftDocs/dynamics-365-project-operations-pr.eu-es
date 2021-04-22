---
title: Benetako datuak
description: Gai honek Microsoft Dynamics 365 Project Operations-en errealitateekin lan egiteko moduari buruzko informazioa eskaintzen du.
author: rumant
manager: AnnBe
ms.date: 04/01/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 304c51a4e502ad6ecec1fd821e98d6604ddd59ba
ms.sourcegitcommit: b4a05c7d5512d60abdb0d05bedd390e288e8adc9
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/02/2021
ms.locfileid: "5852529"
---
# <a name="actuals"></a>Benetako datuak 

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako Project Operations, Lite hedapena - proformaren fakturazioari aurre egitea_

Eguneratzeek proiektu batean berrikusitako eta onartutako finantza eta egutegia adierazten dute. Denbora, gastua, materialaren erabileraren sarrerak eta egunkarietako sarrerak eta fakturak onartzearen ondorioz sortzen dira.

## <a name="journal-lines-and-time-submission"></a>Aldizkari lerroak eta denbora bidaltzea

Denbora sartzeari buruzko informazio gehiago lortzeko, ikusi [Denbora sartzeko ikuspegi orokorra](../time/time-entry-overview.md).

### <a name="time-and-materials"></a>Denbora eta materialak

Aurkezten den denbora-sarrera bat denbora eta materialen kontratu-lerro batera mapatuta dagoen proiektuarekin lotzen denean, sistemak bi aldizkari-lerro sortzen ditu, bata kosturako eta bestea fakturatu gabeko salmentetarako.

### <a name="fixed-price"></a>Prezio finkoa

Prezio finkoa kontratu-lerro batera lotutako proiektu baterako denbora-sarrera bat bidaltzen denean, sistemak kostuaren kutxako liburuaren lerro bat sortzen du.

### <a name="default-pricing"></a>Prezio lehenetsia

Prezio lehenetsiak sortzeko logika kutxako liburuaren lerroan dago. Aldi bateko sarrera-eremuko balioak kutxako liburuaren lerroan kopiatzen dira. Balio hauetan daude transakzioaren data, proiektua esleitu duen kontratuaren lerroa eta dibisaren emaitza prezioen zerrenda egokian.

Prezio lehenetsiei eragiten dieten eremuak, adibidez **Funtzioa** eta **Baliabide-unitatea**, kutxako liburuaren lerroko prezio egokia zehazteko erabiltzen dira. Eremu pertsonalizatua gehi dezakezu denbora-sarreran. Eremuaren balioa benetakoetara hedatzea nahi baduzu, sortu eremua **Benetako datuak** eta **Kutxako liburuaren lerroa** taulak. Erabili kode pertsonalizatua hautatutako eremuaren balioa Denbora-sarreratik Eguneraino aldizkariaren lerroaren bidez transakzio-jatorriak erabiliz hedatzeko. Transakzioen jatorriari eta konexioei buruzko informazio gehiago lortzeko, ikusi [Benetakoak jatorrizko erregistroekin lotzea](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).

## <a name="journal-lines-and-basic-expense-submission"></a>Aldizkari lerroak eta oinarrizko gastuen aurkezpena

Gastuen sarrerari buruzko informazio gehiago lortzeko, ikusi [Gastuen ikuspegi orokorra](../expense/expense-overview.md).

### <a name="time-and-materials"></a>Denbora eta materialak

Aurkezten den oinarrizko gastuaren sarrera bat denbora eta materialen kontratu-lerro batera mapatuta dagoen proiektuarekin lotzen denean, sistemak bi aldizkari-lerro sortzen ditu, bata kosturako eta bestea fakturatu gabeko salmentetarako.

### <a name="fixed-price"></a>Prezio finkoa

Bidalitako oinarrizko gastua kontratu-lerro batera esleitutako proiektu baterako denbora-sarrera bat bidaltzen denean, sistemak kutxako liburuaren lerro bat sortzen du kostuetarako.

### <a name="default-pricing"></a>Prezio lehenetsia

Gastuetarako lehenetsitako prezioak sartzeko logika gastuen kategorian oinarritzen da. Transakzioaren data, proiektua esleitu duen kontratuaren lerroa eta dibisaren emaitza prezio-zerrenda egokia zehazteko erabiltzen dira. Prezio lehenetsiei eragiten dieten eremuak, adibidez **Transakzioaren kategoria** eta **Unitatea**, kutxako liburuaren lerroko prezio egokia zehazteko erabiltzen dira. Hala ere, honek prezioen zerrendako prezioen metodoa dagoenean bakarrik funtzionatzen du **Unitateko prezioa**. Prezioen metodoa bada **Kostuan** edo **Markaketa kostuaren gainetik**, gastu sarrera sortzerakoan sartutako prezioa kosturako erabiltzen da eta salmenta egunkariaren lerroan prezioa prezio metodoaren arabera kalkulatzen da. 

Gastu sarreran eremu pertsonalizatua gehi dezakezu. Eremuaren balioa benetakoetara hedatzea nahi baduzu, sortu eremua **Benetako datuak** eta **Kutxako liburuaren lerroa** taulak. Erabili kode pertsonalizatua hautatutako eremuaren balioa Denbora-sarreratik Eguneraino aldizkariaren lerroaren bidez transakzio-jatorriak erabiliz hedatzeko. Transakzioen jatorriari eta konexioei buruzko informazio gehiago lortzeko, ikusi [Benetakoak jatorrizko erregistroekin lotzea](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).

## <a name="journal-lines-and-material-usage-log-submission"></a>Aldizkari lerroak eta materialaren erabilera erregistroa bidaltzea

Gastuen sarrerari buruzko informazio gehiago lortzeko, ikusi [Materialaren erabilera erregistroa](../material/material-usage-log.md).

### <a name="time-and-materials"></a>Denbora eta materialak

Aurkeztutako materialaren erabilera erregistroaren sarrera denbora eta materialen kontratu lerro batera mapatuta dagoen proiektuarekin lotzen denean, sistemak aldizkari lerro bi sortzen ditu, bata kostuarena eta bestea fakturatu gabeko salmentetarako.

### <a name="fixed-price"></a>Prezio finkoa

Bidalitako materialaren erabilera-erregistroaren sarrera kontratu-lerro batera esleitutako proiektu baterako denbora-sarrera bat bidaltzen denean, sistemak kutxako liburuaren lerro bat sortzen du kostuetarako.

### <a name="default-pricing"></a>Prezio lehenetsia

Materialaren prezio lehenetsiak sartzeko logika produktuaren eta unitateen konbinazioan oinarritzen da. Transakzioaren data, proiektua esleitu duen kontratuaren lerroa eta dibisaren emaitza prezio-zerrenda egokia zehazteko erabiltzen dira. Prezio lehenetsiei eragiten dieten eremuak, adibidez **Produktuaren IDa** eta **Unitatea**, kutxako liburuaren lerroko prezio egokia zehazteko erabiltzen dira. Hala ere, katalogoko produktuetarako bakarrik funtzionatzen du. Idatzi produktuetan, materialaren erabilera erregistroa sortzen denean sartutako prezioa aldizkari lerroetako kostu eta salmenta preziorako erabiltzen da. 

**Materialaren erabilera-erregistroa** sarreran eremu pertsonalizatua gehi dezakezu. Eremuaren balioa benetakoetara hedatzea nahi baduzu, sortu eremua **Benetako datuak** eta **Kutxako liburuaren lerroa** taulak. Erabili kode pertsonalizatua hautatutako eremuaren balioa Denbora-sarreratik Eguneraino aldizkariaren lerroaren bidez transakzio-jatorriak erabiliz hedatzeko. Transakzioen jatorriari eta konexioei buruzko informazio gehiago lortzeko, ikusi [Benetakoak jatorrizko erregistroekin lotzea](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).

## <a name="use-entry-journals-to-record-costs"></a>Erabili sarreren aldizkariak kostuak erregistratzeko

Aldizkariek kostua edo diru-sarrerak erregistratzen dizkizute material, kuota, denbora, gastu edo zerga transakzio klaseetan. Aldizkariak helburu hauetarako erabil daitezke:

- Eraman transakzioen egitateak beste sistema batetik Microsoft Dynamics 365 Project Operations-era.
- Beste sistema batean gertatu diren kostuak erregistratu. Kostu horien artean kontratazio edo azpikontratazio kostuak sar daitezke.

> [!IMPORTANT]
> Aplikazioak ez ditu aldizkari lerro mota edo aldizkari lerroan sartutako erlazionatutako prezioak balioztatzen. Hori dela eta, egiazkoek proiektuan duten kontabilitate-inpaktuaz guztiz jabetzen den erabiltzaileak soilik erabili beharko lituzke sarrera-aldizkariak egiazkoak sortzeko. Aldizkari mota honen eragina dela eta, arretaz aukeratu beharko zenuke nork duen sarbidea aldizkariak sortzeko.

## <a name="record-actuals-based-on-project-events"></a>Erregistratu proiektuen gertaeretan oinarritutako benetako datuak

Project Operations-ek proiektu batean gertatzen diren finantza-transakzioak erregistratzen ditu. Transakzio hauek honela erregistratzen dira: unekoak. Hurrengo tauletan, sortzen diren errealitate mota desberdinak daude, proiektuaren denbora eta materialak, prezio finkoa edo barne proiektua den ala ez, edo aurrez aurreko fasean dagoen ala ez, edo barne-proiektua den.

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a>Baliabidea proiektuaren kontratazio unitateko antolakuntza unitate bera da

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

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a>Baliabidea proiektuaren kontratazio unitateko antolakuntza ez da unitate bera da

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


[!INCLUDE[footer-include](../includes/footer-banner.md)]
