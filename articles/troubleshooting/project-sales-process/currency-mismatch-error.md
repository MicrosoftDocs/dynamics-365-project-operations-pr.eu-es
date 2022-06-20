---
title: Dibisen deskalifikazio-akatsa
description: Artikulu honetan, erregistro-mota espezifikoak gordetzean sortzen den moneta-faltaren akats bati buruzko problemak konpontzeko informazioa ematen da.
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
# <a name="currency-mismatch-error"></a>Dibisen deskalifikazio-akatsa 

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Proiektu, kontratu, kotizazio edo baliabide erreserbagarri bat gordetzen duenean, akatsa jaso daiteke, **enpresa jabearen dibisa ez dator bat kontratazio-unitatearen dibisarekin. Aukeratu enpresa jabe bat edo kontratazio-unitate desberdin bat, jarraitzeko**. Hori da, erregistrorako kontratazio-unitateko monetaren eta enpresa jabearen diruaren artean moneta-desoreka dagoelako.


## <a name="resolution"></a>Ebazpena

Arazo hau saihesteko, egin ezazu honako hau:
- Egiaztatu unitate kontratatzailearen txanpona erregistro horretarako. Moneta antolaketa-unitatearen erregistroa irekiz eta Moneda **zelaiko** betile orokorrean **balioa** egiaztatzen ikus dezakezu.
- Egiaztatu enpresa jabearen txanpona. Enpresa-erregistroan zerikusia duten **kontabilitate-liburuetara** > **joaten** ikus dezakezu txanpona. Egin klik bikoitza enpresari lotutako kontabilitate-erregistroan **eta egiaztatu balioa kontabilitate-moneda** zelaiaren **fitxa orokorrean**.

Kontratazio-unitatean eta kontabilitate-erregistroan ezarritako moneta bat ez badatoz, konfigurazioa doitzen badu edo erregistroa gordetzean ez diren balioak aukeratzen baditu. Sistemak erregistro horiek bat etortzea eskatzen du, konpainien arteko fakturazio-fluxu zuzenak bermatzeko. Enpresen arteko konfigurazioei buruzko informazio gehiago lortzeko, ikus [enpresen](../../project-accounting/create-intercompany-transactions.md) arteko transakzioak sortzen.

Enpresaren erregistroak ez badu lotutako kontabilitate-erregistrorik, horrek adierazten du konfigurazio bat falta dela ingurunea konfiguratzean. Sistemaren administratzaileak zuzendu behar du konfigurazioa. Sistemaren administratzaileak idazkera dualeko konfigurazioetara **joan** behar du, eta Ledgers-en idazkera dualaren mapa **geldiarazi eta berrabiarazi** behar du, mapa horren hasierako sinkronizazioarekin eta aldez aurreko baldintzekin. Informazio gehiagorako, ikus [Project Operations idazketa bikoitzeko mapen bertsioak](../../environment/resource-dual-write-maps.md).
