---
title: Erregistratu aurrebista-harpidetzan - arina
description: Gai honek Project Operations lite-ra harpidetzeko eta hura inplementatzeko moduari buruzko informazioa eskaintzen du. Aurre egin fakturazio proformari.
author: sigitac
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 44edf2613ea4b26dadbd9edc47c784c488c577de
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290029"
---
# <a name="sign-up-for-a-preview-subscription---lite"></a>Erregistratu aurrebista-harpidetzan - arina 

Gai honetan aurrebista bazkideen eskaintzara nola harpidetu eta nola zabaldu azaltzen da Dynamics 365 Project Operations inplementazio arina proforma fakturazioari aurre egin.

> [!NOTE]
> Prozesu hau aldatu egingo da datozen Project Operations-en bertsioetan.

## <a name="prerequisites"></a>Aurrebaldintzak

- Mezu elektroniko bat jasoko duzu aurrebistan parte hartzera gonbidatzen zaituena. Aurreikuspena eska dezakezu [Project Operations webgunea](https://dynamics.microsoft.com/en-us/project-operations/overview/).
- Aurrebista zabaltzen duen erabiltzaileak Azure maizter administratzaile eskubide orokorrak izan behar ditu.
- Berrikusi baldintza guztiak.

## <a name="subscribe"></a>Harpidetu

[Aurrebista-eskaeraren](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) onespena eskatzen duzunean, Microsoft-en bi eskaintza jasoko dituzu posta elektronikoz. Eskaintza hauei esker, Project Operations-en aurrebista hedatu dezakezu:

- Dynamics 365 Project Operations (CRM) - Aurrebista proba
- Office 365 Project Operations - Aurrebista proba

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

## <a name="assign-licenses"></a>Esleitu lizentziak

> [!IMPORTANT]
> Zure erakundeko Microsoft 365 Portal-erako sarbide administratiboa beharko duzu urrats hauek burutzeko.


1. Joan [Microsoft 365 administrazio zentroa](https://portal.office.com/) aukerara, zure erabiltzaileei lizentziak emateko.

![Administrazio zentroaren hasierako orria](./media/14AdminPortal.png)

2. **Erabiltzaile aktiboak** orrian, hautatu lizentzia esleitu nahi diezun erabiltzaileak.

![Esleitu lizentziak](./media/15AssignLicenses.png)

3. Egiaztatu **Dynamics 365 Project Operations (CRM) Aurrebista** eta **Office 365 Project Operations - Aurrebista** lizentziak hautatzen dira. 
4. Hatatu **Gorde aldaketak**.

## <a name="create-a-new-cds-environment"></a>Sortu CDS ingurune bat

1. Eman Project Operations CDS inplementazio ingurune berri bat gaian argibideak jarraituz, [CDS inplementazio-eredua](lite-deployment.md). Ingurune mota hautatzen duzunean, ziurtatu erabiltzen duzula **Proba (harpidetzan oinarrituta)**.
![Ingurune berria](./media/19CreateEnvironment.png)

2. Aukeratu **Gaitu Dynamics 365 aplikazioak** ezarpena, eta utzi **Aplikazio hauek automatikoki zabaldu** hutsik.  
3. Hautatu **Gorde** ingurunea sortzeko.

![Gehitu datu-basea](./media/20CreateEnvironment1.png)

4. Ingurunea sortu ondoren, instalatu **Microsoft Dynamics 365 Project Operations** konponbidea. 

![Instalatu soluzioa](./media/21InstallSolution.png)

## <a name="install-a-cds-configuration-and-setup-demo-data"></a>Instalatu CDS konfigurazioa eta konfiguratu demo-datuak

Instalatu CDS konfigurazioa eta konfiguratu demo datuak gaiko argibideak jarraituz, [Aplikatu demo konfigurazio eta konfigurazio datuak](lite-apply-demo-setup-config-data.md).


[!INCLUDE[footer-include](../includes/footer-banner.md)]