---
title: Baliabide-erreserbak eta zeregin-esleipenak nola daude erlazionatuta
description: Gai honek baliabide izendatuak, baliabideen erreserbak eta zereginen nola kudeatu eta nola erlazionatzen diren informazioa ematen du.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 9/27/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 72c741d8a0644589004ba20afbcd0baff7cfcb06
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993176"
---
# <a name="resource-bookings-and-how-they-relate-to-task-assignments"></a>Baliabide-erreserbak eta zeregin-esleipenak nola daude erlazionatuta

[!include [banner](../includes/psa-now-project-operations.md)]

Bi modu daude izena duten baliabideak proiektu talde batean eta esleitutako proiektu zeregin batean erreserbatzeko:

- Baliabidea zuzenean erreserbatuta daiteke proiektua batean eta, ondoren, esleitu proiektuaren zereginenei.
- Zereginak baliabide orokorra bat bilatu eta ordezkatu, orokorra benetako, izeneko baliabide erabil ondoren bati eslei dakizkioke. 

Kasuetako bi baliabidea booking-act aplikazioak erreserbatzen ditu, baliabidearen ahalmena.

Antolamendu-proiektuan proiektua kudeatzailea proiektua plana eta antolaketa jabea. Orokorra baliabide-esleipena erabiliz eta sortzen baliabide eskaera diozunean proiektua kudeatzailea dezakezu erreserbatutako proiektuan inprimatu baliabideak proiektua plana zehaztutako contours batekin. Erreserbatutako proiektua bat inprimatu baliabideak eta, ondoren, esleitu ahal izateko zereginak dute, hala ere, zeregin contours batekin erreserbatu contours lerrokatzeko modua ez dago. Erreserbak ez du proiektuaren antolaketan eragina.

Kontuan lan hainbat overlapping non mota bereko baliabideak hainbat behar concurrently lan egin proiektua konplexuak. Baliabide bat ez dator bat esleipenetan beren agregatuen duen contour bat buruzko informazioa, da zailago zereginen discrete beren bookings contour eta jatorrizko contours beren zereginak aldatzeko.

Adibide beheko lau zereginak multzo bera baliabidea eskatutako ahalegina guztira ordukoa izango da 62 bi aste-tarte jakin batean zehar eta contour jakin bat dago. Baliabidea Bob batez booked bereko bi asteak zehar baina contour beste batekin ordu 62, eskakizun eta bookings daude lerrokatzea.

| **Zeregina contours**    | **Orduak, guztira** | Al. 6/4 | Ar. 6/5 | Az. 6/6 | Og. 6/7 | Ol. 6/8 | Lr. 6/9 | Ig. 6/10 | Al. 6/11 | Ar. 6/12 | Az. 6/13 | Og. 6/14 | Ol. 6/15 |
|----------------------|-----------------|--------|--------|--------|--------|--------|--------|---------|---------|---------|---------|---------|---------|
| 1. zeregina               | 24              | 8      | 8      | 4      |        |        |        |         |         |         | 4       |         |         |
| 2. zeregina               | 16              |        |        | 4      | 4      |        |        |         | 8       |         |         |         |         |
| 3. zeregina               | 1,0              |        |        |        |        | 4      |        |         |         | 4       |         | 2       |         |
| 4. zeregina               | 12              |        |        |        |        |        |        |         |         |         | 4       |         | 8       |
|                      |                 |        |        |        |        |        |        |         |         |         |         |         |         |
| **Guztizkoak**           | 62              | 8      | 8      | 8      | 4      | 4      |        |         | 8       | 4       | 8       | 2       | 8       |
|                      |                 |        |        |        |        |        |        |         |         |         |         |

### <a name="bobs-availability"></a>Mikelen erabilgarritasuna
| **Baliabideen erreserba** | **Orduak, guztira** | Al. 6/4 | Ar. 6/5 | Az. 6/6 | Og. 6/7 | Ol. 6/8 | Lr. 6/9 | Ig. 6/10 | Al. 6/11 | Ar. 6/12 | Az. 6/13 | Og. 6/14 | Ol. 6/15 |
|------------------------|-----------------|--------|--------|--------|--------|--------|--------|---------|---------|---------|---------|---------|---------|
| Mikel                    | 62              | 4      | 4      | 8      | 8      | 8      |        |         | 4       | 4       | 8       | 8       | 6       |

Halere, ez da ez systematic erreserbatuta ordu contour egun bakoitzeko banaka zereginak esleitu. Proiektua kudeatzailea hartu baliabidea erabilgarritasuna bete eta pertsonalizatzeko proiektua antolaketa aldatu nahi bada, ondoren, ikusiko duten kendu erabiltzaile bat esleipena egiteko eta berrikusten saiatzen erreserbatu contours zeregin guztiak.

Kasuaren non erakunde batek emandako proiektua antolamendu-zeregin proiektua kudeatzailea eta baliabide-kudeatzaile bat proiektua-kudeatzaileak ezartzen ditu, antolaketa eta beharrezko lan contouring dituen. Baliabide-kudeatzailea genituen eragina proiektua kudeatzailea knowledge gabe antolaketa erreserbatu benetako baliabideak da ahalegina contours aldatuz gai izango. Baliabide kudeatzailea osatu da zerbait zer proiektua kudeatzailea eskatu ezberdinak, egon beharko proiektua antolaketan behar diren aldaketak zer buruzko hitzarmena izango zara.

Erreserbak eta esleipenak ez daudenek oso elkartuta, posiblea da profilak erresebatzea, zerreginen profilen ezberdinak direnak, edo esleipenak aldatu egoeretan emaitza emateko, erreserbak eta esleipenak lerrokatzetik kanpo dauden lekuan.

**Kontziliazio ikuspegiak** proiektuaren kudeatzaileari aukera ematen dio erreserbak eta esleipenak ikusteko, proiektuko taldekide bakoitzarenak. Ikuspegia erabiltzen koloreen eta shading erakutsi arteko taldeko kideak ez datoz bat dago dizun bookings eta esleipenetan. Informazio hau oinarrituta proiektua kudeatzailea dezakezu corrective ekintzak gauzatzeko kasuak baliabide bookings zabaltzeko edo esleipenetan eta ez bookings edo utzi bookings non baliabideak booked baina dituzte esleipenetan ez daude aukera emango dizun.

> [!NOTE]
> Zuk profila emandako zeregin bat mugitzen baduzu, profil horiek ez dira mantenduko. Contours, proiektua egutegiak kontu lan egin ataleko aldaketak lanorduekin eta oporrak arabera regenerated dira. Hau sistemak jatorrizko profilaren asmoa zein den ez dakielako gertatzen da, eta ezin du zehaztu mantentzeak zentzua duen edo ez denbora-epe berri batean. Erreserbak eta esleipenak deskonektatuta daudenez, erreserbek jatorrizko erreserba-profilak mantentzen dituzte. Kasu horretan, behar duzu bertan behera utzi eta berri esleipena-contour rebook.



[!INCLUDE[footer-include](../includes/footer-banner.md)]