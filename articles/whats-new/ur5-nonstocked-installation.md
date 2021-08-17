---
title: Eguneratu Project Operations zure Finantza ingurunean
description: Gai honek Project Operations Dynamics 365 Finance ingurunean nola eguneratu jakiteko informazioa eskaintzen du.
author: ruhercul
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 3665bccfa25c759c0f2351c691d24901867c178f7c339f4a524856842666aec5
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6986746"
---
# <a name="update-project-operations-in-your-finance-environment"></a>Eguneratu Project Operations zure Finantza ingurunean

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_


Gai honek Dynamics 365 Project Operations Dynamics 365 Finance ingurunean nola eguneratu jakiteko informazioa eskaintzen du. Project Operations-ek 5 eguneratzera (UR5) eguneratzeko hiru prozedura behar dira:

- [Inportatu paketea aurrebista proiektuan](#import)
- [Aplikatu eguneratzea](#apply)
- [Eguneratu Dataverse ingurunea](#update)

## <a name="import-the-package-into-your-lcs-project"></a><a name="import"></a>Inportatu paketea LCS proiektura

1. Hasi saioa [Lifecycle Services-en (LCS)](https://lcs.dynamics.com/) Proiektuaren jabe edo Ingurumen kudeatzaile gisa.
2. Proiektuen zerrendan, hautatu zure LCS proiektua.
3. **Proiektua** orrialdean, **Inguruneak** taldean, ireki eguneratu nahi duzun ingurunea.
4. Egiaztatu ingurunea martxan dagoela. Hasten ez bada, hasi ingurunea.
5. **Argitalpen berria** sekzioan, **Eguneratze erabilgarriak** atalean, hautatu **Ikusi eguneratzea** 10.0.15 bertsioarena.

![Ikusi eguneratzea botoia.](media/view-update.png)

6. **Eguneratze bitarrak** orrialdean, hautatu **Gorde paketea**.
7. **Berrikusi eta gorde eguneratzeak** orrialdean, hautatu **Gorde paketea**.
8. Irekitzen den **Gorde paketea aktiboen liburutegian** panelean, sartu paketearen izena eta hautatu **Gorde paketea**.
9. LCS paketea gordetzen amaitutakoan, **Eginda** botoia gaituta dago. Hautatu **Eginda**. LCS-k paketea egiaztatuko du. Egiaztapenak minutu batzuk edo gehienez ordubete iraun dezake.


## <a name="apply-the-package-update"></a><a name="apply"></a>Aplikatu pakete-eguneratzea

1. LCSn **Ingurumenaren xehetasunak** orrialdean, hautatu **Mantendu** > **Aplikatu eguneratzeak**.
2. Zerrendan, hautatu lehen gordetako paketea, eta hautatu **Aplikatu**.
3. Aukeratu **Bai** paketea zabaldu nahi duzula baieztatzeko.

![Berretsi paketeak inplementatzeko elkarrizketa-koadroa.](media/confirm-package-deployment.png)

4. Aukeratu **Bai** aplikazioa eguneratu nahi duzula baieztatzeko.

![Berretsi aplikazioa eguneratzeko elkarrizketa-koadroa.](media/confirm-application-update.png)

Inplementazioa eta aplikazioaren eguneratzea hasiko da. 

**Ingurumenaren xehetasunak** orrialdean, goiko eskuineko izkinan, ingurunearen egoera **Zerbitzua ematea** aukerara eguneratuko da. Bi ordutan gutxi gorabehera, eguneratzea osatuko da. Aplikazioaren bertsioaren informazioa eguneratu egingo da **Microsoft Dynamics 365 for Finance and Operations 10.0.15)** eta ingurunearen egoera eguneratu egingo da **Inplementatuta**.


## <a name="update-your-dataverse-environment"></a><a name="update"></a>Eguneratu Dataverse ingurunea

1. Hasi saioa hurrengoan [Power Platform administrazio-zentroa](https://admin.powerplatform.com/).
2. Zerrendan, bilatu eta ireki Project Operations instalatzeko erabili zenuen ingurunea.
3. **Inguruneak** orrialdean, hautatu **Baliabidea** > **Dynamics 365 aplikazioak**.
4. Zerrendan, bilatu **Microsoft Dynamics 365 Project Operations**, eta **Egoera** zutabean, hautatu **Eguneratzea eskuragarri**.
5. Aukeratu **Zerbitzu baldintzak onartzen ditut** kontrol laukia eta, ondoren, hautatu **Eguneratu**. Soluzioaren azken bertsioa instalatuko da.

Instalazioa amaitu ondoren, 4.5.0.134 bertsioa instalatuta izango duzu.

## <a name="configure-new-features"></a>Konfiguratu eginbide berriak

### <a name="enable-dual-write-mapping"></a>Gaitu idazketa dualaren esleipenak

Finance eta Dataverse inguruneak eguneratu eta gero, beharrezko idazketa bikoitzeko mapak gaitu ditzakezu. Osatu prozedura hauek, idazketa dualerako esleipenak gaitzeko.

- [Eguneratu segurtasun-ezarpenak Customer Engagement ingurunean](#security)
- [Freskatu datu-entitateak](#refresh)
- [Eguneratu eta exekutatu idazketa bikoitzeko mapak](#run)

### <a name="update-security-settings-on-the-dataverse-environment"></a><a name="security"></a>Eguneratu segurtasun-ezarpenak Dataverse ingurunean

Entitateen segurtasun pribilegioen eguneratze hauek beharrezkoak dira UR5 eguneratzearen barruan.

1. Dataverse ingurunean, joan **Ezarpenak** aukerara, eta **Sistema** taldean, hautatu **Segurtasuna**.

![Dataverse ingurune-ezarpenak.](media/Picture21.png)

2. Hautatu **Segurtasun-funtzioak**.
3. Funtzioen zerrendan, hautatu **idazketa bikoitzeko aplikazioaren erabiltzailea** eta hautatu **Entitate pertsonalizatuak** fitxa. 
4. Egiaztatu rolak funtzioak badituela **Irakurri** eta **Erantsi honi** honetarako baimenak:

      - **Monetaren truke-tasaren mota**
      - **Kontuen sailkapena** 
      - **Egutegi fiskala** 
      - **Liburua**

5. Segurtasun-funtzio eguneratu ondoren, joan **Ezarpenak** > **Segurtasuna** > **Taldeak** aukerara. Egiaztatu **idazketa bikoitzeko aplikazioaren erabiltzailea** funtzioa aplikatu zaio taldeari. 

### <a name="refresh-data-entities-from-the-update"></a><a name="refresh"></a>Freskatu datu entitateak eguneratzetik

1. Zure Finance ingurunean, ireki **Datuen kudeaketa** laneko eremua eta, ondoren, ireki **Esparru parametroak** orrialdea.
2. **Entitatearen ezarpenak** fitxan, hautatu **Freskatu entitate zerrenda**.
3. Aukeratu **Itxi** entitatearen freskatzea baieztatzeko.

 > [!NOTE]
 > Prozesu horrek 20 bat minutu artean iraun dezake. Freskapena amaitutakoan jakinaraziko zaizu.

### <a name="update-dual-write-mappings"></a><a name="run"></a>Eguneratu idazketa dualaren esleipenak

1. **Datuen kudeaketa** lan-eremuan, hautatu **Idazketa bikoitza**.
2. Aukeratu **Aplikatu soluzioak**, hautatu bi irtenbideak zerrendan eta, ondoren, hautatu **Aplikatu**.
3. **Idazketa bikoitza** orrialdean, hautatu taula-esleipen hauek eta hautatu **Gelditu**.

    - **Project Operations-en integrazioaren benetako datuak (msdynactuals)**
    - **Project Operations-en integratzeko proiektuaren gastuen kategoriak (msdyn_expensecategories)**
    - **Project Operations-en integratzeko benetako datuen proiektuaren gastuen esportazio-entitatea (msdyn_expenses)**

4. **Taula-esleipenaren bertsioa** orrian, aplikatu maparen bertsio berria hiru entitate bakoitzari.
5. **Idazketa bikoitza** orrian, hautatu exekutatu mapak berrabiarazteko.
6. Mapen zerrendan, hautatu **Liburua (msdyn_ledgers)** mapa aurrebaldintza guztiekin eta hautatu **Hasierako sinkronizazioa** kontrol-laukia. 
7. **Hasierako sinkronizaziorako nagusia** eremuan, hautatu **Finance and Operations aplikazioak** eta, ondoren, hautatu **Exekutatu**.
 
 ![Liburuaren esleipenaren sinkronizazioa.](media/DW6.png)
 


[!INCLUDE[footer-include](../includes/footer-banner.md)]