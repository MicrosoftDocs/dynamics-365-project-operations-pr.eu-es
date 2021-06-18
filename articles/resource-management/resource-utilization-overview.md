---
title: Baliabide-erabileraren informazio orokorra
description: Gai honek baliabideen erabilerari buruzko informazioa eskaintzen du Project Operations-en.
author: ruhercul
ms.date: 11/05/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: a683931bcd6a357c5feec9198b190b948ad17a40
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000781"
---
# <a name="resource-utilization-overview"></a>Baliabide-erabileraren informazio orokorra

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Baliabideek xede erabilera fakturagarria izan dezakete. Xede-erabilera hori baliabidearen funtzio lehenetsiko atributu gisa definitzen da edo erreserbatu daitekeen baliabide indibidualaren erregistroan ezartzen da. Erabileraren kalkuluak baliabideek onartutako denbora-sarrerak erabilita jakinarazi dituzten orduetan oinarritzen dira.

Erabilera kalkulatzeko honako formula hauek erabiltzen dira:

  - Erabilera fakturagarria = Kobratu daitezkeen benetako orduak ÷ Baliabidearen ahalmena
  - Erabilera ez fakturagarria = ID motako fakturaziodun denbora erreala = Kobratu ezin dena, osagarria edo eskuragarri ez dagoena ÷ Baliabidearen ahalmena
  - Barnekoa = Salmenta kontraturik gabeko denbora erreala ÷ Baliabideen ahalmena
  - Baliabideen ahalmena = Baliabideen lan orduak – Bulegotik kanpo – Lanik gabeko egunak

**Baliabideen erabilera** ikuspegia **Baliabideak** panelean aurkituko duzu.

Saretako gelaxka bakoitzak baliabidearen erabilera fakturagarriaren ehunekoa adierazten du aldi batean, hala nola, egun batean, astean edo hilean. Gelaxkei kolorea emateko honako formula hauek erabiltzen dira:

  - **Berdea**: Fakturazioaren erabilera >= Baliabidearen helburuko erabilera
  - **Horia**: Helburuaren erabilera – 20 < Fakturazioaren erabilera = < Helburuko erabilera
  - **Gorria**: Erabilera fakturagarria < Helburuko erabilera - 20

**Baliabide-erabilera** ikuspegia antolaketa-panelean oinarrituta dagoenez, antolaketa paneleko iragazkien ahalmenak erabil ditzakezu emaitzak iragazteko.

Saretak helburuko erabilera ezartzea eskatzen du, bai funtzioan, bai baliabide indibidualean. Konfigurazio hori egiteko, joan **Baliabideak** > **Baliabideen funtzioak** atalera.

Gainera, eginkizun lehenetsi bat esleitu behar zaio erreserbatu daitekeen baliabide bakoitzari. Joan **Baliabideak** > **Baliabideak** atalera. **Project Service** fitxan, egiaztatu baliabide funtzioa definituta dagoela, eta **Lehenetsia da** eremua **Bai** gisa ezarrita dagoela. Funtzio osagarriak gehi ditzakezu **Lehenetsia da** = **Ez** den tokian. **Lehenetsia da** = **Bai** aukeran erabiltzen den funtzioa baliabidearen erabilera ebaluatzeko erabiltzen da funtzioaren helburuarekin alderatuz.

**Project Service** fitxan, helburuko erabilera indibiduala ere ezar dezakezu baliabiderako. Ondoren, erabileraren kalkuluak helburuko erabilera hori erabiltzen du baliabidearen helburua ebaluatzeko, baliabidearen funtzio lehenetsiaren helburua ebaluatu beharrean.

Erabilera baliabide gisa erakusten da baliabideak saretan agertzen den aldian kobratu daitekeen denbora onartu badu soilik.


[!INCLUDE[footer-include](../includes/footer-banner.md)]