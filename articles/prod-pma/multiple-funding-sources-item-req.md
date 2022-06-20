---
title: Funts-iturri ugari dituzten proiektu-kontratuen elementuen baldintzak
description: Artikulu honetan, finantzaketa-jatorri bat baino gehiago duten elementuen betekizunak nola konfiguratu eta nola erabili zehazten eta nola erabili zehazten da.
author: sigitac
ms.date: 05/04/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: a54ca1ec5e78d9d0af7b67914f6a63154c7347d3
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8931177"
---
# <a name="item-requirements-for-project-contracts-with-multiple-funding-sources"></a>Funts-iturri ugari dituzten proiektu-kontratuen elementuen baldintzak

_**Honi aplikatzen zaio:** Izakinen edo ekoizpenean oinarritutako egoeretarako Project Operations_

Proiektuetan oinarritutako kontratu-akordio batzuek finantzaketa-iturri ugari eska ditzakete. Artikulu honetan, nahi diren finantzaketa-iturriak nola aukeratu eta konfiguratu azaltzen da, proiektu edo proiektu-kontratu baterako hainbat iturri behar direnean.

## <a name="terminology"></a>Terminologia

- **Finantzaketa-iturria** : proiektuaren kontratua finantzatzen duen erakundea. Erakunde hau barne-antolaketa edo kanpo-fakturako kontu bat izan daiteke (bezeroa edo diru-laguntza).
- **Proiektuaren** bezeroa: proiektuaren lana zein erakunderi ematen zaion.
- **Faktura-kontua** : proiektuaren lana ordaintzen duen kanpoko erakundea.

## <a name="example"></a>Adibidez

Contosok ekipoak berritzeko kontratua irabazi du bere bezeroetako birekin: Adatum US eta Adatum Corporate. Kontratuak hardwarea eta instalazio-zerbitzuak barne hartzen ditu, eta Adatum US (proiektuaren bezeroa) izango da. Hardwarea Adatum Corporate (1 faktura-kontua) erakundeak finantzatuko du, eta instalazio-lana Adatum US (2. faktura-kontua) erakundeak finantzatuko du.

## <a name="set-up-invoice-account-defaulting-rules-for-item-requirements"></a>Faktura-kontuaren aurrez zehaztutako arauak konfiguratzea artikuluen betekizunetarako

### <a name="prerequisites"></a>Aurrebaldintzak

- Microsoft Dynamics 365 Finance and Operations **10.0.27 bertsioa edo ondorengoa** beharrezkoa da hainbat faktura-kontu dituzten artikuluen baldintzak erabiltzeko.
- Sistemaren administratzaileak hainbat finantzaketa-jatorri duten elementuen betekizunak ahalbidetu behar ditu **, ekoizpenean** edo proiektu-eragiketetan **oinarritutako** agertokietarako.

### <a name="set-up-the-invoice-account-defaulting-rules"></a>Fakturen kontua ez betetzearen arauak konfiguratzea

Faktura-konturako aurrez zehaztutako arauak konfiguratzeko, jarraitu urrats horiek.

1. Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Proiektuen kudeaketa eta kontabilitate parametroak**.
1. Betile **Orokorrean**, **Salmenta-eskaerak eta artikuluen baldintzak** atalean, hainbat finantzaketa-iturri dituzten proiektuak baimentzeko **aukera** ezartzen **du**.
1. Aurrez zehaztutako **bezeroaren** arloan, zehaztu nondik datorren aldez aurretik proiektua entregatzeko bezeroa, elementu-betekizunean:

    - **Finantzaketa-iturritik** : aurrez zehaztutako proiektua entregatzeko bezeroa finantzaketa-iturritik dator. Finantzaketa-iturri bat baino gehiago proiektuaren kontratuarekin lotzen badira, zerrendako lehen finantzaketa-iturria erabiliko da.
    - **Proiektutik**: aurrez zehaztutako proiektuak entregatzeko bezeroa proiektuko erregistro-kontuan **hautatutako** bezerotik dator.

1. Aukeran: Proiektuaren erregistroetan aurrez zehaztutako faktura-kontua ezarri edo aldatzea:

    1. Proiektu guztien kudeaketara **eta** \> **kontabilitatera** \> **joan eta proiektuaren erregistroaren xehetasunak ireki.**
    2. **Fitxa orokorrean**, ezarri edo eguneratu eremua **aurrez zehaztutako faktura-kontua**. Zehazten duen kontua aurrez zehaztutako faktura-kontu gisa erabiliko da proiekturako sortzen diren elementuen baldintza berrietarako. Eremua zuri uzten badu, proiektuaren kontratuaren lehen finantzaketa-iturriaren faktura-kontua aurrez zehaztuta erabiliko da. Hala ere, erabiltzaileek kontua aldatu ahal izango dute erregistroa gordetzen dutenean.

### <a name="select-the-invoice-account-to-use-when-you-create-an-item-requirement"></a>Artikulu-betekizun bat sortzean erabili nahi duzun faktura-kontua hautatu

Artikulu-betekizun bat sortzean erabiliko den faktura-kontua aukeratzeko, jarraitu urrats horiek.

1. Proiektu guztiak kudeatu eta **kontabilitatera** \> **·** \> **joan eta proiektuaren erregistroa hautatu.**
1. Betilean **·**, elementuaren **baldintzak** aukeratu.
1. Elementu-betekizunen erregistro berri bat sortzen du.

    - Aurrez zehaztuta, **erregistroaren faktura-kontua** proiekturako ezarritako faktura-kontuan ezartzen da. Eremuaren **balioa** alda dezakezu eta, ondoren, erregistroa gorde. Behin erregistroa gordeta, ezin izango du faktura-kontuaren **balioa** eguneratu. Artikulu-betekizunerako faktura-kontuaren **balioa** eguneratu behar baduzu, ezabatu lehendik dagoen artikuluaren betekizuna, eta, ondoren, beste bat sortzen duzu, nahi den balioa duena.
    - Aurrez zehaztuta, elementuaren betekizunerako Bezeroaren eremua **proiektuen administrazio- eta kontabilitate-parametroetan** ezartzen **den bezero** aurrez zehaztuaren balioaren **arabera ezartzen** da.

    Artikuluen betekizunen erregistroa gordetzen denean, sistemak artikuluen betekizunak saltzeko eskaera-erregistroarekin **lotzen** du. Salmenta irekien eskaera-buru batek ere ez badu aukeratutako faktura-kontua, sistemak bat sortuko du eta artikuluko betekizunen lerroa harekin lotuko du.

> [!NOTE]
> Artikuluaren baldintzak erregistroan ezartzen den faktura-kontura erabat fakturatzen dira beti. Gaur egun sistemak ez du artikuluen baldintzak dituzten funtsak esleitzeko araurik onartzen, eta ez du argitalpena zatituko funtsak esleitzeko arauen konfigurazioaren arabera.

### <a name="create-an-item-requirement-from-an-item-forecast-record"></a>Elementuen aurreikuspen-erregistro batetik abiatuta, elementu-betekizun bat sortzea

Elementuen aurreikuspen-erregistro batetik abiatuta elementu-betekizun bat sortzeko, jarraitu urrats horiek.

1. Proiektu guztiak kudeatu eta **kontabilitatera** \> **·** \> **joan eta proiektuaren erregistroa hautatu.**
1. Betilean **·**, elementuen **aurreikuspenak aukeratu**.
1. Sortu elementuen iragarpen-erregistro berri bat.
1. Aukerakoa: On **Proiektua** fitxan, **Finantziazio iturria** eremuan, hautatu nahi duzun faktura-kontua.
1. Hautatu **Sortu elementuaren eskakizuna**, eta berretsi jasotzen duzun mezua.

    > [!NOTE]
    > Sistemak kopiatzen du **Finantziazio iturria** elementuaren aurreikuspeneko erregistrotik sortu berri den elementuaren eskakizunen erregistrora.

### <a name="default-invoice-account-when-the-system-automatically-creates-an-item-requirement-from-a-purchase-order-line"></a>Faktura-kontu lehenetsia sistemak automatikoki erosketa-eskaeraren lerro batetik elementu-eskakizun bat sortzen duenean

bada **Sortu elementuaren eskakizuna** aukeran ezarrita dago **Bai** gainean **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdean, sistemak automatikoki elementu-eskakizun bat sortzen du proiektuko erosketa-eskaeraren lerro berri bat gordetzen denean. Lehenespenez, **Faktura kontua** eta **Elementuaren eskakizuna** eremuak ren balioarekin ezartzen dira **Faktura-kontu lehenetsia** proiektuaren erregistroko eremua. Sistemak ez du onartzen mota honetako erregistroetarako faktura-kontua eguneratzea edo aldatzea.
