---
title: Proiektuaren fakturen integrazioa
description: Gai honek Project Operations idazketa bikoitzeko integrazioari buruzko informazioa eskaintzen du bezeroaren fakturazio lortzeko.
author: sigitac
ms.date: 04/26/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 61f16ebdbabd6545c09d8d7bd82d99b85dc09975
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/18/2022
ms.locfileid: "9029009"
---
# <a name="project-invoice-integration"></a>Proiektuaren fakturen integrazioa

Gai honek Project Operations idazketa bikoitzeko integrazioari buruzko informazioa eskaintzen du bezeroaren fakturazio lortzeko.

Project Operations-en, proiektuaren kudeatzaileak proiektuaren fakturazioen atzerapena kudeatzen du eta proforma faktura sortzen dio bezeroari Microsoft Dataverse-n. Proforma faktura honetan oinarrituta, Kobratzeko kontuak edo Proiektuaren kontulariak bezeroari begira faktura sortzen du. Idazketa bikoitzeko integrazioak faktura proformaren xehetasunak sinkronizatuta daudela ziurtatzen du finantzen eta eragiketen aplikazioak. Bezeroari begirako faktura argitaratu ondoren, sistemak proiektuaren datuak eguneratzen ditu Dataverse kontabilitate xehetasunarekin. Ondorengo grafikoak integrazio horren goi-mailako ikuspegi kontzeptuala eskaintzen du.

   ![Proiektuaren fakturen integrazioa.](./media/DW5Invoicing.png)

Proiektu kudeatzaileak Dataverse proforma faktura baieztatu ondoren , proforma fakturaren goiburuaren informazioa sinkronizatzen da finantzen eta eragiketen idazketa bikoitzeko taulako mapa erabiltzen duten aplikazioak, **Proiektuaren faktura proposamena V2 (fakturak)**. Hau norabide bakarreko integrazioa da Dataverse-tik finantzen eta eragiketen aplikazioetara. Proiektuaren faktura proposamenak zuzenean sortzea edo ezabatzea finantzen eta eragiketen aplikazioak ez dira onartzen.

Faktura berrespena Dataverse negozioaren logika ere abiarazten du fakturazioarekin lotutako erregistroak sortzeko **Benetako datuak** entitatea. Erregistro horiek sinkronizatuta daude finantzen eta eragiketen idazketa bikoitzeko taulako mapa erabiliz **Project Operations-en integrazioaren benetako datuak (msdyn\_actuals).** Informazio gehiago lortzeko, ikusi [Proiektuaren kalkuluak eta benetako datuak](resource-dual-write-estimates-actuals.md). 

Proiektuen faktura proposamenen lerroak aldian aldiko prozesuaren bidez sortzen dira, **Inportatu inprimakien eszenaratzea**. Prozesu hau fakturatutako salmenten benetako xehetasunetan oinarritzen da **Benetako eszenaratzea** taula. Informazio gehiagorako, ikusi [Kudeatu proiektuaren faktura proposamenak](../invoicing/format-update-project-invoice-proposals.md#create-project-invoice-proposals). 
