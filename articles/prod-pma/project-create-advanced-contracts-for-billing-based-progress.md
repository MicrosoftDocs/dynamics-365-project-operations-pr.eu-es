---
title: Sortu fakturazioaren araberako aurrerapenerako kontratu aurreratuak
description: Gai honetan proiektuen kontratuak nola sortu azaltzen da, bezeroentzako fakturak sortu ahal izateko, egindako lanaren ehunekoan oinarrituta.
author: RadhikaRS
manager: AnnBe
ms.date: 03/26/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 1a83785a9db4dffc4585acf11ef971c08594f312
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071165"
---
# <a name="create-advanced-contracts-for-billing-based-on-progress"></a>Sortu fakturazioaren araberako aurrerapenerako kontratu aurreratuak
[!include [banner](../includes/banner.md)]

Gai honetan proiektuen kontratuak nola sortu azaltzen da, bezeroentzako fakturak sortu ahal izateko, egindako lanaren ehunekoan oinarrituta. Fakturen zenbatekoak automatikoki kalkulatzen dira proiektu baterako konfiguratutako aurrekontu lanen kategorietarako. Fakturaren denbora ezartzen da bezeroarekin proiektuaren kontratua negoziatzen duzunean.

Erabili gai honetako prozedurak kontratua, lotutako proiektu bat eta proiektuarentzako konfiguratu dituzun aurrekontuen lan-kategorien fakturen zenbatekoak kalkulatzen dituzten fakturazio-arauak ezartzeko.

Kontratua eta proiektua sortu ondoren, proiektuaren xehetasunak konfigura ditzakezu. Adibidez, jarduerak definitu eta langileak proiektuan esleitu ditzakezu.

## <a name="example"></a>Adibidez

Zure erakundea softwarea garatzeko enpresa da. Onartzen duzu bezeroarentzako nominaren kontabilitate paketea garatzea, guztira 20.000 dolar (USD) kuotaren truke. Zure erakundeak ados dago bezeroari fakturatzea proiektuaren ehuneko zehatzak burutu ahala. Proiektuen kategoria hauek konfiguratzen dituzu lanerako, fakturazio prozesuan erabil ditzazun:

- Aholkularitza
- Diseinua
- Instalazioa

Fakturazio-arauak konfiguratzen dituzu kategoria bakoitzerako egindako proiektuaren lan portzentajearen fakturen zenbatekoak automatikoki kalkulatzen dituztenak.

Aurrekontu kudeatzaileak proiektuen kategorietarako aurrekontua sortzen du. Egindako lanaren zenbatekoa automatikoki kalkulatzen da benetako lanaren ehuneko gisa, aurrekontuekin alderatuta.

## <a name="prerequisites"></a>Aurrebaldintzak

Fakturazio arauak erabiltzen dituen proiektua sortu aurretik, fakturazio arauen zenbaki sekuentziak eta aurrerapen fakturazioak argitaratzeko erabiltzen den kuota egunkaria ezarri behar dituzu.

1. Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Proiektuen kudeaketa eta kontabilitate parametroak**.
2. **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdean, **Zenbaki sekuentziak** fitxa, konfiguratu fakturazio arauak sortzen direnean erabili nahi duzun zenbaki sekuentzia.
3. Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Egunkariak** \> **Kostua**.
4. **Tasen aldizkaria** orrialdean, hautatu **Berria** , eta idatzi aldizkariaren izena.

## <a name="create-a-contract-for-progress-billings"></a>Sortu aurrerapen fakturazioetarako kontratua

Erabili prozedura hau prezio finko baterako proiektuaren kontratua sortzeko. Proiektuaren faktura sortzen duzu proiektuan amaitutako lana ehuneko jakin batera iristen denean.

1. Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Proiektuak** \> **Proiektu-kontratuak**.
2. **Proiektuaren kontratuak** orrian, hautatu **Berria**.
3. **Proiektuaren kontratu berria** elkarrizketa-koadroan, ezarri eremu hauek:

    - **Izena**
    - **Funts mota**
    - **Finantzaketa iturria**
    - **Salmenten moneta** - Lehenespenez, moneta hau proiektuaren kontratuarekin lotutako bezeroen fakturetarako erabiltzen da. Hala ere, salmenten moneta alda dezakezu bezeroaren faktura jakin batean.

4. Hautatu **Ados**. Informazioa fitxategiaren goiburuan kopiatzen da **Proiektuen kontratuak** orrialdea.
5. **Proiektuen kontratuak** orrialdean, bete proiektuarentzako beharrezko gainerako informazioa.

## <a name="create-a-project-for-progress-billings"></a>Sortu aurrerapen fakturazioetarako proiektua

Jarraitu urrats hauek proiektu bat eta proiektuaren kontratuarekin lotura duten azpiproiektuak sortzeko.

1. Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Proiektuak** \> **Proiektu guztiak**.
2. **Proiektu denak** orrian, hautatu **Berria**.
3. **Proiektu berria** elkarrizketa-koadroan, **Proiektu mota** eremuan, hautatu **Denbora eta materiala**.
4. Hautatu proiektu-taldea. Proiektu talde batek taldeari esleitutako proiektuen argitaratze informazioa definitzen du.
5. Hautatu **Sortu proiektua**.
6. Proiektua sortu ondoren, ezarri proiektuaren etapa **Prozesuan**.

## <a name="create-a-budget-for-a-project"></a>Sortu proiektu baten aurrekontua

Aurrekontu kategoriak kategoria bakoitzerako egindako lan portzentajearen fakturen zenbatekoak automatikoki kalkulatzeko erabiltzen dituztenak. Jarraitu urrats hauei aurrekontu-kategoriak sortzeko kalkulatutako kostuetarako.

1. Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Proiektuak** \> **Proiektu guztiak**.
2. **Proiektu guztiak** orrian, hautatu eta ireki nahi duzun proiektua.
3. **Proiektuak** orrialdeko Ekintza panelean, **Plana** fitxan, **Aurrekontua** taldean, hautatu **Proiektuaren aurrekontua**.
4. **Proiektuaren aurrekontua** orrian, sartu proiektuaren kategoria bakoitzaren kostu estimatua.

## <a name="create-billing-rules-for-progress-billings"></a>Sortu fakturazio arauak aurrerapen fakturazioetarako

1. Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Proiektuak** \> **Proiektu-kontratuak**.
2. **Proiektuen kontratuak** orrian, hautatu eta ireki proiektu-kontratua.
3. Proiektuaren kontratuaren orrian, **Fakturazio arauak** FastTab-en, hautatu **Gehitu**.
4. **Fakturazio araua** orrialdean, **Lerro mota** eremua, hautatu **Aurrerapena**.
5. **Fakturazio arauaren lerroaren xehetasunak** FastTab fitxategian **Kontratuaren balioa** eremuan, sartu kontratuaren balio osoa.
6. **Kategoria** eremuan, hautatu kuota transakzioa bidaltzeko kategoria.
7. **Proiektua** eremuan, hautatu fakturazio arau hau erabiltzen duen proiektua.
8. Aukerakoa: esleitu fakturazio araua proiektu osagarriei. **Proiektua** FastTab fitxategian **Eskuragarri dauden proiektuak** atalean, hautatu proiektu bat eta, ondoren, hautatu eskuineko geziaren botoia proiektua gehitzeko **Aukeratutako proiektuak** atala.
9. Aukerakoa: kalkulatu fakturak fakturatutako ordainketetan bezeroak gordetzen duen ehuneko kopurua. **Ordainketak atxikitzeko baldintzak** FastTab-en, hautatu finantzaketa iturria eta, ondoren, **Atxikipen portzentajea** eremuan, sartu atxikipen ehunekoa.
10. Errepikatu urrats hauek proiektuaren kontratuaren fakturazio arau osagarriak sortzeko.


[!INCLUDE[footer-include](../includes/footer-banner.md)]