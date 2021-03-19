---
title: Eman izena Project Operations-en aurrebista harpidetzak baliabideetan / hornitu gabeko agertokietan
description: Gai honek Project Operations-era harpidetzeko eta hedatzeko moduari buruzko informazioa eskaintzen du berreskuratutako / stockean oinarritutako eszenatokietarako.
author: sigitac
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4c2cd4c5d4dfbb95398932d432864cf0d4d5d54d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276828"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a>Eman izena Project Operations-en aurrebista harpidetzak baliabideetan / hornitu gabeko agertokietan

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Gai honetan aurrebista/bazkide eskaintzara nola harpidetu eta Project Operations-en ingurunea nola hornitu azaltzen da baliabideetan/stockean oinarritutako eszenatokietan.

## <a name="prerequisites"></a>Aurrebaldintzak

- Mezu elektroniko bat jasoko duzu aurrebistan parte hartzera gonbidatzen zaituena. Aurreikuspena eska dezakezu [Project Operations webgunea](https://dynamics.microsoft.com/en-us/project-operations/overview/).
- Aurrebista zabaltzen duen erabiltzaileak Azure maizter administratzaile eskubide orokorrak izan behar ditu.
- Finantza ingurunea hedatzeko baliozko Azure harpidetza behar da ingurune bakoitzeko fakturatuko dena. Zure erakundeetan dagoen harpidetza erabil dezakezu edo [Azure proba](https://azure.microsoft.com/en-us/free/) erabiltzen hasteko. CDS ingurunea doan emango da 30 eguneko epean.

## <a name="subscribe"></a>Harpidetu

Zure [aurrebista eskaera](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) onartuta dago, Microsoft-en hiru eskaintza jasoko dituzu posta elektronikoz. Eskaintza hauei esker, Project Operations-en aurrebista hedatu dezakezu:

- Dynamics 365 Project Operations (CRM) - Aurrebista proba
- Office 365 Project Operations - Aurrebista proba
- Dynamics 365 Finance - Aurrebista proba

> [!IMPORTANT]
> Erakunde bateko pertsona bakarrak, maizter administratzaileak, egin behar du zeregin hori. Bertsio honen harpideduna ez bazara, itxaron zure erakundea erregistratu arte eta zure erabiltzaile kredentzialak jaso arte.

### <a name="dynamics-365-project-operations-crm---preview-trial"></a>Dynamics 365 Project Operations (CRM) - Aurrebista proba 

Hasi aurretik, ziurtatu proiektuaren eragiketen aurrebista nahi duzun maizterrean erabiltzailearen laneko kontua duen arakatzailean saioa hasi duzula.

1. Erabili lehen eskaintza kodea, **Dynamics 365 Project Operations (CRM) - Aurrebista proba** arakatzailearen URLan itsatsita.

![Erabili Eskaintza](./media/16RedeemFirstOfferNew.png)

2. Berretsi eskaera.

![Berretsi eskaera](./media/17ConfirmOrderNew.png)

Baieztapen eskaintza behar bezala berreskuratu dela ikusiko duzu.

![Berrespena](./media/18OrderConfirmationNew.png)

### <a name="office-365-project-operations---preview-trial"></a>Office 365 Project Operations - Aurrebista proba

Errepikatu eskaintzaren lehen kodearen urrats berdinak. Ziurtatu bigarren eskaintza kodea gehitzen duzula lehen eskaintza kodearekin erabilitako erabiltzaile kontu bera erabiliz.

### <a name="dynamics-365-finance-preview-trial"></a>Dynamics 365 Finance aurrebista proba

Errepikatu urrats berdinak Ongietorri posta elektronikoko azken eskaintzarekin.

## <a name="assign-licenses"></a>Esleitu lizentziak

> [!IMPORTANT]
> Zure erakundeko Microsoft 365 Portal-erako sarbide administratiboa beharko duzu urrats hauek burutzeko.

1. Joan [Microsoft 365 administrazio zentroa](https://portal.office.com/) aukerara, zure erabiltzaileei lizentziak emateko.

![Administrazio zentroaren hasierako orria](./media/14AdminPortal.png)

2. **Erabiltzaile aktiboak** orrian, hautatu lizentzia esleitu nahi diezun erabiltzaileak.

![Esleitu lizentziak](./media/15AssignLicenses.png)

3. Egiaztatu **Dynamics 365 Project Operations (CRM) Aurrebista** eta **Office 365 Proiektuaren eragiketak - Aurrebista** lizentzia hautatu eta hautatu **Aldaketak gorde**.

> [!NOTE]
> Finantza probako eskaintza ez zaio erabiltzaile bati esleitu behar.

## <a name="start-a-new-project-in-lcs"></a>Sortu proiektua LCS-n

Sortu LCS proiektu berria gaian azaltzen den moduan, [Hasi proiektu berri bat LCSn](create-lcs-project.md)

## <a name="add-an-azure-subscription-to-an-lcs-project"></a>Gehitu Azure harpidetza LCS proiektu batean

Zeregin hori burutzeko, jarraitu gaiaren urratsak, [Gehitu Azure harpidetza LCS proiektuari](resource-add-azure-subscription-lcs-project.md).

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a>Inplementatu Finantza demo ingurunea, Project Operations-ekin baliabideak/hornitu gabeko agertokietarako

Jarraitu gaiaren argibideak, [Ingurune berria hornitzea](resource-provision-new-environment.md) hedapena osatzeko. Erabili [demo-ingurunea](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) inplementazio mota aurrebistarako. 

## <a name="install-cds-setup-and-configuration-data"></a>Instalatu CDS konfigurazioa eta konfigurazio-datuak

Instalatu CDS konfigurazio eta konfigurazio datuak gaian deskribatutako moduan, [Konfiguratu eta aplikatu konfigurazio datuak Common Data Service](resource-apply-pro-setup-config-data.md).
Osatu urrats hau Finantza demo ingurunea zabaldu eta FOko demo datuak prest egon ondoren.


[!INCLUDE[footer-include](../includes/footer-banner.md)]