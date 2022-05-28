---
title: Sinkronizatu proiektuen kontratuak eta proiektuak zuzenean Project Service Automation-etik Finance-ra
description: Gai honek proiektu-kontratuak eta proiektuak zuzenean sinkronizatzeko erabiltzen diren txantiloia eta azpiko zereginak deskribatzen ditu Microsoft Dynamics 365 Project Service Automation to Dynamics 365 Finance.
author: Yowelle
ms.date: 12/17/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: johnmichalak
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2017-12-13
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 92ebdd864c59168d6f4a4540c6915d6b0dc8a1fb
ms.sourcegitcommit: 2c2a5a11d446adec2f21030ab77a053d7e2da28e
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/04/2022
ms.locfileid: "8684627"
---
# <a name="synchronize-project-contracts-and-projects-directly-from-project-service-automation-to-finance"></a>Sinkronizatu proiektuen kontratuak eta proiektuak zuzenean Project Service Automation-etik Finance-ra 

[!include[banner](../includes/banner.md)]



Gai honek proiektu-kontratuak eta proiektuak zuzenean sinkronizatzeko erabiltzen diren txantiloia eta azpiko zereginak deskribatzen ditu Dynamics 365 Project Service Automation to Dynamics 365 Finance.

> [!NOTE] 
> Enterprise edition 7.3.0 erabiltzen ari bazara, KB 4074835 instalatu behar duzu.

## <a name="data-flow-for-project-service-automation-to-finance"></a>Project Service Automation Finantzararen datu-fluxua

> [!NOTE]
> Project Service Automation to Finance integrazio konponbidea erabili aurretik, Dynamics 365 Data integrazio funtzioa ezagutu beharko zenuke.

Project Service Automation to Finance integrazio irtenbideak Datu integrazio funtzioa erabiltzen du datuak Project Service Automation eta Finance-ren instantzia guztietan sinkronizatzeko. Integrazio-txantiloia eskuragarri dagoen Datu-integrazio eginbideak gaitu egiten du fluxuaren datuak proiektuari buruzko kontratuak, proiektuak, proiektuaren kontratuaren lerroak eta proiektuaren kontratu-lerroak mugarriak Project Service Automation Finantzara.

Ondorengo ilustrazioak erakusten du nola sinkronizatzen diren datuak Project Service Automation eta Finance artean.

[![Project Service Automation Finantzarekin integratzeko datuen fluxua.](./media/ProjectsAndContractsFlow_upd.JPG)](./media/ProjectsAndContractsFlow.JPG)

## <a name="templates-and-tasks"></a>Txantiloiak eta zereginak

Eskuragarri dauden txantiloietara sartzeko, Microsoft Power Apps administratzaile zentroa, hautatu **Proiektuak** eta, ondoren, goiko eskuineko izkinan, hautatu **Proiektu berria** txantiloi publikoak hautatzeko.

Ondorengo txantiloiak eta azpiko zereginak proiektuaren kontratuak eta proiektuak Project Service Automation-etik Finantzara sinkronizatzeko erabiltzen dira:

### <a name="integrating-with-dynamics-365-project-service-automation-v2x"></a>Honekin integratzea Dynamics 365 Project Service Automation v2.x
- **Datuen integrazioko txantiloiaren izena:** Proiektuak eta kontratuak (Project Service Automation-etik Finance-ra)
- **Proiektuko zereginaren izena:**

    - Proiektu-kontratuak Project Service Automation-etik Finance-ra
    - Proiektuak Project Service Automation-etik Finance-ra
    - Proiektuaren kontratuaren lerroak Project Service Automation-etik Finance-ra
    - Proiektuaren kontratuaren lerroaren mugarriak Project Service Automation-etik Finance-ra
  
### <a name="integrating-with-dynamics-365-project-service-automation-v3x"></a>Honekin integratzea Dynamics 365 Project Service Automation v3.x
Project Service Automation-en eskema-aldaketa dago eta horrek Project contract line mugarriko txantiloian eragiten du eta txantiloiaren v2 bertsioaren erabilera beharrezkoa da Project Service Automation v3.x Dynamics 365-ekin integratzeko.

- **Datuen integrazioko txantiloiaren izena:** Proiektuak eta kontratuak (Project Service Automation 3.x bertsiotik Finance-ra) - v2
- **Proiektuko zereginaren izena:**

    - Proiektu-kontratuak Project Service Automation-etik Finance-ra
    - Proiektuak Project Service Automation-etik Finance-ra
    - Proiektuaren kontratuaren lerroak Project Service Automation-etik Finance-ra
    - Proiektuaren kontratuaren lerroaren mugarriak Project Service Automation-etik Finance-ra

Proiektuen kontratuen eta proiektuen sinkronizazioa gertatu aurretik, kontuak sinkronizatu behar dituzu.

## <a name="entity-set"></a>Entitate multzoaren

| Project Service Automation       | Finantzak                                                |
|----------------------------------|--------------------------------------------------------|
| Eskaerak                           | Integrazioaren entitatea proiektuaren kontratua                |
| Proiektuak                         | Proiektuaren datu-bateratuak integrazio entitatea                         |
| Eskaeren lerroak                      | Integrazioaren entitatea proiektuaren kontratu-lerroa           |
| Proiektuaren kontratu-lerroa mugarriak | Integrazioaren entitatea proiektuaren kontratu-lerroa mugarria |

## <a name="entity-flow"></a>Entitate fluxua

Proiektuaren kontratuak Project Service Automation-en kudeatzen dira eta Finantzarekin sinkronizatzen dira proiektuaren kontratuak gisa. Integrazio txantiloiaren zati gisa, Finantzako integrazio iturria ezar dezakezu proiektuaren kontraturako.

Denbora, materiala eta prezio finkoko proiektuak Project Service Automation-en kudeatzen dira eta Finantzarekin sinkronizatzen dira proiektu gisa. Txantiloien integrazioaren zati gisa, proiektuaren integrazio iturria Finantzan ezar dezakezu. Gaur egun, denbora, materiala eta prezio finkoa duten proiektuak bakarrik onartzen dira.


Proiektuaren kontratu-lerroak Project Service Automation-en kudeatzen dira eta Finantzarekin sinkronizatzen dira proiektuaren kontratuaren fakturazio-arauak. Fakturazio-metodoa proiektu mota lehenetsiaren aldean badago, sinkronizazioak proiektu mota kontratu lerroaren proiektuaren eta proiektu taldearen eguneratzen du.

Proiektuaren kontratu-lerroaren mugarriak Project Service Automation-en kudeatzen dira eta Finantzarekin sinkronizatzen dira proiektuaren kontratuaren fakturazio-araua mugarriak.

## <a name="project-service-automation-to-finance-integration-solution"></a>Project Service Automation Finantzararen integrazioaren soluzioa

**Proiektuaren kontratuaren IDa** eremua eskuragarri dago **Proiektuen kontratuak** orrialdea. Eremu hau integrazioari laguntzeko gako natural eta bakarra bihurtu da.

Proiektu kontratu berria sortzen denean, **Proiektuaren kontratuaren IDa** balioa ez da existitzen, zenbaki sekuentzia erabiliz automatikoki sortzen da. Balioa honakoa da **ORD** ondoren, zenbaki sekuentzia hazkundea eta gero sei karaktereko atzizkia. Hemen dago adibidea: **ORD-01022-Z4M9Q0**.

**Proiektuaren zenbakia** eremua eskuragarri dago **Proiektuak** orrialdea. Eremu hau integrazioari laguntzeko gako natural eta bakarra bihurtu da.

Proiektu kontratu berria sortzen denean, **Proiektuaren zenbakia** balioa ez da existitzen, zenbaki sekuentzia erabiliz automatikoki sortzen da. Balioa honakoa da **PRJ** ondoren, zenbaki sekuentzia hazkundea eta gero sei karaktereko atzizkia. Hemen dago adibidea: **PRJ-01049-CCNID0**.

Project Service Automation to Finance integrazio irtenbidea aplikatzen denean, bertsio berritzeko script batek ezartzen du **Proiektuaren kontratuaren IDa** lehendik dauden proiektuen kontratuetarako eta **Proiektuaren zenbakia** Project Service Automation-en dauden proiektuetarako eremua.

## <a name="prerequisites-and-mapping-setup"></a>Aurrebaldintzak eta mapen konfigurazioa

- Proiektuen kontratuen eta proiektuen sinkronizazioa gertatu aurretik, kontuak sinkronizatu behar dituzu.
- Zure konexio multzoan, gehitu integrazio gako eremuen mapak **msdyn\_antolakuntza-unitateak** hurrengora **msdyn\_izena \[Izena\]**. Baliteke proiektu bat konexio multzoari gehitu behar izatea. Informazio gehiagorako, ikus [Integratu datuak Common Data Service Aplikazioetarako](/powerapps/administrator/data-integrator).
- Zure konexio multzoan, gehitu integrazio gako eremuen mapak **msdyn\_proiektuak** hurrengora **msdyn\_proiektuarenzenbakia \[Proiektuaren zenbakia\]**. Baliteke proiektu bat konexio multzoari gehitu behar izatea. Informazio gehiagorako, ikus [Integratu datuak Common Data Service Aplikazioetarako](/powerapps/administrator/data-integrator).
- **SourceDataID** proiektuetarako kontratuak eta proiektuak beste balio batera eguneratu edo mapatik kendu daitezke. Txantiloi balio lehenetsia da **Project Service Automation**.
- **Ordainketa baldintzak** mapak eguneratu behar dira, Finantzan ordainketa baldintzak baliozkoak izan daitezen. Kartografia proiektuaren zereginetik ere kendu dezakezu. Lehenetsitako balioen mapak balio lehenetsiak ditu demo datuetarako. Hurrengo taulan Project Service Automation-eko balioak agertzen dira.

    | Balioa | Deskribapenak   |
    |-------|---------------|
    | 1     | 30 egunera        |
    | 2     | % 2, 10, 30 egun naturalera |
    | 3     | 45 egunera        |
    | 4     | 60 egunera        |

## <a name="power-query"></a>Power Query

Erabili Microsoft Power Query Excel-ek datuak iragazteko baldintza hauek betetzen badira:

- Salmenta aginduak dituzu Dynamics 365 Sales zerbitzuan.
- Antolakuntza unitate ugari dituzu Project Service Automation zerbitzuan, eta antolakuntza unitate horiek Finantzako pertsona juridiko anitzetara mapatuko dira.

Erabili behar baduzu Power Query, jarraitu jarraibide hauek:

- Proiektuak eta kontratuak (PSA Fin eta Ops) txantiloiak iragazki lehenetsia du, salmenta aginduak soilik biltzen dituena **Laneko elementua (msdyn\_ordertype = 192350001)** mota. Iragazki honek Finantzako salmenta-eskaeretarako proiektuen kontratuak ez direla bermatzen laguntzen du. Zure txantiloia sortzen baduzu, iragazki hau gehitu behar duzu.
- Sortu a Power Query integrazio-konexio-multzoaren entitate juridikoarekin sinkronizatu behar diren kontratu-erakundeak soilik biltzen dituen iragazkia. Adibidez, Contoso AEBetako kontratuaren antolakuntza-unitatearekin dituzun proiektuen kontratuak USSI entitate juridikoarekin sinkronizatuta egon beharko lirateke, baina Contoso Global-en kontratuaren antolakuntza-unitatearekin dituzun proiektuen kontratuak USMF entitate juridikoarekin sinkronizatu beharko lirateke. Iragazki hau zure zereginen mapetan gehitzen ez baduzu, proiektuaren kontratu guztiak konexio multzoarentzako definitutako pertsona juridikoarekin sinkronizatuko dira, kontratuaren antolakuntza unitatea edozein dela ere.

## <a name="template-mapping-in-data-integration"></a>Datuen integrazioan txantiloien mapaketa

> [!NOTE] 
> **Bezeroaren erreferentzia**, **HelbideaHiria**, **HelbideaHerrialdeaEskualdeID**, **Helbidea Deskribapena**, **Helbidea 1. lerroa**, **HelbideLinea2**, **HelbideaEstatua**, eta **HelbideaZipKodea** eremuak ez daude proiektuen kontratuen mapaketa lehenetsian sartuta. Datu horiek proiektuen kontratuetarako sinkronizatzea eskatzen baduzu mapak gehi ditzakezu.
>
> **Deskribapena**, **Guraso IDa**, **ProiektuTaldea**, **ProjectManagerPersonnelNumber**, eta **Proiektu mota** eremuak ez daude proiektuen mapaketa lehenetsian sartuta. Datu horiek proiektuen sinkronizatzea eskatzen baduzu mapak gehi ditzakezu.

Ondorengo ilustrazioak Datuen integrazioan txantiloien atazen maparen adibide bat erakusten du. Kartografiak Project Service Automation-etik Finantzara sinkronizatuko den eremuko informazioa erakusten du.

[![Proiektuen kontratuen txantiloien mapaketa.](./media/ProjectContractTemplateMapping.JPG)](./media/ProjectContractTemplateMapping.JPG)

[![Proiektuen txantiloien mapaketa.](./media/ProjectTemplateMapping.JPG)](./media/ProjectTemplateMapping.JPG)

[![Proiektuen kontratuaren lerroen txantiloien mapaketa.](./media/ProjectContractLinesMapping.JPG)](./media/ProjectContractLinesMapping.JPG)

[![Proiektuen kontratuaren lerroen mugarrien txantiloien mapaketa.](./media/ProjectContractLineMilestonesMapping.JPG)](./media/ProjectContractLineMilestonesMapping.JPG)

#### <a name="project-contract-line-milestone-mapping-in-the-projects-and-contracts-psa-3x-to-dynamics---v2-template"></a>Proiektuen kontratuaren lerro mugarriaren proiektuak eta kontratuak (PSA 3.x-ra dinamikara) - v2 txantiloia:

[![Proiektuen kontratuaren lerroen mugarrien mapaketa bertsioaren bi txantiloiekin.](./media/ProjectContractLineMilestoneMapping_v2.jpg)](./media/ProjectContractLineMilestoneMapping_v2.jpg)


[!INCLUDE[footer-include](../includes/footer-banner.md)]