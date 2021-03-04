---
title: Sortu denbora-sarrerak
description: Gai honek denbora sarrerak sortzeari buruzko informazioa ematen du.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 05/20/2019
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
ms.openlocfilehash: 520d3a6e6cc3d486d778c66c2ef7fd3ff20cd582
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5149663"
---
# <a name="create-time-entries"></a>Sortu denbora-sarrerak

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Dynamics 365 Project Service Automation aplikazioaren aurreko bertsioetan, denbora-sarrerak astero idazten ziren. Project Service Automation-en 3. bertsioan, denbora-sarrerak egunero sartzen dira. Hala ere, sarrerak sortu eta denbora gutxira, modu masiboan sortu edo kopiatu ditzakezu.

## <a name="create-a-time-entry"></a>Sortu denbora-sarrera bat

Jarraitu urrats hauei denbora-sarrera sortzeko.

1. **Denbora-sarrerak** orrian, hautatu **Berria**.
2. **Sorrera bizkorra: Denbora-sarrera** elkarrizketa-koadroan, sartu denboraren iraupena minutu, ordu edo egunetan. Iraupena formatu honetan sartu behar da: *x* minutu, *x* ordu edo *x* egun. Orduak eta egunak ere balio hamartarrak erabiliz idatz daitezke, adibidez, *x.x* ordu edo *x.x* egun.
3. Hautatu debora idatziko duzun denbora-sarrera mota eta proiektua.
4. **Proiektuaren zeregina** eremuan, aurkitu zeregina denbora-sarrera honetarako.

    > [!NOTE]
    > Erabiltzaile bati esleituta ez dagoen zereginetarako denbora-sarrera bat sortzen ari bazara, **Proiektuaren zeregina** eremuan, hautatu **Bilatu** botoia, hautatu **Aldatu ikuspegia** eta, ondoren, hautatu **Proiektu aktiboko zeregin guztiak** zeregin guztiak zerrendatzeko.

5. Idatzi deskribapena, deskribapen bat beharrezkoa bada eta, ondoren, hautatu **Gorde eta itxi**.

Denbora-sarrera sortu eta gorde ondoren, denbora-sarreraren saretan editatu ahal izango duzu. Denbora-sarreraren saretak bi formatu onartzen ditu:

- Denbora-sarrerak **hh: mm** formatuan idatz ditzakezu. Formatu hori ordu eta zatiki bihurtzen da.
- Orduak eta zatikiak zuzenean idatz ditzakezu.

Kontuan izan ordu bateko zatikiak ez direla minutuak. Beraz, 1,5 orduk ordu 1 eta 30 minutu adierazten du. Arau bera aplikatzen zaie egun bateko zatikiei. Egun batek 24 ordu ditu, eta 0,5 egunek 12 ordu.

## <a name="bulk-create-time-entries"></a>Sortu denbora-sarrerak modu masiboan

Denbora-sarrera sortu eta minutu batzuk geroago, kopiatu egin ditzakezu denbora-sarrera gehigarriak gehitzeko modu masiboan.

1. **Denbora-sarrerak** orrian, hautatu **Kopiatu astea**.
2. **Aldi honetatik** talde-eremuan, **Hasiera data** eta **Amaiera Data** eremuetan, zehaztu denbora-sarrerak kopiatu behar diren data-tartea.
3. **Aldira** talde-eremuan, **Hasiera data** eremuan, zehaztu zein datarako sortu nahi dituzun sarrerak.
4. Hautatu **Kopiatu** aukera **Epea** eremu-taldean zehaztutako astearen egunari dagozkion denbora-sarreren kopia bat sortzeko. Adibidez, pasa den asteko astelehenerako denbora-sarrera **Epea** eremuko taldean zehaztutako aste honetako astelehenean kopiatzen da.

## <a name="import-data-for-time-entries"></a>Inportatu datuak denbora-sarreretarako

Proiektuen erreserbetatik eta zereginetatik inportatu ditzakezu datuak. Datuak inportatzean, inportatu nahi dituzun erreserben data zehaztu dezakezu eta, ondoren, modu esplizituan hautatu behar dira **Zirriborroa** denbora-sarrerak gisa sortu behar diren erreserbak.

## <a name="group-by-sort-search-and-filter-capabilities"></a>Taldekatu, ordenatu, bilatu eta iragazi gaitasunak

Denbora-sarrerak zutabeetan zehaztutako neurrien arabera multzokatu eta iragazi ditzakezu. **Taldekatu honela** eremuan, hautatu denbora-sarrerak iragazteko erabili beharreko neurria. Denbora-sarreraren erregistroak goranzko edo beheranzko ordenan ordenatu ditzakezu zutabeetako izenburuak ordenatzeko gezia erabilita. Gainera, sarrerak erakutsi edo ezkutatu ditzakezu zutabearen goiburuko **Iragazkia** botoia hautatua eta, ondoren, **Bilatu** laukian, proiektuaren izenaren, proiektuaren ataza, denbora-sarreraren edo baliabidearen arabera denbora-sarrerak bilatzeko erabili behar den testua idatziz.
