---
title: Projektuetan oinarritutako abagunearen lerroak
description: Gai honek proiektuan oinarritutako abagune-lerroekin lan egiteari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 91c53c917846a2b4e4fd64c14bb91782e9d05d66
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5277638"
---
# <a name="project-based-opportunity-lines"></a>Projektuetan oinarritutako abagunearen lerroak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_


Proiektuetan oinarritutako aukera lerroak proiektuetan oinarritutako aukeretan soilik daude eskuragarri. Proiektuan oinarritutako abagune-erregistroek **Mota** eremuaren balioa ezarrita dago **Lanean oinarrituta** .

Proiektuetan oinarritutako aukera-lerroak proiektuaren bidez bezeroari entregatuko zaizkion elementuak dira. Hala ere, proiektu bat ezin da proiektuan oinarritutako aukera lerro batekin lotu. Proiektuak lineako elementuekin lotu daitezke **Eskaintza** fasetik aurrera, normalean aukera tratu baten hasieran gertatzen delako. Bezeroari lana emateko zenbat proiektu erabiliko diren zehaztea salmenta fasean gerora hartzen den erabakia da. Erabili abagunea fasea bezeroarentzako entrega osagai diskretuak identifikatzeko. Osagai horiek emateko erabilitako proiektu kopuruaren inguruko erabakiak kanpora bota daitezke, lanari berari buruzko informazio gehiago jakin arte.

Jarraian proiektuan oinarritutako aukera lerro bateko eremuak daude:

| **Eremua** | **Kokalekua** | **Azalpena** | **Downstream eragina** |
| --- | --- | --- | --- |
| Produktu mota | Fitxa orokorra (ezkutatuta) | Aukera multzo eremu bat da. Dynamics 365 Operations instalatuta baduzu, eskuragarri dauden aukeretako bat hau da, **Proiektuetan oinarritutako zerbitzua**.  | Eremu honen balioa ezarrita dago **Proiektuetan oinarritutako zerbitzua** proiektuan oinarritutako aukera-lerroa Aukeran Aukeran proiektuan oinarritutako lerroen saretik sortzen duzunean. <br> Balio hau aldatzen edo gainidazten baduzu, proiektuaren funtzionalitatea ez da gaituko proiektuan oinarritutako lineako elementuetan. |
| Abagunea | Fitxa orokorra | Eremu hau irakurtzeko soilik da eta lerro-elementu honi dagokion Abagunea erregistro nagusia aipatzen du. | Ez dago alor honen beherako eraginik. |
| Izena | Fitxa orokorra | Lerro-elementu honi identitate laburra emateko erabil daitekeen testu-eremu editagarria da | Balio hau aurrekontuaren marrara eramaten da aukera honetatik aurrekontua sortzen duzunean |
| Bezeroaren aurrekontua | Fitxa orokorra | Moneta-eremu editagarri hau bezeroak lerro-elementu honetarako gastatzeko prest dagoen zenbatekoaren jarraipena egiteko erabil daiteke. | Balio hau eskintzako dagokion eremura eramaten da aukera honetatik aurrekontua sortzen duzunean |
| Fakturazio-metodoa | Fitxa orokorra | Eremu editagarriak balio hauek ditu:</br>- Denbora eta materiala</br>- Prezio finkoa | Balio hau eskintzako dagokion eremura eramaten da aukera honetatik aurrekontua sortzen duzunean. Aurrekontuaren lerroa sortu ondoren, eremua blokeatuta dago eta ezin da aldatu. Esleitu eremuaren balioa ahalik eta zehatzen. Eremu honen balioa aurrekontuaren lerroan aldatu behar baduzu, ezabatu eta berriro sortu aurrekontua. |


[!INCLUDE[footer-include](../includes/footer-banner.md)]