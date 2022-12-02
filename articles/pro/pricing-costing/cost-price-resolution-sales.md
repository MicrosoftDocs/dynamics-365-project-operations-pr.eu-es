---
title: Erabaki proiektu-aurreikuspenen eta benetako datuen kostuaren tasak
description: Artikulu honek proiektuaren kalkulu eta benetako datuetan oinarritutako kostu-tasak zehazteari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 09/01/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: c2295174df1ce766c6d1304f4e9c55d32d5c4775
ms.sourcegitcommit: 60a34a00e2237b377c6f777612cebcd6380b05e1
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/13/2022
ms.locfileid: "9475215"
---
# <a name="determine-cost-rates-for-project-estimates-and-actuals"></a>Erabaki proiektu-aurreikuspenen eta benetako datuen kostuaren tasak

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Kostuaren tasak kalkuluetan eta benetako datuetan zehazteko Microsoft Dynamics 365 Project Operations-en, sistemak sarrerako kalkuluaren edo benetako datuen testuinguruaren data eta moneta erabiltzen ditu kostuen prezioen zerrenda konpontzeko. Benetako testuinguruan zehazki, sistemak erabiltzen du **Transakzio data** eremua zein prezio-zerrenda aplikagarria den zehazteko. Sarrerako estimazioaren edo benetakoaren **Transakzio data** balioa prezio-zerrendako **Hasiera eraginkorra (Ordu-eremuaren independentea)** eta **Amaiera eraginkorra (Ordu-eremuaren independentea)** balioarekin alderatzen da. Kostuen prezioen zerrenda zehaztu ondoren, sistemak kostuen tasa zehazten du. 

## <a name="determining-cost-rates-in-estimate-and-actual-contexts-for-time"></a>Denboraren benetako kostuen tasak zehaztea eta estimazioen eta benetako datuen testuinguruetan

**Denbora** elementuaren testuinguru estimatuak aipatzen du:

- **Denboraren** eskaintzaren lerroen xehetasunak.
- **Denboraren** kontratu-lerroen xehetasunak.
- Proiektuan baliabideak esleitzea.

**Denbora** elementuaren benetako datuen testuingurua aipatzen du:

- Sarrera eta Zuzenketa egunkari-lerroak **Denbora** elementurako.
- Denbora-sarrera bat bidaltzean sortzen diren egunkari-lerroak.

Kostuen prezio zerrenda zehaztu ondoren, sistemak urrats hauek betetzen ditu faktura tasa lehenetsia sartzeko.

1. Sistemak **funtzioa** eta **baliabideen unitatea** eremuak erabiltzen ditu **denbora** elementuaren testuinguru estimatuan edo benetako datuetan prezio-zerrendako funtzioen prezio-lerroetan. Bat-etortze honen arabera, lan kostuaren prezio estandarreko neurriak erabiltzen ari zarela suposatzen da. Bat etortzeko sistemaren eremuak konfiguratu badituzu edo ez horren ordez **Rola** eta **Baliabideen unitatea**, orduan hori da bat datorren rolaren prezio lerroa berreskuratzeko erabiliko den konbinazioa.
1. Sistemak kostuaren tasa duen rola prezio lerro bat aurkitzen badu **Rola** eta **Baliabideen unitatea** konbinazioa, kostuaren tasa lehenetsia da.
1. Sistema ezin bada **Rola**, **Baliabideen enpresa** eta **Baliabideen unitatea** eremuko balioak, ondoren, rolen prezioen lerroak berreskuratzen ditu bat datozen rolekin baina balio baliogabeak **Funtzioa**. Sistemak bat datorren rolaren prezioen erregistroa aurkitu ondoren, kostu-tasa lehenetsiko du erregistro horretatik.

> [!NOTE]
> Lehenespen desberdina konfiguratu baduzu **Rola** eta **Baliabideen unitatea** eremuak, edo lehentasun handiagoa duten beste dimentsio batzuk badituzu, aurreko portaera arabera aldatuko da. Sistemak lehentasun-ordenaren arabera prezio-dimentsio-balio bakoitzarekin bat datozen balioak dituzten rol-prezioaren erregistroak berreskuratzen ditu. Dimentsio horietarako balio nuluak dituzten errenkadak azkenak dira.

## <a name="determining-cost-rates-on-actual-and-estimate-lines-for-expense"></a>Benetako kostuen tasak zehaztea eta Gastuaren kalkulatutako lerroak

**Gastua** elementuaren testuinguru estimatuak aipatzen du:

- **Gastua** eskaintzaren lerroen xehetasunak.
- **Gastua** kontratu-lerroen xehetasunak.
- Proiektuaren gastuen aurreikuspenak.

**Gastua** elementuaren benetako testuingurua aipatzen du:

- Sarrera eta Zuzenketa egunkari-lerroak **Gastua** elementurako.
- Gastu-sarrera bat bidaltzean sortzen diren egunkari-lerroak.

Kostuen prezio zerrenda zehaztu ondoren, sistemak urrats hauek betetzen ditu faktura tasa lehenetsia sartzeko.

1. Sistemak **Kategoria** eta **Unitatea** eremuen konbinazioa erabiltzen du **Gastuaren** testuinguru estimatua edo benetakoa kategoriaren prezio-lerroekin bat datorren prezio-zerrendan.
1. Sistemak kostu tasa duen kategoriako prezio lerro bat aurkitzen badu **Kategoria** eta **Unitatea** konbinazioa, kostu tasa kostu tasa lehenetsi gisa erabiltzen da.
1. Sistema ezin bada **Kategoria** eta **Unitatea** balioak, balioa **0** (zero) gisa ezartzen da lehenespenez.
1. Estimazio testuinguruan, sistema ez badu aurkitzen bat datorren kategoria prezio lerro bat, baina prezioen metodoa ez bada **Unitateko prezioa**, kostuaren tasa **0** (zero) gisa ezartzen da lehenespenez.

## <a name="determining-cost-rates-on-actual-and-estimate-lines-for-material"></a>Materialen kostu tasak zehaztea eta materialaren estimazio lerroak

**Materiala** elementuaren testuinguru estimatuak aipatzen du:

- **Materiala** eskaintzaren lerroen xehetasunak.
- **Materiala** kontratu-lerroen xehetasunak.
- Materialaren aurreikuspenak proiektuan.

**Materiala** elementuaren benetako testuingurua aipatzen du:

- Sarrera eta Zuzenketa egunkari-lerroak **Materiala** elementurako.
- Material-erabileraren erregistro bat bidaltzean sortzen diren egunkari-lerroak.

Kostuen prezio zerrenda zehaztu ondoren, sistemak urrats hauek betetzen ditu faktura tasa lehenetsia sartzeko.

1. Sistemak **Produktua** eta **Unitatea** eremuen konbinazioa erabiltzen du **Materialaren** testuinguru estimatua edo benetakoa prezio-lerroko elementuekin bat datorren prezio-zerrendan.
1. Sistemak kostu tasa duen prezio-zerrenden elementuko lerro bat aurkitzen badu **Produktua** eta **Unitatea** konbinazioa, kostu tasa kostu tasa lehenetsi gisa erabiltzen da.
1. Sistema ezin bada **Produktua** eta **Unitatea** balioak, unitateko kostua **0** (zero) da lehenetsita.
1. Estimazio edo benetako testuinguruan, sistema ez badu aurkitzen bat datorren prezio-zerrendako elementuaren lerro bat, baina prezioen metodoa ez bada **Monetaren kopurua**, unitate-kostua **0** (zero) gisa ezartzen da lehenespenez. Portaera hau Project Operations-ek soilik onartzen duelako gertatzen da **Monetaren zenbatekoa** proiektu batean erabiltzen diren materialen prezioen metodoa.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
