---
title: Moneta bat ez datorren adierazten duen errorea
description: Artikulu honek erregistro-mota zehatzak gordetzen dituzunean gertatzen den moneta-desegokitze-erroreari buruzko arazoak konpontzeko informazioa eskaintzen du.
author: sigitac
ms.date: 12/09/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 5b0973a340dec8e68f326803d75bea9803e19791
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8914709"
---
# <a name="currency-mismatch-error"></a>Moneta bat ez datorren adierazten duen errorea 

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Proiektua, kontratua, eskaintza edo baliabide erreserbagarria gordetzean baliteke **enpresaren moneta ez dator bat kontratatzeko unitatearen monetarekin. Aukeratu proiektuaren kontratuaren enpresa-jabe edo kontratazio-unitate desberdin bat** errorea agertzea. Hau da, erregistroko kontratazio-unitatearen moneta eta enpresa jabearen moneta-desegokitze bat dagoelako.


## <a name="resolution"></a>Ebazpena

Arazo hau konpontzeko egin hurrengoa:
- Egiaztatu erregistro honetarako kontratazio-unitatearen dibisa. Moneta ikus dezakezu antolakuntza-unitateko erregistroa irekiz eta balioa egiaztatuz **Orokorra** fitxan **Moneta** eremua.
- Egiaztatu moneta jabetzadun enpresaren. Dibisa helbidera joanda ikus dezakezu **Erlazionatua** > **Liburuak** enpresaren erregistroan. Egin klik bikoitza enpresarekin lotuta dagoen liburuko erregistroan eta egiaztatu balioa **Orokorra** fitxan **Kontabilitate-moneta** eremua.

Kontratazio-unitatean ezarritako moneta eta liburuko erregistroa bat ez badatoz, egokitu konfigurazioa edo hautatu balio desberdinak erregistroa gordetzean. Sistemak erregistro hauek bat etortzea eskatzen du enpresen arteko fakturazio-fluxu zuzenak bermatzeko. Enpresa arteko konfigurazioei buruzko informazio gehiago lortzeko, ikus [Sortu enpresen arteko transakzioak](../../project-accounting/create-intercompany-transactions.md).

Konpainiaren erregistroak ez badu erlazionatutako liburu-erregistrorik, honek ingurunea konfiguratzerakoan konfigurazio bat falta dela adierazten du. Konfigurazioa sistemaren administratzaileak zuzendu behar du. Sistemaren administratzaileak helbidera joan behar du **Idazketa bikoitzeko konfigurazioak** eta gelditu eta berrabiarazi **Liburuen idazketa bikoitzeko mapa** mapa honen hasierako sinkronizazioarekin eta bere aurrebaldintzak. Informazio gehiagorako, ikus [Project Operations idazketa bikoitzeko mapen bertsioak](../../environment/resource-dual-write-maps.md).
