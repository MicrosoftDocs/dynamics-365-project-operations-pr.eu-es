---
title: Kanpoko antolaketa
description: Artikulu honek kanpoko antolaketari buruzko informazioa ematen du.
author: ruhercul
ms.date: 10/31/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: 746fb3a7c812b2b387ec707e58796d02d2473847
ms.sourcegitcommit: b1a5b9bb8b826678fc52f1d5a3d199a71caccb0a
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/03/2022
ms.locfileid: "9736979"
---
# <a name="external-scheduling"></a>Kanpoko antolaketa

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Kanpoko antolaketa-moduak zereginen xehetasunen egiturarekin (WBSs) zerikusia duten entitateak sortu, eguneratu eta ezabatzeko aukera ematen dizu, baina Microsoft Project for the Web-erako ezartzen dituen egungo mugarik gabe. Balioztapen mugatua ere ematen du. Modu hau bezero hauek bakarrik erabili behar dute:

- Project Operations-ek eskaintzen duen programazio-logikatik kanpo WBS bat definitzeko behar diren tresnak dituzten bezeroak
- Ordutegien hierarkia, mendekotasunak edo zereginen iraupena kudeatu behar duten bezeroak

> [!IMPORTANT]
> Baliteke WBSrekin erlazionatutako entitateetan behar bezala sartu ez diren datuak ez errendatzea baliabideen bateratzearen saretan, estimazioen saretan, jarraipenaren saretan edo baliabideen esleipenen saretan.

## <a name="configuration"></a>Konfigurazioa

Modu lehenetsian gaitzen da eginbidea. Hala ere, proiektuen erabiltzeko prest dagoen orri nagusian, erlazionatutako eremua ez da ikusten lehenespenez. Eremua gaitzeko, Maker Portal-en, ireki proiektuaren entitatearen orri nagusia, hautatu **Antolaketa-motorra** eremua, eta, ondoren, eremua hona aldatu **Lehenespenez ikusgai**. Erabiltzeko prest dagoen proiektuaren orri nagusia erabiltzen ez baduzu, editatu lehendik dagoen orria eta gehitu **Antolaketa-motorra** eremua hari.

## <a name="settings"></a>Ezarpenak

Kanpoko programazio modua erabiltzeko, lehenik proiektu berri bat sortu eta hautatu **Kanpoan antolatua** antolaketa-motorra proiektuaren orri nagusiko goitibeherako zerrendan. Modu hau proiektu baterako konfiguratu ondoren, ezin da aldatu.

## <a name="viewing-the-wbs"></a>WBS ikustea

Proiektu bat kanpoan programatuta badago, Project for the Web-erako sarbidea mugatuta dago proiektu horretarako. WBS ikusteko, jarraipen-saretara joan behar duzu, non WBS osoa erakusten den.

## <a name="creating-and-editing-the-wbs"></a>WBS sortzea eta editatzea

Proiektu batean kanpoko antolaketa gaituta badago, WBSrekin lotutako entitate guztien datuak definitu behar dituzu, zereginak, taldekideak, baliabide-esleipenak eta mendekotasunak barne.

Ondorengo ilustrazioak Proiektuaren antolaketaren datu-eredua erakusten du.

![Proiektua antolatzeko datu-eredua.](media/projectplanningdatamodel.png)

## <a name="functional-limitations"></a>Muga funtzionalak

Kanpoan antolatutako proiektuetan ez dira onartzen ondorengo eragiketak.

### <a name="project-planning"></a>Proiektuaren antolaketa

- **Kopiatu proiektua** – Eragiketa ez da onartzen kanpotik antolatutako proiektuetan.
- **Mugitu proiektua** – Proiektu baten hasiera-dataren aldaketak ez du WBSko zereginen edo baliabide-esleipenen hasiera mugituko.
- **Proiektuaren kudeatzailea eguneratzea** – Proiektuaren orri nagusian proiektuaren kudeatzaileari egindako aldaketek ez dute automatikoki proiektuko taldekide berririk sortuko proiektua bihurtu arte.
- **Proiektuaren lan orduen txantiloia eguneratzea** – Proiektuaren lan orduen txantiloian egindako aldaketek ez dute proiektuaren ordutegia berriro kalkulatuko.
- **Baliabideen esleipenaren ingeradak** – Baliabide-esleipenak sortzeak ez du automatikoki eguneratuko **mdyn\_PlannedWork** eremua. Eremu hau baliabideak esleitzeko ahaleginaren ingerada gordetzeko erabiltzen da. Baliabideen esleipen-sarean edo baliabideen bateratze-sarean denbora-fasean egindako ahalegina erakusten baduzu, baliozko baliabideen esleipen-ingerada definitu behar dituzu. Ingerada hauek behar bezala formatua izan behar dute, kostuen eta salmenta prezioen ingeradaren kalkulua abiarazteko. Project for the Web-ek antolatutako proba-proiektu bat sortzea gomendatzen dugu eta, ondoren, lotutako datuak berrikustea eskakizunak eta formatua berresteko.

### <a name="resource-management"></a>Baliabideen kudeaketa

- **Baliabide orokorrak betetzea** – Baliabide orokorrak betetzea ez da onartzen kanpoan programatutako proiektuetan. Baldintza irekiak aktiboak betetzen saiatzean proiektuko taldekide berriak sortuko dira, baina ez du taldekide generikoa ezabatuko edo taldekide generikoa ordezkatuko lehendik dauden baliabide-esleipenetan.
- **Ezabatu taldeko kidea** – Taldekide bat ezabatzeak ez ditu automatikoki ezabatuko baliabide-esleipenak.

### <a name="quoting-and-contracting"></a>Eskaintzak eta kontratazioa

- **Eskaintza-lerroa eta kontratu-lerroaren xehetasunak inportatzea** – Proiektu batetik eskaintza- edo kontratu-lerroaren xehetasunak inportatzen direnean, aplikazioa probatu da gehienez 500 zeregin soilik onartzen dituen WBAn, zeregin bakoitzeko 20 esleipen muga batean oinarrituta.

### <a name="actuals-and-invoicing"></a>Benetako datuak eta fakturazioa

- WBS eta finantza-transakzioen artean dauden baliozkotzeetan aldaketarik ez dagoen arren, garrantzitsua da erabiltzeko prest dagoen datu-ereduarekin bat egitea, beheranzko transakzio guztiak espero bezala exekutatzen direla ziurtatzeko.
