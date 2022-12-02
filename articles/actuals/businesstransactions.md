---
title: Enpresa-transakzioak Project Operations-en
description: Artikulu honek negozio-transakzioen kontzeptuaren ikuspegi orokorra eskaintzen du Microsoft Dynamics 365 Project Operations.
author: rumant
ms.date: 01/31/2022
ms.topic: overview
ms.prod: ''
audience: Application User
ms.reviewer: johnmichalak
ms.search.scope: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2022-01-31
ms.openlocfilehash: fab0061af6e615c25d0fbf79d024370285dc6f86
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8923265"
---
# <a name="business-transactions-in-project-operations"></a>Enpresa-transakzioak Project Operations-en

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako Project Operations, Lite hedapena - proformaren fakturazioari aurre egitea_

Microsoft Dynamics 365 Project Operations-en , *negozio-transakzioa* edozein entitatek ordezkatzen ez duen kontzeptu abstraktua da. Hala ere, zenbait entitateren eremu eta prozesu komun batzuk negozio-transakzioen kontzeptua erabiltzeko diseinatuta daude. Entitate hauek abstrakziorako erabiltzen dira:

- Eskaintzaren lerroaren xehetasunak
- Kontratuaren lerroaren xehetasunak
- Aurreikuspenaren lerroak
- Kutxako liburuaren lerroak
- Benetakoak

Entitate horien artean, Eskaintzaren lerroaren xehetasunak, Kontratuaren lerroaren xehetasunak eta *estimazio fasean* proiektuaren bizitza zikloan zenbatetsitako fasera sailkatzen dira. Kutxako liburuaren lerroak eta Benetako datuak proiektuaren *exekuzio-fasean* kokatzen dira.

Project Operations-ek bost entitate horietako erregistroak negozio-transakzio gisa hartzen ditu. Bereizketa bakarra zera da: zenbatespen fasera esleitutako entitateetako erregistroak *finantza-aurreikuspen* (eskaintza lerroaren xehetasunak, kontratu lerroaren xehetasunak eta aurreikuspen xehetasunak) gisa hartzen direla, eta, *exekuzio fasean* esleitzen diren entitateetako erregistroak dagoeneko gertatu diren gertaera ekonomikoak direla.

Informazio gehiago lortzeko, ikusi [Aurreikuspenak](../project-management/estimating-projects-overview.md) eta [Benetako datuak](actuals-overview.md).

## <a name="concepts-that-are-unique-to-business-transactions"></a>Negozio-transakzioetarako soilik diren kontzeptuak

Kontzeptu hauek negozio-transakzioen kontzeptuarentzat bakarrak dira:

- Transakzio mota
- Transakzio-klasea
- Transakzioaren jatorria
- Transakzio-konexioa

### <a name="transaction-type"></a>Transakzio mota

Transakzio motak proiektu baten finantza-eraginaren denbora eta testuingurua adierazten ditu. Aukera multzo batek adierazten du, Project Operations-en onartutako balio hauek dituena:

- Kostua
- Proiektu-kontratua
- Fakturatu gabeko salmentak
- Fakturatutako salmentak
- Erakunde arteko salmentak
- Baliabidearen unitate-kostua

### <a name="transaction-class"></a>Transakzio-klasea

Transakzio klaseak proiektuetan sortzen diren kostu mota ezberdinak adierazten ditu. Aukera multzo batek adierazten du, Project Operations-en onartutako balio hauek dituena:

- Ordua
- Gastua
- Materiala
- Prezioa
- Mugarria
- Zergak

> [!NOTE]
> **Mugarria** negozioaren logikak Project Operations-en prezio finkoa fakturatzeko erabiltzen du.

### <a name="transaction-origin"></a>Transakzioaren jatorria

Transakzioaren jatorria entitatea transakzio bakoitzaren jatorriari buruzko datuak gordetzeko diseinatuta dago, txostenak eta trazabilitatea laguntzeko. Proiektuaren exekuzioa abian den heinean, negozio-transakzio bakoitzak beste negozio-transakzio bat sortuko du, eta horrek beste bat sortuko du, eta abar.

### <a name="transaction-connection"></a>Transakzioaren konexioa

Transakzioaren konexioa antzeko negozioen arteko bi negozioren arteko erlazioa gordetzen duen entitatea da, hala nola, kostuen eta erlazionatutako salmenten egiazkoak edo fakturazio-jarduerek eragindako transakzioen itzulketak.

Elkarrekin, transakzioaren jatorria eta transakzioen konexio-erakundeek negozio-transakzio jakin bat sortzea eragiten duten ekintzen eta negozioen arteko harremanak kontrolatzen lagunduko dizute.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
