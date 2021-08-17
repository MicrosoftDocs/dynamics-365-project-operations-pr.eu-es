---
title: Konfiguratu gastuen kudeaketa
description: Artikulu honek Gastuen kudeaketa konfiguratu aurretik plangintza prozesuan zehar hartu behar dituzun gogoetak eta erabakiak deskribatzen ditu Microsoft Dynamics 365 Finance-n.
author: KimANelson
ms.date: 08/29/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: GlobalCategory, ProjCategory, TrvLocations, TrvParameters, TrvPaymethod, TrvPerDiems
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 23001
ms.assetid: aa3fd14d-7e94-4603-985f-ca26d6f860ea
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: eca4362b0ff5d37b131e1d96e311aa48ac20397618314936944ba66e458dbdc2
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "7007446"
---
# <a name="configure-expense-management"></a>Konfiguratu gastuen kudeaketa

Gai honek Gastuen kudeaketa konfiguratu aurretik plangintza prozesuan zehar hartu behar dituzun gogoetak eta erabakiak deskribatzen ditu. Gastuen kudeaketan, ordainketa metodoei, bidaia eskaerei, gastuen txostenei, gidalerroei eta abarri buruzko informazioa gorde dezakezu.

Gastuak kudeatzeko konfigurazioa planifikatzerakoan hartzen dituzun erabaki asko zure erakundearen hierarkian eta finantza egituran oinarritzen direnez, arlo horietako plangintza dokumentuak kontsultatu behar dituzu.

## <a name="intercompany-expenses"></a>Enpresen arteko gastuak

Enpresen arteko gastuak gaitzen dituzunean, pertsona juridikoei eta langileei beste pertsona juridiko baten izenean gastuak egitea baimentzen diezu eta ordainketa zure erakundeko enpleguko pertsona juridikoari kobratzen diozu. Adibidez, A entitate juridikoko langile batek B entitate juridikorako proiektu bat burutzen du eta proiektuak bidaiari lotutako gastuak ditu. Enpresen arteko gastuak gaituta badaude, langileak gastu txostena aurkeztu ahal izango du, gastua B entitate juridikoari bidaliko diona, eta gastua A. entitate juridikoak ordaindu beharko du. Zure erakundeak pertsona juridiko anitz ez baditu, ez duzu Enpresen arteko gastuak gaitu behar dituzte.

**Erabakia:** Enpresen arteko gastuak gaitu nahi dituzu?

## <a name="financial-management"></a>Finantza-kudeaketa

Gastuen kudeaketa oso integratuta dago zure erakundearen finantza kudeaketarekin. Gastuak kudeatzeko konfigurazio asko zure erakundearen ekonomiari buruz hartu dituzun erabakietan oinarrituko dira. Ondorengo ataletan plangintza eta erabakiak behar dituzten hainbat arlo deskribatzen dira, zure erakundearen finantza erabakietan eta zure zuzendaritza taldearen orientazioetan oinarrituta.

### <a name="per-diems"></a>Eguneko dietak

Zure erakundeak eskaintzen dituen dietak langileak zehaztu behar dituzu. Dietak normalean otorduak, ostatua eta bestelako gastuak bezalako gastuak estaltzeko erabiltzen direnez, zure erakundeak eskaintzen dituen dieten hobarien arauak sor ditzakezu. eguneko tasak urteko garaian, bidaiaren kokapenean edo bietan oinarrituta egon daitezke. Eguneko araua definitzen duzunean, eguneko tasaren ehuneko bat gordeko dela zehaztu dezakezu langileak osagarriak diren otorduak edo zerbitzuak jasotzen baditu. Halaber, eguneko tasen mailak ere defini ditzakezu langilearen bidaiari aplikatu ahal izateko gutxieneko eta gehieneko ordu kopurua ere ezar dezakezu.

**Erabakiak:**

- Per diem arau lehenetsiak lehen eta azken egunetarako:

    - Zein da langile batek egun baterako eska dezakeen eta eguneko dietak jaso ditzakeen gutxieneko ordu kopurua?
    - Lehen eguneko eta azken eguneko otorduetarako eskaintzen den kopurua murriztu al da? Murrizketarik badago, zein da murrizketaren ehunekoa?
    - Lehen eguneko eta azken eguneko hoteletarako eskaintzen den kopurua murriztu al da? Murrizketarik badago, zein da murrizketaren ehunekoa?
    - Lehen eguneko eta azken bestelako gastuetarako eskaintzen den kopurua murriztu al da? Murrizketarik badago, zein da murrizketaren ehunekoa?

- Eguneko dietaren arau lehenetsiak:

    - Ba al dago ehuneko dietako hobaria otordu bakoitzeko, adibidez, otordua osagarria bada? Murrizketarik badago, zein da otordu bakoitzaren murrizketaren ehunekoa?
    - Otorduen murrizketa eguneko, bidaia bakoitzeko edo eguneko otordu kopuruaren arabera kalkulatzen da?
    - Eguneko zenbatekoak modu arruntean biribildu edo biribildu behar al dira?
    - Dietak 24 orduko epean edo egun natural batean kalkulatzen dira?

- Kokapenean oinarritutako eguneko arauak:

    - Eguneko tasak aldatu egiten dira kokapenaren arabera? Zer kokapen sartzen dira?
    - Eguneko tasak kokapenaren arabera aldatzen badira, kokapen bakoitzerako, zein ehuneko kopuru ematen da honako gastu mota hauetarako:

        - Otorduak
        - Hotela
        - Bestelako gastuak

### <a name="expense-management-journals-and-accounts"></a>Gastuak kudeatzeko aldizkariak eta kontuak

Gastuen kudeaketak aldizkari eta kontu bat baino gehiago erabiltzea eskatzen du. Adibidez, erabaki behar duzu ea kontu bera erabiltzen den kutxako aurrerakinetan eta kreditu txartelen auzietan.

**Erabakiak:**

- Zein liburu aldizkarietara bidaltzen dira onartutako gastuen txostenak?
- Zein kontu erabiltzen da dirua aurreratzeko?
- Diru aurrerakinak berehala bidali behar al dira?

### <a name="payment-methods"></a>Ordainketa-metodoak

Langileei zure negozioaren izenean gastuak egitea baimentzen diezunean, langileek erabil ditzaketen ordainketa moduak definitu behar dituzu. Adibidez, langileei dirua edo korporazioko kreditu txartela erabiltzeko baimena eman diezaiekezu. Baliteke langileei kreditu txartel pertsonalak erabiltzea baimentzea eta, ondoren, langileak itzultzea. Onartzen dituzun ordainketa modu bakoitzerako erabaki hauek hartu behar dituzu.

**Erabakiak:**

- Zein ordainketa modu onartzen dira?
- Noren jabe da ordainketa metodoaren gastuak?
- Ba al dago offset kontu mota bat? Offset kontu mota badago, zer da?
- Desplazamendu-kontu bat badago, zein da kontua?
- Ordainketa metodoa kreditu txartela bada, ordainketa metodoa inportatutako transakzioekin bakarrik erabili behar al da?

### <a name="expense-categories-and-shared-categories"></a>Gastu kategoriak eta kategoria partekatuak

Langileek gastuen txosten bat sortzen dutenean, erregistratzen duten gastu bakoitza gastu-kategoria batekin lotu behar da. Gastuen kategoriak zure erakundeko pertsona juridikoetan parteka daitezkeen kategoria partekatuetatik eratortzen dira. Kategoria hauek Proiektuen kudeaketan eta kontabilitatean ere parteka daitezke, zure erakundea definitzeko moduaren arabera. Zure erakundearen definizioan eta ezarpen taldearen gidalerroetan oinarrituta, Gastuen kudeaketan erabiltzen diren kategoriak Gastuen kudeaketan soilik erabiliko diren edo beste arlo batzuetan partekatu behar diren zehaztu behar duzu Proiektu-kudeaketaren eta kontabilitatearen eta Gastuen kudeaketaren artean. Kontuan izan kategoria horiek Proiektuen edo gastuen eta ekoizpenaren artean parteka daitezkeela, baina ez gastuen eta ekoizpenaren artean. Gastu kategoria bakoitzerako erabaki hauek hartu behar dituzu.

**Erabakiak:**

- Zer da gastu-kategoria? Adibide gisa, hegaldien, hotelaren edo kilometrajearen kategoriak daude.
- Gastuen kategoria Proiektuen kudeaketan eta kontabilitatean ere erabil al daiteke?
- Zer da gastu mota?
- Zein da gastu kategoriako ordainketa modu lehenetsia?
- Gastu kategoriako gastuak banatu behar al dira?
- Zein da gastu-kategoriako kontu lehenetsi nagusia?
- Zein da gastuen kategorian lehenetsitako salmenten gaineko zerga taldea?
- Ordainketa modu osagarriak onartzen al dira gastuen kategorian? Ordainketa modu osagarriak onartzen badira, zer dira?
- Ba al dago azpikategoririk gastu kategoria honetan? Azpikategoriak badaude, erabaki hauek ere hartu beharko dituzu:

    - Zerga berreskuratzetik kanpo dago azpikategorietako bat?
    - Zein da azpikategorien salmenten gaineko zergaren taldea?

Gastuen kategoria Proiektuen kudeaketan eta kontabilitatean ere erabiltzen bada, erantzun gainerako galderei. Bestela, joan hurrengo atalera.

- Zein kostu kontu erabiliko dira ondorengo gastuetarako?

    - Kostua
    - Nominen esleipena
    - WIP - kostuaren balioa
    - Kostua-elementua
    - WIP-kostuaren balioa-elementua
    - Metatutako galera
    - WIP-metatutako galera

- Zein gastu kontu erabiliko dira ondorengorako?

    - Fakturatutako diru-sarrerak
    - Metatutako diru-sarrerak-salmenten balioa
    - WIP-salmenten balioa
    - Metatutako diru-sarrerak-produkzioa
    - WIP-ekoizpena
    - Metatutako diru-sarrerak-errentagarritasuna
    - WIP-irabaziak
    - Metatutako diru-sarrera-harpidetza
    - WIP-harpidetza

### <a name="taxes"></a>Zergak

Gastuekin lotutako zergetarako, zehaztu behar duzu zer sartzen den edo gaituta dagoen gastuen txostenetan.

**Erabakiak:**

- Salmenten gaineko zerga sartuta al dago gastuen zenbatekoetan?
- Zerga berreskuratzea gaitu behar al da gastuetan?

    > [!NOTE]
    > Liburu nagusia kontutan hartuta, AEBetako salmenten gaineko zerga aplikatzea eta zerga arauak erabiltzea erabaki baduzu, ezin duzu gastuen gaineko zerga berreskuratzea gaitu. (AEBetako salmenten gaineko zerga aplikatzeko eta zergen arauak erabiltzeko, ezarri **Salmenten gaineko zergen gaineko zergen arauak aplikatzea** aukera **Bai**.)

## <a name="policies"></a>Gidalerroak

Gastuen berri emateko gidalerroak sortuz, zure erakundeari denbora eta dirua aurrezten lagun diezaiokezu langileek bere izenean gastuak sortzen dituztenean. Politikek langileek aurrekontuan jarraituko dutela bermatzen dute, beharrezko informazio guztia eskaintzen dute eta dirua eskatzen duten moduan soilik gastatzen dute. Honako erabaki hauek hartu behar dituzu sortzen dituzun gastuen txosteneko politika bakoitzerako eta gastuen txostenak onartzeko gidalerro bakoitzerako.

**Erabakiak:**

- Nola du izena politikak?
- Zertarako gastu politika?
- Aurretik enpresen arteko gastuak gaitzea erabaki baduzu, zure erakundeko zein enpresari aplikatuko zaie politika hau?
- Noiz bihurtzen da politika eraginkorra?
- Noiz iraungitzen da politika?
- Zein da politika araua?
- Zein da politikaren arauaren irteera?


[!INCLUDE[footer-include](../includes/footer-banner.md)]