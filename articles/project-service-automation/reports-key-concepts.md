---
title: Gako-kontzeptuak
description: Gai honek Project Service Automation-en (PSA) baliabideen kudeaketa gako-kontzeptuen inguruko informazioa eskaintzen du.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: f5f96f65-c191-493a-aef7-df7deb52a9cb
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 4a839b828d5e1da1e5a8d8a378197b3d4932e529
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748920"
---
# <a name="key-concepts"></a>Gako-kontzeptuak

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Hurrengo taulan, Dynamics 365 Project Service Automation aplikazioan erabiltzen diren gako-kontzeptuak zehazten dira.

| Kontzeptuak                    | Definizioa |
|----------------------------|------------|
| Proiektu-taldeko kidea        | Proiektu-taldeko zati gisa, proiektu-taldeko kidea erreserbak dituen baliabide izendatu bat, erreserbaziorik ez duen baliabide izendatua edo baliabide orrokorra izan daiteke. Baliabide orokorrek ez dute erreserbarik, proiektuarentzat lokalak dira eta ez dute gaitasun-mugarik proiektuetan. |
| Proiektuko baliabide orokorra   | Baliabidearen izena jakin gabe taldea sortzeko edo proiektuaren planerako langileak hartzea ahalbidetzen duen leku-marka baliabidea. Proiektuaren egutegia baliabide orokorren egutegi gisa erabiltzen da. Baliabide orokorrak proiektu-taldera gehitu eta zereginetara esleitu daitezke. |
| Erreserbatutako orduak               | Baliabide-orduak irmotasunez erreserbatzen dira proiektu baten aurrean, proiektuaren lana amaituta dagoela bermatzeko. Erreserbatutako orduak baliabidearen ahalmen orokorretik kontsumitzen dira. Erreserbak izendatutako baliabideekin soilik egin daitezke, eta ez baliabide orokorrekin. |
| Esleitutako orduak             | Baliabide orduak proiektuaren antolaketako zereginetan esleitzen dira. Esleipenak izendatutako baliabideei edo baliabide orokorrei egin daitezke. Esleipenak erreserbengandik independentea izan daitezke. |
| Beharrezko orduak             | Behar den gaitasuna, baina baliabide izendatuak oraindik ez ditu betetzen. Beharrezko orduak garrantzitsuak dira baliabide eskakizunak sortu dituzten taldekide orokorrentzat soilik. |
| Eskaera                     | Uneko eta sarrerako lan karga. Project Service Automation-en, eskaera baliabide-eskakizun edo baliabide-eskaera gisa erakusten da. |
| Baliabideen eskakizuna       | Entitate bat ohituta dago beharrezko orduak, hasiera- eta amaiera-datak, trebetasunak, geografia eta beharrezkoak diren baliabidetarako prezio-neurriak ateratzen. Baliabideen eskakizunak proiektu-taldeko kideek sortutakoak edo bakarka sortutakoak dira. |
| Baliabide-eskaera           | Baliabide-kudeatzaile batek bete behar duen baliabide-eskakizuna egiteko "gutunazal" gisa erabiltzen den entitatea. |
| Baliabide-funtzioa lehenetsia      | Erabilera kalkulatzeko baliabide bat taldekatzen duen funtzioa. Baliabideak funtziorako beharrezkoak diren gaitasunak izango dituela eta funtzio horren xede-erabilera betetzeko balio duela uste da. |
| Baliabideen antolaketa unitatea | Baliabide bati esleitzen zaion antolaketa unitatea. |
| Ingerada                    | Zereginak, eskakizunak edo esleipen orduak egunero banatzen dira. Adibidez, bost eguneko 40 orduko zeregina 5 egunez jar daiteke eguneko zortzi ordu eginda. |
| Kontziliazioaren ikuspegia        | Proiektu-taldeko kide bakoitzeko erreserbak eta zereginak erakusten dituen ikuspegia. Ikuspegi honek proiektu-kudeatzaileari erreserben eta zereginen arteko desoreka bilatzeko eta bat ez datozenean zuzentzeko neurriak hartzeko aukera ematen dio. |
| Lanorduak                 | Baliabideen ahalmena eta lanaldiko zein lanaldikoak ez diren orduak identifikatzeko erabiltzen den entitatea. Erakunde horri baliabideen egutegia ere deitzen zaio. |
