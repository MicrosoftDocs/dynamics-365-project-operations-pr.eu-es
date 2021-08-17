---
title: Microsoft Project client integrazioa
description: Proiektuen egutegia planifikatzea eta mantentzea konplexua izan daiteke, beraz, proiektuen kudeatzaileek zeregin hori kudeatzen lagunduko dieten tresnak erabili behar dituzte. Microsoft Project Client-ekin integratzeak proiektuaren lanen banakako egitura irekitzeko eta kudeatzeko laguntza eskaintzen du.
author: Yowelle
ms.date: 06/16/2021
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjWbsTemplate
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2017-12-04
ms.dyn365.ops.version: 7.2999999999999998
ms.openlocfilehash: 8ef34bc984510f23ab77cc1710c06abbcf80f721703685d696fea28eeaddd732
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6988006"
---
# <a name="microsoft-project-client-integration"></a>Microsoft Project client integrazioa

[!include [banner](../includes/banner.md)]

Proiektuen egutegia planifikatzea eta mantentzea konplexua izan daiteke, beraz, proiektuen kudeatzaileek zeregin hori kudeatzen lagunduko dieten tresnak erabili behar dituzte. Microsoft Project Client-ekin integratzeak proiektuaren lanen banakako egitura irekitzeko eta kudeatzeko laguntza eskaintzen du. Proiektuaren kudeatzaileak edozein aldaketa argitaratu ahal izango ditu Dynamics 365 Finance proiektuaren zereginen xehetasunen egitura.

> [!NOTE]
> Uztaileko eguneratzea erabiltzen baduzu (10.0.4 bertsioa), KB 4054797 eta 4055884 instalatu behar dituzu.

## <a name="configure-the-microsoft-project-client-add-in"></a>Konfiguratu Microsoft Project Client gehigarria
Microsoft Project Client-ekin bateratzea ahalbidetzeko, a Microsoft Dynamics 365 gehigarriak erabiltzailearen bezero Microsoft Project aplikazioan instalatu behar dira. Hau irekitzen da **Proiektuak kudeatzeko lan eremua**.

•   Egin klik **Konfiguratu proiektuaren bezeroaren gehigarria** hurrengotik **Estekak** > **Konfigurazioa** lan-eremuko atala.

•   Egin klik **Ireki**, egin klik **Exekutatu** galdetutakoan.

## <a name="open-and-edit-an-existing-draft-work-breakdown-structure-in-microsoft-project-client"></a>Ireki eta editatu lehendik dagoen proiektuaren zirriborroen egitura Microsoft Project Client-en
Proiektu bat bada Dynamics 365 Finance dagoeneko zereginen xehetasunen egitura sortu da, zereginen xehetasunen egitura Microsoft Project Client aplikazioan ireki ahal izango da lan banakako egitura zirriborro egoeran badago. Irekitzeko **Proiektua** orrialdean, egin klik **Ireki Microsoft Project-en** estekatik **Plana** fitxa. Orri hau Microsoft Project Client aplikazioaren barruan ere ireki daiteke klik eginez **Irekia** urtean **Microsoft Dynamics 365** fitxa. Aukeratu **Pertsona juridikoa** eta **Proiektua** zerrendatik.

> [!NOTE]
> Erabiltzen ari bazara Internet Explorer zure arakatzaile gisa, klik egin beharko duzu **Gorde** fitxategia deskargatu den kokapenetik eskuz irekitzeko. Edo, egin klik **Gorde eta ireki** fitxategia Microsoft Project Client-en irekitzeko. Ez aldatu izena gordetzean fitxategiaren izena.

Microsoft Project Client-ekin fitxategian aldaketak egin aurretik, egiaztatu egin behar duzu. Egin klik **Errebisatu** urtean **Microsoft Dynamics 365** fitxa. Horrek saihestuko du beste erabiltzaile batzuek lanaren banakako egitura aldi berean Finantza barrutik editatzea. Edizioak egin ondoren lanaren banakako egitura argitaratzeko, egin klik **Sartu** gainean **Microsoft Dynamics 365** fitxa.

Finantza proiektuan proiektu talde bat dagoeneko gehitu bada, baliabideen zerrenda taldekideekin osatuko da. Proiektu talde bat oraindik proiektuan gehitu ez bada, baliabideak hauta ditzakezu eta taldea Microsoft Project Client-en sortu dezakezu klik eginez **Baliabideak** botoian **Microsoft Dynamics 365** fitxa. 

Datu hauek Finantzarekin sinkronizatuko dira check-in prozesuaren barruan:

•   Zereginaren izena

•   Hasiera data

•   Amaieraren data

•   Aurrekoak

•   Baliabide izenak

•   Kategoria

•   Baliabide kategoria

•   Lan-orduak

•   Oharrak

•   Lehentasuna

> [!NOTE]
> Microsoft Project Client fitxategian beste zutabe batzuk gehitzen badituzu, ez dira fitxategian gordeko eta ez dira bistaratuko fitxategia berriro irekitzen denean.

## <a name="create-the-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a>Sortu lehendik dagoen proiektu baterako lanen banaketa egitura Microsoft Project Client erabiliz
Sortzeko zereginen xehetasunen egitura berria erabiliz Microsoft Project Client hurrengo pauso hauek:


1.  Ireki Microsoft Project Client.

2.  **Microsoft Dynamics 365** fitxan, klik egin **Ireki**.

3.  Hautatu **Legezko entitatea** proiektuarentzat.

4.  Hautatu **Proiektua**.

5.  Klik egin **Bilatu** hurrengoan **Microsoft Dynamics 365** fitxan.

6.  Finantzan argitaratzeko prest zaudenean, egin klik **Sartu** gainean **Microsoft Dynamics 365** fitxa.

## <a name="replace-the-existing-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a>Ordezkatu existitzen den proiektu baterako lanen banaketa egitura Microsoft Project Client erabiliz
Microsoft Project Client erabiliz lanaren banakako egitura berria sortzeko eta lehendik dagoen proiektu baten lehendik dagoen banakako egitura ordezkatzeko, jarraitu urrats hauei:

1.  Ireki Microsoft Project Client.

2.  Sortu antolaketa Microsoft Project Client.

3.  Gainean **Microsoft Dynamics 365** fitxa, egin klik **Aldaketak gorde** > **Ordeztu dagoen proiektua**.

4.  Hautatu **Legezko entitatea** proiektuarentzat.

5.  Hautatu **Proiektua**.

6.  Sakatu **Ados**.

## <a name="create-a-new-project-from-within-microsoft-project-client"></a>Sortu proiektu berria Microsoft Project Client-etik


1.  Ireki Microsoft Project Client.

2.  Sortu antolaketa Microsoft Project Client.

3.  Gainean **Microsoft Dynamics 365** fitxa, egin klik **Aldaketak gorde** > **Gorde proiektu berria**.

4.  Hautatu **Legezko entitatea** proiektuarentzat.

5.  Sartu **Proiektuaren IDa**, Beharrezkoa bada.

6.  Idatzi **Proiektuaren izena**.

7.  Aukeratu **Proiektu mota**, **Proiektu taldea** eta **Proiektuaren kontratuaren IDa**. Bestela, proiektuaren kontratu berria sor dezakezu klik eginez **Berria**.

8.  Aukeratu **Egutegia** baliabideetarako erabiltzeko.

11. Sakatu **Ados**.

> [!NOTE]
> Project Client gehigarriak ez ditu proiektuaren ID formatuan karaktere hauek onartzen:
> 
>   - Azpimarra
>   - Aldia
>   - Zuriune-barra
>   - Barra

[!INCLUDE[footer-include](../includes/footer-banner.md)]
