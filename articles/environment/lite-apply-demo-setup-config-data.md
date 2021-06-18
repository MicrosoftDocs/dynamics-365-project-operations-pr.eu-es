---
title: Aplikatu demo-konfigurazioa eta konfigurazio-datuak - arina
description: Gai honek Project Operations-eko demo-konfigurazioa eta konfigurazio datuak nola aplikatu jakiteko informazioa eskaintzen du.
author: sigitac
ms.date: 01/27/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7729b4a9ef5f498b78af298f7233d7dd45434bb3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997136"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a>Aplikatu Project Operations-erako demo-konfigurazioa eta konfigurazio-datuak - arina 

_**Oinarrizko inplementazioa: kudeatu proformako fakturak_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a>Aurrebaldintzak

Konfigurazioa hasi aurretik, hau eduki behar duzu Common Data Service (CDS) ingurunea Dynamics 365 Project Operations-etarako hornituta.


## <a name="instructions"></a>Instrukzioak

1. Deskargatu [Datu nagusien paketea](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData-%20CE%20only.zip). 
2. Joan karpetara *ProjOpsSampleSetupData - CE bakarrik CMT* eta exekutatu fitxategi exekutagarria,*DataMigrationUtility*.
3. Common Data Service konfigurazio-migrazioaren (CMT) morroiko 1. orrian, hautatu **Inportatu datuak** eta, ondoren, hautatu **Jarraitu**.

    ![Konfigurazioaren migrazioa](./media/1ConfigurationMigration.png)

4. CMT morroiaren 2. orrian, hautatu **Microsoft 365** **Inplementazio mota** gisa.
5. Aukeratu **Erakutsi eskuragarri dauden erakundeen zerrenda** eta **Erakutsi aurreratua** kontrol-laukiak.
6. Aukeratu zure maizterraren eskualdea, sartu zure kredentzialak eta hautatu **Saioa hasi**.

   ![Konfigurazioaren saio-hasiera](./media/2ConfigurationSignin.png)

7. 3. orrialdean, Maizterraren Erakundeen zerrendan, hautatu zein erakundetan inportatu nahi dituzun demo datuak eta hautatu **Saioa hasi**.
8. 4. orrialdean, hautatu zip fitxategia, *SampleSetupAndConfigData* paketatu gabeko karpetatik, *ProjOpsSampleSetupData - CE bakarrik CMT*.

   ![Zip fitxategia](./media/3ZipFile.png)

   ![Hautatu fitxategi bat](./media/4SelectAFile.png)

9. Zip fitxategia hautatu ondoren, hautatu **Inportatu datuak**.

   ![Inportatu datuak](./media/5ImportData.png)

10. Inportazioa gutxi gorabehera bi-hamar minutu iraungo du sareko abiaduraren arabera. Bukatu ondoren, irten CMT morroitik. 
11. Egiaztatu zure erakundeak 18 entitate hauetako datuak dituen:

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

    ![Inportazio osoa](./media/6CompleteImport.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
