---
title: Konfiguratu kreditu-txartelaren integrazioa
description: Gai honetan gastuekin lotutako kreditu txarteleko transakzioekin nola lan egin azaltzen da.
author: suvaidya
ms.date: 04/02/2021
ms.topic: article
ms.prod: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 51c364dff41d856e493581e1b87fd29571f641c70e7233bdebb910efbc64b983
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6996196"
---
# <a name="set-up-credit-card-integration"></a>Konfiguratu kreditu-txartelaren integrazioa

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Gastuei lotutako kreditu txartelaren eragiketak konfiguratu daitezke, aldian-aldiko programazioan automatikoki inportatzeko. Bestela, transakzioak eskuz inporta daitezke beharrezkoak diren neurrian. Kreditu txartelaren transakzioak kreditu-txartelaren transakzioen datuen entitatearen bidez inportatzen dira.

## <a name="import-credit-card-transactions"></a>Inportatu kreditu txartelaren eragiketak

Kreditu txartelaren eragiketak inportatzeko, jarraitu urrats hauei:

1. **Kreditu-txartelaren eragiketak** orrialdean, hautatu **Inportazio transakzioak**. Datuen kudeaketa lehen aldiz irekitzen ari bazara, sistemak datu-entitateen zerrenda eguneratu beharko du jarraitu ahal izateko.
2. **Izena** eremuan, sartu inportazio lanaren deskribapen bakarra.
3. **Iturriaren datuen formatua** eremuan, hautatu inportatu beharreko kreditu txartelaren transakzioak dituen fitxategiaren formatua.
4. Hautatu **Kargatu** eta, ondoren, bilatu eta hautatu inportatzeko fitxategia.
5. Fitxategia kargatu ondoren, baliozkotu kreditu txartelaren transakzio fitxategiaren mapak eta kreditu-txartelaren transakzioen datu entitatearen zutabeak hautatu **Ikusi mapa** esteka fitxan. Kartografia akatsak badaude, edo mapaketa aldatu behar baduzu, egin maparen aldaketak **Mapen bistaratzea** fitxa edo **Kartografia xehetasunak** fitxa.
6. Kreditu txartelaren eragiketak automatizatzeko, hautatu **Sortu aldizkako datuen lana**. Kreditu txartelaren eragiketak zenbat aldiz inportatu behar diren zehazten duen errepikapena ezar dezakezu. Bukatu duzunean, hautatu **Ados**.
7. Aukeratutako fitxategia orain inportatzeko, hautatu **Inportatu**.
8. Inportazioan zehar akatsak gertatzen badira, exekuzio erregistroa edo faseko datuak ikus ditzakezu inportazio arrakastatsua ziurtatzen laguntzeko konpondu behar dituzun akatsak ikusteko.

> [!NOTE]
> Fitxategi formatu bat baino gehiago inportatu behar badituzu, inportazio lan bereiziak sortu behar dituzu formatu mota bakoitzerako.

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a>Kargatu bajako langileentzako kreditu txartelaren eragiketak

Langilearen erregistroa amaitu ondoren, langilearen Active Directory domeinu zerbitzuak (AD DS) kontua desgaituta dago. Hala ere, baliteke kreditu txartelarekin egindako transakzio aktiboak oraindik gastatu eta itzuli behar direnak. **Kreditu txartelaren eragiketak** orrialdean, langilea berriro esleitu ahal izango duzu lotutako langilea amaitu den kreditu txartelarekin egindako edozein transakzioetarako.

Aukeratu kreditu txartelaren transakzio bat edo gehiago, eta hautatu **Transakzioak berriro esleitu**. Kreditu txartelaren eragiketak esleitzeko beste langile bat hauta dezakezu. Kreditu txartelaren eragiketak berriro esleitu ondoren, gastuen txostena aukeratu eta gastuen txostena itzultzeko ohiko prozesuaren bidez ordain daitezke.

## <a name="delete-credit-card-transactions"></a>Ezabatu kreditu txartelaren eragiketak 

Batzuetan, kreditu txartelarekin egindako transakzioak inportatu ondoren, baliteke transakzio batzuk ezabatu behar izatea. Gerta liteke transakzioak bikoiztuak direlako edo baliteke datuak zehatzak ez izateagatik. Administratzaileek **"Ezabatu kreditu txartelaren transakzioak"** funtzioa diren kreditu txarteleko eragiketak hautatu eta ezabatzeko **erantsita ez** gastuen txosten batera. 

1. Joan **Aldizkako zereginak** > **Ezabatu kreditu txartelaren eragiketak**.
2. Aukeratu **Iragazi** eta informazioa eman erregistroak identifikatzeko.
3. Hautatu **Ados** erregistroak ezabatzeko. 

[!INCLUDE[footer-include](../includes/footer-banner.md)]
