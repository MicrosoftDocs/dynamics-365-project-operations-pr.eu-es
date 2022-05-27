---
title: Konfiguratu kreditu-txartelaren integrazioa
description: Gai honetan gastuekin lotutako kreditu txarteleko transakzioekin nola lan egin azaltzen da.
author: suvaidya
ms.date: 11/17/2021
ms.topic: article
ms.prod: ''
ms.search.form: ''
audience: Application User
ms.reviewer: johnmichalak
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 2c9d993f1999b0be24794bbe828afa8eb74744e9
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8577038"
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
6. Kreditu txartelaren eragiketak automatizatzeko, hautatu **Sortu aldizkako datuen lana**. Kreditu txartelaren eragiketak zenbat aldiz inportatu behar diren zehazten duen errepikapena ezar dezakezu. Amaitzen duzunean, hautatu **ADOS**.
7. Aukeratutako fitxategia orain inportatzeko, hautatu **Inportatu**.
8. Inportazioan zehar akatsak gertatzen badira, exekuzio erregistroa edo faseko datuak ikus ditzakezu inportazio arrakastatsua ziurtatzen laguntzeko konpondu behar dituzun akatsak ikusteko.

> [!NOTE]
> Fitxategi formatu bat baino gehiago inportatu behar badituzu, inportazio lan bereiziak sortu behar dituzu formatu mota bakoitzerako.

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a>Kargatu bajako langileentzako kreditu txartelaren eragiketak

Langileen erregistroa amaitu ondoren, langilearen Active Directory Domain Services (AD DS) kontua desgaitu egiten da. Hala ere, baliteke kreditu txartelarekin egindako transakzio aktiboak oraindik gastatu eta itzuli behar direnak. **Kreditu txartelaren eragiketak** orrialdean, langilea berriro esleitu ahal izango duzu lotutako langilea amaitu den kreditu txartelarekin egindako edozein transakzioetarako.

Aukeratu kreditu txartelaren transakzio bat edo gehiago, eta hautatu **Transakzioak berriro esleitu**. Kreditu txartelaren eragiketak esleitzeko beste langile bat hauta dezakezu. Kreditu txartelaren eragiketak berriro esleitu ondoren, gastuen txostena aukeratu eta gastuen txostena itzultzeko ohiko prozesuaren bidez ordain daitezke.

## <a name="delete-credit-card-transactions"></a>Ezabatu kreditu txartelaren eragiketak 

Batzuetan, kreditu txartelarekin egindako transakzioak inportatu ondoren, baliteke transakzio batzuk ezabatu behar izatea. Hau izan daiteke transakzioak bikoiztuak direlako edo datuak zehatzak ez direlako. Administratzaileek **"Ezabatu kreditu txartelaren transakzioak"** funtzioa diren kreditu txarteleko eragiketak hautatu eta ezabatzeko **erantsita ez** gastuen txosten batera. 

1. Joan **Aldizkako zereginak** > **Ezabatu kreditu txartelaren eragiketak**.
2. Aukeratu **Iragazi** eta informazioa eman erregistroak identifikatzeko.
3. Hautatu **Ados** erregistroak ezabatzeko. 

## <a name="storing-credit-card-numbers"></a>Kreditu txartelaren zenbakiak gordetzea

Hiru aukera daude kreditu-txartelen zenbakiak gordetzeko. Kreditu-txartelen zenbakiak gailuan gordetzen dira **Gastuak kudeatzeko parametroak** orrialdea.

- **Saihestu txartelaren zenbakia sartzea** – Kreditu-txartelen zenbakiak ez dira gordetzen.
- **Hash txartelaren zenbakiak (gordetu azken lau digituak)** – Kreditu-txartelen zenbakien azken lau digituak formatu enkriptatu batean gordetzen dira.
- **Gorde txartelaren zenbakiak** – Kreditu-txartelen zenbakiak zifratu gabeko formatu batean gordetzen dira. Aukera honek ez du betetzen Payment Card Industry (PCI) Datuen Segurtasun Estandarra (DSS). Hori dela eta, beren erakundeak PCI DSS araudia betetzen jarraitzeko, erakundeko administratzaileek aukeratu beharko lukete kreditu-txartelen zenbakiak ez gordetzea edo hash-txartelen zenbakiak gordetzea.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
