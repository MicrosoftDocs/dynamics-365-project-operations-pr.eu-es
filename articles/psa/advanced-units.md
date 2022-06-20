---
title: Salmenta-unitateak eta unitateak
description: Artikulu honetan unitate eta unitate taldeei buruzko informazioa ematen da.
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: ed413cc927901308a111263dbad1a59af8fce620
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8933385"
---
# <a name="unit-groups-and-units"></a>Salmenta-unitateak eta unitateak

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Salmenta-unitate eta unitateak oinarrizko erakundeak dira Microsoft Dynamics 365-en. Unitatea neurri-unitate bakarra da, eta unitate ugari salmenta-unitatetan multzokatu daitezke. Salmenta-unitatea batzuetan aipatzen da unitate antolatu gisa Dynamics 365 erabiltzailearen interfazean (UI). 

Hona hemen unitate eta salmenta-unitateen adibide batzuk:
 
- **Salmenta-unitateak**: distantzia 
    - **Unitateak** : milia, kilometroa eta abar.
- **Salmenta-unitatea**: denbora
    - **Unitateak** : ordua, eguna, astea eta abar. 

Salmenta-unitate batean hainbat unitate konfiguratzen dituzunean, haien arteko bihurketa-faktore bat ere ezarri behar duzu salmenta-unitate lehenetsi edo lehenetsi gisa ezarri duzun lehen unitatea izendatuz. 

Adibidez, **Denbora** salmenta-unitatean, konfiguratzen baduzu **Ordua** lehen unitate gisa, sistemak izendatzen du **Ordua** unitate lehenetsi gisa. Konfiguratu duzun hurrengo unitatea bada **Eguna**, bihurketa faktorea konfiguratu behar duzu **Eguna** unitatetik **Ordua** unitatera. Gero gehitzen baduzu **Astea** hirugarren unitate gisa, bihurketa faktore bat ezarri behar duzu **Astea** unitaterako **Eguna** edo **Ordua** unitateei jarraituz. 

Hurrengo irudian, adibideen konfigurazioa erakusten da **Eguna** unitaterako, non **Kopurua** eremuak egun bateko ordu kopurua erakusten duen, eta **Astea** unitaterako, non **Kopurua** eremuak aste barruan dauzkan egun kopurua erakusten duen.

> ![Salmenta-unitatea: informazio orria.](media/advanced-2.png)

## <a name="using-units-and-unit-groups"></a>Unitateak eta salmenta-unitateak erabili

Dynamics 365 Project Service Automation-ek unitateak eta salmenta-unitateak erabiltzen ditu gastu eta denborarentzako aurreikuspenak eta sarrerak prozesatzeko. 

Gastuetarako, gastu kategoria bakoitzak unitate eta salmenta-unitate lehenetsiak ditu. Balio horiek balio lehenetsiak bezala sartzen dira gastu kategorien prezioen zerrendako sarreretan. 

Adibidez, **Distantzia** izena duen gastu kategoria bat duzu. **Distantzia** izena duen salmenta-unitatea da eta izen bereko unitate lehenetsia **Mile** da. Konfiguratu baduzu **Distantzia** unitate multzoa bi unitate izan dezan (**Milia** eta **Kilometroa**) bi prezio ezar ditzakezu **Distantzia** prezio-zerrenda bateko kategorian: miliako prezioa eta kilometroko prezioa.

| Gastu-kategoria  | Salmenta-unitatea  | Unitatea      | Prezio-metodoa  | Prezioa unitate bakoitzeko  |
|-------------------|---------------|-----------|-------------------|-------------------|
| Distantzia           | Distantzia      | Miliak      | Prezioa unitate bakoitzeko    | 10 USD            |
| Distantzia           | Distantzia      | Kilometroak | Prezioa unitate bakoitzeko    |  6 USD            |

Proiektu batean gastu bat sartzen duzunean, sistemak gastua kategoria eta unitatearen konbinazioaren bidez zehazten du. 

| Gastuen azalpena        | Gastu-kategoria  | Unitatea  | Kopurua  | Unitate-prezioa   |
|----------------------------|---------------------|-------|-----------|----------------|
| Gidatu bezeroaren kokapenera | Distantzia             | Miliak  | 10        | 10 USD         |

Denbora luzez, prezio-zerrendako goiburu bakoitzak **Lehenespeneko denbora-unitatea** eremua du. Balioa prezio-zerrendaren goiburua sortzean ezartzen da. Unitate hau erabiltzen da funtzioan oinarritutako prezio guztiak prezio-zerrenda horretan ezartzeko.

**Eskaintzako denbora** eremuko aurreikusitako lerroak denboraren edozein unitateetan adieraz daitezke. Nolanahi ere, proiektu- eta denbora- sarrerak aurreikusteko, soilik erabil dezakezu **Ordua** denbora-unitatea Denbora-sarrerako edo aurreikuspenaren lerroko unitateak ez badu funtzio horretako prezio-zerrendako unitatearekin bat egiten, sistemak prezioaren proiektuaren aurreikuspenean edo proiektuaren benetako transakzioan definitzen diren unitateetara bihurtzen du prezioa.

Hurrengo adibidean, PSAk salmenta-unitateak, unitateak eta bihurketa faktoreak nola erabiltzen dituen erakusten du.
- Unitateak

   - **Salmenta-unitatea**: denbora 
   - **Unitateak** : ordua 
    
    - **Eguna**: bihurketa-faktorea: 8 ordu       
    - **Astea**: bihurketa-faktorea: 40 ordu  
        
- Prezio-zerrenda A proiektuaren konfigurazioan:

    - **Izena** : Erresuma Batuko salmenta prezioak 2016 
    - **Lehenetsitako denbora-unitatea** : eguna 
    - **Moneta**: GBP

| Funtzioa      | Salmenta-unitatea | Unitatea | Erakunde-unitatea | Prezioa   |
|-----------|------------|------|---------------------|---------|
| Garatzailea | Time       | Day  | Badiola UK          | 800 GBP |

### <a name="time-entry"></a>Denbora-sarrera

Hurrengo taulan, PSAk hiru orduko proiekturako sortutako salmenta-aldeen transakzioa erakusten du.


| Proiektua   | Ataza    | Funtzioa      | Kopurua | Unitatea  | Unitate-prezioa | Fakturatu gabeko kopurua |
|-----------|---------|-----------|----------|-------|------------|-----------------------|
| A proiektua | Diseinua  | Garatzailea | 3        | Hour  | 100 GBP    | 300 GBP               |

## <a name="time-unit-faq"></a>Denbora-unitatearen FAQ (ohiko galderak)

### <a name="does-psa-convert-to-different-units-in-the-case-of-expenses"></a>PSA unitate desberdinetara bihurtzen al da gastuen kasuan?
Ez. Unitate bihurketak denborarako bakarrik funtzionatzen du. Gastuetarako, sistemak gastuen kategoria eta unitatea konbinatzeko preziorik ezin badu aurkitu, lehenetsitako prezio hau du: 0,00.

### <a name="why-does-psa-convert-time-units"></a>Zergatik bihurtzen ditu PSAk denbora-unitateak?
Herrialde edo eskualde batzuetan lege-baldintza dago fakturen tasak egunetan ezarri behar direla. Prezioen negoziazioa eta aurrekontuaren beherapena eskaintzaren zikloan eguneko tasak erabiliz egiten da fakturazio-funtzio bakoitzeko. Antolaketaren aurreikuspena eta denbora-sarrera orduetan egiten dira. Denbora-unitateen desberdintasun hori onartzeko, PSAk denbora-unitateak bihurtzen ditu.

### <a name="can-time-units-be-changed-on-project-estimates"></a>Denbora-unitateak alda daitezke proiektuaren aurreikuspenen arabera?
Ez. Antolaketaren aurreikuspena orduetara mugatuta dago eta ezin da aldatu.

### <a name="can-units-and-unit-groups-be-edited-deleted-and-added"></a>Unitateak eta salmenta-unitateak editatu, ezabatu eta gehitu al daitezke?
Bai. Salbuespena: **Denbora** salmenta-unitatea eta **Ordua** unitatea. Beste unitate guztiak ezabatu edo editatu daitezke eta unitate berriak gehitu daitezke. PSAn, **Denbora** unitate multzoa eta **Ordua** unitatea ezin dira ezabatu. Hala ere, itzulpenerako testu batekin eguneratu daitezke **Izena** eremurako.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
