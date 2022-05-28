---
title: Kudeatu produktuetan oinarritutako kontratuaren lerroen unitate konplexuak - arina
description: Gai honek harpidetzan oinarritutako produktuen salmentari laguntzeko informazioa eskaintzen du.
author: rumant
ms.date: 10/28/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 214593c5b3fbfc5194031af3d3bef59d01750099
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8593965"
---
# <a name="manage-complex-units-for-product-based-contract-lines---lite"></a>Kudeatu produktuetan oinarritutako kontratuaren lerroen unitate konplexuak - arina

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Dynamics 365 Project Operations-ek kantitate faktoreak erabiltzen ditu harpidedun oinarritutako produktuen salmenta sustatzeko. Harpidetzetan oinarritutako produktuetarako, kontratuan edo proiektuaren kontratuaren lerroan erabiltzaile-hilabete kopurua adierazten da.

Harpidedun softwarearen prezioa katalogoan gordetzen da erabiltzaile bakoitzeko prezio gisa. Salmenta prozesuan, kontratuaren lerroko prezioa erabiltzaile bakoitzeko, salmentako agentearen bidez negoziatu eta deskontatu zen hileko prezioa izan ohi da. Akordio bakoitzak erabiltzaile kopurua eta harpidetza hilabete desberdinak ditu. Kontratuaren lerroaren zenbatekoa kalkulatzeko erabiltzen den kantitatea erabiltzaile kopurua eta harpidetza hilabeteen produktua da.

Salmenta mota hori onartzeko, Project Operations laguntzak *kantitate faktoreen* kontzeptua sartu zuen. Kopuru-faktoreek produktuaren atributuetan oinarritzen dira. Produktu baterako propietate espezifikoak konfiguratzen dituzunean, propietate horien edo propietate guztien azpimultzoa uzten dizu kantitate faktore gisa.

Project Operations-ek balioztatzen du zenbakizko datu mota bat duten zenbakizko propietateak edo produktuaren propietateak kantitate faktore gisa markatzen direla. Konfiguratutako kantitate faktoreak dituen produktu bat kontratu lerro bati gehitzen zaionean, **Kopurua** eremua irakurtzeko soilik bihurtzen da. Kantitate faktoreak diren produktuaren propietateen balioak sartu ondoren, Project Operations-ek kontratuaren lerroaren kantitatea kalkulatzen du.

Adibidez, Dynamics 365 Sales-ek propietate hauek izan ditzake:

- **Erabiltzaile kop**: erabiltzaile kopurua.
- **Hilabete kop**: harpidetza-hilabete kopurua.
- **Produktuaren SKUa** : Produktuaren stock unitatea (SKU).

**Erabiltzaile kop** eta **Hilabete kop** propietateak kantitate faktore gisa markatu daitezke produktuaren lerroko propietateak editatzean.

Produktuaren propietateetatik kantitate faktoreak sortzeko, jarraitu urrats hauek.

1. **Project Operations** aukeran, hautatu **Salmenta-produktuak**.
2. Ireki kantitate faktoreak ezarri behar dituzun produktua. Ziurtatu produktuak dagoeneko konfiguratutako propietateak dituela.
3. **Proiektuaren informazioa** orrian, hautatu **Zenbatekoaren faktoreak** fitxa.
4. Azpisaretan, hautatu **+ Eremu berriaren konputazioa**.
5. Idatzi **Kopuru faktorea** eremuaren izena eta hautatu eremuaren kalkuluarekin mapatzen den propietate balioa.
6. Gorde eta itxi inprimakia.
7. Errepikatu 2-6 urratsak batera produktuan oinarritutako kontratu linearen kopurua osatuko duten propietate guztientzat.

Kopuru faktoreak konfiguratuta, erabiltzaileak produktu honetarako kontratu lerro bat sortzen duenean, kontratu lerroaren kopurua blokeatuta dago. Kopurua kontratu lerro horretako jabetza balioen produktu gisa kalkulatzen da.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]