---
title: Eman ingurune berri bat
description: Gai honek Project Operations ingurune berri bat emateari buruzko informazioa eskaintzen du.
author: sigitac
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 044a942a068b33318b98041cc94944d90c1d63c3
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121158"
---
# <a name="provision-a-new-environment"></a>Eman ingurune berri bat

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai honek Dynamics 365 Project Operations ingurune berri bat emateko moduari buruzko informazioa eskaintzen du berreskuratutako / stockean oinarritutako eszenatokietarako.

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a>Gaitu Project Operations hornidura automatikoa LCS proiektu batean

Erabili urrats hauek zure LCS proiekturako Project Operations hornidura-fluxu automatikoa gaitzeko.

1. Joan [LCS](https://lcs.dynamics.com/v2) aukerara eta hautatu **Aurreikusi funtzioen kudeaketa** lauza.
2. **Aurrebista eginbidea** zerrendan, hautatu **Project Operations eginbidea** eta, ondoren, hautatu **Aurrebista eginbidea gaituta** Project Operations gaitzeko.

> [!NOTE]
> Urrats hau LCS proiektu bakoitzeko behin bakarrik egiten da.

## <a name="provision-a-project-operations-environment"></a>Project Operations ingurunea hornitzea

1. Ireki Dynamics 365 Finance [demo-ingurunea](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) edo [sandbox / produkzio ingurunea](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) inplementazioa. 
2. **Ingurumen hornidura** morroia eramatea. 

> [!IMPORTANT]
> Ziurtatu hautatutako aplikazioaren bertsioa 10.0.13 edo berriagoa dela.

3. Project Operations hornitzeko, **Ezarpen aurreratuak** aukeran, hautatu **Common Data Service**. 
4. Gaitu **Common Data Service ezarpena** **Bai** hautatuta, eta ondoren sartu informazioa beharrezko eremuetan:

  - Izena
  - Eskualdea
  - Hizkuntza
  - Moneta
 
5. **Common Data Service txantiloia** eremuan, hautatu **Project Operations** 

6. Hautatu inplementazioaren ingurune mota. Harpidetzan oinarritutako probak CDS ingurunea 30 egunez zabaltzen utziko dizu. 

![Inplementazio-ezarpenak](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> Aukeratu **Ados** zerbitzuaren baldintzak onartzeko eta ondoren hautatu **Eginda** inplementazio-ezarpenetara itzultzeko.

![Inplementazioaren onespena](./media/2DeploymentConsent.png)

7. Osatu morroian beharrezko gainerako eremuak eta berretsi inplementazioa. Ingurumena hornitzeko denbora aldatu egiten da ingurune motaren arabera. Hornidurak sei ordu behar izan ditzake.

  Inplementazioa ondo burutu ondoren, ingurunea honela agertuko da **Inplementatuta**.

8. Ingurunea ondo zabaldu dela ziurtatzeko, hautatu **Saioa hasi** eta saioa hasi ingurunean berresteko.

![ Ingurune-xehetasunak](./media/3EnvironmentDetails.png)

## <a name="apply-project-operations-finance-demo-data-optional-step"></a>Aplikatu Project Operations Finance demo-datuak (aukerako urratsa)

Aplikatu Project Operations Finance demo-datuak 10.0.13 zerbitzuaren bertsioan Hodeian ostatatutako ingurunean deskribatutako moduan [artikulu hau](resource-apply-finance-demo-data.md).

## <a name="apply-updates-to-the-finance-environment"></a>Aplikatu eguneratzeak Finance ingurunean

Project Operations-ek Finance ingurunea behar dute aplikazioaren **10.0.13 (10.0.569.20009)** bertsioarekin edo berriagoarekin.

Baliteke kalitate-eguneratzeak aplikatzea zure Finance inguruneari bertsio hau jasotzeko.

1. LCSn **Ingurumenaren xehetasunak** orrialdean, **Eguneratze erabilgarriak** sekzioan, hautatu **Ikusi eguneratzea**.

![Ikusi eguneratzeak](./media/5ViewUpdates.png)

2. **Eguneratze bitarrak** orrialdean, hautatu **Gorde paketea.**

![Gorde paketea](./media/6SavePackage.png)

3. Sakatu **Hautatu guztiak** eta hautatu **Gorde paketea**.

![Berrikusi eta gorde eguneratzeak](./media/7ReviewAndSaveUpdates.png)

4. Idatzi paketearen izena eta deskribapena, eta hautatu **Gorde**. Interneteko konexioaren arabera, baliteke prozesu honek denbora pixka bat behar izatea.

![Kargatu paketea Aktiboen liburutegira](./media/8UploadPackageToAssetsLibrary.png)

5. Paketea gorde ondoren, hautatu **Eginda** eta gorde pakete hau Aktiboen liburutegian zure LCS proiektuan.

Paketea gorde eta balioztatzeak ~ 15 minutu behar izan ditzake.

6. Eguneratzea aplikatzeko, joan **Ingurumenaren xehetasunak** orrialdea LCSn eta hautatu **Mantendu** > **Aplikatu eguneratzeak**.

![Mantendu inguruneak](./media/9MaintainEnvironment.png)

7. Eguneratzeen zerrendan hautatu sortu duzun paketea eta hautatu **Aplikatu**.

![Aplikatu eguneraketak](./media/10ApplyUpdates.png)

Ingurumena zaintzeko denbora pixka bat beharko da. Bukatu ondoren, ingurunea hedatutako egoerara itzuliko da.

![Inplementatutako inguruneak](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a>Ezarri idazketa dualeko konexioa 

1. Zure LCS proiektuan, joan **Ingurumenaren xehetasunak** orrialdera.
2. **Common Data Service Ingurumenari buruzko informazioa** aukeran, hautatu **Lotu aplikazioetarako CDS**.
3. Esteka osatu ondoren, hautatu **Estekatu aplikazioetarako CDS** berriro. Finantzetan Idazketa Dualera bideratuko zaituzte.

![Estekatu CDSra](./media/12LinktoCDS.png)

4. Aukeratu **Aplikatu irtenbidea** integrazioan mapatuko diren entitateetara sartzeko.

![Aplikatu soluzioak](./media/13ApplySolutions.png)

5. Aukeratu bi irtenbideak, **Dynamics 365 Finance and Operations Idazketa bikoitzeko entitateen mapa** eta **Dynamics 365 Project Operations Idazketa bikoitzeko entitateen mapak** eta, ondoren, hautatu **Aplikatu**.

![Berretsi irtenbideak](./media/14ConfirmSolutions.png)

Irtenbideak aplikatu ondoren, Idazketa Dualeko entitateak inguruneari aplikatuko zaizkio.

![Soluzioak aplikatzea](./media/15ApplyingSolutions.png)

Entitateak aplikatu ondoren, erabilgarri dauden mapaketa guztiak ingurunean zerrendatzen dira.

![Idazketa dualaren esleipenak](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a>Freskatu datu-entitateak eguneratu ondoren

1. Finantzetan, joan **Datuen kudeaketa** lan eremua.

![Datu-kudeaketarren laneko area](./media/16DataManagement.png)

2. Aukeratu **Esparru parametroak** lauza.

![Esparru-parametroak](./media/17FrameworkParameters.png)

3. **Entitatearen ezarpenak** orrialdean, hautatu **Freskatu entitate zerrenda**.

![Freskatu entitate-zerrenda](./media/18RefreshEntityList.png)

Freskatzeak 20 minutu inguru iraungo du. Amaitutakoan alerta jasoko duzu.

![Freskatzeko berrespena](./media/19RefreshConfirmation.png)

## <a name="run-project-operations-dual-write-maps"></a>Exekutatu Proiektuaren eragiketen idazketa dualaren esleipenak

1. Zure LCS proiektuan, joan **Ingurumenaren xehetasunak** orrialdera.
2. **Common Data Service Ingurumenari buruzko informazioa** aukeran, hautatu **Lotu aplikazioetarako CDS**. Esteka hautatu ondoren, mapen entitateen zerrendara birbideratuko zaituzte.
3. Hasi esleipenak hurrengo taulan deskribatzen den bezala. Ziurtatu zerrendatutako sekuentzia jarraitzen duzula.

| **Entitate-esleipena** | **Freskatu entitatea** | **Hasierako sinkronizazioa** | **Hasierako sinkronizazioaren eredua** | **Exekutatu aurrebaldintzak** | **Aurrebaldintzen hasierako sinkronizazioa** |
| --- | --- | --- | --- | --- | --- |
| **Enpresa guztientzako proiektuaren baliabideen eginkizunak (bookableresourcecategories)** | +Ez | Yes | Common Data Service | +Ez | E/E |
| **Legezko entitateak (cdm\_companies)** | +Ez | Yes | Finance and Operations aplikazioak | +Ez | E/E |
| **Project Operations-en integrazioaren benetako datuak (msdyn\_actuals)** | +Ez | +Ez | E/E | Yes | +Ez |
| **Proiektuetako kontratuaren lerroak (salesorderdetails)** | +Ez | +Ez | E/E | +Ez | +Ez |
| **Proiektuen transakzio harremanetarako integrazio entitatea (msdyn\_transactionconnections)** | +Ez | +Ez | E/E | +Ez | E/E |
| **Project Operations-ek integratzeko kontratu lerroaren mugarriak (msdyn\_contractlinesscheduleofvalues)** | +Ez | +Ez | E/E | +Ez | E/E |
| **Project Operations-ek integratzeko entitatea gastuen kalkuluen arabera (msdyn\_estimateslines)** | +Ez | +Ez | E/E | +Ez | E/E |
| **Project Operations-ek integratzeko proiektuaren gastuak kategoriak esportatzeko entitatea (msdyn\_expensecategories)** | +Ez | +Ez | E/E | +Ez | E/E |
| **Project Operations-ek integratzeko proiektuaren gastuak esportatzeko entitatea (msdyn\_expenses)** | Yes | +Ez | E/E | +Ez | E/E |
| **Project Operations-ek integratzeko entitatea orduen kalkuluen arabera (msdyn\_resourceassignments)** | Yes | +Ez | E/E | +Ez | E/E |


4. Entitatea freskatzeko, hautatu maparen izena eta hautatu **Freskatu entitateak**. 


![Freskatu mapa](./media/20RefreshMapping.png)

5. Freskatzen osatu eta gero, exekutatu mapa. Hurrengo mapa gaitu aurretik, egiaztatu taulako mapa egoera batean dagoela **Exekutatzen**. Aurrebaldintza kopuru handiagoa duten mapak exekutatzeak denbora pixka bat behar izan dezake.

Aurrebaldintzak dituen mapa exekutatzeko, gaitu **Erakutsi erlazionatutako entitateen mapak** txandakatu. Taulak adierazten badu **Hasierako sinkronizazioa** da **Ez**, egiaztatu **Hasierako sinkronizazioa** bandera da **Desaktibatuta** exekutatu aurretik aurrebaldintza-mapa guztietan.

![Exekutatu mapa](./media/21RunMap.png)

6. Balioztatu proiektuarekin lotutako mapa guztiak martxan daudenean.

![Mapa guztiak martxan](./media/22AllMapsRunning.png)


## <a name="apply-configuration-data-in-cds-for-project-operations-optional"></a>Aplikatu konfigurazio-datuak Project Operations-en CDS-n (aukerakoa)

Demo datuak Finantza inguruneari aplikatu badizkiozu, ikusi [Konfiguratu eta aplikatu konfigurazio datuak Common Data Service Project Operations-erako](resource-apply-pro-setup-config-data.md) CDS inguruneari demo datuak aplikatzeko.


Zure Project Operations ingurunea hornitu eta konfiguratuta dago orain. 
