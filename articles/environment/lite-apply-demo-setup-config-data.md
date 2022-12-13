---
title: Aplikatu demo-konfigurazioa eta konfigurazio-datuak - arina
description: Gai honek Project Operations-eko demo-konfigurazioa eta konfigurazio datuak nola aplikatu jakiteko informazioa eskaintzen du.
author: sigitac
ms.date: 11/29/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 8ac8c910ce2d91fa47df08e8fb6efb723c0dc5fa
ms.sourcegitcommit: 38cb012502cbd640abbc21a0912b195112b27ccb
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/30/2022
ms.locfileid: "9811010"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a>Aplikatu Project Operations-erako demo-konfigurazioa eta konfigurazio-datuak - arina 

_**Oinarrizko inplementazioa: kudeatu proformako fakturak_



## <a name="prerequisites"></a>Aurrebaldintzak

Konfigurazioa hasi aurretik, hau eduki behar duzu Dataverse ingurunea Dynamics 365 Project Operations-etarako hornituta.


## <a name="instructions"></a>Instrukzioak

1. Deskargatu [Konfiguratu datu-paketea](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData-%20CE%20only.zip). 
1. Joan karpetara *ProjOpsSampleSetupData - CE bakarrik CMT* eta exekutatu fitxategi exekutagarria,*DataMigrationUtility*.
1. Common Data Service konfigurazio-migrazioaren (CMT) morroiko 1. orrian, hautatu **Inportatu datuak** eta, ondoren, hautatu **Jarraitu**.

    ![Konfigurazioaren migrazioa.](./media/1ConfigurationMigration.png)

1. CMT morroiaren 2. orrian, hautatu **Microsoft 365** **Inplementazio mota** gisa.
1. Aukeratu **Erakutsi eskuragarri dauden erakundeen zerrenda** eta **Erakutsi aurreratua** kontrol-laukiak.
1. Aukeratu zure maizterraren eskualdea, sartu zure kredentzialak eta hautatu **Saioa hasi**.

   ![Konfigurazioaren saio-hasiera.](./media/2ConfigurationSignin.png)

1. 3. orrialdean, Maizterraren Erakundeen zerrendan, hautatu zein erakundetan inportatu nahi dituzun demo datuak eta hautatu **Saioa hasi**.
1. 4. orrialdean, hautatu zip fitxategia, *SampleSetupAndConfigData* paketatu gabeko karpetatik, *ProjOpsSampleSetupData - CE bakarrik CMT*.

   ![Zip fitxategia.](./media/3ZipFile.png)

   ![Hautatu fitxategi bat.](./media/4SelectAFile.png)

1. Zip fitxategia hautatu ondoren, hautatu **Inportatu datuak**.

   ![Inportatu datuak.](./media/5ImportData.png)

1. Inportazioa gutxi gorabehera bi-hamar minutu iraungo du sareko abiaduraren arabera. Bukatu ondoren, irten CMT morroitik. 
1. Egiaztatu zure erakundeak 18 entitate hauetako datuak dituen:

    -   Moneta
    -   Account
    -   Erakundearen unitatea
    -   Contact
    -   Unitatea
    -   Salmenta-unitatea
    -   Prezio-zerrenda
    -   Proiektuaren parametroen prezio-zerrenda 
    -   Fakturen maiztasuna
    -   Baliabide erreserbagarriaren kategoria
    -   Transakzio-kategoria
    -   Gastu-kategoria
    -   Funtzioaren prezioa
    -   Transakzio-kategoriaren prezioa
    -   Ezaugarria
    -   Baliabide erreserbagarria
    -   Baliabide erreserbagarriaren kategoriaren erlazioa
    -   Baliabide erreserbagarriaren ezaugarria

    ![Inportazio osoa.](./media/6CompleteImport.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
