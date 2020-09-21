---
title: Project Service Automation-en ikuspegi orokorra
description: Gai honek informazioari buruzko informazioa eskaintzen du Dynamics 365 Project Service Automation hurrengora Dynamics 365 Finance integrazio irtenbidea.
author: KimANelson
manager: AnnBe
ms.date: 07/25/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: 897e1a1c-d31c-42b8-bb59-6b67202d8d61
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 080a545d8713e52d9778367aec1969b815d683e5
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748887"
---
# <a name="project-service-automation-overview"></a>Project Service Automation-en ikuspegi orokorra

[!include[banner](../includes/banner.md)]

Project Service Automation hurrengora Finantza integrazioaren soluzioak erabiltzen du Datu integrazioaren eginbidea sinkronizatzeko datuak instantzien artean Dynamics 365 Finance eta Dynamics 365 Project Service Automation bidez Common Data Service. Integrazio-txantiloiak eskuragarri daudenak Datu-integrazioaren eginbidearekin gaitzen du proiektuen fluxua, proiektu-kontratuak, proiektu-kontratu lerroak, proiektu-kontratu lerroen mugarriak, proiektu-zereginak, gastuen transakzio kategoriak, aurreikusitako orduak, eta gastu-aurreikusiak Project Service Automation Finantzara.

> [!NOTE]
> - Bertsioa 7.3.0 erabiltzen ari bazara, KB 4074835 instalatu behar duzu. Orduan, prezio finkoaren proiektuak integratu ahal izango dituzu.
> - 7.3.0 bertsioa erabiltzen ari bazara eta Project Service Automation-etik kuoten transakzioak ekartzen badituzu, KB 4345320 instalatu behar duzu tasak proiektuaren fakturan sartzeko.
> - 8.0 bertsioa erabiltzen ari bazara, gai izango zara erabiltzeko proiektuaren zereginen integrazioa, gastuen transakzioen kategoriak, orduen kalkuluak, gastuen kalkuluak eta funtzionalitate blokeoa.
> - 8.0.1 bertsioa edo berriagoa erabiltzen baduzu, benetakoak sinkronizatu ahal izango dituzu.

Project Service Automation Finance integratu aurretik, Project Service Automation integrazio parametroak konfiguratu behar dituzu. Informazio gehiagorako, ikusi [Project Service Automation integrazio-parametroak](PSA-parameters.md).

Integrazio irtenbide honek zuzeneko sinkronizazioa ahalbidetzen du agertoki hauetan:

- Mantendu proiektuen kontratuak Project Service Automation zerbitzuan eta sinkronizatu zuzenean Project Service Automationetik Finantzara.
- Sortu proiektuak Project Service Automation zerbitzuan eta sinkronizatu zuzenean Project Service Automationetik Finantzara.
- Mantendu proiektuen kontratu-lerroak Project Service Automation zerbitzuan eta sinkronizatu zuzenean Project Service Automationetik Finantzara.
- Mantendu proiektuen kontratu-lerroen mugarriak Project Service Automation zerbitzuan eta sinkronizatu zuzenean Project Service Automationetik Finantzara.
- Mantendu proiektuen zereginak kontratuak Project Service Automation zerbitzuan eta sinkronizatu zuzenean Project Service Automationetik Finantzara.
- Mantendu gastuen transakzio-kategoriak Finantzan, eta sinkronizatu horiek zuzenean Finantzatik Project Service Automation.
- Sortu proiektuak aurreikusitako orduak Project Service Automation zerbitzuan eta sinkronizatu zuzenean Project Service Automationetik Finantzara.
- Sortu proiektuak aurreikusitako gastuak Project Service Automation zerbitzuan eta sinkronizatu zuzenean Project Service Automationetik Finantzara.
- Sortu proiektuaren denbora, gastua eta kuoten errealitatea Project Service Automation-en eta sortu proiektuaren transakzioak Project Service Automation integrazio aldizkarian, Finantzan argitaratu ahal izateko.

## <a name="data-synchronization"></a>Datuen sinkronizazioa

Ondorengo ilustrazioak erakusten du nola sinkronizatzen diren datuak integrazioaren parte gisa Project Service Automation eta Finance artean.

> [!NOTE]
> Txantiloi guztiak ez daude unean eskuragarri. Txantiloiak amaitu ahala kaleratuko dira.

[![Project Service Automation Finantzarekin integratzeko](./media/PSA-integration.png)](./media/PSA-integration.png)

## <a name="system-requirements-for-finance"></a>Finantzetarako sistemaren eskakizunak

Project Service Automation to Finance integrazio konponbidea erabiltzeko, Enterprise edition 7.3 instalatu behar duzu Plataforma 12 bertsio berriagoa edo berriagoarekin.

## <a name="system-requirements-for-project-service-automation"></a>Sistemaren eskakizunak Project Service Automation

Project Service Automation to Finance integrazio irtenbidea erabiltzeko, osagai hauek instalatu behar dituzu:

- Dynamics 365 Project Service Automation 9.0.0.0 bertsioa edo berriagoa
- Dynamics 365 Sales-erako dirua ateratzeko irtenbidea, 1.14.0.0 (v14) bertsioa edo berriagoa
- Project Service Automation to Finance irtenbidea Dynamics 365 Project Service Automation 1.0.0.0 bertsioa edo berriagoa

## <a name="install-the-project-service-automation-to-finance-integration-solution-in-your-project-service-automation-instance"></a>Instalatu Project Service Automation to Finance integrazio konponbidea zure Project Service Automation instantzia

Deskargatu Project Service Automation to Finance integrazio irtenbidea [Microsoft Deskarga Zentroa](https://www.microsoft.com/download/details.aspx?id=57016), eta jarraitu irtenbidearekin bat datozen argibideak.
