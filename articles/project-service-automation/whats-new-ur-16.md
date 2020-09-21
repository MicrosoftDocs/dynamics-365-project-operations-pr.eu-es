---
title: Project Service Automation eguneratzea 16, V3 bertsioari buruzko berritasunak
description: Gai honek Project Service Automation V3, 16. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: business-applications
ms.custom: dyn365-projectservice
ms.date: 02/18/2020
ms.topic: article
ms.prod: ''
ms.technology: Microsoft Dynamics 365 Project Service Automation 3.x
ms.assetid: b890a7b6-1664-4812-8732-fed77653cc05
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 0f4c206fd5b7a36d940e966b28c2437525812a98
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748861"
---
# <a name="project-service-automation-v3-update-release-16"></a>Project Service Automation V3, eguneratzea 16
Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.

Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu soluzio hobetsi bat](https://docs.microsoft.com/dynamics365/project-service/upgrade-psa-home-page). Gai honek PSA V3, 16. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honek V3.10.6.34 konpilazio-zenbakia du eta, oro har, 2020ko urtarrilean jarriko da erabilgarri automatikoki eguneratzeko moduan

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

