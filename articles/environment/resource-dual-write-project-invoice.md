---
title: Proiektuaren fakturen integrazioa
description: Gai honek Project Operations idazketa bikoitzeko integrazioari buruzko informazioa eskaintzen du bezeroaren fakturazio lortzeko.
author: sigitac
ms.date: 04/26/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 1e7294360f041b030efca225c6754fe3bbc0eadf
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8581223"
---
# <a name="project-invoice-integration"></a>Proiektuaren fakturen integrazioa

Gai honek Project Operations idazketa bikoitzeko integrazioari buruzko informazioa eskaintzen du bezeroaren fakturazio lortzeko.

Project Operations-en, proiektuaren kudeatzaileak proiektuaren fakturazioen atzerapena kudeatzen du eta proforma faktura sortzen dio bezeroari Microsoft Dataverse-n. Proforma faktura honetan oinarrituta, Kobratzeko kontuak edo Proiektuaren kontulariak bezeroari begira faktura sortzen du. Idazketa bikoitzeko integrazioak bermatzen du proformako fakturaren xehetasunak Finantza eta Operazioen aplikazioekin sinkronizatzen direla. Bezeroari begirako faktura argitaratu ondoren, sistemak proiektuaren datuak eguneratzen ditu Dataverse kontabilitate xehetasunarekin. Ondorengo grafikoak integrazio horren goi-mailako ikuspegi kontzeptuala eskaintzen du.

   ![Proiektuaren fakturen integrazioa.](./media/DW5Invoicing.png)

Proiektuaren kudeatzaileak proforma faktura baieztatu ondoren Dataverse, proforma fakturaren goiburuko informazioa Finantza eta Operazioen aplikazioekin sinkronizatzen da idazketa bikoitzeko taularen mapa erabiliz, **Proiektuaren faktura-proposamena V2 (fakturak)**. Norabide bakarreko integrazioa da Dataverse Finantza eta Operazio aplikazioetara. Ez da onartzen Proiektuaren faktura-proposamenak zuzenean Finantza eta Operazioen aplikazioetan sortzea edo ezabatzea.

Faktura berrespena Dataverse negozioaren logika ere abiarazten du fakturazioarekin lotutako erregistroak sortzeko **Benetako datuak** entitatea. Erregistro hauek Finantza eta Operazioekin sinkronizatzen dira idazketa bikoitzeko taularen mapa erabiliz, **Project Operations integrazio errealak (msdyn\_ benetakoak).** Informazio gehiago lortzeko, ikusi [Proiektuaren kalkuluak eta benetako datuak](resource-dual-write-estimates-actuals.md). 

Proiektuen faktura proposamenen lerroak aldian aldiko prozesuaren bidez sortzen dira, **Inportatu inprimakien eszenaratzea**. Prozesu hau fakturatutako salmenten benetako xehetasunetan oinarritzen da **Benetako eszenaratzea** taula. Informazio gehiagorako, ikusi [Kudeatu proiektuaren faktura proposamenak](../invoicing/format-update-project-invoice-proposals.md#create-project-invoice-proposals). 
