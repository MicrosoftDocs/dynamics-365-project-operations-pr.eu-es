---
title: Konfiguratu kilometrajea kilometrajearen tasaren mailak erabiliz
description: Artikulu honek kilometraje-tasei eta kilometraje-tasari buruzko informazioa eskaintzen du.
author: suvaidya
ms.date: 05/20/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: suvaidya
ms.openlocfilehash: 03ca18c8fef6228f2ba553ebe50447beda5a857c
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8930119"
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


[!INCLUDE[footer-include](../includes/footer-banner.md)]
