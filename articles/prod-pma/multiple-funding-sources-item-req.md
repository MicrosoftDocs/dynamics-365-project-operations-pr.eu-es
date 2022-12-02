---
title: Funts-iturri ugari dituzten proiektu-kontratuen elementuen baldintzak
description: Artikulu honek finantzaketa-iturri anitzekin elementuen baldintzak konfiguratu eta erabiltzeari buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 05/04/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 079856e7cf2ffa9b80ab31ebad1c1b5dbe36a4ad
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/18/2022
ms.locfileid: "9028458"
---
# <a name="item-requirements-for-project-contracts-with-multiple-funding-sources"></a>Funts-iturri ugari dituzten proiektu-kontratuen elementuen baldintzak

_**Honi aplikatzen zaio:** Izakinen edo ekoizpenean oinarritutako egoeretarako Project Operations_

Proiektuetan oinarritutako produktuetarako kontratu-hitzarmen batzuek finantzaketa-iturri anitz behar izan ditzakete. Artikulu honek nahi diren finantzaketa-iturriak nola hautatu eta konfiguratu azaltzen du proiektu edo proiektu-kontratu baterako hainbat iturri behar direnean.

## <a name="terminology"></a>Terminologia

- **Finantziazio iturria** – Proiektuaren kontratuaren obra finantzatzen duen erakundea. Entitate hau barne erakunde bat edo kanpoko faktura-kontu bat izan daiteke (bezeroa edo diru-laguntza).
- **Proiektuaren bezeroa** – Proiektu-lana entregatzen zaion erakundeari.
- **Faktura kontua** – Proiektuaren lana ordaintzen duen kanpoko erakundea.

## <a name="example"></a>Adibidez

Contoso-k ekipamenduak berritzeko kontratua irabazi du bere bezeroetako birekin: Adatum US eta Adatum Corporate. Kontratuak Adatum US (proiektuaren bezeroa) entregatuko dituen hardware eta instalazio zerbitzuak barne hartzen ditu. Hardwarea Adatum Corporate-k finantzatuko du (1. faktura-kontua), eta instalazio lanak Adatum US-ek (2. faktura-kontua).

## <a name="set-up-invoice-account-defaulting-rules-for-item-requirements"></a>Konfiguratu faktura-kontuaren lehenetsitako arauak elementuen eskakizunetarako

### <a name="prerequisites"></a>Aurrebaldintzak

- Microsoft Dynamics 365 Finance-ren **10.0.27 bertsioa edo berriagoa** behar duzu faktura-kontu bat baino gehiago dituzten elementuen eskakizunak erabiltzeko.
- Zure sistema-administratzaileak gaitu behar du **Baimendu elementuen eskakizunak finantzaketa-iturri anitz dituzten Project Operations hornitutako/produkzioan oinarritutako eszenatokietarako** ezaugarria **Ezaugarrien kudeaketa** laneko arean.

### <a name="set-up-the-invoice-account-defaulting-rules"></a>Konfiguratu faktura-kontuaren arau lehenetsiak

Faktura-kontuaren arau lehenetsiak konfiguratzeko, jarraitu urrats hauek.

1. Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Proiektuen kudeaketa eta kontabilitate parametroak**.
1. **Orokorra** fitxan, **Salmenta eskaerak eta elementuen eskakizunak** atalean, ezarri **Finantza-iturri anitz dituzten proiektuak baimendu** aukera **Bai**.
1. **Bezero lehenetsia** eremuan, zehaztu elementuaren eskakizunaren proiektuaren entrega-bezeroa nondik datorren lehenespenez:

    - **Finantza-iturritik** – Proiektua entregatzeko bezero lehenetsia finantzaketa-iturritik dator. Proiektuaren kontratuarekin hainbat finantzaketa-iturri lotzen badira, zerrendako lehen finantzaketa-iturria erabiliko da.
    - **Proiektutik** – Proiektuaren entrega-bezero lehenetsia atalean aukeratutako bezeroarengandik dator **Proiektuaren erregistro-kontua** eremua.

1. Aukerakoa: ezarri edo aldatu faktura-kontu lehenetsia proiektuaren erregistroetan:

    1. Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Proiektuak** \> **Proiektu guztiak** eta ireki proiektuaren erregistroaren xehetasunak.
    2. **Orokorra** fitxan, ezarri edo eguneratu **Faktura-kontu lehenetsia** eremua. Zehazten duzun kontua faktura-kontu lehenetsi gisa erabiliko da proiekturako sortzen diren elementu berrien eskakizunetarako. Eremua hutsik uzten baduzu, lehen proiektuaren kontratuaren finantzaketa iturriaren faktura-kontua erabiliko da lehenespenez. Hala ere, erabiltzaileek kontua aldatzeko aukera izango dute erregistroa gordetzen dutenean.

### <a name="select-the-invoice-account-to-use-when-you-create-an-item-requirement"></a>Hautatu elementu-eskakizun bat sortzen duzunean erabiliko duzun faktura-kontua

Hautatzeko elementu-eskakizun bat sortzen duzunean erabiliko duzun faktura-kontua, jarraitu urratsak.

1. Joan **Proiektuen kudeaketa eta kontabilitate** \> **Proiektuak** \> **Proiektu guztiak** eta hautatu proiektuaren erregistroa.
1. **Plana** fitxan, hautatu **Elementuaren eskakizunak**.
1. Sortu elementuaren eskakizun-erregistro berria.

    - Lehenespenez, **Faktura kontua** Erregistroko eremua proiekturako ezarrita dagoen faktura-kontuan ezartzen da. **Faktura kontua** eremuko balioa alda dezakezu eta, ondoren, erregistroa gorde. Erregistroa gorde ondoren, ezin duzu eguneratu **Faktura kontua** balioa. Eguneratu behar baduzu **Faktura kontua** elementuaren eskakizunaren balioa, ezabatu lehendik dagoen elementuaren eskakizuna eta, ondoren, sortu nahi duzun balioa duen berri bat.
    - Lehenespenez, **Bezeroa** elementuaren eskakizunaren eremuan oinarrituta ezartzen da **Bezero lehenetsia** ezartzen den balioa **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea.

    Elementuaren eskakizunen erregistroa gordetzen denean, sistemak lotzen du **Elementu-eskakizunen salmenta-eskaera** goiburuko erregistroarekin. Salmenta-eskaeraren goiburu irekirik ez badago hautatutako faktura-kontua, sistemak bat sortuko du eta harekin lotuko du elementuen eskakizun-lerroa.

> [!NOTE]
> Elementuaren eskakizunak erregistroan ezartzen den faktura-kontuan fakturatzen dira beti. Sistemak ez ditu onartzen elementuen eskakizunak dituzten finantza-esleipen-arauak, eta ez du argitalpena banatuko finantza-esleipen-arauen konfigurazioaren arabera.

### <a name="create-an-item-requirement-from-an-item-forecast-record"></a>Sortu elementu-eskakizuna elementuen aurreikuspen-erregistro batetik

Sortzeko elementu-eskakizuna elementuen aurreikuspen-erregistro batetik, jarraitu urratsak.

1. Joan **Proiektuen kudeaketa eta kontabilitate** \> **Proiektuak** \> **Proiektu guztiak** eta hautatu proiektuaren erregistroa.
1. **Plana** fitxan, hautatu **Elementuaren iragarpenak**.
1. Sortu elementuaren iragarpen-erregistro berria.
1. Aukerakoa: **Proiektua** fitxan, **Finantziazio iturria** eremuan, hautatu nahi duzun faktura-kontua.
1. Hautatu **Sortu elementuaren eskakizuna**, eta berretsi jasotzen duzun mezua.

    > [!NOTE]
    > Sistemak kopiatzen du **Finantziazio iturria** elementuaren aurreikuspeneko erregistrotik sortu berri den elementuaren eskakizunen erregistrora.

### <a name="default-invoice-account-when-the-system-automatically-creates-an-item-requirement-from-a-purchase-order-line"></a>Faktura-kontu lehenetsia sistemak automatikoki erosketa-eskaeraren lerro batetik elementu-eskakizun bat sortzen duenean

**Sortu elementuaren eskakizuna** aukera ezarrita badago **Bai** gisa **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdean, sistemak automatikoki elementu-eskakizun bat sortzen du proiektuko erosketa-eskaeraren lerro berri bat gordetzen denean. Lehenespenez, **Faktura kontua** eta **Elementuaren eskakizuna** eremuak **Faktura-kontu lehenetsia** eremuaren baliora ezartzen dira proiektuaren erregistroan. Une honetan sistemak ez du onartzen faktura-kontua eguneratzea edo aldatzea mota honetako erregistroetarako.
