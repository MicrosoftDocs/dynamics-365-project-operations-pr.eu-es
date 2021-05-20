---
title: Proiektuaren fakturen integrazioa
description: Gai honek Project Operations idazketa bikoitzeko integrazioari buruzko informazioa eskaintzen du bezeroaren fakturazio lortzeko.
author: sigitac
ms.date: 04/26/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 102a7cdba467a2071119c5b32d2e75e48170c783
ms.sourcegitcommit: 02f00960198cc78a5e96955a9e4390c2c6393bbf
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/28/2021
ms.locfileid: "5955695"
---
# <a name="project-invoice-integration"></a>Proiektuaren fakturen integrazioa

Gai honek Project Operations idazketa bikoitzeko integrazioari buruzko informazioa eskaintzen du bezeroaren fakturazio lortzeko.

Project Operations-en, proiektuaren kudeatzaileak proiektuaren fakturazioen atzerapena kudeatzen du eta proforma faktura sortzen dio bezeroari Microsoft Dataverse-n. Proforma faktura honetan oinarrituta, Kobratzeko kontuak edo Proiektuaren kontulariak bezeroari begira faktura sortzen du. Idazketa bikoitzeko integrazioak faktura proformaren xehetasunak sinkronizatuta daudela ziurtatzen du Finance and Operations aplikazioak. Bezeroari begirako faktura argitaratu ondoren, sistemak proiektuaren datuak eguneratzen ditu Dataverse kontabilitate xehetasunarekin. Ondorengo grafikoak integrazio horren goi-mailako ikuspegi kontzeptuala eskaintzen du.

   ![Proiektuaren fakturen integrazioa](./media/DW5Invoicing.png)

Proiektu kudeatzaileak proforma faktura baieztatu ondoren Dataverse, proforma fakturaren goiburuaren informazioa sinkronizatzen da Finance and Operations idazketa bikoitzeko taulako mapa erabiltzen duten aplikazioak, **Proiektuaren faktura proposamena V2 (fakturak)**. Hau norabide bakarreko integrazioa da Dataverse Finance and Operations aplikazioetara. Proiektuaren faktura proposamenak zuzenean sortzea edo ezabatzea Finance and Operations aplikazioak ez dira onartzen.

Faktura berrespena Dataverse negozioaren logika ere abiarazten du fakturazioarekin lotutako erregistroak sortzeko **Benetako datuak** entitatea. Erregistro horiek sinkronizatuta daude Finance and Operations idazketa bikoitzeko taulako mapa erabiliz **Project Operations-en integrazioaren benetako datuak (msdyn\_actuals)**. Informazio gehiago lortzeko, ikusi [Proiektuaren kalkuluak eta benetako datuak](resource-dual-write-estimates-actuals.md). 

Proiektuen faktura proposamenen lerroak aldian aldiko prozesuaren bidez sortzen dira, **Inportatu inprimakien eszenaratzea**. Prozesu hau fakturatutako salmenten benetako xehetasunetan oinarritzen da **Benetako eszenaratzea** taula. Informazio gehiagorako, ikusi [Kudeatu proiektuaren faktura proposamenak](../invoicing/format-update-project-invoice-proposals.md#create-project-invoice-proposals). 
