---
title: Enpresa-eragiketak Proiektu Eragiketetan
description: Gai honek Microsoft-en negozio-transakzioen kontzeptuaren ikuspegi orokorra eskaintzen du Dynamics 365 Project Operations.
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
ms.openlocfilehash: 0c6fe583af0dcaa62204b35c1093746b13b6e00e
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8582189"
---
# <a name="business-transactions-in-project-operations"></a>Enpresa-eragiketak Proiektu Eragiketetan

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako Project Operations, Lite hedapena - proformaren fakturazioari aurre egitea_

Microsoft-en Dynamics 365 Project Operations, *transakzioa* kontzeptu abstraktu bat da, edozein entitatek adierazten ez duena. Hala ere, zenbait entitateren eremu eta prozesu komun batzuk negozio-transakzioen kontzeptua erabiltzeko diseinatuta daude. Entitate hauek abstrakziorako erabiltzen dira:

- Eskaintzaren lerroaren xehetasunak
- Kontratuaren lerroaren xehetasunak
- Aurreikuspenaren lerroak
- Kutxako liburuaren lerroak
- Benetakoak

Entitate hauetatik, Aurrekontu lerroaren xehetasunak, Kontratuaren lerroaren xehetasunak eta Estimazioaren lerroak mapan daude *estimazio fasea* proiektuaren bizi-zikloan. Aldizkari-lerroak eta Errealak entitateak mapan daude *exekuzio fasea* proiektuaren bizi-zikloan.

Project Operations-ek bost entitate horietako erregistroak negozio-transakzio gisa hartzen ditu. Bereizketa bakarra estimazio-fasean mapatzen diren entitateetako erregistroak (Kuota-lerroaren xehetasunak, Kontratu-lerroaren xehetasunak eta Estimazio-lerroak) kontuan hartzen dira.*finantza-aurreikuspenak*, berriz, exekuzio fasera mapatzen diren entitateetako erregistroak (Aldizkaria lerroak eta Errealak) kontuan hartzen dira.*finantza-gertaerak* dagoeneko gertatu direnak.

Informazio gehiago lortzeko, ikusi [Aurreikuspenak](../project-management/estimating-projects-overview.md) eta [Benetako datuak](actuals-overview.md).

## <a name="concepts-that-are-unique-to-business-transactions"></a>Negozio-transakzioetarako soilik diren kontzeptuak

Kontzeptu hauek negozio-transakzioen kontzeptuarentzat bakarrak dira:

- Transakzio mota
- Transakzio-klasea
- Transakzioaren jatorria
- Transakzio-konexioa

### <a name="transaction-type"></a>Transakzio mota

Transakzio motak proiektu baten finantza-eraginaren denbora eta testuingurua adierazten ditu. Proiektuaren Eragiketetan onartzen diren balio hauek dituen aukera multzo batek definitzen du:

- Kostua
- Proiektu-kontratua
- Fakturatu gabeko salmentak
- Fakturatutako salmentak
- Erakunde arteko salmentak
- Baliabidearen unitate-kostua

### <a name="transaction-class"></a>Transakzio-klasea

Transakzio klaseak proiektuetan sortzen diren kostu mota ezberdinak adierazten ditu. Proiektuaren Eragiketetan onartzen diren balio hauek dituen aukera multzo batek definitzen du:

- Ordua
- Gastua
- Materiala
- Prezioa
- Mugarria
- Zergak

> [!NOTE]
> The **Mugarria** Balioa normalean negozio-logikak erabiltzen du proiektu-eragiketetan prezio finkoko fakturaziorako.

### <a name="transaction-origin"></a>Transakzioaren jatorria

Transakzioaren jatorria negozio-transakzio bakoitzaren jatorria gordetzen duen entitate bat da, txostenak egiten eta trazabilitatean laguntzeko. Proiektua gauzatzen hasten den heinean, negozio-transakzio bakoitzak beste negozio-transakzio bat sortzen du, eta, aldi berean, beste negozio-transakzio bat sortuko du, eta abar.

### <a name="transaction-connection"></a>Transakzioaren konexioa

Transakzio-konexioa antzeko bi negozio-transakzioren arteko erlazioa gordetzen duen entitate bat da, hala nola, kostuak eta erlazionatutako salmenten errealak edo fakturazio-jarduerek abiarazten dituzten transakzio-itzulketak, hala nola fakturaren berrespena edo fakturaren zuzenketak.

Elkarrekin, Transakzio-jatorria eta Transakzio-konexio-entitateek negozio-transakzioen eta negozio-transakzio zehatz bat sortzea eragin duten ekintzen arteko erlazioak jarraitzen laguntzen dizute.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
