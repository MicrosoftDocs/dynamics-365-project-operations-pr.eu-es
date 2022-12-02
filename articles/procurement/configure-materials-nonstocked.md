---
title: Konfiguratu izakinik gabeko materialak eta ordaindu gabeko saltzaileen fakturak
description: Gai honetan hornitzen ez diren materialak eta zain dauden saltzaileen fakturak nola gaitu azaltzen da.
author: sigitac
ms.date: 06/22/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 6473ef3510f0d3641a2d61b6a1b1f28980993277
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8913743"
---
# <a name="configure-non-stocked-materials-and-pending-vendor-invoices"></a>Konfiguratu izakinik gabeko materialak eta ordaindu gabeko saltzaileen fakturak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

## <a name="minimum-version-requirement"></a>Bertsioaren gutxieneko eskakizuna

Biltegiratu gabeko materialak eta saltzailearen fakturak zain egotea Dynamics 365 Project Operations stockean ez dauden / baliabideetan oinarritutako eszenatokiek bertsio hauek behar dituzte:

Dynamics 365 Dataverse irtenbideak:

- Project Operations – 4.9.0.221 edo berriagoa
- Idazketa bikoitzeko aplikazioen orkestrazioaren irtenbidea - 2.2.2.23 edo berriagoa

Dynamics 365 Finance:
- 10.0.18 (10.0.793.52) edo handiagoa. Ziurtatu zure Finantza ingurunea unekoa dela eta kalitate eguneratze guztiak bertsio minimoaren baldintzak betetzeko aplikatzen direla.

## <a name="run-dual-write-maps-for-non-stocked-materials-and-vendor-invoice-integration"></a>Exekutatu idazketa bikoitzeko mapak hornitu gabeko materialetarako eta saltzailearen fakturak integratzeko

Atal honetan material ez hornituetarako eta saltzailearen fakturetarako beharrezkoak diren mapei buruzko informazioa ematen da. Egiaztatu zerrendan agertzen diren aurrebaldintza-mapak direla [Ingurune berria hornitzea](../environment/resource-provision-new-environment.md#run-project-operations-dual-write-maps) gaia zure ingurunean martxan dago.

1. Joan Lifecycle Services (LCS) atalera, joan LCS proiektura eta joan **Ingurumenaren xehetasunak** orrialdea.
2. **Common Data Service Ingurumenari buruzko informazioa** atalean, hautatu **Estekatu Aplikazioetarako CDS**. Esteka hautatu ondoren, mapen entitateen zerrendara birbideratuko zaituzte.
3. Ziurtatu mapa hauek martxan daudela. Exekutatzen ez badira, abiarazi eta ziurtatu erlazionatutako taula-mapa guztiak sartzen dituzula.

    - CDS-ek produktu desberdinak kaleratu ditu (produktuak)
    - Saltzaileak v2 (msdyn_vendors)
    - Project Operations taula materialen kalkuluen arabera (msdyn_estimatelines)
    - Project Operations integrazioa proiektuaren saltzailearen faktura esportatzeko entitatea (msdyn_projectvendorinvoices)
    - Project Operations integrazioa proiektuaren saltzailearen faktura-lerroa esportatzeko entitatea (msdyn_projectvendorinvoicelines)
    - Project Operations-en integrazioaren benetako datuak (msdynactuals). Ziurtatu maparen 1.0.0.14 bertsioa edo berriagoa exekutatzen ari zarela. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktiba dezakezu hautatuta **Taula maparen bertsioa** eta ondoren hautatutako bertsioa gorde.

Demo datu estandarrak erabiltzen ari bazara, baliteke entitateen mapa hauek gelditzea eta berrabiaraztea ere hasierako sinkronizazioarekin:
  - Ordainketa egunak CDS V2 (msdyn_paymentdays)
  - Ordainketa egutegia (msdyn_paymentschedules)
  - Ordainketa baldintzak (msdyn_paymentterms)
  - Saltzaile taldeak (msdyn_vendorgroups)
  - Unitateak (uom)

> [!NOTE]
> Saltzaile taldeen eta unitateen hasierako sinkronizazioak huts egin dezake lehendik dauden demo datu multzoan erregistro batzuetan. Hutsegiteei jaramonik egin diezaiekezu, Project Operations-ekin demo datuak erabiltzea eragotziko ez baitute.

## <a name="configure-prerequisites-in-dataverse"></a>Konfiguratu aurrebaldintzak Dataverse-n

### <a name="activate-workflow-to-create-accounts-based-on-vendor-entity"></a>Aktibatu lan-fluxua saltzailearen entitatean oinarritutako kontuak sortzeko

Dual Write Orchestration irtenbideak eskaintzen du [Saltzaileek integrazio nagusia](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/vendor-mapping). Ezaugarri honen aurrebaldintza gisa, saltzailearen datuak sortu behar dira **Kontuak** entitatea. Aktibatu txantiloien lan fluxuaren prozesua saltzaileak sortzeko **Kontuak** taula deskribatutako moduan [Saltzailearen diseinuen artean aldatu](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/vendor-switch).

### <a name="set-products-to-be-created-as-active"></a>Ezarri produktuak aktibo gisa sortzeko

Biltegiratu gabeko materialak honela konfiguratu behar dira **Kaleratutako produktuak** Finantzetan. Dual Write Orchestration irtenbideak kutxaz kanpoko zerbitzua eskaintzen du [Kaleratutako produktuen integrazioa Dataverse Produktuen katalogoa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/product-mapping). Berez, Finantzako produktuak sinkronizatuta daude Dataverse zirriborro egoeran. Produktua egoera aktiboarekin sinkronizatzeko, materiala erabiltzeko dokumentuetan edo zain dauden saltzailearen fakturetan zuzenean erabili ahal izateko, joan hona: **Sistema** > **Administrazioa** > **Sistemaren administrazioa** > **Sistemaren ezarpenak** eta **Salmentak** fitxa, ezarri **Sortu produktuak egoera aktiboan** aukera **Bai** gisa.

## <a name="configure-prerequisites-in-finance"></a>Konfiguratu aurrebaldintzak Finance-n

### <a name="enable-the-feature-key-for-pending-vendor-invoices"></a>Gaitu funtzioaren gakoa zain dauden saltzaileen fakturen kasuan

Osatu urrats hauek funtzionalitatea gaitzeko, saltzailearen faktura lerroetan proiektuaren xehetasunak gehitzeko.

1. Finantzetan, joan **Ezaugarrien kudeaketa** lan eremua.
2. Ezaugarrien zerrendan, bilatu **Gaitu Project Operations-en saltzailearen fakturak zain, baliabideetan oinarritutako / gordeta ez dauden eszenatokietarako** eginbidea eta hautatu **Gaitu**.

### <a name="define-category-groups-and-project-categories-for-items"></a>Definitu elementuen kategoria taldeak eta proiektuen kategoriak

Konfiguratu gutxienez kategoria talde bat **Elementua** transakzio mota, eta gutxienez proiektu kategoria bat talde hau erabiliz. Informazio gehiagorako, ikus [Konfiguratu proiektuaren kategoriak](../project-accounting/configure-project-categories.md#category-groups).

Berrikusi proiektuaren kostuen eta diru-sarreren profilak, eta konfiguratu liburuaren kontabilitate-elementuen transakzioetarako. Informazio gehiagorako, ikusi [Konfiguratu fakturagarriak diren proiektuen kontabilitatea](../project-accounting/configure-accounting-billable-projects.md).

### <a name="set-up-a-write-in-product"></a>Konfiguratu katalogotik kanpoko produktua

Project Operations-en, kaleratutako produktuen katalogoan konfiguratuta dauden katalogoko produktuetarako eta idazteko produktuetarako materialen kalkuluak eta erabilera erregistratu ditzakezu. Idazteko produktuak erabiltzeak askatutako produktu bakarra behar du horretarako Finantzan konfiguratuta dagoena. Bete urrats hauek idazteko produktu bat konfiguratzeko. Errepikatu urrats hauek Baliabideen / stockik gabeko eszenatokietarako Project Operations erabiltzen dituen pertsona juridiko bakoitzean.

1. Finantzetan, joan hona **Produktuaren informazioaren kudeaketa** > **Produktuak** > **Kaleratutako produktuak**, eta hautatu **Berria** gisa.
2. **Produktu mota** eremuan, hautatu **Elementua** eta **Produktuen azpimota** eremua, hautatu **Produktua** aukera.
3. Idatzi produktuaren zenbakia (WRITEIN) eta produktuaren izena (Idatzi produktua).
4. Aukeratu elementu eredu taldea. Ziurtatu hautatu duzun elementu eredu taldeak baduela **Inbentario-politika Produktu gordea** eremua ezarrita dago **Gezurra**.
5. Hautatu balioak **Elementu taldea**, **Biltegiratze dimentsio taldea** eta **Jarraipen dimentsio taldea** eremuak. Erabili **Biltegiratze dimentsioa** **Gunean** bakarrik, eta **Jarraipenaren neurriak** eremuan, hautatu **Bat ere ez**.
6. Hautatu balioak **Inbentarioaren unitatea**, **Erosketa unitatea** eta **Salmenta-unitatea** eremuetan eta gorde aldaketak.
7. **Plana** fitxan, ezarri ordena ezarpen lehenetsiak eta **Inbentarioa** fitxa, ezarri gune eta biltegi lehenetsiak.
8. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Proiektuen kudeaketa eta kontabilitate parametroak** eta ireki **Project Operations Dynamics 365 Dataverse-n**. 
9. **Materialak** fitxan, **Katalogotik kanpoko produktua** eremuan, hautatu sortu duzun produktua.
10. Dataverse ingurunean, gunearen mapan, ireki **Produktuak** entitatea eta bilatu idatzi produktuaren erregistroa. 
11. Ireki erregistroaren xehetasunak eta ezarri produktuaren egoera **Erretiratua** aukerara. Produktuaren egoera honek edonork erregistro hau ustekabean materialen estimazioetan eta erabilera dokumentuetan zuzenean erabiltzea eragozten du.

### <a name="set-up-a-procurement-integration-account"></a>Konfiguratu kontratazioen integrazio kontua

Kontratazioaren integrazio kontua konpentsazio kontu gisa erabiltzen da proiektu bati egotzitako lerroekin zain dagoen saltzailearen faktura argitaratzerakoan.

Sistemak zain dagoen saltzailearen faktura argitaratzen duenean, kontu hori proiektuaren kostuaren zenbatekoan erabiltzen da. Saltzailearen fakturen datuak urtean prozesatzen dira Dataverse-n, eta dagokion proiektu erreala sortzen da. Benetako proiektuaren informazioa Project Operations Integration aldizkarian gehitzen da. Integrazio aldizkaria argitaratzen duzunean, zenbatekoa kontratazio integrazio kontutik garbitu eta proiektuaren kostuan erregistratzen da.

1. Erosketa-integrazioaren kontua konfiguratzeko, joan **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Proiektuen kudeaketa eta kontabilitate parametroak** eta ireki **Project Operations Dynamics 365 Dataverse-n**. 
2. Aukeratu **Materialak** fitxa eta hautatu balio bat **Kontratazioen integrazio kontua** eremuan.

#### <a name="set-up-project-category-defaults-for-an-item"></a>Konfiguratu proiektu baten kategoriako elementu lehenetsiak

1. Finance-n, joan **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Proiektuen kudeaketa eta kontabilitate parametroak** eta ireki **Project Operations Dynamics 365 Dataverse-n**. 
2. **Proiektuaren kategoria lehenetsiak** fitxan, **Elementua** eremuan, hautatu balio bat. Proiektuaren kategoria hau material transakzioetarako erabiltzen da, baldin eta proiektuaren kategoria proiektuaren benetako erregistroan ezarri ez bada.
