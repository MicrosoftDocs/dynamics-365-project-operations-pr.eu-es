---
title: Eman izena Project Operations-en aurrebista harpidetzak baliabideetan / hornitu gabeko agertokietan
description: Gai honek Project Operations-era harpidetzeko eta hedatzeko moduari buruzko informazioa eskaintzen du berreskuratutako / stockean oinarritutako eszenatokietarako.
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 75ee31e67018fe2a7655d8a8f11e40b433a9a5db6f8f2addac27844f18fffe8d
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "7007851"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a>Eman izena Project Operations-en aurrebista harpidetzak baliabideetan / hornitu gabeko agertokietan

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Gai honetan azaltzen da nola harpidetu probako eskaintzan eta nola zabaldu Project Operations ingurunea baliabideetan / stockean oinarritutako eszenatokietan.

## <a name="prerequisites"></a>Aurrebaldintzak
- Aurrebista zabaltzen duen erabiltzaileak Azure maizter administratzaile eskubide orokorrak izan behar ditu. Maizterra sor dezakezu lehenengo eskaintzaren amortizazioan. 
- Finantza ingurunea hedatzeko baliozko Azure harpidetza behar da ingurune bakoitzeko fakturatuko dena. Zure erakundeetan dagoen harpidetza erabil dezakezu edo [Azure proba](https://azure.microsoft.com/en-us/free/) erabiltzen hasteko. CDS ingurunea doan emango da 30 eguneko epean.

> [!IMPORTANT]
> Erakunde bateko pertsona bakarrak, maizter administratzaileak, egin behar du zeregin hori. Bertsio honen harpideduna ez bazara, itxaron zure erakundea erregistratu arte eta zure erabiltzaile kredentzialak jaso arte.
> 
> Probak erabilera bakarrekoak dira maizterrean. Probak behin bakarrik exekutatu ditzakezu. Probarako helburuarekin maizter berri bat sortzea gomendatzen dizugu.


### <a name="dynamics-365-project-operations-ce---preview-trial"></a>Dynamics 365 Project Operations (CE) - Aurrebista proba 

Hasi aurretik, ziurtatu proiektuaren eragiketen aurrebista nahi duzun maizterrean erabiltzailearen laneko kontua duen arakatzailean saioa hasi duzula.

1. Erabili lehen eskaintza kodea, **Dynamics 365 Project Operations** hemen [Project Operations proba](https://aka.ms/try-po).
2. Berretsi eskaera.

  Baieztapen eskaintza behar bezala berreskuratu dela ikusiko duzu.

### <a name="dynamics-365-finance-preview-trial"></a>Dynamics 365 Finance aurrebista proba

Joan [Dynamics 365 for Finance aurrebista proba](https://aka.ms/trypoche) eta errepikatu aurreko ataleko urratsak eskaintzarekin, Erregistratu hodeian ostatatutako ingurunean.  

## <a name="assign-licenses"></a>Esleitu lizentziak

> [!IMPORTANT]
> Zure erakundeko Microsoft 365 Portal-erako sarbide administratiboa beharko duzu urrats hauek burutzeko.

1. Joan [Microsoft 365 administrazio zentroa](https://portal.office.com/) aukerara, zure erabiltzaileei lizentziak emateko.

2. **Erabiltzaile aktiboak** orrian, hautatu lizentzia esleitu nahi diezun erabiltzaileak.

3. Egiaztatu **Dynamics 365 Project Operations** lizentzia hautatu dela eta hautatu **Aldaketak gorde**.

> [!NOTE]
> Finantza probako eskaintza ez zaio erabiltzaile bati esleitu behar.

## <a name="start-a-new-project-in-lcs"></a>Sortu proiektua LCS-n

Sortu LCS proiektu berria gaian azaltzen den moduan, [Hasi proiektu berri bat LCSn](create-lcs-project.md)

## <a name="add-an-azure-subscription-to-an-lcs-project"></a>Gehitu Azure harpidetza LCS proiektu batean

Zeregin hori burutzeko, jarraitu gaiaren urratsak, [Gehitu Azure harpidetza LCS proiektuari](resource-add-azure-subscription-lcs-project.md).

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a>Inplementatu Finantza demo ingurunea, Project Operations-ekin baliabideak/hornitu gabeko agertokietarako

Jarraitu gaiaren argibideak, [Ingurune berria hornitzea](resource-provision-new-environment.md) hedapena osatzeko. Erabili [demo-ingurunea](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) inplementazio mota aurrebistarako. 

## <a name="install-cds-setup-and-configuration-data"></a>Instalatu CDS konfigurazioa eta konfigurazio-datuak

Instalatu CDS konfigurazio eta konfigurazio datuak gaian deskribatutako moduan, [Konfiguratu eta aplikatu konfigurazio datuak Common Data Service](resource-apply-pro-setup-config-data.md).
Egin urrats hau Finantzako demo ingurunea inplementatu eta demo datuak prest egon ondoren.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
