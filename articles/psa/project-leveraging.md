---
title: Salmenten aurreikuspenak eta proiektuak
description: Gai honek salmenta prozesuko antolaketa eta aurreikuspenak aprobetxatzeari buruzko informazioa eskaintzen du.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: eafe60362003198a223026526f56261de414bb4a
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071054"
---
# <a name="sales-estimates-and-projects"></a>Salmenten aurreikuspenak eta proiektuak

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Salmenta prozesuan zehar, salmenten aurreikuspenak sor ditzakezu proiektu bat salmenta-eskaintzari lotuz. Horrela, salmenta prozesuan aurreikuspen determinista gerta daiteke proiektuen antolaketa eta aurreikuspen gaitasunak aprobetxatzeko. Salmentak aurrera egiten badu, salmenten aurreikuspena egiteko erabilitako antolaketa erabil daiteke proiektuaren plana berriro finkatzeko oinarri gisa.

## <a name="linking-a-project-to-a-quote-line"></a>Estekatu proiektua eskaintzaren lerro bati

Proiektuetan oinarritutako eskaintzaren lerroa sortzen duzunean, beste proiektu bat sor dezakezu edo lehendik dagoen proiektu batekin lotu **Eskaintzaren lerroa** orrian. 

> ![Eskaintzaren lerroaren inprimakia](media/project-8.png)
 
Eskaintzaren lerroko xehetasunetatik abiatuta beste proiektu bat sortzen duzunean, proiektuaren txantiloiak aprobetxatu ditzakezu. Proiektuaren txantiloiak erakunde baten proiektu tipikoen planak eta finantza-aurreikuspenak adierazten dituzten proiektu ereduak dira. Aurreko proiektuetako proiektu-planen eta aurreikuspenen kopiak ere irudikatu ahal izango dituzte.

> ![Eskaintzaren lerroaren xehetasunak](media/project-9.png)
  
Proiektu bat eskaintza batetik sortzean, proiektua automatikoki lotuko da eskaintzaren lerroarekin.

## <a name="components-of-estimates-in-a-project"></a>Proiektu bateko aurreikuspenen osagaiak

Antolaketak lana zereginetan banatzen, zereginen hierarkia mantentzen, zereginak burutzeko zer baliabide behar diren zehazten eta zeregin bat burutzeko behar den ahaleginaren aurreikuspena esleitzen laguntzen dizu.

Laneko ahalegina eta antolaketaren aurreikuspenak zehaztu ditzakezu **Antolaketa** fitxako eremuak erabiliz **Proiektua** orrian. Prezio-zerrenda bat proiektuarekin lotuta dagoenez, finantza-aurreikuspenak kalkulatzen dira prezioen zerrendan zehazten diren kostu eta salmenta prezioak erabiliz.

## <a name="importing-estimates-from-a-project-into-a-quote"></a>Inportatu aurreikuspenak proiektu batetik eskaintza batera

Proiektuaren aurreikuspenak zehaztu ondoren, eskaintzaren lerrora inporta ditzakezu. **Eskaintzaren lerroaren xehetasunak** orrian, hautatu **Inportatu kalkuluetatik** aukera zintan proiektuaren aurreikuspenak laburbiltzeko transakzio mota, funtzioa edo zeregin mailaren arabera.
