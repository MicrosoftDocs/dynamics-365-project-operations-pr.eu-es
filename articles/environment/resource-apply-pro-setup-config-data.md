---
title: Konfiguratu eta aplikatu konfigurazio-datuak Common Data Service-n
description: Artikulu honetan, proiektu-eragiketetan konfigurazio-datuak nola konfiguratu eta aplikatzeko informazioa ematen da.
author: sigitac
ms.date: 05/10/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 2c918425e9a6c5fe8888ed8a4258ca59f0464828
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8928003"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service"></a>Konfiguratu eta aplikatu konfigurazio-datuak Common Data Service-n 

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_



## <a name="prerequisites"></a>Aurrebaldintzak

Datuak konfiguratzen hasi aurretik Common Data Service (CDS), honako baldintza hauek bete behar dira:

1.  CDS ingurunea eta Dynamics 365 Finance ingurua hornituko ditu proiektuaren operazioetarako.
2.  Dynamics 365 Finance-ko pertsona juridikoen informazioa CDSren inguruan partekatzen da. Horrek esan nahi du **Enpresa** CDS erakundeak konpainiaren erregistro hauek ditu:
  - THPM
  - USPM
  - GBPM

## <a name="install-setup-and-configuration-data"></a>Instalatu konfigurazioa eta konfigurazio-datuak

1. Deskargatu, desblokeatu eta deskonprimatu [Konfigurazio eta konfigurazio datu paketea](https://download.microsoft.com/download/e/2/d/e2da6c98-d5dd-450c-aabe-fd6bf2ba374b/ProjOpsSampleSetupData-%20Integrated%20Latest.zip).
2. Joan deskonprimatutako karpetara eta exekutatu fitxategi exekutagarria, *DataMigrationUtility*.
3. Common Data Service konfigurazio-migrazioaren (CMT) morroiko 1. orrian, hautatu **Inportatu datuak** eta, ondoren, hautatu **Jarraitu**.

![Konfigurazioaren migrazioa.](./media/1ConfigurationMigration.png)

4. CMT morroiaren 2. orrian, hautatu **Microsoft 365** **Inplementazio mota** gisa.
5. Aukeratu **Erakutsi eskuragarri dauden erakundeen zerrenda** eta **Erakutsi aurreratua** kontrol-laukiak.
6. Aukeratu zure maizterraren eskualdea, sartu zure kredentzialak eta hautatu **Saioa hasi**.

![Konfigurazioaren saio-hasiera.](./media/2ConfigurationSignin.png)

7. 3. orrialdean, maizterraren erakundeen zerrendan, hautatu zein erakundetan inportatu nahi dituzun demo datuak eta hautatu **Saioa hasi**.
8. 4. orrialdean, hautatu zip fitxategia, *SampelSetupAndConfigData*, paketatu gabeko karpetatik.

![Zip fitxategien hautaketa.](./media/3ZipFile.png)

![Hautatu fitxategi bat.](./media/4SelectAFile.png)

9. Zip fitxategia hautatu ondoren, hautatu **Inportatu datuak**.

![Inportatu datuak.](./media/5ImportData.png)

10. Inportazioa gutxi gorabehera bi-hamar minutu iraungo du sareko abiaduraren arabera. Inportatu ondoren, irten CMT morroitik. 
11. Egiaztatu zure erakundeak 26 entitate hauetako datuak dituen:

  - Moneta
  - Kontuen sailkapena
  - Egutegi fiskala
  - Moneta Truke Tasa Motak
  - Ordainketa-eguna
  - Ordainketa-antolaketa
  - Ordainketa-baldintzak
  - Erakundearen unitatea
  - Contact
  - Zerga Taldea
  - Bezero-taldea
  - Saltzaile taldea
  - Unitatea
  - Salmenta-unitatea
  - Prezio-zerrenda
  - Proiektuaren parametroen prezio-zerrenda
  - Fakturen maiztasuna
  - Baliabide erreserbagarriaren kategoria
  - Transakzio-kategoria
  - Gastu-kategoria
  - Funtzioaren prezioa
  - Transakzio-kategoriaren prezioa
  - Ezaugarria
  - Baliabide erreserbagarria
  - Baliabide erreserbagarriaren kategoriaren erlazioa
  - Baliabide erreserbagarriaren ezaugarria

![Inportazio osoa.](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a>Eguneratu Project Operations-en konfigurazioak

1. Nabigatu CE ingurunera. Fitxategia irekita aurki dezakezu [Power Platform Administrazio zentroa](https://admin.powerplatform.microsoft.com/environments), ingurunea hautatuz, eta ondoren hautatuz **Ingurune irekia**. 

![Ireki ingurunea.](./media/7OpenEnvironment.png)

2. Joan **Proiektuak** > **Baliabideak** aukerara eta, ondoren, hautatu **Berria** zure erabiltzailearentzako baliabide erreserbagarria sortzeko.

![Baliabide erreserbagarriak.](./media/8BookableResources.png)

3. **Orokorra** fitxan, hautatu administratzailearen erabiltzailea. Egiaztatu ordu-zona bat zarenarekin bat datorrela. 

![Baliabide erreserbagarri berria.](./media/9NewBookableResource.png)

4. **Programazioa** fitxan, **Enpresa** eremuan, aukeratu **USPM** enpresa, eta gero hautatu **Gorde**. 

![Antolaketa fitxa.](./media/10SchedulingTab.png)

5. Hautatu **Lanorduak** fitxa.  

![Lanorduak.](./media/11WorkHours.png)

6. Egin klik bikoitza egutegiko edozein balioetan eta hautatu **Editatu** > **Serieko gertaera guztiak**. 

![Lan-egutegia.](./media/12WorkCalendar.png)

7. Aldatu laneko orduak zortzi (8) orduko lanegunera, markatu asteburuak lanik gabeko egun gisa eta ziurtatu ordu-zona bat datorrenarekin. 
8. Hautatu **Gorde eta itxi**.

![Eguneratu egutegia.](./media/13UpdateCalendar.png)

9. Joan **Ezarpenak** > **Egutegiaren txantiloiak** eta hautatu **Berria**.
 
 ![Egutegiaren txantiloiak.](./media/14CalendarTemplates.png)
 
 10. Idatzi izen bat, hautatu sortu duzun txantiloiaren baliabidea eta hautatu **Gorde**. 
 
 ![Gorde egutegiaren txantiloia.](./media/15SaveCalendarTemplate.png)
 
 11. Joan **Parametroak** eta egin klik bikoitza erregistroan. 
 
 ![Proiektuaren parametroak.](./media/16ProjectParameters.png)
 
12. Eguneratu eremu hauek:

 - **Enpresa lehenetsia**: USPM
 - **Antolakuntza Unitate Lehenetsia**: Contoso Robotics Global
 - **Fakturen maiztasuna**: Zazpigarren eta Azken eguna
 - **Lan orduko txantiloia**: Sortu duzun txantiloira aldatu.

13. Sakatu **Gorde**. 

![Proiektuen parametro eguneratuak.](./media/17UpdatedProjectParameters.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
