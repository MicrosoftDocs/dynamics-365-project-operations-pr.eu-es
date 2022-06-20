---
title: Project Service Automation eguneratzearen 16, V3 bertsioko berrikuntzak edo aldaketak
description: Artikulu honek Project Service Automation Update Release 16, V3-n eskuragarri dauden funtzioak eta konponketak zerrendatzen ditu.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/18/2020
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
ms.reviewer: johnmichalak
ms.openlocfilehash: e4429ace3d8206369b91917cf87f6968fbb12277
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8926485"
---
# <a name="project-service-automation-update-release-16-v3"></a>Project Service Automation 16, V3 eguneratze-bertsioa

[!include [banner](../includes/psa-now-project-operations.md)]

Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.  Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu soluzio hobetsi bat](/dynamics365/project-service/upgrade-psa-home-page).
Artikulu honek PSA V3, 16. bertsioaren eguneraketa berria edo aldatu diren ezaugarriak eta konponketak zerrendatzen ditu. Bertsio honek V3.10.6.34 konpilazio-zenbakia du eta, oro har, 2020ko urtarrilean jarriko da erabilgarri automatikoki eguneratzeko moduan.


## <a name="update-release-16"></a>16. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

-   Denbora eta gastua

    -   Konponduta: ezabatutako denboraren eta gastuen sarrerak onartzeko bidaltzen saiatzen diren erabiltzaileek errore-mezuak jasoko dituzte.

-   Proiektuen kudeaketa

    -   Konponduta: txantiloietan taldekideek zehaztutako resourcing unitateak txantiloiak proiektu berri bati aplikatzen zaizkio.

    -   Konponduta: Erregistroen jabetza berriro esleitzea hobeto kudeatzea.

    -   Konponduta: kopia prozesuan dauden proiektuei ezin zaie kopiatu baimendu operazio guztiak amaitu arte.

-   Baliabideen kudeaketa

    -   Konponduta: Luzatu erreserbak orain arteko iraupen laburrak behar bezala kudeatzen ditu eta ez du zero ordu sortzen erreserba luzatuetarako.

    -   Konponduta: bateratze ikuspegia proiektuaren ordu-eremua +5:30 GMT denean eta erabiltzailearen denbora bakar bat desberdina denean ematen da.

-   Sales

    -   Konponduta: proiektu bat kontratatu lerrora kendutakoan eta proiektu berri bat mapatzen denean, proiektu berriaren benetako erregistroak ez ziren berriro ebaluatu kontratuaren lerroan zehaztutako fakturazio- eta prezio-arauen arabera. Hori konpondu da bertsio honetan. Mapatu berri den proiektuaren prezioak eta benetako erregistroak behar bezala berraztertu eta berriro sortuko dira, kontratuaren lerroko prezio eta fakturazio arauetan oinarrituta. Mapatu gabeko proiektuaren benetako erregistroak berriro ebaluatu eta berriro sortuko dira.

    -   Konponduta: balioztapen gehigarria gehitu zaio estimazio lerroari **Zenbatekoa** eremua balio nuluak ez direla irauten ziurtatzeko.

    -   Konponduta: proiektuak eguneratu direnean, freskatze botoia gehitu da proiektuaren formulario nagusian, erabiltzaileak berriak sinkronizatu ahal izateko.

    -   Konponduta: erabiltzaileak 2.X bertsiotik 3.X bertsiora berritzen dutenean, proiektuaren NULL balioa duten proiektuak baimenduko dira.



[!INCLUDE[footer-include](../includes/footer-banner.md)]
