---
title: Desaktibatu prezio-dimentsioa
description: Gai honek prezio-dimentsioak Project Service soluzioan nola ezarri erakusten du.
author: Rumant
ms.custom:
- dyn365-projectservice
ms.date: 11/06/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: f308104246efe671d2001e660aa8c0ab9ef44c7a
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8581683"
---
# <a name="turn-off-a-pricing-dimension"></a>Desaktibatu prezio-dimentsioa

[!include [banner](../includes/psa-now-project-operations.md)]

Baliteke prezioen estrategia berrikusi eta eguneratu behar izatea zenbait urtean behin. Egin ditzakezun eguneratzeek lehendik dagoen prezio-dimentsioa desaktibatzea eta berri bat sortzea eska dezakete. Adibidez, baliteke aurrez prezioa **Funtzioa** aukerare arabera jarrita izatean, baina orain prezioa **Lan esperientzia** aukeraren arabera jartzea erabaki duzu. Horrek **Funtzioa** prezio-dimentsio gisa desaktibatzea eta pezio-dimentsio berri gisa **Lanaren esperientzia** sortzea eska diezazuke. 

Prezio-dimentsio bat desaktibatzeko, aurretiaz prestatutakoa edo pertsonalizatua den kontuan izan gabe, ezarri prezio-dimentsioaren **Kostuari aplikagarria** eta **Salmentei aplikagarria** eremuak **Ez** gisa.

Hala ere, hau egiten duzunean, errore-mezu hau jaso dezakezu.

![Prezio-dimentsio bat desaktibatzean ager daitekeen negozio-prozesuaren errorea.](media/Business-Process-Error.png)


Errore-mezu horrek desaktibatu nahi den dimentsiorako aurrez konfiguratutako prezioen erregistroak daudela adierazten du. Dimentsio bati erreferentzia egiten dioten **Funtzio-prezioa** eta **Funtzio-prezioaren gainprezioa** erregistro guztiak ezabatu egin behar dira dimentsioaren aplikagarritasuna **Ez** gisa ezarri ahal izateko. Arau hori aurretiaz prestatutako prezio-dimentsioei eta sortu ditzakezun prezio-dimentsio pertsonalizatuei aplikatzen zaie. Balidazio horren arrazoia Project Service-k **Funtzio-prezioa** erregistro bakoitzak dimentsioen konbinazio esklusiboa izan behar duela zehaztu duela da. Adibidez, **2018ko AEBetako kostu-tasak** izeneko prezio-zerrendan, honako **Funtzio-prezio** errenkada hauek dituzu. 

| Titulu estandarra         | Erakunde-unitatea    |Unitatea   |Prezioa  |Moneta  |
| -----------------------|-------------|-------|-------|----------|
| Sistemen ingeniaria|Contoso US|Hour| 100|USD|
| Sistemen ingeniari nagusia|Contoso US|Hour| 150| USD|


**Titulu estandarra** prezio-dimentsio gisa desaktibatzen duzunean eta Project Service-ren prezioen motorrak prezioa bilatzen duenean, sarrerako testuinguruko **Erakunde-unitatea** balioa soilik erabiliko du. Sarrerako testuinguruaren **Erakunde-unitatea** "Contoso US" bada, emaitza ez-determinista izango da bi errenkadak bat etorriko direlako. Egoera hori ekiditeko, **Funtzio-prezioa** erregistroak sortzen dituzunean, Project Service-k dimentsioen konbinazioa esklusiboa dela balioztatzen du. Dimentsioa **Funtzio-prezioa** erregistroak sortu ondoren desaktibatzen bada, muga hori urratu daiteke. Hori dela eta, beharrezkoa da dimentsioa desaktibatu aurretik dimentsio-balio hori beteta duten **Funtzio-prezioa** eta **Funtzio-prezioaren gainprezioa** errenkada guztiak ezabatzea.



[!INCLUDE[footer-include](../includes/footer-banner.md)]
