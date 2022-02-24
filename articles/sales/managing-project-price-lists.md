---
title: Kudeatu proiektuen prezio-zerrendak eskaintza batean
description: Gai honek proiektuaren prezio-zerrendaren entitateari buruzko informazioa ematen du.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 5fc8691984e22b2fa35e26b1a7d94cc56c25c26d
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/30/2020
ms.locfileid: "4177181"
---
# <a name="manage-project-price-lists-on-a-quote"></a>Kudeatu proiektuen prezio-zerrendak eskaintza batean

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations-ek Prezioen zerrenda entitatea luzatzen du Dynamics 365 Sales-en. 

## <a name="key-entities"></a>Entitate gakoak

Prezio-zerrendan lau erakunde desberdinek eskaintzen duten informazioa biltzen da:

- **Prezio-zerrenda**: entitate honek testuinguruari, monetari, daten eraginkortasunari eta denbora unitateari buruzko informazioa gordetzen du prezio-denborarako. Testuinguruak erakusten du prezio-zerrendan kostu-tasak edo salmenta-tasak adierazten diren ala ez. 
- **Moneta**: entitate honek prezioen moneta prezio-zerrendan gordetzen du. 
- **Data**: entitate hau sistemak transakzio bateko prezio lehenetsiak sartzen saiatzen denean erabiltzen da. Transakzioaren data biltzen duen data eraginkortasuna duen prezioen zerrenda hautatzen du. Transakziorako data eraginkorra den prezio-zerrenda bat baino gehiago aurkitzen badu eta horri lotutako eskaintzari, kontratuei edo antolakuntza unitateari erantsita, orduan ez da preziorik lehenetsiko. 
- **Ordua**: entitate honek prezioak adierazitako denbora-unitatea gordetzen du, hala nola eguneko- edo orduko-tasak. 

Prezio-zerrendako erakundeak erlazionatutako hiru taula ditu, prezioak gordetzen dituztenak:

  - **Funtzio-prezioa**: taula honek funtzio- eta antolaketa-unitateen balioak konbinatzeko tasa gordetzen du eta giza baliabideen funtzioan oinarritutako prezioak ezartzeko erabiltzen da.
  - **Transakzioen kategoria prezioa**: taula honek prezioak transakzioen kategorien arabera gordetzen ditu eta gastu kategoriako prezioak ezartzeko erabiltzen da.
  - **Prezio-zerrendako elementuak**: taula honek katalogoko produktuen prezioak gordetzen ditu.
 
Prezio-zerrenda tasa-txartela da. Tasa-txartela prezio-zerrendako entitatearen eta erlazionatutako errenkaden funtzio-prezioaren konbinaketa da, transakzioen kategoriako prezioa eta prezio zerrendako elementuen tauletan daude.

## <a name="resource-roles"></a>Baliabide-funtzioak

*Baliabide-funtzioa* terminoak pertsona batek proiektu batean zeregin multzo zehatz bat egiteko izan behar dituen gaitasun, konpetentzia eta ziurtagirien multzoari egiten dio erreferentzia.

Giza baliabideen denbora normalean proiektu jakin batean betetzen duen eginkizunaren arabera kotizatzen da. Giza baliabideen denborarako, baliabideen funtzioan oinarritutako kostuak eta fakturazioa onartzen ditu. Denbora **Ordua** salmenta-unitateko edozein unitatean preziatu daiteke.

**Denbora** unitate-taldea Project Operations instalatzean sortzen da. Lehenetsitako unitate bat du: **Ordua**. Ezin dituzu atributuak ezabatu, berrizendatu edo editatu **Ordua** salmenta-unitaterako edo **Ordua** unitaterako. Hala ere, beste unitate batzuk gehitu ditzakezu **Ordua** salmenta-unitatean. Ezabatzen saiatzen bazara **Denbora** salmenta-unitatea edo **Ordua** unitatea, negozioaren logikan porrotak sor ditzakezu.
 
## <a name="transaction-categories-and-expense-categories"></a>Transakzio kategoriak eta gastu kategoriak

Proiektuen aholkulariek sortzen dituzten bidaiak eta gainerako gastuak normalean bezeroari fakturatzen zaizkio. Gastu kategorien prezioak prezio-zerrendaren arabera eginda daude. Aireportua, hotela eta autoen alokairua gastu kategorien adibide dira. Gastuen prezio-zerrendaren lerro bakoitzak gastu-kategoria jakin baterako prezioak zehazten ditu. Hiru metodo hauek erabiltzen dira gastuen kategoriak preziatzeko:

- **Kostuan**: gastuaren kostua bezeroari fakturatzen zaio eta ez da gainpreziorik aplikatuko.
- **Gainprezio portzentajea**: benetako kostuaren gaineko portzentajea bezeroari fakturatzen zaio. 
- **Prezioa unitateko**: gastu-kategoriako unitate bakoitzeko fakturazio-prezioa ezartzen da. Bezeroari fakturatzen zaion zenbatekoa kontsultariak jakinarazten duen gastu unitateen arabera kalkulatzen da. Kilometrajeak prezio bakoitzeko prezioaren metodoa erabiltzen du. Adibidez, kilometro-gastuen kategoria 30 dolar (USD) eguneko edo 2 USD kilometroko izateko konfiguratu daiteke. Aholkulari batek proiektu baten kilometrajea jakinarazten duenean, fakturatu beharreko zenbatekoa aholkulariak jakinarazi duen kilometro kopuruaren arabera kalkulatzen da.
 
## <a name="project-sales-pricing-and-overrides"></a>Proiektuen salmentako prezioak eta baliogabetzeak

Proiektuen eskaintzen eta kontratuen kasuan, proiektuen prezio-zerrendak produktuen prezio-zerrenda baino beste prezio eredu bat du. Produktuen katalogoan oinarritutako eskaintzaren lerroan, prezioa zuzendu eta funtzioetara zuzendu daiteke eskaintzaren lerroan. Eskaintzaren lerro bakoitzak katalogoko elementu bat besterik ez duelako. Dena den, proiektuan oinarritutako eskaintzaren lerroan, ezin duzu prezioa zuzendu eskaintzaren lerroan eta kategorietan zuzenean. Erabili proiektuaren prezioen zerrenda bi gainidazketa eredu desberdinak onartzeko.

> [!NOTE]
> Zure proiektuaren baliabideen eta katalogoko elementuen prezio-zerrenda berezi bat izatea gomendatzen dugu, prezioak baliogabetzen dituzunean bien arteko portaera desberdintasunak direla eta.

Erakunde hauetako bakoitzak salerosketako prezioe-zerrenda bat edo gehiago izan ditzake proiektuaren prezioetarako:

- Bezeroa (kontua) 
- Abagunea 
- Eskaintza 
- Proiektu-kontratua

Prezio-zerrenda duten entitate horien elkartea proiektuaren prezio-zerrendek adierazten dute. Prezio-zerrenda bat edo gehiago bezeroak, abagunean, eskaintzak eta proiektu-kontratuaren salmentako entitateekin lotu ditzakezu.

Lehenetsitako proiektuen prezio-zerrenda ez da automatikoki sartu bezeroaren erregistroan. Hala ere, proiektuaren prezio-zerrenda eskuz erantsi dezakezu bezeroaren erregistroan. Nolanahi ere, proiektuaren prezio-zerrenda eskuz erantsi behar zenuke bezeroarekin prezioen akordio pertsonalizatua denean. 

Proiektuen prezioen zerrenda salmenta erakunde bati atxikitakoan, informazio hau balioztatzen du:

- Prezio-zerrenda testuinguru bat da **Salmentak**. 
- Monetak prezio-zerrendaren monetarekin bat dator. 

Proiektu baten kontratuan, lehentasun hurrenkera hau proiektuaren inguruko prezioen zerrendak automatikoki ezartzeko:

1. Eskaintza
2. Abagunea
3. Bezeroa 
4. Ezarpen orokorrak 

Proiektuen prezio-zerrenda lehenespenez sartzen denean, sistemak balioztatzen du moneta bezeroaren monetarekin bat datorrela eta sartu diren prezio-zerrenden lehenetsiak testuinguruan **salmentak**.

Prezio-zerrenda bat edo gehiago bezeroak, abagunean, eskaintzak eta proiektu-kontratuaren salmentako entitateekin lotu ditzakezu. Gaitasun honek iraupen luzeko proiektu kontratuetarako zehaztutako prezioak onartzen ditu, non prezio-zerrenda bat baino gehiago eska dezakezun inflazioaren ondorioz gertatzen diren prezioen eguneratzeak kontatzeko. Hala ere, bezeroa, abagunea, eskaintza edo proiektu-kontratuaren entitatearekin lotzen dituzun prezioen zerrendek data eraginkortasun bat badute, baliteke prezio lehenetsiak okerrak izatea. Hori dela eta, ziurtatu behar duzu data eraginkortasuna bata bestearen gainjartzen duten proiektuen prezio-zerrendak ez daudela entitate horiekin lotuta.

### <a name="deal-specific-price-overrides"></a>Eskaintzari buruzko prezioen baliogabetzea

Eskaintzaren berariazko berrientzat sor ditzakezu eskaintzaren edo proiektu-kontratuan lehenetsitako proiektuen prezio-zerrendetan.

Berez, proiektu-kontratuak salmenta prezio-zerrenda nagusiaren kopia bat lortzen du beti harekin lotura zuzena izan beharrean. Jokabide horrek bezeroari lanaren aitorpenerako (SOW) bezeroari egiten dizkion prezioen hitzarmenak bermatzen laguntzen du prezio-zerrenda nagusia aldatzen bada.

Hala ere, eskaintzan, prezio-zerrenda maisua erabil dezakezu. Bestela, prezioe-zerrenda nagusia kopiatu eta editatu dezakezu eskaintza horietara soilik aplikatzen den prezio-zerrenda pertsonalizatua sortzeko. Eskaintzen inguruko prezio-zerrenda berria sortzeko, **Eskaintza** orrian, hautatu **Sortu prezio pertsonalizatuak**. Eskaintzen proiektuaren berariazko prezio-zerrendara sar dezakezu eskaintzetan soilik. 

Proiektuen prezio-zerrenda pertsonalizatua sortzen duzunean, prezio-zerrendako proiektuaren osagaiak soilik kopiatzen dira. Bestela esanda, eskaintzan erantsitako proiektuaren prezio-zerrendaren kopia gisa sortu da prezio-zerrenda berria, eta prezio-zerrenda berri honek funtzio prezioak eta transakzioen kategorien prezioak soilik ditu.
  
## <a name="tracking-costs"></a>Kostuen segimendua

Project Operations-en proiektuen giza baliabideen denboraren kostuak kontrolatzen ditu. Proiektuan zehar sortzen diren beste gastu batzuen kostuak ere kontrolatzen ditu, hala nola bidaien gastuak.

Fakturen tasak bezala, giza baliabideen kostu tasak ere ezartzen dira prezio-zerrendak erabiliz. Hona hemen kostuen prezio-zerrendaren eta salmenten prezio-zerrendaren portaeraren desberdintasun nagusiak:

- Baliabide baten kostu-tasa ezin da proiektu, kontratu edo eskaintza jakin batean gainidatzi. Hala eta guztiz ere, fakturen tasak salbuetsi daitezke salerosketa bakoitzaren arabera, tratuaren izaeraren araberako aldaketak egiten badira. 

- Hurrengo eskaera kostuen prezio-zerrenda ebazteko erabiltzen da:

    1. Unitate antolatzaileari atxikitako kostuen prezio-zerrenda.
    2. Project Operations-eko parametroei atxikitako kostuen prezio-zerrenda. Parametroetara kostuen prezio-zerrendak erantsi daitezkeenez, moneta bat egiten du proiektuaren, kontratuaren edo eskaintzaren unitate antolatzailearen kontratuaren moneta eta kostuen prezio-zerrendaren monetaren artean.
    3. Gastuei dagokienez, kostu prezioen eta gainprezioaren gaineko prezioen metodoak ez dira kostuen prezio-zerrendetan aplikatzen. Nahiz eta prezio metodo horiek kostu prezio-zerrendako lerroetan erabili, transakzioen kategorien kostuak konfiguratzeko, sistemak ez ditu jaramonik egiten eta ez da kostu prezio lehenetsirik sartuko.
