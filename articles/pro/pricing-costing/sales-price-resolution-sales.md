---
title: Erabaki proiektu-aurreikuspenen eta benetako datuen salmenta-prezioak
description: Artikulu honek proiektuaren estimazioen eta benetakoen salmenta-prezioak nola zehazten diren buruzko informazioa eskaintzen du.
author: rumant
ms.date: 09/01/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 1288a571d50604ee400db9c16822719d0649628b
ms.sourcegitcommit: 60a34a00e2237b377c6f777612cebcd6380b05e1
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/13/2022
ms.locfileid: "9475169"
---
# <a name="determine-sales-prices-for-project-estimates-and-actuals"></a>Erabaki proiektu-aurreikuspenen eta benetako datuen salmenta-prezioak

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Microsoft-en estimazioetan eta egiazkoetan salmenta-prezioak zehazteko Dynamics 365 Project Operations, sistemak data eta moneta erabiltzen ditu sarrerako estimazioan edo benetako testuinguruan salmenta prezioen zerrenda zehazteko. Benetako testuinguruan zehazki, sistemak erabiltzen du **Transakzio data** eremua zein prezio-zerrenda aplikagarria den zehazteko. The **Transakzio data** Sarrerako estimazioaren edo benetakoaren balioa rekin alderatzen da **Hasiera eraginkorra (Ordu-eremuaren independentea)** eta **Amaiera eraginkorra (Ordu-eremuaren independentea)** prezioen zerrendako balioak. Salmenten prezioen zerrenda zehaztu ondoren, sistemak salmenta edo faktura-tasa zehazten du.

## <a name="determining-sales-rates-on-actual-and-estimate-lines-for-time"></a>Denborarako benetako eta zenbatespen-lerroen salmenta-tasak zehaztea

Estimatu testuingurua **Denbora** aipatzen du:

- Aipatu lerroaren xehetasunak **Denbora**.
- Kontratuaren lerroaren xehetasunak **Denbora**.
- Proiektu bateko baliabideak esleitzea.

Benetako testuingurua **Denbora** aipatzen du:

- Sarrera eta Zuzenketa aldizkarirako lerroak **Denbora**.
- Denbora-sarrera bat bidaltzean sortzen diren aldizkari-lerroak.
- Faktura-lerroaren xehetasunak **Denbora**. 

Salmentetarako prezioen zerrenda zehaztu ondoren, sistemak hurrengo urratsak betetzen ditu faktura-tasa lehenetsia sartzeko.

1. Sistemaren konbinazioarekin bat dator **Rola** eta **Baliabideen Unitatea** estimazioko edo benetako testuinguruko eremuak **Denbora** prezioen zerrendako rol-prezio-lerroen aurka. Bat-etortze honek suposatzen du fakturazio-tasetarako kutxaz kanpoko prezio-dimentsioak erabiltzen ari zarela. Prezioak konfiguratu badituzu, hauez gain edo beste eremu batzuetan oinarrituta egon dadin **Rola** eta **Baliabideen Unitatea**, eremuen konbinazio hori bat datorren rolaren prezio-lerroa berreskuratzeko erabiltzen da.
1. Sistemak faktura-tasa duen rol-prezio-lerro bat aurkitzen badu **Rola** eta **Baliabideen Unitatea** konbinazioa, faktura-tasa hori faktura-tasa lehenetsi gisa erabiltzen da.
1. Sistemak ezin badu bat etorri **Rola** eta **Baliabideen Unitatea** balioak, balioak bat datozen rol-prezio lerroak berreskuratzen ditu **Rola** eremua baina balio nuluak **Baliabideen Unitatea** eremua. Sistemak bat datorren rolaren prezio-erregistroa aurkitu ondoren, erregistro horretako faktura-tasa erabiliko da faktura-tasa lehenetsi gisa. Bat-etortze honek kutxaz kanpoko konfigurazioa suposatzen du lehentasun erlatiborako **Rola** aurka **Baliabideen Unitatea** salmenta prezioen dimentsio gisa.

> [!NOTE]
> Beste lehentasun bat konfiguratzen baduzu **Rola** eta **Baliabideen Unitatea** eremuak, edo lehentasun handiagoa duten beste dimentsio batzuk badituzu, aurreko portaera horren arabera aldatuko da. Sistemak lehentasun-ordenaren arabera prezio-dimentsio-balio bakoitzarekin bat datozen balioak dituzten rol-prezioaren erregistroak berreskuratzen ditu. Dimentsio horietarako balio nuluak dituzten errenkadak azkenak dira.

## <a name="determining-sales-rates-on-actual-and-estimate-lines-for-expense"></a>Gastuen benetako eta zenbatespen-lerroen salmenta-tasak zehaztea

Estimatu testuingurua **Gastua** aipatzen du:

- Aipatu lerroaren xehetasunak **Gastua**.
- Kontratuaren lerroaren xehetasunak **Gastua**.
- Proiektu bateko gastuen kalkulu-lerroak.

Benetako testuingurua **Gastua** aipatzen du:

- Sarrera eta Zuzenketa aldizkarirako lerroak **Gastua**.
- Gastu-sarrera bat bidaltzean sortzen diren aldizkari-lerroak.
- Faktura-lerroaren xehetasunak **Gastua**. 

Salmentetarako prezioen zerrenda zehaztu ondoren, sistemak urrats hauek betetzen ditu salmenten prezio lehenetsia sartzeko.

1. Sistemaren konbinazioarekin bat dator **Kategoria** eta **Unitatea** kalkuluen lerroko eremuak **Gastua** prezioen zerrendako kategoriako prezio-lerroen aurka.
1. Sistemak salmenta-tasa duen kategoriako prezio-lerro bat aurkitzen badu **Kategoria** eta **Unitatea** konbinazioa, salmenta-tasa hori salmenta-tasa lehenetsi gisa erabiltzen da.
1. Sistemak bat datorren kategoriako prezio-lerro bat aurkitzen badu, baliteke prezioen metodoa erabil daiteke salmenta-prezio lehenetsia sartzeko. Ondorengo taulak proiektuen eragiketetako gastuen prezioen lehenetsitako portaera erakusten du.

    | Testuingurua | Prezio-metodoa | Lehenetsitako prezioa |
    | --- | --- | --- |
    | Aurreikuspena | Prezioa unitate bakoitzeko | Kategoriaren prezio-lerroan oinarrituta. |
    |        | Kostuan | 0.00 |
    |        | Markaketa kostuaren gainetik | 0.00 |
    | Unekoa" | Prezioa unitate bakoitzeko | Kategoriaren prezio-lerroan oinarrituta. |
    |        | Kostuan | Lotutako kostu errealean oinarrituta. |
    |        | Markaketa kostuaren gainetik | Markatu bat aplikatzen zaio, kategoriako prezio-lerroaren arabera, erlazionatutako kostu errealaren unitate-kostu-tasari. |

1. Sistemak ezin badu bat etorri **Kategoria** eta **Unitatea** balioak, salmenta-tasa ezarrita dago **0** (zero) lehenespenez.

## <a name="determining-sales-rates-on-actual-and-estimate-lines-for-material"></a>Materialaren benetako eta zenbatespen-lerroen salmenta-tasak zehaztea

Estimatu testuingurua **Materiala** aipatzen du:

- Aipatu lerroaren xehetasunak **Materiala**.
- Kontratuaren lerroaren xehetasunak **Materiala**.
- Proiektu baten materialaren estimazio-lerroak.

Benetako testuingurua **Materiala** aipatzen du:

- Sarrera eta Zuzenketa aldizkarirako lerroak **Materiala**.
- Materialaren erabileraren erregistroa bidaltzean sortzen diren aldizkari-lerroak.
- Faktura-lerroaren xehetasunak **Materiala**. 

Salmentetarako prezioen zerrenda zehaztu ondoren, sistemak urrats hauek betetzen ditu salmenten prezio lehenetsia sartzeko.

1. Sistemaren konbinazioarekin bat dator **Produktua** eta **Unitatea** kalkuluen lerroko eremuak **Materiala** prezioen zerrendako elementuen lerroen aurka.
1. Sistemak prezioen zerrendako elementu-lerro bat aurkitzen badu salmenta-tasa duen **Produktua** eta **Unitatea** konbinazioa, eta prezioen metodoa bada **Dibisaren zenbatekoa**, prezioen zerrendako lerroan zehazten den salmenta prezioa erabiltzen da. 
1. bada **Produktua** eta **Unitatea** eremuen balioak ez datoz bat, edo prezioen metodoa beste zerbait bada **Moneta kopurua**, salmenta-tasa ezarrita dago **0** (zero) lehenespenez. Portaera hau Project Operations-ek soilik onartzen duelako gertatzen da **Dibisaren zenbatekoa** Proiektu batean erabiltzen diren materialen prezioen metodoa.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
