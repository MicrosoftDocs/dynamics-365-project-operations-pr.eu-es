---
title: Erregistratu aurrebista-harpidetzan - arina
description: Gai honek Project Operations lite-ra harpidetzeko eta hura inplementatzeko moduari buruzko informazioa eskaintzen du. Aurre egin fakturazio proformari.
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 3b06ac29e8021967490534d3aefc8b5ce733413b
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8587985"
---
# <a name="sign-up-for-a-preview-subscription---lite"></a>Erregistratu aurrebista-harpidetzan - arina 

Gai honek probako eskaintzan harpidetu eta nola inplementatu Dynamics 365 Project Operations lite inplementazioa azaltzen du - proforma fakturazioari aurre egin.

> [!NOTE]
> Prozesu hau aldatu egingo da datozen Project Operations-en bertsioetan.

## <a name="prerequisites"></a>Aurrebaldintzak
- Aurrebista zabaltzen duen erabiltzaileak Azure maizter administratzaile eskubide orokorrak izan behar ditu. Maizterra sor dezakezu lehenengo eskaintzaren amortizazioan.

> [!IMPORTANT]
> Erakunde bateko pertsona bakarrak, maizter administratzaileak, egin behar du zeregin hori. Bertsio honen harpideduna ez bazara, itxaron zure erakundea erregistratu arte eta zure erabiltzaile kredentzialak jaso arte.
> 
> Probak erabilera bakarrekoak dira maizterrean. Probak behin bakarrik exekutatu ditzakezu. Probarako helburuarekin maizter berri bat sortzea gomendatzen dizugu.

### <a name="dynamics-365-project-operations-trial"></a>Dynamics 365 Project Operations proba 

Hasi aurretik, ziurtatu proiektuaren eragiketen aurrebista nahi duzun maizterrean erabiltzailearen laneko kontua duen arakatzailean saioa hasi duzula.

1. Joan [Project Operations probara](https://aka.ms/try-po) lehenengo eskaintza kodea erabiltzeko, **Dynamics 365 Project Operations**.
2. Berretsi eskaera.

  Berrespen eskaintza behar bezala berreskuratu dela ikusiko duzu.

## <a name="assign-licenses"></a>Esleitu lizentziak

> [!IMPORTANT]
> Zure erakundeko Microsoft 365 atarirako sarbide administratiboa beharko duzu urrats hauek burutzeko.


1. Joan [Microsoft 365 administrazio zentroa](https://portal.office.com/) zure erabiltzaileei lizentziak esleitzeko.
2. **Erabiltzaile aktiboak** orrian, hautatu lizentzia esleitu nahi diezun erabiltzaileak.
3. Egiaztatu **Dynamics 365 Project Operations** lizentzia hautatuta dagoela. 
4. Hatatu **Gorde aldaketak**.

## <a name="create-a-new-dataverse-environment"></a>Sortu Dataverse ingurune berria

1. Eman Project Operations Dataverse inplementazio ingurune berri bat gaiko argibideak jarraituz, [Dataverse inplementazio eredua](lite-deployment.md). Ingurune mota hautatzen duzunean, ziurtatu erabiltzen duzula **Proba (harpidetzan oinarrituta)**.

  ![Ingurune berria.](./media/19CreateEnvironment.png)

2. Aukeratu **Gaitu Dynamics 365 aplikazioak** ezarpena, eta utzi **Aplikazio hauek automatikoki zabaldu** hutsik.  
3. Hautatu **Gorde** ingurunea sortzeko.

  ![Gehitu datu-basea.](./media/20CreateEnvironment1.png)

4. Ingurunea sortu ondoren, instalatu **Microsoft Dynamics 365 Project Operations** konponbidea. 

![Instalatu soluzioa.](./media/21InstallSolution.png)

## <a name="install-a-cds-configuration-and-setup-demo-data"></a>Instalatu CDS konfigurazioa eta konfiguratu demo-datuak

Instalatu CDS konfigurazioa eta konfiguratu demo datuak gaiko argibideak jarraituz, [Aplikatu demo konfigurazio eta konfigurazio datuak](lite-apply-demo-setup-config-data.md).


[!INCLUDE[footer-include](../includes/footer-banner.md)]
