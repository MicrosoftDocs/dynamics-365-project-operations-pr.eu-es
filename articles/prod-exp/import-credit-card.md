---
title: Inportatu eta mantendu kreditu-txartelaren eragiketak
description: Gai honetan gastuekin lotutako kreditu txartelaren eragiketak nola inportatu eta nola mantendu azaltzen da. Transakzio hauek konfiguratu daitezke, aldian-aldiko programazioan automatikoki inportatzeko edo eskuz inportatu ahal izateko beharrezkoak diren neurrian.
author: KimANelson
manager: AnnBe
ms.date: 01/12/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvPbsMainDataLines
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 274023
ms.assetid: 3605eda1-a7ed-4675-8031-5279c5a8f5e4
ms.search.region: Global
ms.author: suvaidya
ms.dyn365.ops.version: Version 1611
ms.search.validFrom: 2016-11-30
ms.openlocfilehash: 6cec15e436bc699e361577c970dd5845c6c68908
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071189"
---
# <a name="import-and-maintain-credit-card-transactions"></a>Inportatu eta mantendu kreditu-txartelaren eragiketak

[!include [banner](../includes/banner.md)]

Gastuei lotutako kreditu txartelaren eragiketak konfiguratu daitezke, aldian-aldiko programazioan automatikoki inportatzeko. Bestela, transakzioak eskuz inporta daitezke beharrezkoak diren neurrian. Kreditu txartelaren transakzioak Kreditu txartelaren transakzioen datuen entitatearen bidez inportatzen dira.

Datu-entitateei buruzko informazio gehiago lortzeko, ikusi [Datu-entitateak ](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/data-entities/data-entities).

## <a name="import-credit-card-transactions"></a>Inportatu kreditu txartelaren eragiketak

1. **Kreditu-txartelaren eragiketak** orrialdean, hautatu **Inportazio transakzioak**. Datuen kudeaketa lehen aldiz irekitzen ari bazara, sistemak datu-entitateen zerrenda eguneratu beharko du jarraitu ahal izateko.
2. **Izena** eremuan, sartu inportazio lanaren deskribapen bakarra.
3. **Iturriaren datuen formatua** eremuan, hautatu inportatu beharreko kreditu txartelaren transakzioak dituen fitxategiaren formatua.
4. Hautatu **Kargatu** eta, ondoren, bilatu eta hautatu inportatzeko fitxategia.
5. Fitxategia kargatu ondoren, baliozkotu kreditu txartelaren transakzio fitxategiaren mapak eta Kreditu txartelaren transakzioen datu entitatearen zutabeak hautatu **Ikusi mapa** esteka fitxan. Kartografia akatsak badaude, edo mapaketa aldatu behar baduzu, egin maparen aldaketak **Mapen bistaratzea** fitxa edo **Kartografia xehetasunak** fitxa.
6. Kreditu txartelaren eragiketak automatizatzeko, hautatu **Sortu aldizkako datuen lana**. Kreditu txartelaren eragiketak zenbat aldiz inportatu behar diren zehazten duen errepikapena ezar dezakezu. Bukatu duzunean, hautatu **Ados**.
7. Aukeratutako fitxategia orain inportatzeko, hautatu **Inportatu**.
8. Inportazioan zehar akatsak gertatzen badira, exekuzio erregistroa edo faseko datuak ikus ditzakezu inportazio arrakastatsua bermatzen laguntzeko konpondu behar dituzun akatsak ikusteko.

> [!NOTE]
> Fitxategi formatu bat baino gehiago inportatu behar badituzu, inportazio lan bereiziak sortu behar dituzu formatu mota bakoitzerako.

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a>Kargatu bajako langileentzako kreditu txartelaren eragiketak

Langilearen erregistroa amaitu ondoren, langilearen Active Directory domeinu zerbitzuak (AD DS) kontua desgaituta dago. Hala ere, baliteke kreditu txartelarekin egindako transakzio aktiboak oraindik gastatu eta itzuli behar direnak. Tik **Kreditu txartelaren eragiketak** orrialdean, langilea berriro esleitu ahal izango duzu lotutako langilea amaitu den kreditu txartelarekin egindako edozein transakzioetarako.

Aukeratu kreditu txartelaren transakzio bat edo gehiago, eta hautatu **Transakzioak berriro esleitu**. Kreditu txartelaren eragiketak esleitzeko beste langile bat hauta dezakezu. Kreditu txartelaren eragiketak berriro esleitu ondoren, gastuen txostena aukeratu eta gastuen txostena itzultzeko ohiko prozesuaren bidez ordain daitezke.