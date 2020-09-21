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
ms.prod: ''
ms.technology: ''
ms.assetid: eb5ab6a1-fdff-490e-9c2a-19aef493de11
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 4431c1c894a01bfecc132575d8981ebc9fe50b51
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748843"
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
