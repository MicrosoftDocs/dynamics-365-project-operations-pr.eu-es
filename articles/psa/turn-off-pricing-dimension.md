---
title: Desaktibatu prezio-dimentsioa
description: Gai honek prezio-dimentsioak Project Service soluzioan nola ezarri erakusten du.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/06/2018
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 1ae95430c368370145c7081a5d94d6161a7700b4
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071121"
---
# <a name="turn-off-a-pricing-dimension"></a>Desaktibatu prezio-dimentsioa

Baliteke prezioen estrategia berrikusi eta eguneratu behar izatea zenbait urtean behin. Egin ditzakezun eguneratzeek lehendik dagoen prezio-dimentsioa desaktibatzea eta berri bat sortzea eska dezakete. Adibidez, baliteke aurrez prezioa **Funtzioa** aukerare arabera jarrita izatean, baina orain prezioa **Lan esperientzia** aukeraren arabera jartzea erabaki duzu. Horrek **Funtzioa** prezio-dimentsio gisa desaktibatzea eta pezio-dimentsio berri gisa **Lanaren esperientzia** sortzea eska diezazuke. 

Prezio-dimentsio bat desaktibatzeko, aurretiaz prestatutakoa edo pertsonalizatua den kontuan izan gabe, ezarri prezio-dimentsioaren **Kostuari aplikagarria** eta **Salmentei aplikagarria** eremuak **Ez** gisa.

Hala ere, hau egiten duzunean, errore-mezu hau jaso dezakezu.

![Prezio-dimentsio bat desaktibatzean ager daitekeen negozio-prozesuaren errorea](media/Business-Process-Error.png)


Errore-mezu horrek desaktibatu nahi den dimentsiorako aurrez konfiguratutako prezioen erregistroak daudela adierazten du. Dimentsio bati erreferentzia egiten dioten **Funtzio-prezioa** eta **Funtzio-prezioaren gainprezioa** erregistro guztiak ezabatu egin behar dira dimentsioaren aplikagarritasuna **Ez** gisa ezarri ahal izateko. Arau hori aurretiaz prestatutako prezio-dimentsioei eta sortu ditzakezun prezio-dimentsio pertsonalizatuei aplikatzen zaie. Balidazio horren arrazoia Project Service-k **Funtzio-prezioa** erregistro bakoitzak dimentsioen konbinazio esklusiboa izan behar duela zehaztu duela da. Adibidez, **2018ko AEBetako kostu-tasak** izeneko prezio-zerrendan, honako **Funtzio-prezio** errenkada hauek dituzu. 

| Titulu estandarra         | Erakunde-unitatea    |Unitatea   |Prezioa  |Moneta  |
| -----------------------|-------------|-------|-------|----------|
| Sistemen ingeniaria|Contoso US|Hour| 100|USD|
| Sistemen ingeniari nagusia|Contoso US|Hour| 150| USD|


**Titulu estandarra** prezio-dimentsio gisa desaktibatzen duzunean eta Project Service-ren prezioen motorrak prezioa bilatzen duenean, sarrerako testuinguruko **Erakunde-unitatea** balioa soilik erabiliko du. Sarrerako testuinguruaren **Erakunde-unitatea** "Contoso US" bada, emaitza ez-determinista izango da bi errenkadak bat etorriko direlako. Egoera hori ekiditeko, **Funtzio-prezioa** erregistroak sortzen dituzunean, Project Service-k dimentsioen konbinazioa esklusiboa dela balioztatzen du. Dimentsioa **Funtzio-prezioa** erregistroak sortu ondoren desaktibatzen bada, muga hori urratu daiteke. Hori dela eta, beharrezkoa da dimentsioa desaktibatu aurretik dimentsio-balio hori beteta duten **Funtzio-prezioa** eta **Funtzio-prezioaren gainprezioa** errenkada guztiak ezabatzea.
