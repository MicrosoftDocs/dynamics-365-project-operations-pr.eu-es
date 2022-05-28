---
title: Errore bat dibisa desegokitzea
description: Gai honek erregistro-mota zehatzak gordetzen dituzunean gertatzen den moneta-desegokitze-erroreari buruzko arazoak konpontzeko informazioa eskaintzen du.
author: sigitac
ms.date: 12/09/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 5bb54a121f0dc22f1c0ea88ada9c922c1d4c6544
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8589733"
---
# <a name="currency-mismatch-error"></a>Errore bat dibisa desegokitzea 

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Proiektu, kontratu, aurrekontu edo erreserba daitekeen baliabide bat gordetzen duzunean, baliteke errorea jasotzea.**Enpresaren jabea den moneta ez dator bat kontratazio-unitateko diruarekin. Aukeratu enpresa jabea edo kontratazio unitate desberdinak jarraitzeko**. Hau da, erregistroko kontratazio-unitatearen moneta eta enpresa jabearen moneta-kopuruaren artean moneta-desegokia dagoelako.


## <a name="resolution"></a>Ebazpena

Arazo honi aurre egiteko, egin hau:
- Egiaztatu erregistro honetarako kontratazio-unitatearen dibisa. Moneta ikus dezakezu antolakuntza-unitateko erregistroa irekiz eta balioa egiaztatuz **Orokorra** fitxan **Moneta** eremua.
- Egiaztatu enpresa jabearen moneta. Dibisa helbidera joanda ikus dezakezu **Erlazionatua** > **Liburuak** enpresaren erregistroan. Egin klik bikoitza enpresarekin lotuta dagoen liburuko erregistroan eta egiaztatu balioa **Orokorra** fitxan **Kontabilitate-moneta** eremua.

Kontratazio-unitatean ezarritako moneta eta liburuko erregistroa bat ez badatoz, egokitu konfigurazioa edo hautatu balio desberdinak erregistroa gordetzean. Sistemak erregistro hauek bat etortzea eskatzen du enpresen arteko fakturazio-fluxu zuzenak bermatzeko. Enpresa arteko konfigurazioei buruzko informazio gehiago lortzeko, ikus [Sortu enpresen arteko transakzioak](../../project-accounting/create-intercompany-transactions.md).

Konpainiaren erregistroak ez badu erlazionatutako liburu-erregistrorik, honek ingurunea konfiguratzerakoan konfigurazio bat falta dela adierazten du. Konfigurazioa sistemaren administratzaileak zuzendu behar du. Sistemaren administratzaileak helbidera joan behar du **Idazketa bikoitzeko konfigurazioak** eta gelditu eta berrabiarazi **Liburuen idazketa bikoitzeko mapa** mapa honen hasierako sinkronizazioarekin eta aurrebaldintzekin. Informazio gehiagorako, ikus [Project Operations idazketa bikoitzeko mapen bertsioak](../../environment/resource-dual-write-maps.md).
