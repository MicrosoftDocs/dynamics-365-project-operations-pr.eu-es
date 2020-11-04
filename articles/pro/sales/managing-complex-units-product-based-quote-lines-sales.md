---
title: Unitate konplexuak kudeatzea; adibidez, erabiltzaile bakoitzeko, hileroko produktuetan oinarritutako eskaintzaren lerroetarako
description: Gai honek produktuetan oinarritutako eskaintza-lerroetako unitate konplexuak kudeatzeari buruzko lerroei buruzko informazioa ematen du.
author: rumant
manager: Annbe
ms.date: 10/06/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 741230e69302138cce8f7379f520f7178e1c80af
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070968"
---
# <a name="managing-complex-units-such-as-per-user-per-month-for-product-based-quote-lines"></a>Unitate konplexuak kudeatzea; adibidez, erabiltzaile bakoitzeko, hileroko produktuetan oinarritutako eskaintzaren lerroetarako

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Dynamics 365 Project Operations-ek kantitate faktoreak erabiltzen ditu harpidedun oinarritutako produktuen salmenta sustatzeko. Harpidetzetan oinarritutako produktuetarako, aurrekontuan edo proiektuaren kontratuaren lerroan erabiltzaile-hilabete kopurua adierazten da.

Normalean, harpidedun softwarearen prezioa katalogoan gordetzen da erabiltzaile bakoitzeko prezio gisa. Salmenta prozesuan, aurrekontuen lerroko prezioa erabiltzaile bakoitzeko, salmentako IT agentearen bidez negoziatu eta deskontatu zen hileko prezioa izan ohi da. Akordio bakoitzak erabiltzaile kopurua eta harpidetza hilabete desberdinak ditu. Aurrekontuen lerroa kalkulatzeko erabiltzen den kantitatea erabiltzaile kopurua eta harpidetza hilabeteen produktua da.

Salmenta mota hori onartzeko, Project Operations-ek kantitate faktoreen kontzeptua sartu zuen. Kopuru-faktoreek produktuaren atributuetan oinarritzen dira Dynamics 365-en. Produktu baterako propietate espezifikoak konfiguratzen dituzunean, Project Operations-ek propietate horien edo propietate guztien azpimultzoa uzten dizu kantitate faktore gisa.

Project Operations-ek balioztatzen du zenbakizko datu mota bat duten zenbakizko propietateak edo produktuaren propietateak kantitate faktore gisa markatzen direla. Aurrekontu lerro batean kantitate faktoreak dituen produktua gehitzen duzunean **Kopurua** eremua irakurtzeko soilik bihurtzen da. Kantitate faktoreak diren produktuaren propietateen balioak sartu ondoren, Project Operations-ek aurrekontuen lerroaren kantitatea kalkulatzen du.

Adibidez, Dynamics 365 Sales-ek propietate hauek izan ditzake:

- **Erabiltzaile kop** : erabiltzaile kopurua
- **Hilabete kop** : harpidetza-hilabete kopurua
- **SKU produktua**

**Erabiltzaile kop** eta **Hilabete kop** propietateak kantitate faktore gisa markatu daitezke produktuaren lerroko propietateak editatzean.

Produktuaren propietateetatik Kopuru faktoreak sortzeko, jarraitu urrats hauei:

1. Project Operations ezkerreko nabigazio-panelean, joan **Salmentak** > **Produktuak** aukerara.
2. Ireki kantitate faktoreak konfiguratu behar dituzun produktua. Ziurtatu produktuak dagoeneko konfiguratutako propietateak dituela.
3. Produktua orriko **Proiektuaren informazioa** orrian, hautatu **Kopuru faktoreak** fitxa.
4. Azpisaretan, hautatu **+ Eremu berriaren konputazioa**.
5. Idatzi Kopuru faktorearen izena eta hautatu eremuaren kalkuluarekin mapatzen den propietate balioa.
6. Gorde eta itxi inprimakia. Errepikatu urrats hauek produktuan oinarritutako aurrekontu lerroaren kantitatea kalkulatzeko erabili beharreko propietate guztietan.

Produktuan oinarritutako aurrekontu lerroa sortzen duzunean, aurrekontu lerroaren kopurua blokeatuta egongo da. Kopurua aurrekontu lerro horretarako sartu dituzun propietate balioen produktu gisa kalkulatuko da.
