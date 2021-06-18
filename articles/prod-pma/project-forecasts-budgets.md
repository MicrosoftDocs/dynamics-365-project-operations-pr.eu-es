---
title: Proiektuaren aurreikuspenak eta aurrekontuak
description: Microsoft Dynamics 365 Finance proiektuen aurreikuspenak eta proiektuen aurrekontuak eskaintzen ditu zure proiektuak kudeatu eta kontrolatzeko.
author: Yowelle
ms.date: 10/25/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ForecastModel, ProjYearEndProcess
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 23501
ms.assetid: 4e6d1384-19a2-4232-b3f3-d2590c218bd7
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: c1c1cde984334af8cc30e7899e3cf0b38467666f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999611"
---
# <a name="project-forecasts-and-budgets"></a>Proiektuaren aurreikuspenak eta aurrekontuak

[!include [banner](../includes/banner.md)]

BI bide daude kudeatzeko eta kontrolatu zure proiektuak: proiektuaren iragarpenak eta proiektuaren aurrekontuak. 

Erabili proiektuaren aurreikuspenak erabil ditzakezu zure erakundeak ikuspegi operatiboa badu eta transakzio zehatz batzuetatik eratorritako diru-sarrera eta kostuetara bideratzen bada. Erabili proiektuaren aurrekontua egitean zure erakundeak ardazten badu gehiago finantza-kopuruak. 

Proiektuaren aurreikuspenek zein proiektuaren aurrekontuek aurreikusitako ereduak erabiltzen dituzte aurreikusitako transakzioen zenbatekoak mantentzeko. 

Metodo bakoitzak bere abantailak ditu. Zure erakunderako metodoa hautatu aurretik, honako puntu hauek kontuan hartu beharko zenituzke.

|   Esleipen-metodoa       |           Proiektuaren aurreikuspena            |        Proiektuaren aurrekontua                           |
|---------------------------|------------------------------------------|----------------------------------------------------|
| **Aldiaren esleipena**     | Ezin dituzu transakzioak esplizituki banatu aldi fiskal batean. Horren ordez, aurreikuspena eta iragarpenaren kontrola proiektuaren bizitzan oinarritzen dira. Aurreikuspenak data zehatz batean oinarritzen direnez, epea datatik ondorioztatu behar duzu. | Banatu ditzakezu transakzioak proiektu osoaren gainean edo aldi fiskalean. Epe batean esleitzen baduzu, erabili gabeko zenbatekoak hurrengo aldi fiskalera eraman ditzakezu. |
| **Transakzioak ikustea**  | Transakzioak aurreikuspen inprimakietan ikus ditzakezu, eta bertan enpresa osoarentzako eta proiektu guztietarako aurreikuspenak ikus ditzakezu, hierarkia edozein dela ere. Proiektu jakin batera bideratzeko, datuak iragazi behar dituzu.                                       | Aurreikusitako transakzioak proiektuaren hierarkia bakar baterako ikus ditzakezu. Hori dela eta, guraso proiektu baten edo haren azpiproiektuen transakzioen xehetasunak ikus ditzakezu.                 |
| **Transakzio aldagaiak** | Aurreikusitako transakzioak sartzerakoan, dauden atributu guztiak erabil ditzakezu benetako transakzio baterako. Horrek iragarpenean xehetasun gehiago lortzeko aukera ematen du. Adibidez, kantitateei, langileei, elementuei edo lineako propietateei buruzko xehetasunak sar ditzakezu.         | Aurrekontuaren xehetasunak sartzean, zenbatekoak, kategoriak eta jarduerak soilik erabil ditzakezu.                    |
| **Segurtasuna**              | Iragarpena aurreikuspen inprimakietan sartutako transakzioetan oinarritzen da eta ez du prozesuaren kontrol mekanismorik. Aurreikuspen inprimakirako baimenak dituen edozein langilek informazioa berrikusi dezake onartu gabe.                                        | Aurrekontuek lan-fluxuen sistema erabiltzen dute, aldaketen kudeaketa ahalbidetzen duena eta berrikuspenen historia gordetzea ahalbidetzen duena.         |
| **Sarrera mota**           | Aurreikusitako transakzioen sarrerak unitate kopuruaren eta kostuaren eta salmentaren unitate prezioen arabera daude.  | Aurrekontuaren xehetasunak zenbatekoetan oinarrituta daude, kostuen eta sarreren artean banatuta.                                          |
| **Iragarpen ereduak**       | Iragarpen bakoitza eredu batekin lotu behar denez, iragarpen eredu ugari sor ditzakezu eta azpimodelak ere konfigura ditzakezu.           | Proiektuaren aurrekontuak aurrekonturako erabiltzen diren aurreikuspen ereduak mugatzen ditu. Iragarpen eredu gutxiagok proiekzioen koherentzia handitzen lagun dezakete.                           |
| **Kostuak gainditzea**         | Kostuak gainditzea eragingo duten transakzioen sarrera baimendu edo debekatu dezakezu.   | Proiektuaren aurrekontuak kontrolerako aukera osagarriak eskaintzen dizkie erabiltzaileei. Abisuak eta gehiegikeriak baimendu ditzakezu.                    |
| **Kontrola**               | Iragarpenaren kontrola iragarpenen murrizketa erabiliz egiten da. Benetako zenbatekoak aurreikusitako transakzio saldoetatik kentzen dira, inolako ikuskapen arrastorik gabe. Horrek benetako transakzioak non gertatu diren azaltzea zaildu dezake.                   | Proiektuaren aurrekontuaren kontrolean, gainerako aurrekontuko zenbatekoetatik benetako kopuruak kentzen dira. Horrek auditoria pista argiagoa egiteko aukera ematen du.                                   |

## <a name="project-forecasts"></a>Proiektuaren aurreikuspenak
Proiektuen iragarpena erabiltzen duzunean, iragarpen transakzioak transakzio mota bakoitzerako iragarpen inprimakietan sar ditzakezu. Benetako transakzio baterako erabilgarri dauden atributu guztiak aurreikusitako transakzio baterako erabil daitezke, adibidez, lineako errentagarritasuna, lineako atributuak, langileak edo deskribapenak. Halaber, kostu bat igaro ondoren bezeroari fakturatuko diozun proiektatu dezakezu. 

Proiektuak aurreikusteko eragiketak unitateetan eta zenbatekoetan oinarritzen dira. 

Proiektuaren iragarpen bakoitza iragarpen eredu batekin lotu behar duzu. Aurreikuspen transakzio bat sartzen duzunean, iragarpen eredu bat iradokitzen da automatikoki. Iragarpen ereduak aurreikusitako transakzioen edukiontzi gisa jokatzen du. 

Iragarpen ereduak eredu baten azpimodel gisa izendatu ditzakezu. Horrek eskualdearen, denboraren edo sailaren arabera aurreikus dezake. Iragarpen transakzioak eredu batean kopia ditzakezu eredu berri bat sortzeko, eta transakzioak liburu nagusira ere transferi ditzakezu. Aurreikuspenen eta eredu baten artean harreman bat eta bat dagoelako, iragarpen eredu bakoitzak proiektu baterako aurrekontu bereizia osatzen du. 

Iragarpen ereduek aurreikuspenen murrizketa erabil dezakete proiektuen kontrol mekanismo gisa. Aurreikuspenen murrizketan, benetako transakzioek aurreikusitako transakzio saldoak murrizten dituzte. Hala ere, aurreikuspenen murrizketa hierarkiako proiektu altuenari aplikatzen zaionez, aurreikuspenen aldaketen ikuspegi mugatua eskaintzen du. Adibidez, langilea azpiproiektu batekin lotzen bada, langilearen benetako transakzioak proiektu nagusian argitaratuko dira. Horrek aldaketen jarraipena zaildu dezake, ezin delako zehaztu zein transakziok zein azpiproiektu eragin duen aurreikusitako zenbatekoa murriztea. Hori dela eta, ideia ona da iragarpen-ereduaren kopia bat erabiltzea, aurreikuspenak murrizteko erabil dezaten. Ondoren, txostenak erabil ditzakezu hasieran aurreikusitakoa ikusteko. 

Proiektuaren iragarpenak berrikusi, kopiatu, ezabatu edo transferi ditzakezu liburu-aurrekontu orokor batera. Hala ere, ez dago prozesuen kontrolik. Aurreikuspen inprimakirako baimena dituen edozein langilek egin berrikusteak dezake berrikusi gabe.

-   **Berrikusi** - Aurreikusitako transakzioa jatorrizko sarrerak egin ziren inprimaki berdinetan berrikusi dezakezu.
-   **Kopiatu edo ezabatu** - Iragarpen transakzioak kopiatzean, iragarpen eredu bateko transakzio lerroak beste iragarpen eredu batera kopiatzen dituzu. Iragarpen bat ezabatzen duzunean, iragarpen transakzioak iragarpen eredu batetik ezabatzen dituzu. Kopiatu edo ezabatzen diren aurreikusitako transakzioak mugatzeko, hautatu transakzio mota eta data zehatzak. Horrek iragarpenaren zati zehatzak soilik kopiatu edo ezabatu ahal izango dituzu.
-   **Transferentzia** - Proiektuaren iragarpena liburu nagusiko aurrekontu batera transferitzen duzunean, iragarpen eredu baten iragarpen transakzioak liburu aurrekontu orokor batera transferitzen dituzu. Aurretik transferitutako transakzioak gainidatzi ditzakezu zure proiektuaren iragarpena transferitzen duzun liburu nagusiaren aurrekontuan.

## <a name="project-budgets"></a>Proiektuaren aurrekontuak
Proiektuen aurrekontua iragarpena baino metodo errazagoa da, nahiz eta iragarpen ereduekin integratzen den. Sarrera inprimaki bakarra erabiltzen du aurrekontuaren jatorrizko xehetasunak eta berrikuspenak egiteko, eta zenbatekoan, kategorian edo jardueran soilik oinarritzen diren proiekzioak baimentzen ditu. 

Proiektuaren aurrekontuetan, jatorrizko aurrekontu eta berrikuspen guztiak proiektuaren lan-fluxura bidali behar dira onar ditzaten. Lan-fluxuek prozesuaren gaineko kontrol handiagoa ematen dute eta aldaketen historiaren erregistroa sortzen dute. 

Proiektuaren aurrekontuak liburu nagusien aurrekontuaren antza du, baina azkarrago eta errazago konfiguratzen da. Liburu orokorren aurrekontuen aukera asko, hala nola zenbaki sekuentziak edo moneta, ez dira proiektuetarako bereizita ezarri behar.

Proiektuaren aurrekontuak automatikoki lotzen dira bi iragarpen ereduekin, bat jatorrizko aurrekontuarekin eta bestea gainerako aurrekontuarekin. Hori dela eta, iragarpen ereduetan oinarritutako txostenek aurrekontu datuak erabil ditzakete. Proiektuaren aurrekontua konprometitzen denean, sistemak aurreikusitako transakzioak sortzen ditu lotutako ereduetan oinarrituta, eta horiek salatzeko eta kontrolatzeko erabiltzen dira.

## <a name="forecast-models"></a>Iragarpen ereduak
Iragarpen ereduek geruza bakarreko hierarkia dute. Horrek esan nahi du proiektuaren iragarpen bat iragarpen eredu batekin lotu behar dela.

Proiektuen iragarpena erabiltzen baduzu, ereduak azpimodelo gisa identifika ditzakezu. Orduan iragarpenak sor ditzakezu departamenduaren, denboraldiaren edo eskualdearen arabera. Adibidez, urtebeteko iragarpen eredua sor dezakezu eta, ondoren, eskualdeetako buruek aurkezten dituzten Ipar-ekialdeko, Hego-ekialdeko, Ipar-mendebaldeko eta Hego-mendebaldeko eskualdeetako aurreikuspenak azpimodelak sor ditzakezu. Eskuragarri dauden txostenetan aukera desberdinak hautatuta, informazioa aurreikuspen osoaren edo azpimodelaren arabera ikus dezakezu.





[!INCLUDE[footer-include](../includes/footer-banner.md)]