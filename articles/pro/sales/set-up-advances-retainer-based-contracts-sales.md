---
title: Aurrerakinak eta atxikipenetan oinarritutako kontratuak
description: Gai honek proiektuetan oinarritutako kontratazio-ereduetan eta aurrerakinari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 10/20/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 87e275cb72f1edc5a2a9913b4aa47d461d1f3d3d9bf177bf0ffba8b463f4ce01
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6994396"
---
# <a name="advances-and-retainer-based-contracts"></a>Aurrerakinak eta atxikipenetan oinarritutako kontratuak


_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations-ek atxikipenetan oinarritutako kontratuak onartzen ditu. Atxikipenean oinarritutako kontratua bezeroak proiektu baten iraupen berdinean banatutako ordainketen multzo negoziatua da. Kontratu mota hau denboran eta materialean edo kontsumoan oinarritutako fakturazio ereduetarako erabiltzen da, bezeroari aurreikusteko faktura eta ordainketa egutegia emateko beharra dagoenean. Aldi bakoitzean sortutako diru-sarrerak bezeroarengandik jasotako ordainketarekin bateratzen dira aldi horren hasieran. Denboraren eta materialaren fakturazio ereduaren kontzeptuarekin bat etorriz, aldi bakoitzean sortutako diru-sarreren balioak sortutako kostuen arabera alda daitezke. Sortutako diru-sarrerak aldiaren hasieran jasotako zenbatekoa baino gehiago badira, proiektua entregatzeko enpresak honako hau egin dezake:

- Gehitu bezeroari faktura soilik 
- Atzeratu diru-sarreren bateragarritasuna hurrengo fakturazio-aldira eta egin azken faktura bat proiektuaren amaieran bateratu gabeko gainerako diru-sarrerengatik

Proiektuen Eragiketetan atxikipenean oinarritutako kontratazio ereduaren eta prezio finkoko kontratu ereduaren arteko desberdintasun nagusia hau da: prezio finkoko kontratu ereduan fakturaren zenbatekoa ez dago lotuta edo sortutako kostuekin lotuta. Fakturazioak mugarrietan oinarritutako planteamendu bat jarraitzen du, aldi horretan sortutako kostuekin bat etorriz. Atxikipenean oinarritutako kontratu batean, faktura daitezkeen diru-sarrerak fakturazio-metodoaren arabera erregistratzen dira kontratuaren lerroan. Fakturazio metodoa garaia eta materiala denean, fakturagarriak diren diru-sarrerak aldi bakoitzean sortutako kostuekin lotzen dira eta aldi batetik bestera alda daitezke. Hala ere, bezeroari aldizkako atxikipenaren zenbatekoa soilik fakturatzen zaio. Sistemak beste faktura bat erabiltzen du epea amaitzean, aldian erregistratutako fakturagarriak diren sarrerak bezeroari epearen hasieran fakturatutako zenbatekoarekin bateratzeko.

Metodo honen abantaila da bezeroaren kostuak aurreikus daitezkeela atxikitzeko ordutegian, denbora eta material eredu normalean ez bezala. Proiektua entregatzen duen erakundeak ere badu tarte bat, prezio finkoaren eredu batek onartuko ez lukeen esparrua handitzeagatik sortutako kostuak berreskuratzeko arriskua estaltzeko.

Aldizkako mantentze-lanetan oinarritutako ordutegiaz gain, Proiektuaren Eragiketek bezero baten aurrerapen bakarra erregistratu dezakete eta proiektuaren kostuaren osagai desberdinekin bateratu.

Proiektuaren eragiketetako atxikipena ez dago erabiltzeko erabilgarri bezeroari fakturatu arte. Azpisarean aurrerapen eta atxikipenetarako honako eremuek adierazten dute hori.

| Eremua | Deskribapena | Downstream eragina |
| --- | --- | --- |
| Eskuragarri dagoen zenbatekoa | Atxikipenean edo aurretiazko erregistroan erabil daitekeen kopurua. | Aurrerakina edo atxikipena fakturatu arte, ez da erabilgarri egongo, hau da, eskuragarri dagoen zenbatekoa zero izango da. |
| Erabilitako zenbatekoa | Atxikipenean edo aurrerapenean erabilitako kopurua. | Aurrerakina edo atxikipena fakturan partzialki bateratu daitezke benetako kostuekin, zati bat lehendik erabilitako edo kontsumitutako gisa markatuta egongo baita. Aurrerakinaren edo atxikipenaren gainerako zenbatekoa eskuragarri dago etorkizuneko fakturan benetako kostuekin bateratzeko. |


[!INCLUDE[footer-include](../../includes/footer-banner.md)]