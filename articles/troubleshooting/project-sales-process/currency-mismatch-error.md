---
title: Errore bat dibisa desegokitzea
description: Gai honek erregistro-mota zehatzak gordetzen dituzunean gertatzen den moneta-desegokitze-erroreari buruzko arazoak konpontzeko informazioa eskaintzen du.
author: sigitac
ms.date: 12/09/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 52e33ad3728e1a393e8c7e3ca4e0a4b506d0b774
ms.sourcegitcommit: 04dc8d952e6da3ab3eb2a20131c6f7cee6040876
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/10/2021
ms.locfileid: "7903608"
---
# <a name="currency-mismatch-error"></a>Errore bat dibisa desegokitzea 

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Proiektu, kontratu, aurrekontu edo erreserba daitekeen baliabide bat gordetzen duzunean, baliteke errorea jasotzea.**Enpresaren jabea den moneta ez dator bat kontratazio-unitateko diruarekin. Aukeratu enpresa jabea edo kontratazio unitate desberdinak jarraitzeko**. Hau da, erregistroko kontratazio-unitatearen moneta eta enpresa jabearen moneta-kopuruaren artean moneta-desegokia dagoelako.


## <a name="resolution"></a>Ebazpena

Arazo honi aurre egiteko, egin hau:
- Egiaztatu erregistro honetarako kontratazio-unitatearen dibisa. Moneta ikus dezakezu antolakuntza-unitatearen erregistroa irekiz eta balioa egiaztatuz **Orokorra** fitxan **Moneta** eremua.
- Egiaztatu enpresa jabearen moneta. Dibisa helbidera joanda ikus dezakezu **Erlazionatua** > **Liburuak** enpresaren erregistroan. Egin klik bikoitza enpresarekin lotuta dagoen liburuko erregistroan eta egiaztatu balioa **Orokorra** fitxan **Kontabilitate-moneta** eremua.

Kontratazio-unitatean ezarritako moneta eta liburuko erregistroa bat ez badatoz, egokitu konfigurazioa edo hautatu balio desberdinak erregistroa gordetzean. Sistemak erregistro hauek bat etortzea eskatzen du enpresen arteko fakturazio-fluxu zuzenak bermatzeko. Enpresa arteko konfigurazioei buruzko informazio gehiago lortzeko, ikus [Sortu enpresen arteko transakzioak](../../project-accounting/create-intercompany-transactions.md).

Konpainiaren erregistroak ez badu erlazionatutako liburu-erregistrorik, honek ingurunea konfiguratzerakoan konfigurazio bat falta dela adierazten du. Konfigurazioa sistemaren administratzaileak zuzendu behar du. Sistemaren administratzaileak helbidera joan behar du **Idazketa bikoitzeko konfigurazioak** eta gelditu eta berrabiarazi **Liburuen idazketa bikoitzeko mapa** mapa honen hasierako sinkronizazioarekin eta aurrebaldintzekin. Informazio gehiagorako, ikus [Project Operations idazketa bikoitzeko mapen bertsioak](../../environment/resource-dual-write-maps.md).
