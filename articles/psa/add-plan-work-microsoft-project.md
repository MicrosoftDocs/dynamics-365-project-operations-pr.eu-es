---
title: Erabili Project Service gehigarria Microsoft Project-ekin lanaren plangintza egiteko | MicrosoftDocs
description: Gai honek Microsoft Project gehigarria Microsoft Project Service-en nola gehitu, konfiguratu eta erabiltzeko informazioa ematen du.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 04/06/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 86b676a0cf74e0257fd76cf32271497eebc06e75
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642753"
---
# <a name="use-the-project-service-automation-add-in-to-plan-your-work-in-microsoft-project"></a>Antolatu Microsoft Project lana formateatzeko, Project Service Automation Proiektua Gehitu add-in erabili

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] aplikazioak proiektuen plangintza egiten errazten du, baita gutxi gorabeherakoak ere. Lana daitezen kostuen, ahalegina eta salmenta balio behin betiko proposamena bidali gisa markatu gabe zehatz ditzakezu.  

 Orain [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] instalatu eta lanaren plangintza egin dezakezu [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ingurune ezagunean. Erabili [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikazioaren antolatzeko eta kudeatzeko gaitasun indartsuak eta eguneratu proiektu-plana Project Service Automation-en.  

> [!IMPORTANT]
> - SharePoint dokumentu-kudeaketa [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] proiektuetako zure [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] fitxategiak gordetzeko erabiltzeko, zure [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] administratzaileak dokumentu-kudeaketa aktibatu beharko du. 
> - [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] bateragarria da [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition bertsioarekin.  

## <a name="download-and-install-the-add-in"></a>Deskargatu eta instalatu gehigarria  
 Izan zure [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] saioa hasteko informazioa prest. Informazio hau beharko duzu [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikaziotik [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] aplikaziora konektatzeko.  

1.  Deskarga-zentrotik, deskargatu Project Service-en bertsioa onartzen duen gehigarria [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) edo [V3.4 +](https://www.microsoft.com/download/details.aspx?id=57956).  

2.  Sakatu deskargatu esteka.  

3.  Deskarga amaitzen denean, sakatu **Bai** gehigarria instalatzeko.  

## <a name="configure-the-add-in"></a>Konfiguratu osagarria  

1. Ireki [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] eta sakatu **Project Service** fitxa.  

2. Sakatu **Konektatu**.  

3. Sartu zure saio-informazioa eta, ondoren, sakatu **Saioa**.  

   Orain erabiltzen has zaitezke gehigarria.  

## <a name="read-from-a-template"></a>Irakurri txantiloi bat  
 Irakurri [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] aplikazioan sortu duzun txantiloi batetik eta kopiatu [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikazioan, proiektuaren plangintza hasteko. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Sortu proiektu-txantiloia (Project Service Automation)](../psa/create-project-template.md)  

1.  **Project Service** fitxan, sakatu **Irakurri** > **Project Service Automation proiektu-txantiloia**.  

2.  Aukeratu proiektua txantiloi bat zerrendatik eta, ondoren, sakatu **Ireki**.  

    > [!NOTE]
    >  Modu lehenetsian, dira kopiatu txantiloiaren Proiektua zeregin gisa ezartzen dira eskuz gisa antolatu.  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a>Esleitu [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] funtzioak proiektuaren baliabideei  

1.  Ireki proiektua bat eta sakatu **Zeregina** zinta.  

2.  Sakatu **Gantt diagrama** menua eta, ondoren, aukeratu **Baliabide Orria**.  

3.  Baliabide-Orria, sakatu, **Project Service Automation Baliabide Funtzioak** goitibeherako menuan eta hautatu Project Service Automation funtzio bat.  

## <a name="staff-your-project-with-resources"></a>Zure proiektua baliabideekin staff  

1.  Project Service fitxan aurki daiteke, errenkada bat hautatu eta sakatu **Bilaketa-baliabideak**.  

2.  Atalean, **Liburua Baliabide** pantailan, hautatu proiektuan erabili nahi duzun baliabidea.  

3.  Sakatu **Erreserbatu** eta, ondoren, sakatu **Ados**.  

## <a name="publish-your-project"></a>Zure proiektua argitaratu  
Hurrengo urratsera inportatu eta argitaratzeko, atalean proiektua da antolamendu-proiektua zure bukatuta duzunean, [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

Proiektuan inportatzeko da [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. Prezioak eta taldeak sorrerako prozesu aplikatzen dira. Aplikazioan proiektua ireki [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] duzun taldea, proiektua estimates eta diren kanpaina-xehatzea egitura lan egin ikusteko sortu da. Taula honetan emaitzak non aurkit erakusten da:


|                                                                                          |                                                                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Gantt diagrama**   | [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Zereginen xehetasunen egitura** pantailara inportatzen du. |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Baliabideen orria** |   [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Proiektuko taldekideak** pantailara inportatzen du.   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **Erabili erabilera**    |    [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Proiektuaren aurreikuspenak** pantailara inportatzen du.     |

**Proiektua inportatzeko eta argitaratzeko**  
1. **Project Service** fitxan, sakatu **Argitaratu** > **Project Service Automation berria**.  

2. Tresna-barran **Project Service-n proiektu berria argitaratu** elkarrizketa-koadroan, idatzi- **Proiektuaren izena** eta hautatu **Bezeroa**.  

3. Egiaztatu nahi izanez gero, **Estekatu proiektu-plana Project Service Automation-era** Proiektua fitxategiaren plana Project Service Automation-era estekatzeko.  

4. Sakatu **Argitaratu**.  

   Esteka bat Project fitxategia [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] nagusia fitxategi Proiektua eta lana diren kanpaina-xehatzea egitura [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] batera irakurtzeko soilik.  Proiektu-planean aldaketak egiteko, [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikazioan egin eta eguneratze gisa argitaratu behar dituzu [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] aplikazioan.  

## <a name="edit-a-project-thats-been-imported"></a>Editatu proiektua inportatzen dira  
 [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] aplikaziora inportatu den proiektu-planean aldaketak egiteko, bi aukera dituzu:  

- Ireki fitxategia nagusia eta editatu [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikazioan.  

- Kendu esteka fitxategiari eta editatu zuzenean Project Servicen. Modu lehenetsian, [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikaziotik kargatu den proiektua blokeatuta dago eta Proiektua atalean soilik edita daiteke. Fitxategia [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] aplikazioan editatzeko, fitxategiak askatuta izan behar da.  

### <a name="edit-in-pn_microsoft_project"></a>Editatu [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikazioan  

1. Menu nagusian, sakatu **Project Service** > **Proiektuak**.  

2. Proiektuen zerrendan, ireki [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikazioan sortu duzuna.  

3. Sakatu **Ireki MS Project** zintaren batetik. Estekatutako fitxategi nagusia irekiko da [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]-en.  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a>Kendu esteka fitxategiari eta editatu zuzenean [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]-n  

1. Menu nagusian, sakatu **Project Service** > **Proiektuak**.  

2. Proiektuen zerrendan, ireki [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikazioan sortu duzuna.  

3. Sakatu **Kendu esteka MS Project-ik** zintaren batetik.  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a>SharePoint-eko edo Office Taldeak aplikaziora proiektu-fitxategia kargatu  
 SharePoint-eko proiektu-fitxategia kargatu eta erlazionatutako dokumentuak atalean aurki dezakezu zure [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] proiektua.  Zure administratzaileak SharePoint dokumentu-kudeaketa konfiguratu eta aktibatu behar du Proiektua entitaterako. 

 Office Taldeak konfiguratuta baduzu ere karga dezakezu Proiektua fitxategia [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] aplikazioan.

### <a name="upload-a-file-for-sharepoint"></a>Kargatu fitxategi bat SharePoint-en  

1. Menu nagusian, sakatu **Project Service** > **Kargatu**.  

2. Hautatu **Project Service Automation proiektuaren dokumentuak**.  

3. **Gaitu Ireki [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** elkarrizketan, hautatu **Bai** edo **Ez**.  

   - **Bai** sakatzen baduzu, **Ireki [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**-en botoia hautatu ahal izango duzu Project Service Automation aplikazioan eta [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] abiarazi eta proiektu-fitxategia kargatu ahal izango duzu SharePoint dokumentu-liburutegian.  

   - **Ez** sakatzen baduzu, **Ireki [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** botoiaren estekak ez du funtzionatuko.  

4. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] fitxategia [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] aplikazioan ere aurki daiteke [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] proiektuari dagokion **Dokumentuak** atalean.  

### <a name="upload-a-file-for-office-groups"></a>Fitxategi bat kargatzeko Office Taldeak  

1. Menu nagusian, sakatu **Project Service** > **Kargatu**.  

2. Hautatu **Project Service Automation proiektuaren dokumentuak**.  

3. **Gaitu Ireki [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** elkarrizketan, hautatu **Bai** edo **Ez**.  

   - **Bai** sakatzen baduzu, **Ireki [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**-en botoia hautatu ahal izango duzu Project Service Automation aplikazioan eta [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] abiarazi eta proiektu-fitxategia kargatu ahal izango duzu SharePoint dokumentu-liburutegian.  

   - **Ez** sakatzen baduzu, **Ireki [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** botoiaren estekak ez du funtzionatuko.  

4. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] fitxategia [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] aplikazioan ere aurki daiteke [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] proiektuari dagokion **Dokumentuak** atalean.  

## <a name="publish--your-project-as-a-template"></a>Zure proiektua txantiloi gisa argitaratu  
 Zure proiektua gorde dezakezu eta aplikazioan proiektua txantiloi gisa gorde arabera erabiltzeko [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  Aplikazioan antzekoentzat proiektua planak dira proiektua txantiloiak [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Sortu proiektu-txantiloia (Project Service Automation)](../psa/create-project-template.md)  

1. **Project Service** fitxan, sakatu **Argitaratu** > **Project Service Automation proiektuaren txantiloia**.  

2. **Project Service-n proiektu txantiloia argitaratu** elkarrizketa-koadroan, idatzi- **Proiektu-txantiloiaren izena**.  

3. Nahi izanez gero, egiaztatu **Estekatu proiektu-plana Project Service Automation-era** Proiektua fitxategia [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]-ra estekatzeko.  

4. Sakatu **Argitaratu**.  

Esteka bat Project fitxategia [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] nagusia fitxategi Proiektua eta lana diren kanpaina-xehatzea egitura [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] txantiloi batera irakurtzeko soilik.  Proiektu-planean aldaketak egiteko, [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikazioan egin eta eguneratze gisa argitaratu behar dituzu [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] aplikazioan.

## <a name="read-a-resource-loaded-schedule"></a>Irakurri baliabideak kargatutako programazioa

Project Service Automation-etik proiektu bat irakurtzean, baliabidearen egutegia ez da mahaigaineko bezeroarekin sinkronizatzen. Zereginen iraupenean, esfortzuan edo amaieran desberdintasunak badaude, ziurrenik baliabideek eta mahaigaineko bezeroak ez dutelako proiektuari aplikatutako lan ordu txantiloien egutegi bera.


## <a name="data-synchronization"></a>Datuen sinkronizazioa

Hurrengo taulan datuak Project Service Automation eta Microsoft Project mahaigaineko gehigarriaren artean nola sinkronizatzen diren azaltzen da.

| **Entitatea** | **Eremua** | **Microsoft Project Project Service Automation-en** | **Project Service Automation Microsoft Project-en** |
| --- | --- | --- | --- |
| Proiektuaren zeregina | Epemuga | ● | - |
| Proiektuaren zeregina | Aurreikusitako ahalegina | ● | - |
| Proiektuaren zeregina | MS Project bezeroaren IDa | ● | - |
| Proiektuaren zeregina | Zeregin nagusia | ● | - |
| Proiektuaren zeregina | Project | ● | - |
| Proiektuaren zeregina | Proiektuaren zeregina | ● | - |
| Proiektuaren zeregina | Proiektuaren zereginaren izena | ● | - |
| Proiektuaren zeregina | Baliabidearen unitatea (zaharkitua 3.0 bertsioan) | ● | - |
| Proiektuaren zeregina | Antolatutako iraupena | ● | - |
| Proiektuaren zeregina | Hasiera-data | ● | - |
| Proiektuaren zeregina | WBS IDa | ● | - |

| **Entitatea** | **Eremua** | **Microsoft Project Project Service Automation-en** | **Project Service Automation Microsoft Project-en** |
| --- | --- | --- | --- |
| Taldeko kidea | MS Project bezeroaren IDa | ● | - |
| Taldeko kidea | Lanpostuaren izena | ● | - |
| Taldeko kidea | proiektua | ● | ● |
| Taldeko kidea | Proiektu-taldea | ● | ● |
| Taldeko kidea | Baliabide-unitatea | - | ● |
| Taldeko kidea | Funtzioa | - | ● |
| Taldeko kidea | Lanorduak | Sinkronizatu gabe | Sinkronizatu gabe |

| **Entitatea** | **Eremua** | **Microsoft Project Project Service Automation-en** | **Project Service Automation Microsoft Project-en** |
| --- | --- | --- | --- |
| Baliabide-esleipena | Hasiera-data | ● | - |
| Baliabide-esleipena | ordu | ● | - |
| Baliabide-esleipena | MS Project bezeroaren IDa | ● | - |
| Baliabide-esleipena | Planifikatutako lana | ● | - |
| Baliabide-esleipena | Project | ● | - |
| Baliabide-esleipena | Proiektu-taldea | ● | - |
| Baliabide-esleipena | Baliabide-esleipena | ● | - |
| Baliabide-esleipena | Ataza | ● | - |
| Baliabide-esleipena | Amaiera-data | ● | - |

| **Entitatea** | **Eremua** | **Microsoft Project Project Service Automation-en** | **Project Service Automation Microsoft Project-en** |
| --- | --- | --- | --- |
| Proiektuen zereginen mendekotasunak | Proiektuaren zereginen mendekotasuna | ● | - |
| Proiektuen zereginen mendekotasunak | Esteka mota | ● | - |
| Proiektuen zereginen mendekotasunak | Aurreko zeregina | ● | - |
| Proiektuen zereginen mendekotasunak | Project | ● | - |
| Proiektuen zereginen mendekotasunak | Hurrengo zeregina | ● | - |

### <a name="see-also"></a>Ikusi baita ere  
 [Proiektu-kudeatzailearen gida](../psa/project-manager-guide.md)
