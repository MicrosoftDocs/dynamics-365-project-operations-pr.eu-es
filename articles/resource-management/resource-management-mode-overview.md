---
title: Baliabideen kudeaketaren moduen informazio orokorra
description: Artikulu honetan, baliabideen administrazioaren funtzionaltasunari buruzko informazioa ematen da Dynamics 365 Project Operations.
author: ruhercul
ms.date: 10/01/2020
ms.topic: overview
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: dd50d12686a6ad17f6a95ccf0c2f1447cc470bf7
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8928417"
---
# <a name="resource-management-modes-overview"></a>Baliabideen kudeaketaren moduen informazio orokorra

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_


Dynamics 365 Project Operations-ek bi modu onartzen ditu erreserba-fluxu orokorra exekutatu ahal izateko. Kudeaketa modua proiektuaren parametro gisa definitzen da eta zure negozioa aldatu behar bada alda daiteke.    

## <a name="central-mode"></a>Modu zentrala
Proiektuetarako baliabideen zuzkidura zentralizatzen duten erakundeentzat, Modu Zentralak proiektuaren kudeatzaileek proiektuaren mailan baliabideen eskakizunak definitu ahal izateko modua eskaintzen du. Baliabideen eskakizunak betetzea Baliabideen kudeatzaileari eskuordetzen zaio. Proiektuen kudeatzaileek baliabideen kudeatzaileak proposatutako baliabideak onartu edo baztertu ditzakete.

![Modu zentrala.](./media/resource-management-central.png)

Baliabideak Erdiko moduarekin kudeatzeko, ikusi:

- [Esleitu baliabide erreserbagarri generikoak zeregin bati eta sortu baliabide-eskakizunak](/dynamics365/project-service/assign-generic-bookable-resource)
- [Erreserbatu izena duten baliabideak baliabide-eskakizunetatik](/dynamics365/project-service/book-named-resource)
- [Bidali baliabide-eskaera bat](/dynamics365/project-service/submit-resource-request)
- [Bete baliabide-eskaera](/dynamics365/project-service/resource-management-fulfill-requests)
- [Onartu edo baztertu proposatutako proiektuaren baliabidea baliabide-eskaera batetik](/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a>Modu hibridoa
Baliabideen banaketan malgutasuna behar duten erakundeentzat, modu hibridoak proiektuen kudeatzaileei eta baliabideen kudeatzaileei baliabideak erreserbatzeko aukera ematen die.

![Modu hibridoa.](./media/resource-management-hybrid.png)

Prozesu zentral onartuaz gain, kontsultatu artikulu hauek, hibridoan onartutako gainerako erreserba-fluxu guztiak administratzeko:

Erreserbatu baliabide bat zuzenean proiektu bati:
- [Erreserbatu baliabide erreserbagarriak proiektuko talde bati eta esleitu zereginak](/dynamics365/project-service/assign-named-bookable-resource)

Erreserbatu baliabide bat baliabide-eskakizunetatik:
- [Esleitu baliabide erreserbagarri generikoak zeregin bati eta sortu baliabide-eskakizunak](/dynamics365/project-service/assign-generic-bookable-resource)
- [Erreserbatu izena duten baliabideak baliabide-eskakizunetatik](/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]