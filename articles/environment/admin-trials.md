---
title: Eman izena Project Operations-en doako probak lortzeko
description: Gai honek Dynamics 365 Project Operations proba bat inplementatzeari buruzko informazioa ematen du.
author: ruhercul
ms.date: 10/04/2021
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 1c8ae111acffb45fef1c2e6435849471ae331796
ms.sourcegitcommit: 05ee415093d152b5b9e1203c3db0ea7f0c5a75a5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/04/2021
ms.locfileid: "7599198"
---
# <a name="sign-up-for-project-operations-trials"></a>Eman izena Project Operations-en doako probak lortzeko 

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako Project Operations, Lite hedapena - proformaren fakturazioari aurre egitea eta produkzioan oinarritutako eszenatokien proiektuaren eragiketak_ 

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Gai honetan aurrebista bazkideen eskaintzara nola harpidetu eta nola hedatu azaltzen da Dynamics 365 Project Operations ingurunea.

Project Operations proba berriarekin, onartutako hiru inplementazio eszenatokietako bat automatikoki inplementa dezakezu, inplementazio planteamendu onena gomendatzen duen galdeketa bat osatuta. Gai honek benetako datuei buruzko informazioa ematen du:

- Erabili proba-eskaintza.
- Hasi hornidura.
- Konfiguratu idazketa dualeko integrazioa.
- Project Operations buruzko informazio gehiago. 

Ondorengo taulan probako eskaintza berriaren xehetasunak azaltzen dira.

| **Eskaintza elementua**               | **Xehetasunak**                                  |
|------------------------------|----------------------------------------------|
| Eskaintza mota                   | Eskaintza mota hau administratzaile nagusia da, beraz maizter administratzailea beharrezkoa da trukatu ahal izateko. |
| Erabilera eskaini                    | Maizter bakoitzeko denbora bat                          |
| Eskaintzaren iraupena               | 30 eguneko egutegia                             |
| Errentamenduak maizter bakoitzeko       | 1                                            |
| Erabiltzaile kopurua              | 25                                           |
| Luzapena                    | Luzapen 1, 30 egutegi egun               |
| Probako inguruneen kopurua | 3                                            |


## <a name="admin-trial-details"></a>Administratzailearen proba xehetasunak
Hurrengo taulan probaren xehetasunak eta inplementazio mota bakoitzari nola aplikatzen zaizkion azaltzen da.

| **Elementua**                      | **Lite**                                     | **Izakinak ez dituzten materialak** | **Izakinak dituzten materialak** |
|-------------------------------|----------------------------------------------|---------------------------|-----------------------|
| Emandako konfigurazio datuak           | Yes                                          | Yes                       | Bai (USSI)            |
| Transakzio-datuak            | No                                           | No                        | No                    |
| Hornitzeko denbora minututan  | 15                                           | 90                        | 30                    |
 
## <a name="prerequisites"></a>Aurrebaldintzak
Hurrengo aurrebaldintzak eskatzen dira proba inplementatzeko Dynamics 365 Project Operations.

- Erregistratzeko [Dynamics 365 Project Operations - Aurrebista proba](https://www.aka.ms/try-po).
- Aurrebista zabaltzen duen erabiltzaileak Azure maizter administratzaile eskubide orokorrak izan behar ditu.

> [!IMPORTANT]
> Erakunde bateko pertsona bakarrak, maizter administratzaileak, egin behar du zeregin hori. Bertsio honen harpideduna ez bazara, itxaron zure erakundea erregistratu arte eta zure erabiltzaile kredentzialak jaso arte.

### <a name="dynamics-365-project-operations---preview-trial"></a>Dynamics 365 Project Operations - Aurrebista proba 

Hasi aurretik, hasi saioa arakatzailean erabiltzaileen laneko kontuarekin Project Operations aurrebista nahi duzun maizterrean.

1. Erabili lehen eskaintza kodea, **Dynamics 365 Project Operations - Aurrebista proba** arakatzailearen URLan itsatsita.

    ![Erabili Eskaintza](./media/16RedeemFirstOfferNew.png)

2. Berretsi eskaera.

    ![Berretsi eskaera](./media/17ConfirmOrderNew.png)

  Berrespen eskaintza behar bezala berreskuratu dela ikusiko duzu.

   ![Berrespena](./media/18OrderConfirmationNew.png)

  Helbidera birbidaliko zaituzte [Power Platform administratzaile zentroa](https://admin.powerplatform.microsoft.com/projectoperationstrial).

## <a name="questionnaire-and-provisioning"></a>Galdeketa eta hornidura

1.  Joan [Power Platform administrazio-zentroa](https://admin.powerplatform.com/projectoperationstrial) eta osatu galdetegia.  
2.  Berrikusi gomendatutako inplementazio mota eta hautatu **Hasi konfigurazioa** hornidura hasteko.
3.  Berrikusi baldintzak betetzera eta, ondoren, hautatu **Hasi**.

   Hornidura hasi ondoren, inguruneko zerrendara birbideratuko zaituzte Power Platform administratzaile zentroa. Hornidura martxan dagoen bitartean, zure ingurunearen egoera dago **Instantzia prestatzen**.
 
  Hornidura amaitutakoan, zure ingurunearen egoera da **Prest**. Ingurunea hornitzeak demo datuak zabaltzea dakar.
 
4.  Aukeratu dagokion Microsoft Dataverse URLa eta Finance and Operations aplikazioen URLak inplementazioa balioztatzeko.

## <a name="configuring-dual-write"></a>Konfiguratuz idazketa duala
Hornitu gabeko materialen inplementazioetarako soilik, konfiguratu idazketa bikoitzeko mapak. Informazio gehiagorako, ikus [Project Operations idazketa bikoitzeko mapen bertsioak](resource-dual-write-maps.md).

## <a name="assign-licenses"></a>Esleitu lizentziak

Zure erakundeko Microsoft 365 Portal-erako sarbide administratiboa beharko duzu urrats hauek burutzeko.

1. Joan [Microsoft 365 administrazio zentroa](https://portal.office.com/) lizentziak zure erabiltzaileei esleitzeko.

   ![Administrazio zentroaren hasierako orria](./media/14AdminPortal.png)

2. **Erabiltzaile aktiboak** orrian, hautatu lizentzia esleitu nahi diezun erabiltzaileak.

   ![Esleitu lizentziak](./media/15AssignLicenses.png)

3. Egiaztatu **Dynamics 365 Project Operations Aurrebista**  lizentzia hautatu da, eta gero hautatu **Gorde aldaketak**.

## <a name="additional-resources"></a>Baliabide gehigarriak

Ondorengo baliabideek orientazio lagungarria eskaintzen dute Project Operations bidaia hasten duzunean:

- [Bideo Multzoa -Project Operations Ikuspegia, murgiltze sakonak eta bide orria](https://youtube.com/playlist?list=PLcakwueIHoT_LJ3Fr1tHnkPk5lioqE6uH)
- [Dynamics 365 Project Operations](/learn/modules/examine-dynamics-365-project-operations/)
- [Zehaztu inplementazio mota](determine-deployment-type.md)

## <a name="frequently-asked-questions"></a>Maiz egiten diren galderak

### <a name="what-if-i-require-alm-or-elm-for-my-finance-and-operations-apps-environment"></a>Niretzat ALM edo ELM behar baditut Finance and Operations aplikazioen ingurunea?

- Ingurune osoaren bizi-zikloa kudeatzeko gaitasunak behar dituzten bazkideentzat, ikusi [Bazkide Sandbox lizentzia eskaera](https://experience.dynamics.com/requestlicense) bazkide eskaintza berria berrikusteko. 
- Barne Erabilera Eskubideei buruzko informazio gehiago bilatzen duten bazkideentzako, ikus [Barne Erabilera Eskubideen hodeia eta softwarearen onura (microsoft.com](https://partner.microsoft.com/membership/internal-use-software).

### <a name="can-i-extend-my-trial-beyond-30-days"></a>Proba luzatu al dezaket 30 egunez harago?
Probaldia luzatzeko, jarraitu urrats hauek.

1. Hurrengoan **Microsoft 365 administrazio-zentroa**, joan **Fakturazioa** > **Zure produktuak**.
2. Hautatu **Dynamics 365 Project Operations (CE) - Aurrebistaren proba**.
3. Azpian **Iraungitze Data**, hautatu **Luzatu Data**.

### <a name="can-i-upgrade-from-the-lite-deployment-to-the-resourcenon-stocked-based-scenario-deployment"></a>Ba al dezaket bertsio berriaren bertsiotik berreskuratzeko baliabiderik / stockean oinarritutako eszenatokien hedapenera?
Gaur egun, ez dago ingurunerik bertsio berritik bertsio berritik hornitzeko ez dagoen inplementaziorako euskarririk.

### <a name="can-i-access-lifecycle-services-lcs-for-my-finance-environments"></a>Sar al naiteke Lifecycle Services (LCS) nire Finantza inguruneetarako?  
Ez. Proba hauetarako, hedapena bidez kudeatzen da Power Platform Administrazio zentroa. Finantza ingurunerako sarbidea mugatuta dago.

### <a name="can-i-install-my-trial-on-an-existing-environment"></a>Instalatu al dezaket nire proba dagoeneko dagoen ingurune batean?
Lehendik dagoen ingurunea baduzu, baimenduko zaizu lite inplementazioa lehendik dagoen salmentetan instalatzea Dataverse ingurunea Power Platform Administrazio zentroa.

[!INCLUDE[footer-include](../includes/footer-banner.md)]