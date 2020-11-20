---
title: Produktuetan oinarritutako eskaintzaren lerroak
description: Gai honek eskaintza eta produktuetan oinarritutako lerroei buruzko informazioa ematen du.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/06/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 9c3b2b35abe894e79d6f55a7ddd6e5c64d0f12f2
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4123183"
---
# <a name="product-based-quote-lines"></a>Produktuetan oinarritutako eskaintzaren lerroak

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]


Produktuetan oinarritutako aurrekontu lerroak sor ditzakezu Dynamics 365 Project Service Automation-en. Produktuen araberako aurrekontu-ildoak "idazteko" lerroak izan daitezke, edo produktuen katalogoko elementuak izan daitezke.

## <a name="product-catalog"></a>Produktuen katalogoa

Dynamics 365 produktuen katalogoko produktuek unitate eta unitate multzo lehenetsiak dituzte. Hainbat produktuk atributu multzo bera partekatzen badute, ezaugarri horiek ere badituen produktuen familia sor dezakezu. Produktu familia bateko produktu guztiek ezaugarri berdinak heredatzen dituzte.

Adibidez, enpresa batek harpidetzako lizentziak saltzen ditu software askotarako. Harpidetza software guztiek bi atributu hauek dituzte:

- Erabiltzaile kopurua 
- Harpidetzaren iraupena (hilabeteetan)

Katalogo mota hau mantentzeko modu ona da izena duen produktu familia sortzea **Harpidetza softwarea**, eta horrek badu **Erabiltzaile kopurua** eta **Harpidetzaren iraupena** atributu gisa. Ondoren, produktu indibidualak gehi ditzakezu, adibidez **Dynamics 365 Sales** edo **Dynamics 365 Field Service** aplikazioak **Harpidetza software** familia produktura.

## <a name="adding-product-catalog-items-to-a-project-quote"></a>Produktuen katalogoko elementuak proiektuaren aurrekontuan gehitzea

Proiektuen eskaintza eta proiektuaren kontratu orriek bi lerro mota dituzte ataletan: proiektuan oinarritutako ildoak eta produktuetan oinarritutako lineak. Produktuetan oinarritutako ildoetarako, Dynamics 365 erabiltzen da produktuen katalogoko elementuak eskaintza batean gehitzeko. Eskaintzen edo proiektuaren kontratuaren lerroko goitibeherako zerrendak aurrekontuari edo proiektuaren kontratuei atxikitako produktuen prezio-zerrendako unitate eta unitate guztiak barne hartzen ditu. Eskaintzen produktu-zerrendako zati ez diren produktuak ere gehi ditzakezu.

Gainera, produktuak beste prezio-zerrendetatik hauta ditzakezu edo produktuak zuzenean katalogotik hauta ditzakezu. Produktuak katalogo batetik zuzenean hautatzen dituzunean, produktu horren prezioen zerrenda lehenetsia erabiltzen da produktuaren salmenta prezioa lortzeko. Lehenetsitako prezioen zerrenda zehazten ez bada, prezioa 0 (zero) izango da.

Aurrekontu-lerro bat produktuen katalogoan oinarrituta badago, salmenta-prezioa zuzenean alda dezakezu aurrekontuen lerroan. Kontuan izan Dynamics 365-en aurrekontu-lerroak baduela **Prezioak** eremua. Bi balio daude:

- Gainidatzi prezioa  
- Erabili balio lehenetsiak

Eremu hau ezarrita baduzu **Gainidatzi prezioa**, Dynamics 365-ek ez du prezio lehenetsirik zehazten. Produktuaren prezioa sartu behar duzu aurrekontuen lerroan. Eremu hau ezarrita baduzu **Erabili lehenetsia**, Dynamics 365-ek salmenta-prezio lehenetsia erabiltzen du eta eremua blokeatzen du edizioa ekiditeko.

PSA instalatu ondoren, salmenta prezio lehenetsiak produktuaren araberako lerroetan sartzen dira aurrekontu batean. **Prezioa** eremua, eremuan ezarri behar da **Gainidatzi prezioak** eskaintzaren lerroetan prezio lehenetsia editatu ahal izateko.

> ![Ezarri fakturaren prezioak](media/basic-guide-10.png)
 
## <a name="quantity-factors-for-products"></a>Produktuen kantitate faktoreak

PSAk kantitate faktoreak erabiltzen ditu harpidedun oinarritutako produktuen salmenta sustatzeko. Harpidetzetan oinarritutako produktuetarako, aurrekontuan edo proiektuaren kontratuaren lerroan erabiltzaile-hilabete kopurua adierazten da.

Normalean, harpidedun softwarearen prezioa katalogoan gordetzen da erabiltzaile bakoitzeko prezio gisa. Hala ere, beste denbora deskribapen batzuk erabil ditzakezu. Salmenta prozesuan, aurrekontuen lerroko prezioa erabiltzaile bakoitzeko, salmentako IT agentearen bidez negoziatu eta deskontatu zen hileko prezioa izan ohi da. Akordio bakoitzak erabiltzaile kopurua eta harpidetza hilabete desberdinak ditu. Aurrekontuen lerroaren zenbatekoa kalkulatzeko erabiltzen den kantitatea erabiltzaile kopurua eta harpidetza hilabeteen produktua da.

Salmenta mota hori onartzeko, PSAk kantitate faktoreen kontzeptua sartu zuen. Kopuru-faktoreek produktuaren atributuetan oinarritzen dira Dynamics 365-en. Produktu baterako propietate espezifikoak konfiguratzen dituzunean, PSAk propietate horien edo propietate guztien azpimultzoa uzten dizu kantitate faktore gisa.

PSAk balioztatzen du zenbakizko datu mota bat duten zenbakizko propietateak edo produktuaren propietateak kantitate faktore gisa markatzen direla. Kantitate-faktoreak konfiguratutako produktu bat aurrekontu-lerrora gehitzen denean, **Kopurua** aurrekontuen lerroan irakurtzeko soilik eremu bihurtzen da. Kantitate faktoreak diren produktuaren propietateen balioak sartu ondoren, PSAk aurrekontuen lerroaren kantitatea kalkulatzen du.

Adibidez, Dynamics 365-ek propietate hauek izan ditzake: 

- **Erabiltzaile kop**: erabiltzaile kopurua 
- **Hilabete kop**: harpidetza-hilabete kopurua
- **SKU produktua** 

**Erabiltzaile kop** eta **Hilabete kop** propietateak kantitate faktore gisa markatu daitezke produktuaren lerroko propietateak editatzean. 

> ![Erabiltzaileen kopurua eta hilabete kopurua ez izatea kalitate faktore gisa](media/basic-guide-11.png)
 
