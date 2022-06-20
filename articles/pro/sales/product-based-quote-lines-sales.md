---
title: Produktuetan oinarritutako eskaintzaren lerroen ikuspegi orokorra - arina
description: Artikulu honek produktuetan oinarritutako aurrekontu-lerroekin lan egiteari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 10/30/2020
ms.topic: overview
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: db0700e789202a8fdd0ef3b49959421ac54fb9ad
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8914295"
---
# <a name="product-based-quote-lines-overview---lite"></a>Produktuetan oinarritutako eskaintzaren lerroen ikuspegi orokorra - arina

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Produktuetan oinarritutako aurrekontu lerroak sor ditzakezu Dynamics 365 Project Operations-en. Produktuen araberako aurrekontu-ildoak eskuz gehi daitezke, edo produktuen katalogoko elementuak izan daitezke.

## <a name="product-catalog"></a>Produktuen katalogoa

Produktuen katalogoko produktu bakoitzak unitate eta unitate multzo lehenetsiak ditu. Hainbat produktuk atributu multzo bera partekatzen badute, ezaugarri horiek ere badituen produktuen familia sor dezakezu. 

Adibidez, enpresa batek harpidetzako lizentziak saltzen ditu software askotarako. Harpidetza software guztiek bi atributu hauek dituzte:

- Erabiltzaile kopurua
- Harpidetzaren iraupena hilabeteetan neurtuta

Katalogo mota hau mantentzeko izena duen produktu familia sortzea **Harpidetza softwarea**, eta horrek badu erabiltzaile kopurua eta harpidetzaren iraupena atributu gisa gehitzeko. Ondoren, produktu indibidualak gehi ditzakezu **Harpidetza softwarea** produktuen familia.

## <a name="add-product-catalog-items-to-a-project-quote"></a>Gehitu produktuen katalogoko elementuak proiektuaren aurrekontuan

**Proiektuen eskaintza** eta **Proiektuaren kontratua** orriek atalak dituzte proiektuan oinarritutako ildoak eta produktuetan oinarritutako lineak. Produktuetan oinarritutako lerroetarako, eskaintzen edo proiektuaren kontratuaren lerroko goitibeherako zerrendak prezio-zerrendako unitate eta unitate guztiak barne hartzen ditu. Produktu-zerrendako zati ez diren produktuak ere gehi ditzakezu.

Gainera, produktuak beste prezio-zerrendetatik hauta ditzakezu edo zuzenean katalogotik hauta ditzakezu. Produktuak katalogo batetik zuzenean hautatzen dituzunean, produktu horren prezioen zerrenda lehenetsia erabiltzen da produktuaren salmenta prezioa lortzeko. Lehenetsitako prezioen zerrenda zehazten ez bada, prezioa (0) izango da.

Aurrekontu-lerro bat produktuen katalogoan oinarrituta badago, salmenta-prezioa zuzenean alda dezakezu aurrekontuen lerroan. Aurrekontuaren lerroa **Prezioak** bi balio erabilgarri dituen eremua:

- **Gainidatzi prezioa**
- **Erabili lehenetsia**

Hautatzen baduzu **Gainidatzi prezioak**, lehenetsitako prezioa ez dago ezarrita. Edo, produktuaren prezioa sartu behar duzu aurrekontuen lerroan. Hautatzen baduzu **Erabili lehenetsia**, salmenta prezio lehenetsia erabiltzen da eta eremua blokeatuta dago editatzeko.

Salmenta prezio lehenetsiak produktuaren araberako lerroetan sartzen dira aurrekontu batean. **Prezioa** eremua, eremuan ezarri behar da **Gainidatzi prezioak** eskaintzaren lerroetan prezio lehenetsia editatu ahal izateko. Hau da, Dynamics 365 Sales-en produktuan oinarritutako lerroen portaeraren gaineko Project Operations-en berariazko gainidazketa.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]