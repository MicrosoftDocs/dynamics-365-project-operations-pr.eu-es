---
title: Baliabide-kudeaketaren moduen informazio orokorra
description: Gai honek Baliabide kudeaketa funtzioari buruzko informazioa eskaintzen du Dynamics 365 Project Operations-en.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 4a8e605109e48b50da68abeee989f8ac8d3d659c
ms.sourcegitcommit: cf79185c8c84c55fbae55f9cfc1b17840e072b49
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/01/2020
ms.locfileid: "3930076"
---
# <a name="resource-management-modes-overview"></a>Baliabide-kudeaketaren moduen informazio orokorra

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_


Dynamics 365 Project Operations-ek bi modu onartzen ditu erreserba-fluxu orokorra exekutatu ahal izateko. Kudeaketa modua proiektuaren parametro gisa definitzen da eta zure negozioa aldatu behar bada alda daiteke.    

## <a name="central-mode"></a>Modu zentrala
Proiektuetarako baliabideen zuzkidura zentralizatzen duten erakundeentzat, Modu Zentralak proiektuaren kudeatzaileek proiektuaren mailan baliabideen eskakizunak definitu ahal izateko modua eskaintzen du. Baliabideen eskakizunak betetzea Baliabideen kudeatzaileari eskuordetzen zaio. Proiektuen kudeatzaileek baliabideen kudeatzaileak proposatutako baliabideak onartu edo baztertu ditzakete.

![Modu zentrala](./media/resource-management-central.png)

Baliabideak Erdiko moduarekin kudeatzeko, ikusi:

- [Esleitu baliabide erreserbagarri generikoak zeregin bati eta sortu baliabide-eskakizunak](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [Erreserbatu izena duten baliabideak baliabide-eskakizunetatik](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
- [Bidali baliabide-eskaera bat](https://docs.microsoft.com/dynamics365/project-service/submit-resource-request)
- [Bete baliabide-eskaera](https://docs.microsoft.com/dynamics365/project-service/resource-management-fulfill-requests)
- [Onartu edo baztertu proposatutako proiektuaren baliabidea baliabide-eskaera batetik](https://docs.microsoft.com/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a>Modu hibridoa
Baliabideen banaketan malgutasuna behar duten erakundeentzat, modu hibridoak proiektuen kudeatzaileei eta baliabideen kudeatzaileei baliabideak erreserbatzeko aukera ematen die.

![Modu hibridoa](./media/resource-management-hybrid.png)

Onartutako Erdiko moduaren prozesua ez ezik, ikusi gai hauek Hibrido moduan onartutako erreserba-fluxu guztiak kudeatzeko:

Erreserbatu baliabide bat zuzenean proiektu bati:
- [Erreserbatu baliabide erreserbagarriak proiektuko talde bati eta esleitu zereginak](https://docs.microsoft.com/dynamics365/project-service/assign-named-bookable-resource)

Erreserbatu baliabide bat baliabide-eskakizunetatik:
- [Esleitu baliabide erreserbagarri generikoak zeregin bati eta sortu baliabide-eskakizunak](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [Erreserbatu izena duten baliabideak baliabide-eskakizunetatik](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
