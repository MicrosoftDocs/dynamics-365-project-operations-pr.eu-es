---
title: Eman ingurune berri bat
description: Artikulu honek Project Operations ingurune berri bat hornitzeari buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 09/13/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 78f40ebe79c038799fbc59902442ad6c23fb94d4
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/18/2022
ms.locfileid: "9028482"
---
# <a name="provision-a-new-environment"></a>Eman ingurune berri bat

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_



Artikulu honek berri bat hornitzeari buruzko informazioa eskaintzen du Dynamics 365 Project Operations baliabideetan/ez hornituta oinarritutako eszenatokietarako ingurunea.

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a>Gaitu Project Operations hornidura automatikoa LCS proiektu batean

Erabili urrats hauek zure LCS proiekturako Project Operations hornidura-fluxu automatikoa gaitzeko.

1. Joan [LCS](https://lcs.dynamics.com/v2) aukerara eta hautatu **Aurreikusi funtzioen kudeaketa** lauza.
2. **Aurrebista eginbidea** zerrendan, hautatu **Project Operations eginbidea** eta, ondoren, hautatu **Aurrebista eginbidea gaituta** Project Operations gaitzeko.

   > [!NOTE]
   > Urrats hau LCS proiektu bakoitzeko behin bakarrik egiten da.

## <a name="provision-a-project-operations-environment"></a>Project Operations ingurunea hornitzea

1. Ireki Dynamics 365 Finance berri bat [demo ingurunea](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) edo [sandbox/produkzio ingurunea](/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) hedapena. 
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

     ![Inplementazio-ezarpenak.](./media/1DeploymentSettings.png)

    > [!IMPORTANT]
    > Aukeratu **Ados** zerbitzuaren baldintzak onartzeko eta ondoren hautatu **Eginda** inplementazio-ezarpenetara itzultzeko.
    >
    >![Inplementazioaren onespena.](./media/2DeploymentConsent.png)

7. Aukerakoa - Aplikatu demo datuak inguruneari. Joan **Ezarpen aurreratuak** aukerara, hautatu **Pertsonalizatu SQL datu basearen konfigurazioa**, eta ezarri **Zehaztu datu-basea aplikazioen datu-baserako** **Demoa** gisa.
8. Osatu morroian beharrezko gainerako eremuak eta berretsi inplementazioa. Ingurunea hornitzeko denbora aldatu egiten da ingurune motaren arabera. Hornidurak sei ordu behar izan ditzake.

   Inplementazioa ondo burutu ondoren, ingurunea honela agertuko da **Inplementatuta**.

9. Ingurunea behar bezala zabaldu dela baieztatzeko, hautatu **Hasi saioa** eta saioa hasi ingurunean berresteko.

    ![Ingurumen-xehetasunak.](./media/3EnvironmentDetails.png)

## <a name="apply-updates-to-the-finance-environment"></a>Aplikatu eguneratzeak Finance ingurunean

Project Operations-ek Finance ingurunea behar dute aplikazioaren **10.0.13 (10.0.569.20009)** bertsioarekin edo berriagoarekin.

Baliteke kalitate-eguneratzeak aplikatzea zure Finance inguruneari bertsio hau jasotzeko.

1. LCSn **Ingurumenaren xehetasunak** orrialdean, **Eguneratze erabilgarriak** sekzioan, hautatu **Ikusi eguneratzea**.

    ![Ikusi eguneratzeak.](./media/5ViewUpdates.png)

2. **Eguneratze bitarrak** orrialdean, hautatu **Gorde paketea.**

    ![Gorde paketea.](./media/6SavePackage.png)

3. Sakatu **Hautatu guztiak** eta hautatu **Gorde paketea**.

    ![Berrikusi eta gorde eguneratzeak.](./media/7ReviewAndSaveUpdates.png)

4. Idatzi paketearen izena eta deskribapena, eta hautatu **Gorde**. Interneteko konexioaren arabera, baliteke prozesu honek denbora pixka bat behar izatea.

    ![Kargatu paketea Aktiboen liburutegira.](./media/8UploadPackageToAssetsLibrary.png)

5. Paketea gorde ondoren, hautatu **Eginda** eta gorde pakete hau Aktiboen liburutegian zure LCS proiektuan.

   Paketea gorde eta balioztatzeak ~ 15 minutu behar izan ditzake.

6. Eguneratzea aplikatzeko, joan **Ingurumenaren xehetasunak** orrialdea LCSn eta hautatu **Mantendu** > **Aplikatu eguneratzeak**.

    ![Mantendu inguruneak.](./media/9MaintainEnvironment.png)

7. Eguneratzeen zerrendan hautatu sortu duzun paketea eta hautatu **Aplikatu**.

    ![Aplikatu eguneratzeak.](./media/10ApplyUpdates.png)

   Ingurumena zaintzeko denbora pixka bat beharko da. Bukatu ondoren, ingurunea hedatutako egoerara itzuliko da.

    ![Inplementatutako inguruneak.](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a>Ezarri idazketa dualeko konexioa 

1. Zure LCS proiektuan, joan **Ingurumenaren xehetasunak** orrialdera.
2. **Common Data Service Ingurumenari buruzko informazioa** aukeran, hautatu **Lotu aplikazioetarako CDS**.
3. Esteka osatu ondoren, hautatu **Estekatu aplikazioetarako CDS** berriro. Finantzetan Idazketa Dualera bideratuko zaituzte.

    ![Estekatu CDSra.](./media/12LinktoCDS.png)

4. Aukeratu **Aplikatu irtenbidea** integrazioan mapatuko diren entitateetara sartzeko.

    ![Aplikatu soluzioak.](./media/13ApplySolutions.png)

5. Aukeratu bi irtenbideak, **Dynamics 365 Finance Idazketa bikoitzeko entitateen mapa** eta **Dynamics 365 Project Operations Idazketa bikoitzeko entitateen mapak**, eta gero hautatu **Aplikatu**.

    ![Berretsi irtenbideak.](./media/14ConfirmSolutions.png)

    Irtenbideak aplikatu ondoren, Idazketa Dualeko entitateak inguruneari aplikatuko zaizkio.

    ![Soluzioak aplikatzea.](./media/15ApplyingSolutions.png)

    Entitateak aplikatu ondoren, erabilgarri dauden mapaketa guztiak ingurunean zerrendatzen dira.

    ![Idazketa dualaren esleipenak.](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a>Freskatu datu-entitateak eguneratu ondoren

1. Finantzetan, joan **Datuen kudeaketa** lan eremua.

    ![Datu-kudeaketaren laneko area.](./media/16DataManagement.png)

2. Aukeratu **Esparru parametroak** lauza.

    ![Esparru-parametroak.](./media/17FrameworkParameters.png)

3. **Entitatearen ezarpenak** orrialdean, hautatu **Freskatu entitate zerrenda**.

    ![Freskatu entitate-zerrenda.](./media/18RefreshEntityList.png)

Freskatzeak 20 minutu inguru iraungo du. Amaitutakoan alerta jasoko duzu.

  ![Freskatzeko berrespena.](./media/19RefreshConfirmation.png)

## <a name="update-security-settings-on-project-operations-on-dataverse"></a>Eguneratu Project Operations-eko segurtasun-ezarpenak aktibatuta Dataverse-n

1. Joan Project Operations aukerara, Dataverse ingurunean. 
2. Joan **Ezarpenak** > **Segurtasuna** > **Segurtasun-funtzioak** aukerara. 
3. **Segurtasun-funtzioak** orrialdean, funtzioen zerrendan, hautatu **idazketa bikoitzeko aplikazioaren erabiltzailea** eta hautatu **Entitate pertsonalizatuak** fitxa.  
4. Egiaztatu rolak **Irakurri** eta **Erantsi honi** baimenak dituela entitate hauetarako:
      
      - **Monetaren truke-tasaren mota**
      - **Kontuen sailkapena**
      - **Egutegi fiskala**
      - **Liburua**
      - **Enpresa**
      - **Gastua**

5. Segurtasun-funtzio eguneratu ondoren, joan **Ezarpenak** > **Segurtasuna** > **Taldeak** aukerara, eta hautatu lehenetsitako taldea **Tokiko negozioaren jabea** taldearen ikuspegia.
6. Aukeratu **Kudeatu funtzioak** eta egiaztatu **idazketa bikoitzeko aplikazioaren erabiltzailea** segurtasun-pribilegioa talde honi aplikatzen zaio.

## <a name="run-project-operations-dual-write-maps"></a>Exekutatu Proiektuaren eragiketen idazketa dualaren esleipenak

1. Zure LCS proiektuan, joan **Ingurumenaren xehetasunak** orrialdera.
2. **Common Data Service Ingurumenari buruzko informazioa** aukeran, hautatu **Lotu aplikazioetarako CDS**. Esteka hautatu ondoren, mapen entitateen zerrendara birbideratuko zaituzte.
3. Hasi mapak. Informazio gehiagorako, ikusi [Project Operations idazketa dualeko mapen bertsioak](resource-dual-write-maps.md#project-operations-dual-write-maps)
4. Balioztatu proiektuarekin lotutako mapa guztiak martxan daudenean.

    ![Mapa guztiak martxan.](./media/22AllMapsRunning.png)


## <a name="apply-configuration-data-in-cds-for-project-operations-optional"></a>Aplikatu konfigurazio-datuak Project Operations-en CDS-n (aukerakoa)

Demo datuak Finantza inguruneari aplikatu badizkiozu, ikusi [Konfiguratu eta aplikatu konfigurazio datuak Common Data Service Project Operations-erako](resource-apply-pro-setup-config-data.md) CDS inguruneari demo datuak aplikatzeko.


Zure Project Operations ingurunea hornitu eta konfiguratuta dago orain. 


[!INCLUDE[footer-include](../includes/footer-banner.md)]
