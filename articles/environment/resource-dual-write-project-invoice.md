---
title: Proiektuaren fakturen integrazioa
description: Artikulu honek Project Operations-en idazketa bikoitzeko integrazioari buruzko informazioa eskaintzen du bezeroen fakturaziorako.
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

Artikulu honek Project Operations-en idazketa bikoitzeko integrazioari buruzko informazioa eskaintzen du bezeroen fakturaziorako.

Project Operations-en, proiektuaren kudeatzaileak proiektuaren fakturazioen atzerapena kudeatzen du eta proforma faktura sortzen dio bezeroari Microsoft Dataverse-n. Proforma faktura honetan oinarrituta, Kobratzeko kontuak edo Proiektuaren kontulariak bezeroari begira faktura sortzen du. Idazketa bikoitzeko integrazioak bermatzen du proformako fakturaren xehetasunak finantza- eta eragiketa-aplikazioekin sinkronizatzen direla. Bezeroari begirako faktura argitaratu ondoren, sistemak proiektuaren datuak eguneratzen ditu Dataverse kontabilitate xehetasunarekin. Ondorengo grafikoak integrazio horren goi-mailako ikuspegi kontzeptuala eskaintzen du.

   ![Proiektuaren fakturen integrazioa.](./media/DW5Invoicing.png)

Proiektuaren kudeatzaileak proforma faktura baieztatu ondoren Dataverse, proformako fakturen goiburuko informazioa finantza eta eragiketen aplikazioekin sinkronizatzen da idazketa bikoitzeko taularen mapa erabiliz, **Proiektuaren faktura-proposamena V2 (fakturak)**. Norabide bakarreko integrazioa da Dataverse finantzaketa eta eragiketa aplikazioetarako. Ez da onartzen Project faktura-proposamenak zuzenean finantza- eta operazio-aplikazioetan sortzea edo ezabatzea.

Faktura berrespena Dataverse negozioaren logika ere abiarazten du fakturazioarekin lotutako erregistroak sortzeko **Benetako datuak** entitatea. Erregistro hauek finantza eta eragiketekin sinkronizatzen dira idazketa bikoitzeko taularen mapa erabiliz, **Project Operations integrazio errealak (msdyn\_ benetakoak).** Informazio gehiago lortzeko, ikusi [Proiektuaren kalkuluak eta benetako datuak](resource-dual-write-estimates-actuals.md). 

Proiektuen faktura proposamenen lerroak aldian aldiko prozesuaren bidez sortzen dira, **Inportatu inprimakien eszenaratzea**. Prozesu hau fakturatutako salmenten benetako xehetasunetan oinarritzen da **Benetako eszenaratzea** taula. Informazio gehiagorako, ikusi [Kudeatu proiektuaren faktura proposamenak](../invoicing/format-update-project-invoice-proposals.md#create-project-invoice-proposals). 
