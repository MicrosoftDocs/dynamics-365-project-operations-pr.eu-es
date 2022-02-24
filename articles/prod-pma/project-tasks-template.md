---
title: Sinkronizatu proiektuaren zereginak zuzenean Project Service Automation-etik Finance and Operations
description: Gai honek deskribatzen du txantiloiak eta azpiko zeregina erabiliak direnak sinkronizatzeko zereginen proiektuak zuzenean Microsoft Dynamics 365 Project Service Automation hurrengora Dynamics 365 Finance.
author: Yowelle
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 0383607a07def6c21562bf4b0893fe3ce3db6a04
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071018"
---
# <a name="synchronize-project-tasks-directly-from-project-service-automation-to-finance-and-operations"></a>Sinkronizatu proiektuaren zereginak zuzenean Project Service Automation-etik Finance and Operations

[!include[banner](../includes/banner.md)]

Gai honek deskribatzen du txantiloiak eta azpiko zeregina erabiliak direnak sinkronizatzeko zereginen proiektuak zuzenean Dynamics 365 Project Service Automation hurrengora Dynamics 365 Finance.

> [!NOTE]
> - Proiektuaren zereginen integrazioa, gastuen transakzioen kategoriak, orduen kalkuluak, gastuen kalkuluak eta funtzionalitate blokeoa eskuragarri daude 8.0 bertsioan.
> - KB 4132657 eta KB 4132660 instalatu ondoren Enterprise edition 7.3.0 erabiltzen ari bazara, txantiloiak erabil ditzakezu proiektuaren zereginak, gastuen transakzioen kategoriak, orduen kalkuluak, gastuen kalkuluak eta benetakoak konfiguratzeko eta konfiguratzeko funtzionalitate blokeoa. Kontabilitate banaketak berrezarri behar badituzu, KB 4131710 ere instalatzea gomendatzen dizugu.
> - Datu bateratuen integrazioa eskuragarri dago 8.0.1 bertsioan edo hurrengoan.

## <a name="data-flow-for-project-service-automation-to-finance"></a>Project Service Automation Finantzararen datu-fluxua

Project Service Automation to Finance integrazio irtenbideak Datu integrazio funtzioa erabiltzen du datuak Project Service Automation eta Finance-ren instantzia guztietan sinkronizatzeko. Datuak integratzeko funtzioarekin eskuragarri dauden integrazio txantiloiek proiektuaren zereginen inguruko datuen fluxua ahalbidetzen dute Project Service Automation-etik Finantzara.

Ondorengo ilustrazioak erakusten du nola sinkronizatzen diren datuak Project Service Automation eta Finance artean.

[![Project Service Automation Finantzarekin integratzeko datuen fluxua](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)

## <a name="template-and-task"></a>Txantiloia eta zeregina

Txantiloietara sartzeko, Microsoft Power Apps administratzaile zentroa, hautatu **Proiektuak** eta, ondoren, goiko eskuineko izkinan, hautatu **Proiektu berria** txantiloi publikoak hautatzeko.

Ondorengo txantiloia eta azpiko zereginaren proiektuaren zereginen Project Service Automation-etik Finantzara sinkronizatzeko erabiltzen dira:

- **Datuen integrazioko txantiloiaren izena:** Proiektuaren zereginak (PSA Fin eta Ops)
- **Proiektuko zereginen izena:** Proiektuaren zereginak

Proiektuen zereginen sinkronizazioa gertatu aurretik, kontuak sinkronizatu proiektuaren kontratuak eta proiektuak behar dituzu.

## <a name="entity-set"></a>Entitate multzoaren

| Project Service Automation | Finantzak                             |
|----------------------------|-------------------------------------|
| Proiektuen zereginak              | Proiektuaren zeregina datu-bateratuak integrazio entitatea |

## <a name="entity-flow"></a>Entitate fluxua

Proiektuaren zereginak Project Service Automation-en kudeatzen dira eta Finantzarekin sinkronizatzen dira proiektuaren jarduerak gisa.

## <a name="prerequisites-and-mapping-setup"></a>Aurrebaldintzak eta mapen konfigurazioa

Proiektuen zereginen sinkronizazioa gertatu aurretik, kontuak sinkronizatu proiektuaren kontratuak eta proiektuak behar dituzu.

## <a name="power-query"></a>Power Query

Microsoft Power Query Excel-era erabili behar duzu datuak iragazteko baldintza hori gertatzean:

- Baliabideen araberako erregistroak dituzu proiektuko zeregin batean.

Power Query erabili behar baduzu, jarraitu jarraibide hori:

- Project tasks (PSA to Fin and Ops) txantiloiak iragazki lehenetsia du, baliabide espezifikoak erregistroak proiektuko zereginetik kanpo uzten dituena iragazkia ezarriz **IsLineTask** hurrengora **Gezurra**. Zure txantiloia sortzen baduzu, iragazki hau gehitu behar duzu.

## <a name="template-mapping-in-data-integration"></a>Datuen integrazioan txantiloien mapaketa

Ondorengo ilustrazioak Datuen integrazioan txantiloien atazen mapen adibide bat erakusten du. Kartografiak Project Service Automation-etik Finantzara sinkronizatuko den eremuko informazioa erakusten du.

[![Txantiloien mapaketa](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)
