---
title: Konfiguratu kilometrajea kilometrajearen tasaren mailak erabiliz
description: Artikulu honek kilometraje-tasei eta kilometraje-tasari buruzko informazioa eskaintzen du.
author: suvaidya
ms.date: 05/20/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: suvaidya
ms.openlocfilehash: 9689bbaf4c4f88ad9f746c3f98676f97e634ab6c
ms.sourcegitcommit: 5e1f549a2e55a87351b2979e3aff402ed35487e1
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/29/2022
ms.locfileid: "9064263"
---
# <a name="set-up-mileage-using-mileage-rate-tiers"></a>Konfiguratu kilometrajea kilometrajearen tasaren mailak erabiliz

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gastu bat jakinarazi eta hautatutako gastu kategoria denean **Kilometrajea**, gastu lerro horren zenbatekoa *kilometro bakoitzeko tasa* zenbatekoa. Zenbateko hori zehaztutako kilometrajearen mailak erabiliz zehazten da edo, kilometrajearen tasa mailak ez badira, kilometrajearen tasa estandarra jarraituz zehazten da. 

Kilometraje-tasaren mailak joanda joan daitezke **Gastuen kudeaketa** > **Konfigurazioa** > **Orokorra** > **Gastu kategoriak** > **Kilometrajea** > **Kategoria konfiguratzea** aukerara.

10.0.18 bertsioa berritu ondoren, zure erakundeak kilometrajearen gastuen kategoria erabiltzen badu, kontuan hartu kilometrajearen funtzioa gaitzea beheko diseinu aldaketak aztertu ondoren. 

Kilometraje-tasen diseinu berriak eragina du **Kopurua** eremua prozesatu da. 18.08.18 argitaratu baino lehen, balioa **Kopurua** eremua beheko mugatzat jotzen zen. Metaketak balio hori gainditu zuenean, dagokion tasa erabili zen.  10.0.18tik aurrera, balioa **Kopurua** eremua goiko mugatzat jotzen da. Dagokion tasa erabiltzen da kilometrajea metatzean balioa baino txikiagoa denean **Kopurua** eremuan.  Kilometrajearen mailetarako eredu berriak kilometrajearen mailen koherentzia eta erabilgarritasuna hobetzen laguntzen du.   

Onartutako gastuen txosten guztiak argitaratzerakoan berriro kalkulatuko dira diseinu berriaren arabera.

## <a name="example"></a>Adibidez
 
### <a name="before-version-10018"></a>10.0.18 bertsioaren aurretik
Kilometrajearen bi mailekin, **Kopurua** maila bakoitzeko eremuak kilometrajearen muga txikiagoa adierazten du. Gaur egun, lehen mailakoak zero (0) eta 0,45 tasa du, eta bigarren mailakoak 1000 eta 0,25eko tasa du. Metatutako milia edo kilometroek eremuan balioa zeharkatzen badute, erlazionatutako tasa erabiliko da. Zenbaterik gabeko lerroik ez badago, sistemak Gastuen kudeaketan zehaztutako kilometrajea erabiltzen du. 
 
Langile batek 1.500 kilometroko gastuen txostena aurkezten badu, argitaratutako gastuen txostenaren bi kilometro lerroak honakoak lirateke: 1000 (0,45 tasa) + 500 (0,25 tasa) = 575,00.

### <a name="after-version-10018"></a>10.0.18 bertsioaren ondoren
18.08.10ean **Kopurua** maila bakoitzeko eremuak mailaren goiko muga adierazten du. Gaur egun, lehen mailakoak 999 eta 0,45 tasa du, eta bigarren mailakoak 999.999.999,00 eta 0,25eko tasa du. Metatutako milia edo kilometroek **Kopurua** eremuan balioa zeharkatzen badute, erlazionatutako tasa erabiliko da. Goiko muga guztiak gainditzen badira, sistemak Gastuen kudeaketan zehaztutako kilometrajea erabiltzen du. 
 
Eszenatoki bera behar bezala kalkulatzeko, konfiguratutako maila aldatu behar da. **Kopurua** lehen mailako eremuak 999,00 balioa du eta bigarren mailan 999.999.999,00 balioa. Langile batek lehen mailako milia edo kilometro kopurua gainditzen badu, sistemak Gastuen kudeaketan zehaztutako kilometrajea erabiltzen du. 
  
Langile batek 1.500 kilometroko gastuen txostena aurkezten badu, argitaratutako gastuen txostenaren bi kilometro lerroak honakoak lirateke: 1000 (0,45 tasa) + 500 (0,25 tasa) = 575

## <a name="enable-the-mileage-amount-calculation-for-multiple-mileage-tiers-with-same-rate-feature"></a>Gaitu Kilometrajearen zenbatekoa kalkulatzea tasa bera duten kilometraje maila anitzetarako

**Kilometrajearen zenbatekoa kalkulatzea tasa bera duten kilometraje maila anitzetarako** eginbideak kilometrajearen kalkulu-tasa hobetzen du. Egin urrats hauek eginbide hau gaitzeko.

1. Joan **Languneak** > **Eginbideen kudeaketa** atalera. 
2. Zerrendan, bilatu eta hautatu **Kilometroaren zenbatekoa kalkulatzea tasa bera duten kilometro-maila anitzetarako**, eta hautatu **Gaitu orain**.

Ezaugarria gaitu ondoren, berrezarri kilometrajearen mailak **Kopurua** eremua. 

## <a name="enable-the-mileage-totals-calculation-by-fiscal-year-feature"></a>Gaitu Kilometrajearen guztizkoen kalkulua urte fiskal funtzioaren bidez

The **Kilometrajearen guztizkoen kalkulua urte fiskal arabera** Ezaugarriak Gastuen kudeaketa parametroetan ezarpen berri bat gaitzen du, kilometrajearen guztizko kalkuluak egiten dituena urte fiskal arabera, urte naturalaren ordez. Egin urrats hauek eginbide hau gaitzeko.

1. Joan **Languneak** > **Eginbideen kudeaketa** atalera.
1. Zerrendan, bilatu eta hautatu **Kilometrajearen guztizkoen kalkulua urte fiskal arabera**, eta gero hautatu **Gaitu orain**.
1. Joan **Gastuen Kudeaketa** > **Konfigurazioa** > **Orokorra** > **Gastuak kudeatzeko parametroak**.
1. Gainean **Gastuak kudeatzeko parametroak** orrialdea, kokatu eta gaitu **Erabili urte fiskal kilometroen guztizkoetarako**.

Gaitu ondoren **Erabili urte fiskal kilometroen guztizkoetarako**, kilometroen guztirakoak urte fiskal arabera kalkulatzen dira.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
