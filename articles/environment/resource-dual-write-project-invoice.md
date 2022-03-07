---
title: Proiektuaren fakturen integrazioa
description: Gai honek Project Operations idazketa bikoitzeko integrazioari buruzko informazioa eskaintzen du bezeroaren fakturazio lortzeko.
author: sigitac
ms.date: 04/26/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 37549080d76e3bffd7cb002aee8e3c46b9eeb18e3cec915cd971881b69747534
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6993226"
---
# <a name="project-invoice-integration"></a>Proiektuaren fakturen integrazioa

Gai honek Project Operations idazketa bikoitzeko integrazioari buruzko informazioa eskaintzen du bezeroaren fakturazio lortzeko.

Project Operations-en, proiektuaren kudeatzaileak proiektuaren fakturazioen atzerapena kudeatzen du eta proforma faktura sortzen dio bezeroari Microsoft Dataverse-n. Proforma faktura honetan oinarrituta, Kobratzeko kontuak edo Proiektuaren kontulariak bezeroari begira faktura sortzen du. Idazketa bikoitzeko integrazioak faktura proformaren xehetasunak sinkronizatuta daudela ziurtatzen du Finance and Operations aplikazioak. Bezeroari begirako faktura argitaratu ondoren, sistemak proiektuaren datuak eguneratzen ditu Dataverse kontabilitate xehetasunarekin. Ondorengo grafikoak integrazio horren goi-mailako ikuspegi kontzeptuala eskaintzen du.

   ![Proiektuaren fakturen integrazioa.](./media/DW5Invoicing.png)

Proiektu kudeatzaileak proforma faktura baieztatu ondoren Dataverse, proforma fakturaren goiburuaren informazioa sinkronizatzen da Finance and Operations idazketa bikoitzeko taulako mapa erabiltzen duten aplikazioak, **Proiektuaren faktura proposamena V2 (fakturak)**. Hau norabide bakarreko integrazioa da Dataverse Finance and Operations aplikazioetara. Proiektuaren faktura proposamenak zuzenean sortzea edo ezabatzea Finance and Operations aplikazioak ez dira onartzen.

Faktura berrespena Dataverse negozioaren logika ere abiarazten du fakturazioarekin lotutako erregistroak sortzeko **Benetako datuak** entitatea. Erregistro horiek sinkronizatuta daude Finance and Operations idazketa bikoitzeko taulako mapa erabiliz **Project Operations-en integrazioaren benetako datuak (msdyn\_actuals)**. Informazio gehiago lortzeko, ikusi [Proiektuaren kalkuluak eta benetako datuak](resource-dual-write-estimates-actuals.md). 

Proiektuen faktura proposamenen lerroak aldian aldiko prozesuaren bidez sortzen dira, **Inportatu inprimakien eszenaratzea**. Prozesu hau fakturatutako salmenten benetako xehetasunetan oinarritzen da **Benetako eszenaratzea** taula. Informazio gehiagorako, ikusi [Kudeatu proiektuaren faktura proposamenak](../invoicing/format-update-project-invoice-proposals.md#create-project-invoice-proposals). 
