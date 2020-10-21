---
title: Konfiguratu eta aplikatu konfigurazio-datuak Project Operations-en Common Data Service-n
description: Gai honek Project Operations-eko konfigurazio-datuak konfiguratzeari eta aplikatzeari buruzko informazioa eskaintzen du.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d99ab4c7b2ebf6ba56b86a3e0151036c6247e484
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948730"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service-for-project-operations"></a>Konfiguratu eta aplikatu konfigurazio-datuak Project Operations-en Common Data Service-n

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

## <a name="install-setup-and-configuration-data"></a>Instalatu konfigurazioa eta konfigurazio-datuak

1. Deskargatu, desblokeatu eta deskonprimatu [Konfigurazio eta konfigurazio datu paketea](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).
2. Joan deskonprimatutako karpetara eta exekutatu fitxategi exekutagarria, *DataMigrationUtility*.
3. Common Data Service konfigurazio-migrazioaren (CMT) morroiko 1. orrian, hautatu **Inportatu datuak** eta, ondoren, hautatu **Jarraitu**.

![Konfigurazioaren migrazioa](./media/1ConfigurationMigration.png)

4. CMT morroiaren 2. orrian, hautatu **Office 365** **Inplementazio mota** gisa.
5. Aukeratu **Erakutsi eskuragarri dauden erakundeen zerrenda** eta **Erakutsi aurreratua** kontrol-laukiak.
6. Aukeratu zure maizterraren eskualdea, sartu zure kredentzialak eta hautatu **Saioa hasi**.

![Konfigurazioaren saio-hasiera](./media/2ConfigurationSignin.png)

7. 3. orrialdean, maizterraren erakundeen zerrendan, hautatu zein erakundetan inportatu nahi dituzun demo datuak eta hautatu **Saioa hasi**.
8. 4. orrialdean, hautatu zip fitxategia, *SampelSetupAndConfigData*, paketatu gabeko karpetatik.

![Zip fitxategien hautaketa](./media/3ZipFile.png)

![Hautatu fitxategia.](./media/4SelectAFile.png)

9. Zip fitxategia hautatu ondoren, hautatu**Inportatu datuak**.

![Inportatu datuak](./media/5ImportData.png)

10. Inportazioa gutxi gorabehera bi-hamar minutu iraungo du sareko abiaduraren arabera. Inportatu ondoren, irten CMT morroitik. 
11. Egiaztatu zure erakundeak 19 entitate hauetako datuak dituen:

  - Moneta
  - Erakundearen unitatea
  - Contact
  - Zerga Taldea
  - Bezero-taldea
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

![Inportazio osoa](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a>Eguneratu Project Operations-en konfigurazioak

1. Nabigatu CE ingurunera. Fitxategia irekita aurki dezakezu [Power Platform Administrazio zentroa](https://admin.powerplatform.microsoft.com/environments), ingurunea hautatuz, eta ondoren hautatuz **Ingurune irekia**. 

![Ireki ingurunea](./media/7OpenEnvironment.png)

2. Joan **Proiektuak** > **Baliabideak** aukerara eta, ondoren, hautatu **Berria** zure erabiltzailearentzako baliabide erreserbagarria sortzeko.

![Baliabide erreserbagarriak](./media/8BookableResources.png)

3. **Orokorra** fitxan, hautatu administratzailearen erabiltzailea. Egiaztatu ordu-zona bat zarenarekin bat datorrela. 

![Baliabide erreserbagarri berria](./media/9NewBookableResource.png)

4. **Programazioa** fitxan, **Enpresa** eremuan, aukeratu **USPM** enpresa, eta gero hautatu **Gorde**. 

![Antolaketa fitxa](./media/10SchedulingTab.png)

5. Hautatu **Lanorduak** fitxa.  

![Lanorduak](./media/11WorkHours.png)

6. Egin klik bikoitza egutegiko edozein balioetan eta hautatu **Editatu** > **Serieko gertaera guztiak**. 

![Lan-egutegia](./media/12WorkCalendar.png)

7. Aldatu laneko orduak zortzi (8) orduko lanegunera, markatu asteburuak lanik gabeko egun gisa eta ziurtatu ordu-zona bat datorrenarekin. 
8. Hautatu **Gorde eta itxi**.

![Eguneratu egutegia](./media/13UpdateCalendar.png)

9. Joan **Ezarpenak** > **Egutegiaren txantiloiak** eta hautatu **Berria**.
 
 ![Egutegiaren txantiloiak](./media/14CalendarTemplates.png)
 
 10. Idatzi izen bat, hautatu sortu duzun txantiloiaren baliabidea eta hautatu **Gorde**. 
 
 ![Gorde egutegiaren txantiloia](./media/15SaveCalendarTemplate.png)
 
 11. Joan **Parametroak** eta egin klik bikoitza erregistroan. 
 
 ![Proiektuaren parametroak](./media/16ProjectParameters.png)
 
12. Eguneratu eremu hauek:

 - **Enpresa lehenetsia**: USPM
 - **Antolakuntza Unitate Lehenetsia**: Contoso Robotics Global
 - **Fakturen maiztasuna**: Zazpigarren eta Azken eguna
 - **Lan orduko txantiloia**: Sortu duzun txantiloira aldatu.

13. Sakatu **Gorde**. 

![Proiektuen parametro eguneratuak](./media/17UpdatedProjectParameters.png)
