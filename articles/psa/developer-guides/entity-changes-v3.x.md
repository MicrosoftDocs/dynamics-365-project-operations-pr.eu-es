---
title: Entitatea, kontrola eta erabiltzaile-interfazearen aldaketak (Project Service Automation 3.x)
description: Gai honetan irtenbide aldaketak deskribatzen dira Microsoft Dynamics Project Service Automation 3.x-rako.
author: makk
ms.custom:
- dyn365-projectservice
ms.date: 03/15/2019
ms.topic: article
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: da43e0d15e655977c0c1be7348192a0189a56a6c
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8597553"
---
# <a name="entity-control-and-user-interface-changes-project-service-automation-3x"></a>Entitatea, kontrola eta erabiltzaile-interfazearen aldaketak (Project Service Automation 3.x)

[!include [banner](../../includes/psa-now-project-operations.md)]


Microsoft Dynamics Project Service Automation (PSA) 3.x-ren kaleratzearekin batera, aldaketa ugari egin dira entitateetan, kontroletan, bistaratzeetan eta erabiltzaile-interfazean. GAi honekaldaketa garrantzitsu hauei buruzko informazioa du:

## <a name="parent-child-relationships-for-sales-document-sales-document-line-sales-document-line-detail-entities"></a>Lehen eta bigarren mailako harremanak salmentarako dokumentuetarako, salmenten dokumentuen lerroetarako, entitateen salmenten dokumentuen lerroaren xehetasunetarako
Bertsioetan Dynamics 365 Project Service Automation (PSA) 3.0 bertsioa baino lehen kaleratu zen, salmenten dokumentuen, salmenta dokumentuen lerroen eta entitateen salmenten dokumentuen lerroaren xehetasunen arteko erlazio batzuk erlazionatutako entitatearen GUIDaren katearen sorrera-eremuen bidez gauzatu ziren. Hori soluzioaren zerbitzariaren eta bezeroaren aldeetan kode pertsonalizatuak garrantzitsuak eskatzen zituzten plataformen mugengatik izan zen, harreman horiek funtsezkoak izan zitezen Dynamics CRM entitate harremanak eta kate-eremuak bilaketa-eremuak bezala jarduteko.

PSA 3.0 eguneratu da salmenta-agiriaren eta salmenta-dokumentuen lerroko entitateen arteko harreman berriak aprobetxatzeko.

Bilatze-eremuak entitateen erreferentziak adierazteko erabil daitezkeenez, aurreko bertsioetan erlazionatutako GUIDaren kate balioa zuten eremuak ez dira gehiago behar, eta beraz, gaitzetsi dira. Legatuko kate-eremuek definitutako harremanak kudeatzen dituen bezero eta zerbitzariaren alboko kodea ere gaitzetsi dira.

### <a name="entity-schema-changes"></a>Entitatearen eskema aldatu da
Hurrengo taulan, gaitzetsitako kate-eremuen eta entitateen bilaketa-eremu berrien banakako zerrenda eskaintzen dira. 

 Entitatea |   Gaitzetsitako eremua (katea) | Bilaketa berria (bilaketa)
--- | --- | ---
invoicedetail (fakturaren lerroa) |  msdyn_contractline |    msdyn_contractlineid
msdyn_actual (unekoa) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_contractlineinvoiceschedule (proiektuko kontratuaren lerroaren faktura-antolaketa) |    msdyn_contractline |    msdyn_contractlineid
msdyn_contractlinescheduleofvalue (proiektuko kontratuaren lerroaren mugarria) |   msdyn_contractline |    msdyn_contractlineid
msdyn_fact (gertaera) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_invoicelinetransaction (fakturaren lerroaren xehetasuna) | msdyn_invoiceline <br> msdyn_salescontractline | msdyn_invoicelineid <br> msdyn_salescontractlineid
msdyn_journalline (kutxako liburuaren lerroa) |  msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_orderlineresourcecategory (Proiektu-kontratuaren lerroko baliabide-kategoria) | msdyn_salescontractline |   msdyn_contractlineid
msdyn_orderlinetransaction (Proiektu-kontratuaren lerroaren xehetasuna) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_orderlinetransactioncategory (Proiektu-kontratuaren lerroko transakzio-kategoria) |   msdyn_contractline |    msdyn_contractlineid
msdyn_orderlinetransactionclassification (Proiektu-kontratuaren lerroko transakzio-sailkapena) |   msdyn_contractline |    msdyn_contractlineid
msdyn_quotelineinvoiceschedule (eskaintzaren lerroko fakturazio-antolaketa) |  msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelineresourcecategory (eskaintzaren lerroko baliabide-kategoria) |    msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinescheduleofvalue (eskaintzaren lerroko mugarria) | msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransaction (eskaintzaren lerroko xehetasuna) |    msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransactioncategory (eskaintzaren lerroko transakzio-kategoria) |  msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransactionclassification (eskaintzaren lerroko transakzio-sailkapena) |  msdyn_quoteline |   msdyn_quotelineid
SalesOrderDetail (eskaera lerroa) | msdyn_quotelineid | msdyn_quoteline 

### <a name="deprecated-custom-views-and-controls"></a>Gaitzetsitako ikuspegiak eta kontrolak
Hurrengo ikuspegi pertsonalizatuak eta kontrolak eta horiekin erlazionatutako artefaktuak gaitzetsi dira.

- Aplikagarritasun ikuspegia.
- Saretako kontrol pertsonalizatuak eskaintzaren lerroko xehetasunak erakusteko eskaintzaren lerroko **Proiektuaren informazioa** orrialdean.
- Saretako kontrol pertsonalizatuak proiektu-kontratuaren lerroko xehetasunak erakusteko salmenta-eskaera lerroko **Proiektuaren informazioa** orrialdean.

> [!NOTE]
> Gaitzetsitako baliabideen zerrenda osoa ikusteko, ikusi [gaitzetsitako web baliabideak Project Service Automation v3.x-en](../developer-guides/web-resources-deprecated-v3.x.md)

## <a name="unified-client-interface-app-module"></a>Bezero-interfazearen aplikazio bateratua
Bezero-interfazearen (UCI) aplikazio moduluaren sarrerarekin, PSAren gunearen maparen sarrerak sistematik kendu dira.  
Abagunea, eskaintza, eskaera eta faktura inprimakiak aldatzeari lotutako funtzionaltasuna gaitzetsi da jada beharrezkoa ez delako UCI aplikazio moduluak inprimakien PSA bertsioak baino ez dituelako.  

Web-baliabide hauek gaitzetsi dira:

- msdyn_\SalesDocument\SalesDocumentFormLoader.js
- msdyn_\SalesDocument\PSSalesDocumentCustomFormIds.js

> [!NOTE]
> Gaitzetsitako baliabideen zerrenda osoa ikusteko, ikusi [gaitzetsitako web baliabideak Project Service Automation v3.x-en](../developer-guides/web-resources-deprecated-v3.x.md).




[!INCLUDE[footer-include](../../includes/footer-banner.md)]
