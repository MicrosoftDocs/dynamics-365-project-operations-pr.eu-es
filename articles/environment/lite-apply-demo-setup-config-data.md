---
title: Aplikatu demo-konfigurazioa eta konfigurazio-datuak
description: Gai honek Project Operations-eko demo-konfigurazioa eta konfigurazio datuak nola aplikatu jakiteko informazioa eskaintzen du.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 33b85115963f3561718b8951e5b518fd34de7723
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070901"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations-lite-deployment---deal-to-proforma-invoicing"></a>Aplikatu demo konfigurazio eta konfigurazio datuak Project Operations lite inplementazioan - aurre proforma fakturazioari

_**Oinarrizko inplementazioa: kudeatu proformako fakturak_

1. Deskargatu [Datu nagusien paketea](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip). 
2. Joan *ProjOpsDemoDataSetupAndMaster - CMT integratua* karpetara eta exekutatu fitxategi exekutagarria, *DataMigrationUtility*.
3. Common Data Service konfigurazio-migrazioaren (CMT) morroiko 1. orrian, hautatu **Inportatu datuak** eta, ondoren, hautatu **Jarraitu**.

![Konfigurazioaren migrazioa](./media/1ConfigurationMigration.png)

4. CMT morroiaren 2. orrian, hautatu **Microsoft 365** **Inplementazio mota** gisa.
5. Aukeratu **Erakutsi eskuragarri dauden erakundeen zerrenda** eta **Erakutsi aurreratua** kontrol-laukiak.
6. Aukeratu zure maizterraren eskualdea, sartu zure kredentzialak eta hautatu **Saioa hasi**.

![Konfigurazioaren saio-hasiera](./media/2ConfigurationSignin.png)

7. 3. orrialdean, Maizterraren Erakundeen zerrendan, hautatu zein erakundetan inportatu nahi dituzun demo datuak eta hautatu **Saioa hasi**.
8. 4. orrialdean, hautatu zip fitxategia, *MasterAndSetupData* paketatu gabeko karpetatik, *ProjOpsDemoDataSetupAndMaster - CMT integratua*.

![Zip fitxategia](./media/3ZipFile.png)

![Hautatu fitxategia.](./media/4SelectAFile.png)

9. Zip fitxategia hautatu ondoren, hautatu **Inportatu datuak**.

![Inportatu datuak](./media/5ImportData.png)

10. Inportazioa gutxi gorabehera bi-hamar minutu iraungo du sareko abiaduraren arabera. Bukatu ondoren, irten CMT morroitik. 
11. Egiaztatu zure erakundeak 20 entitate hauetako datuak dituen:

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
- Fakturen maiztasunaren xehetasunak
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
