---
title: Proiektuetan oinarritutako abagunearen lerroak - arina
description: Gai honek proiektuan oinarritutako abagune-lerroei buruzko informazioa eskaintzen du. (Pro)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: bba555003b76e3e87412679b274f74f68ac7203b
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/31/2020
ms.locfileid: "4180987"
---
# <a name="project-based-opportunity-lines---lite"></a>Proiektuetan oinarritutako abagunearen lerroak - arina

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proiektuetan oinarritutako aukera lerroak proiektuetan oinarritutako aukeretan soilik daude eskuragarri. Proiektuan oinarritutako abagune-erregistroek **Mota** eremuaren balioa ezarrita dago **Lanean oinarrituta** .

Proiektuetan oinarritutako aukera-lerroak proiektuaren bidez bezeroari entregatuko zaizkion elementuak dira. Hala ere, proiektu bat ezin da proiektuan oinarritutako aukera lerro batekin lotu. Proiektuak lineako elementuekin lotu daitezke **Eskaintza** fasean eta handik aurrera, normalean aukera tratu baten bizi-zikloaren hasieran gertatzen delako. Bezeroari lana emateko zenbat proiektu erabiliko diren zehaztea salmenta fasean gerora hartzen den erabakia da. Abagunea fasea erabil dezakezu bezeroarentzako entrega osagai diskretuak identifikatzeko. Osagai horiek emateko erabilitako proiektu kopuruaren inguruko erabakiak kanpora bota daitezke, lanari berari buruzko informazio gehiago jakin arte.

Jarraian proiektuan oinarritutako aukera lerro bateko eremuak daude:

| **Eremua** | **Kokalekua** | **Azalpena** | **Downstream eragina** |
| --- | --- | --- | --- |
| Produktu mota | Fitxa orokorra (ezkutatuta) | Aukera hauetako hauta dezakezu:</br>- Proiektuetan oinarrituako zerbitzua (Dynamics 365 Project Operations instalatuta baduzu soilik)</br>- Produktua (Project Operations eta Dynamics 365 Sales instalatuta badituzu soilik) | Eremu honen balioa ezarrita dago **Proiektuetan oinarritutako zerbitzua** proiektuan oinarritutako aukera-lerroa Aukeran Aukeran proiektuan oinarritutako lerroen saretik sortzen duzunean. <br> Balio hau aldatzen edo gainidazten baduzu, proiektuaren funtzionalitatea ez da gaituko proiektuan oinarritutako lineako elementuetan. |
| Abagunea | Fitxa orokorra | Eremu hau irakurtzeko soilik da eta lerro-elementu honi dagokion Abagunea erregistro nagusia aipatzen du. | Ez dago alor honen beherako eraginik. |
| Izena | Fitxa orokorra | Lerro-elementua identitate laburra emateko erabil daitekeen testu-eremu editagarria da. | Balio hau aurrekontuaren marrara eramaten da aukera honetatik aurrekontua sortzen duzunean. |
| Bezeroaren aurrekontua | Fitxa orokorra | Moneta-eremu editagarri hau bezeroak lerro-elementu honetarako gastatzeko prest dagoen zenbatekoaren jarraipena egiteko erabil daiteke. | Balio hau eskintzako dagokion eremura eramaten da aukera honetatik aurrekontua sortzen duzunean. |
| Fakturazio-metodoa | Fitxa orokorra | Eremu editagarriak balio hauek ditu:</br>- Denbora eta materiala</br>- Prezio finkoa | Balio hau eskintzako dagokion eremura eramaten da aukera honetatik aurrekontua sortzen duzunean. Aurrekontuaren lerroa sortu ondoren, eremua blokeatuta dago eta ezin da aldatu. Esleitu eremuaren balioa ahalik eta zehatzen. Eremu honen balioa aurrekontuaren lerroan aldatu behar baduzu, ezabatu eta berriro sortu aurrekontua. |
