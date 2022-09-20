---
title: Proiektuetan oinarritutako estimazioen eta errealen kostu-tasak zehaztea
description: Artikulu honek proiektuetan oinarritutako estimazioen eta egiazkoen kostu-tasak nola zehazten diren buruzko informazioa eskaintzen du.
author: rumant
ms.date: 9/12/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 822a7bd8ae87d4fd4044d8b46347bfe1b4ca13ca
ms.sourcegitcommit: 60a34a00e2237b377c6f777612cebcd6380b05e1
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/13/2022
ms.locfileid: "9475247"
---
# <a name="determine-cost-rates-for-project-based-estimates-and-actuals"></a>Proiektuetan oinarritutako estimazioen eta errealen kostu-tasak zehaztea

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Microsoft-en estimazioetan eta egiazkoetan kostu-prezioak zehazteko Dynamics 365 Project Operations, sistemak data eta moneta erabiltzen ditu sarrerako estimazioan edo benetako testuinguruan salmenta prezioen zerrenda zehazteko. Benetako testuinguruan zehazki, sistemak erabiltzen du **Transakzio data** eremua zein prezio-zerrenda aplikagarria den zehazteko. The **Transakzio data** Sarrerako estimazioaren edo benetakoaren balioa rekin alderatzen da **Hasiera eraginkorra (Ordu-eremuaren independentea)** eta **Amaiera eraginkorra (Ordu-eremuaren independentea)** prezioen zerrendako balioak. Kostuen prezioen zerrenda zehaztu ondoren, sistemak kostu-tasa zehazten du.

## <a name="determining-cost-rates-in-estimate-and-actual-contexts-for-time"></a>Kostu-tasak zehaztea denborarako zenbatespen eta benetako testuinguruetan

Estimatu testuingurua **Denbora** aipatzen du:

- Aipatu lerroaren xehetasunak **Denbora**.
- Kontratuaren lerroaren xehetasunak **Denbora**.
- Proiektu bateko baliabideak esleitzea.

Benetako testuingurua **Denbora** aipatzen du:

- Sarrera eta Zuzenketa aldizkarirako lerroak **Denbora**.
- Denbora-sarrera bat bidaltzean sortzen diren aldizkari-lerroak.

Kostu-prezioen zerrenda zehaztu ondoren, sistemak hurrengo pausoak betetzen ditu kostu-tasa lehenetsia sartzeko.

1. Sistemaren konbinazioarekin bat dator **Rola**, **Enpresa**, eta **Baliabideen Unitatea** estimazioko edo benetako testuinguruko eremuak **Denbora** prezioen zerrendako rol-prezio-lerroen aurka. Bat-etortze honek suposatzen du eskulanaren kosturako prezioen dimentsio estandarrak erabiltzen ari zarela. Sistema konfiguratu baduzu, ez diren edo harekin batera dauden eremuekin bat etortzeko **Rola**, **Enpresa** eta **Baliabideen Unitatea**, beste konbinazio bat erabiltzen da bat datorren rolaren prezio-lerroa berreskuratzeko.
1. Sistemak kostu-tasa duen rol-prezio-lerroa aurkitzen badu **Rola**, **Enpresa**, eta **Baliabideen Unitatea** konbinazioa, kostu-tasa hori kostu-tasa lehenetsi gisa erabiltzen da.
1. Sistemak ezin badu bat etorri **Rola**, **Enpresa**, eta **Baliabideen Unitatea** balioak, lehentasun txikiena duen dimentsioa kentzen du, beste bi dimentsio-balioekin bat datozen rol-prezio-lerroak bilatzen ditu eta dimentsioak pixkanaka jaisten jarraitzen du bat datorren rol-prezioaren errenkada bat aurkitu arte. Erregistro horretako kostu-tasa lehenetsitako kostu-tasa gisa erabiliko da. Sistemak ez badu bat datorren rolaren prezioaren errenkadarik aurkitzen, prezioa honela ezarriko da **0** (zero) lehenespenez.

> [!NOTE]
> Beste lehentasun bat konfiguratzen baduzu **Rola** eta **Baliabideen Unitatea** eremuak, edo lehentasun handiagoa duten beste dimentsio batzuk badituzu, aurreko portaera horren arabera aldatuko da. Sistemak lehentasun-ordenaren arabera prezio-dimentsio-balio bakoitzarekin bat datozen balioak dituzten rol-prezioaren erregistroak berreskuratzen ditu. Dimentsio horietarako balio nuluak dituzten errenkadak azkenak dira.

## <a name="determining-cost-rates-on-actual-and-estimate-lines-for-expense"></a>Gastuen benetako eta zenbatespen-lerroen kostu-tasak zehaztea

Estimatu testuingurua **Gastua** aipatzen du:

- Aipatu lerroaren xehetasunak **Gastua**.
- Kontratuaren lerroaren xehetasunak **Gastua**.
- Proiektu baten gastuen kalkuluak.

Benetako testuingurua **Gastua** aipatzen du:

- Sarrera eta Zuzenketa aldizkarirako lerroak **Gastua**.
- Gastu-sarrera bat bidaltzean sortzen diren aldizkari-lerroak.

Kostu-prezioen zerrenda zehaztu ondoren, sistemak hurrengo pausoak betetzen ditu kostu-tasa lehenetsia sartzeko.

1. Sistemaren konbinazioarekin bat dator **Kategoria** eta **Unitatea** estimazioko edo benetako testuinguruko eremuak **Gastua** prezioen zerrendako kategoriako prezio-lerroen aurka.
1. Sistemak kostu-tasa duen kategoriako prezio-lerro bat aurkitzen badu **Kategoria** eta **Unitatea** konbinazioa, kostu-tasa hori kostu-tasa lehenetsi gisa erabiltzen da.
1. Sistemak ezin badu bat etorri **Kategoria** eta **Unitatea** balioak, prezioa ezarrita dago **0** (zero) lehenespenez.
1. Estimazioaren testuinguruan, sistemak bat datorren kategoriako prezio-lerroa aurki dezake, baina prezioen metodoa beste zerbait da **Prezioa Unitateko**, kostu-tasa ezarrita dago **0** (zero) lehenespenez.

## <a name="determining-cost-rates-on-actual-and-estimate-lines-for-material"></a>Materialaren benetako eta zenbatespen-lerroen kostu-tasak zehaztea

Estimatu testuingurua **Materiala** aipatzen du:

- Aipatu lerroaren xehetasunak **Materiala**.
- Kontratuaren lerroaren xehetasunak **Materiala**.
- Proiektu baten estimazio materialak.

Benetako testuingurua **Materiala** aipatzen du:

- Sarrera eta Zuzenketa aldizkarirako lerroak **Materiala**.
- Materialaren erabileraren erregistroa bidaltzean sortzen diren aldizkari-lerroak.

Kostu-prezioen zerrenda zehaztu ondoren, sistemak hurrengo pausoak betetzen ditu kostu-tasa lehenetsia sartzeko.

1. Sistemak konbinazioa erabiltzen du **Produktua** eta **Unitatea** estimazioko edo benetako testuinguruko eremuak **Materiala** prezioen zerrendako elementuen lerroen aurka.
1. Sistemak prezio-zerrendako elementu-lerro bat aurkitzen badu kostu-tasa duen **Produktua** eta **Unitatea** konbinazioa, kostu-tasa hori kostu-tasa lehenetsi gisa erabiltzen da.
1. Sistemak ezin badu bat etorri **Produktua** eta **Unitatea** balioak, kostu unitarioa ezarrita dago **0** (zero) lehenespenez.
1. Estimazioaren edo benetako testuinguruan, sistemak bat datorren prezio-zerrendako elementu-lerroa aurki badezake, baina prezioen metodoa ez bada **Dibisaren zenbatekoa**, kostu unitarioa ezarrita dago **0** lehenetsiz. Portaera hau Project Operations-ek soilik onartzen duelako gertatzen da **Dibisaren zenbatekoa** Proiektu batean erabiltzen diren materialen prezioen metodoa.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
