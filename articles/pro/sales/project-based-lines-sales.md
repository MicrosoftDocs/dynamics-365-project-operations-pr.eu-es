---
title: Proiektuetan oinarritutako abagunearen lerroak - arina
description: Artikulu honetan proiektuetan oinarritutako aukera-ildoei buruzko informazioa ematen da. (Pro)
author: rumant
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 8b5a8fc32ca903d7da2e090137bed358b364902a
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8914249"
---
# <a name="project-based-opportunity-lines---lite"></a>Proiektuetan oinarritutako abagunearen lerroak - arina

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proiektuetan oinarritutako aukera lerroak proiektuetan oinarritutako aukeretan soilik daude eskuragarri. Proiektuan oinarritutako abagune-erregistroek **Mota** eremuaren balioa ezarrita dago **Lanean oinarrituta** .

Proiektuetan oinarritutako aukera-lerroak proiektuaren bidez bezeroari entregatuko zaizkion elementuak dira. Hala ere, proiektu bat ezin da proiektuan oinarritutako aukera lerro batekin lotu. Proiektuak lineako elementuekin lotu daitezke **Eskaintza** fasean eta handik aurrera, normalean aukera tratu baten bizi-zikloaren hasieran gertatzen delako. Bezeroari lana emateko zenbat proiektu erabiliko diren zehaztea salmenta fasean gerora hartzen den erabakia da. Abagunea fasea erabil dezakezu bezeroarentzako entrega osagai diskretuak identifikatzeko. Osagai horiek emateko erabilitako proiektu kopuruaren inguruko erabakiak kanpora bota daitezke, lanari berari buruzko informazio gehiago jakin arte.

Jarraian proiektuan oinarritutako aukera lerro bateko eremuak daude:

| **Eremua** | **Kokalekua** | **Azalpena** | **Downstream eragina** |
| --- | --- | --- | --- |
| Produktu mota | Fitxa orokorra (ezkutatuta) | Aukera hauetako hauta dezakezu:</br>- Proiektuetan oinarritutako zerbitzua (Dynamics 365 Project Operations instalatuta dagoenean soilik)</br>- Produktua (Project Operations eta Dynamics 365 Sales instalatuta badituzu soilik) | Eremu honen balioa ezarrita dago **Proiektuetan oinarritutako zerbitzua** proiektuan oinarritutako aukera-lerroa Aukeran Aukeran proiektuan oinarritutako lerroen saretik sortzen duzunean. <br> Balio hau aldatzen edo gainidazten baduzu, proiektuaren funtzionalitatea ez da gaituko proiektuan oinarritutako lineako elementuetan. |
| Abagunea | Fitxa orokorra | Eremu hau irakurtzeko soilik da eta lerro-elementu honi dagokion Abagunea erregistro nagusia aipatzen du. | Ez dago alor honen beherako eraginik. |
| Izena | Fitxa orokorra | Lerro-elementua identitate laburra emateko erabil daitekeen testu-eremu editagarria da. | Balio hau aurrekontuaren marrara eramaten da aukera honetatik aurrekontua sortzen duzunean. |
| Bezeroaren aurrekontua | Fitxa orokorra | Moneta-eremu editagarri hau bezeroak lerro-elementu honetarako gastatzeko prest dagoen zenbatekoaren jarraipena egiteko erabil daiteke. | Balio hau eskintzako dagokion eremura eramaten da aukera honetatik aurrekontua sortzen duzunean. |
| Fakturazio-metodoa | Fitxa orokorra | Eremu editagarriak balio hauek ditu:</br>- Denbora eta materiala</br>- Prezio finkoa | Balio hau eskintzako dagokion eremura eramaten da aukera honetatik aurrekontua sortzen duzunean. Aurrekontuaren lerroa sortu ondoren, eremua blokeatuta dago eta ezin da aldatu. Esleitu eremuaren balioa ahalik eta zehatzen. Eremu honen balioa aurrekontuaren lerroan aldatu behar baduzu, ezabatu eta berriro sortu aurrekontua. |


[!INCLUDE[footer-include](../../includes/footer-banner.md)]