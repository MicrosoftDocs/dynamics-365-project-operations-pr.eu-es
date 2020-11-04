---
title: Projektuetan oinarritutako abagunearen lerroak
description: Gai honek proiektuan oinarritutako abagune-lerroekin lan egiteari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 7b255d607ac8180c249a9b9831db6f8d0cd3937b
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070897"
---
# <a name="project-based-opportunity-lines"></a>Projektuetan oinarritutako abagunearen lerroak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_


Proiektuetan oinarritutako aukera lerroak proiektuetan oinarritutako aukeretan soilik daude eskuragarri. Proiektuan oinarritutako abagune-erregistroek **Mota** eremuaren balioa ezarrita dago **Lanean oinarrituta** .

Proiektuetan oinarritutako aukera-lerroak proiektuaren bidez bezeroari entregatuko zaizkion elementuak dira. Hala ere, proiektu bat ezin da proiektuan oinarritutako aukera lerro batekin lotu. Proiektuak lineako elementuekin lotu daitezke **Eskaintza** fasetik aurrera, normalean aukera tratu baten hasieran gertatzen delako. Bezeroari lana emateko zenbat proiektu erabiliko diren zehaztea salmenta fasean gerora hartzen den erabakia da. Erabili abagunea fasea bezeroarentzako entrega osagai diskretuak identifikatzeko. Osagai horiek emateko erabilitako proiektu kopuruaren inguruko erabakiak kanpora bota daitezke, lanari berari buruzko informazio gehiago jakin arte.

Jarraian proiektuan oinarritutako aukera lerro bateko eremuak daude:

| **Eremua** | **Kokalekua** | **Garrantzia, xedea eta orientazioa** | **Downstream eragina** |
| --- | --- | --- | --- |
| Produktu mota | Fitxa orokorra (ezkutatuta) | Aukera multzo eremu bat da. Dynamics 365 Operations instalatuta baduzu, eskuragarri dauden aukeretako bat hau da, **Proiektuetan oinarritutako zerbitzua**.  | Eremu honen balioa ezarrita dago **Proiektuetan oinarritutako zerbitzua** proiektuan oinarritutako aukera-lerroa Aukeran Aukeran proiektuan oinarritutako lerroen saretik sortzen duzunean. <br> Balio hau aldatzen edo gainidazten baduzu, proiektuaren funtzionalitatea ez da gaituko proiektuan oinarritutako lineako elementuetan. |
| Abagunea | Fitxa orokorra | Eremu hau irakurtzeko soilik da eta lerro-elementu honi dagokion Abagunea erregistro nagusia aipatzen du. | Ez dago alor honen beherako eraginik. |
| Izena | Fitxa orokorra | Lerro-elementu honi identitate laburra emateko erabil daitekeen testu-eremu editagarria da | Balio hau aurrekontuaren marrara eramaten da aukera honetatik aurrekontua sortzen duzunean |
| Bezeroaren aurrekontua | Fitxa orokorra | Moneta-eremu editagarri hau bezeroak lerro-elementu honetarako gastatzeko prest dagoen zenbatekoaren jarraipena egiteko erabil daiteke. | Balio hau eskintzako dagokion eremura eramaten da aukera honetatik aurrekontua sortzen duzunean |
| Fakturazio-metodoa | Fitxa orokorra | Eremu editagarriak balio hauek ditu:</br>- Denbora eta materiala</br>- Prezio finkoa | Balio hau eskintzako dagokion eremura eramaten da aukera honetatik aurrekontua sortzen duzunean. Aurrekontuaren lerroa sortu ondoren, eremua blokeatuta dago eta ezin da aldatu. Esleitu eremuaren balioa ahalik eta zehatzen. Eremu honen balioa aurrekontuaren lerroan aldatu behar baduzu, ezabatu eta berriro sortu aurrekontua. |
