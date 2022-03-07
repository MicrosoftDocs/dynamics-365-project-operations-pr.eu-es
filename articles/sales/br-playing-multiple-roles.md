---
title: Kalkulatu proiektuaren salmentak eta kostuak, erreserbatu daitekeen baliabide batek proiektu bateko eginkizun ugari betetzen dituenean
description: Gai honetan azaltzen da nola erabili prezioen dimentsioak proiektu bateko eginkizun ugari betetzen dituen baliabide baten prezioei eta kostuei buruzko estimazioak onartzeko.
author: rumant
ms.date: 11/16/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 28a67e79b03dfbc38e9786350c931838ef27891a3d26787fc0334e0572528228
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6990121"
---
# <a name="estimate-project-sales-and-costs-when-a-bookable-resource-fills-multiple-roles-on-a-project"></a>Kalkulatu proiektuaren salmentak eta kostuak, erreserbatu daitekeen baliabide batek proiektu bateko eginkizun ugari betetzen dituenean 

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako Project Operations, Lite hedapena - proformaren fakturazioari aurre egitea eta produkzioan oinarritutako eszenatokien proiektuaren eragiketak_ 

Proiektuetan oinarritutako enpresek baliabide baten beharra izaten dute proiektu batean eginkizun ugari betetzeko. Rol bakoitzaren prezioa eta kostua desberdinak izan daitezke. Horrek esan nahi du baliabide berak proiektuan izandako denborak finantza estimazio desberdina lor dezakeela eginkizun bakoitzaren fakturaren eta kostu tasen arabera. Taldeko kideen erregistroan baloreak konfiguratu ditzakezu izendatutako baliabidearen gainidatziekin, taldekideari esleitutako zeregin bakoitzean.

Hurrengo adibidean balio baten gainidazketa soilak baliabide batek kostu eta faktura tasa desberdinekin proiektu batean rol anitz izatea ahalbidetzen du.

## <a name="create-tasks"></a>Sortu zereginak
Zereginak sortzeko, zereginak gehitu behar dituzu, baita laburpeneko zereginak ere, eta ondoren zeregina esleitu behar duzu zereginen iraupena gehitu aurretik. 

### <a name="add-tasks-and-summary-tasks"></a>Gehitu zereginak eta laburpen zereginak
Zeregina gehitzeko, bete pauso hauek.

1. Joan **Proiektuak** aukerara, eta ireki atazak gehitu nahi dizkiozun proiektua.
2. Hautatu **Gehitu zeregin berria**. Izendatu zeregina eta sakatu **Sartu**.
3. Idatzi beste zeregin-izen bat eta sakatu **Sartu**. Errepikatu hau zereginen zerrenda osoa izan arte.
3. Zereginak azpian koskatzeko **Laburpena** zereginak, hautatu hiru puntu bertikalak atazaren izenaren arabera, eta hautatu **Egin azpiataza**. 

  > [!TIP]
  > Zeregin bat baino gehiago hautatzeko, hautatu zeregin bat, luze sakatu **Ktrl**, eta hautatu beste zeregin bat.
  >
  > Aukera dezakezu ere **Sustatu azpiataza** zereginak azpitik ateratzeko **Laburpena** zereginak.

### <a name="assign-tasks"></a>Esleitu zereginak

Osatu urrats hauek zereginak esleitzeko.

1. Zereginaren **Honi esleituta** zutabean, hautatu pertsonaren ikonoa.
2. Aukeratu zerrendako taldekide bat edo idatzi testua izen bat bilatzeko.

### <a name="add-task-duration-and-columns"></a>Gehitu atazaren iraupena eta zutabeak

Errazena izaten da zure proiektua iraupenarekin eraikitzen hastea. Osatu urrats hauek zereginaren iraupena gehitzeko.

1. Zereginaren **Iraupena** zutabean, idatzi zeregina betetzeko behar duen egun kopurua. Denbora unitate desberdina erabili nahi baduzu, idatzi zenbaki bat gehi **orduak**, **asteak** edo **hilabeteak** hitza.
2. Zure zeregina diamante itxurako mugarri gisa agertzea nahi baduzu **Denbora-lerroa** ikuspegian, **Iraupena** zutabean, sartu **0 egun**.
3. Sakatu **Sartu** hurrengo zereginera joateko **Iraupena** eremuan eta jarraitu iraupenak sartzen.

  > [!NOTE]
  > Ezin duzu laburpen zereginetarako iraupenik sartu.

Zutabeak gehi ditzakezu zure proiektuari xehetasun gehiago emateko. Horretarako, hautatu **Gehitu zutabea**. 

Informazio gehiago lortzeko, ikusi [Sortu proiektua](https://support.microsoft.com/en-us/office/create-a-project-a5b5e823-fb2e-45fd-be00-7d84422d9749).

## <a name="set-up-the-role-and-organization-unit-for-a-generic-project-team-member"></a>Konfiguratu eginkizuneko eta taldeko unitateko eginkizuna eta antolakuntza unitatea
Osatu urrats hauek taldekide generiko batentzako rol eta antolakuntza unitatea konfiguratzeko.

1. **Zereginak** orrian, hautatu **Zeregina** errenkada **A ataza**. 
2. **Honi esleituta** aukera, hautatu **Gehitu baliabide generikoa**. Honek irekitzen du **Taldeko kidea azkar sortzeko** orrialdea.
3. **Talde-kidearen sorrera azkarra** orrian, zehaztu zeregin hori egin dezakeen talde-kide orokorraren atributuak.
4. Hautatu funtzio eta antolaketa-unitate egokia, eta hautatu **Gorde eta itxi**. Talde-kide orokor bat sortu eta zeregin horri esleitzen zaio. 
5. Errepikatu 1-4 urratsak **B atazan**. Hala ere, **B ataza** taldeko kide generikoari eginkizuna eta antolakuntza unitate desberdinak izan behar ditu **A ataza**. 

## <a name="set-up-the-role-and-organization-unit-for-a-project-task"></a>Konfiguratu proiektu-zereginaren funtzioa eta antolakuntza-unitatea
Osatu urrats hauek zeregin batentzako rol eta antolakuntza unitatea konfiguratzeko.

1. Sortu ondoren **A ataza**, hautatu zeregina eta, ondoren, hautatu **i** ikonoa irekitzeko **Zereginaren xehetasunak** panela. 
2. **Zereginaren xehetasunak** panelean, joan behealdera eta hautatu **Ikusi xehetasunak** irekitzeko **Zereginaren xehetasunak** orrialdea.
3. **Zereginaren xehetasunak** orrialdean, **Rola** eta **Antolakuntza Unitatea**, gehitu baliabiderako zeregin hori egiteko beharrezkoak diren balioak. 

  > [!NOTE]
  > Agertoki hau Project Operations demo datuak erabiliz osatzen baduzu, hautatu **Aholkularitza arduraduna** rolerako, eta **Fabrikam US** antolakuntza unitate gisa.

4. Hautatu **B zeregina**, eta ondoren hautatu zeregina.
5. Aukeratu **i** ikonoa irekitzeko **Zereginaren xehetasunak** panela. 
6. **Zereginaren xehetasunak** panelean, joan behealdera eta hautatu **Ikusi xehetasunak** irekitzeko **Zereginaren xehetasunak** orrialdea.
7. **Zereginaren xehetasunak** orrialdean, **Rola** eta **Antolakuntza Unitatea**, gehitu baliabidearen beharrezko balioak zeregin hori egiteko. **Rola** eta **Antolakuntza Unitatea** **B atazarako** desberdinak izan behar dira **A atazakoetatik**. 

  > [!NOTE]
  > Agertoki hau Project Operations demo datuak erabiliz osatzen baduzu, hautatu **Sare-teknikaria** rolerako, eta **Fabrikam US** antolakuntza unitate gisa.

8. Gorde eta itxi **Zereginaren xehetasunak** orria. 

## <a name="team-member-and-estimates-behavior"></a>Taldekidea eta portaera kalkulatzen du 
**Taldeko kidea** saretaren eta kalkuluen portaera ulertzeko, jarraitu urrats hauek.

1. **Taldeko kidea** saretan, hautatu bi taldeko kide generikoak, eta hautatu **Sortu eskakizunak**. Baliabideen eskakizun orokorrak sortuko dira. 
2. Hautatu **Aholkularitza-arduraduna** eginbidearen talde-kidea eta, ondoren, hautatu **Erreserbatu**. Ordutegien taula baliabideen zerrendarekin irekitzen da. Aukeratu baliabide bat eta hautatu **Liburua** baliabidea baldintza horretarako erreserbatzeko.
3. Hautatu **Sare-teknikaria** eginbidearen talde-kidea eta, ondoren, hautatu **Erreserbatu**. Ordutegien taula baliabideen zerrendarekin irekitzen da. Aukeratu goikoaren baliabide berdina eta hautatu **Liburua** baliabidea baldintza horretarako erreserbatzeko.

### <a name="team-member-grid"></a>Talde-kideen sareta 

**Taldeko kidea** saretan, taldeko bi kideen erregistro generikoak ezabatu eta baliabide bakarrarekin ordezkatuko dira. Baliabide horren balio multzo bat dago, balio multzo lehenetsia dena **Rola** eta **Antolakuntza Unitatea**.

Taldekideen erregistro horren errenkada zabaltzen duzunean, zeregin desberdinak ikus ditzakezu taldeko kideen erregistroan bi zereginetarako. Zereginen errenkada bakoitzak **Funtzioa** eta **Antolaketa-unitatea** funtzioen balio zehatzak ditu. 

### <a name="estimates-grid"></a>Aurreikuspenen sareta 

**Aurrekontuak** saretan, baliabide beraren bi zereginek prezio desberdinak dituzte. **A zeregineko** baliabidearen esleipena **Aholkularitza-arduraduna** eremuaren **Funtzioa** atributuaren balioa erabiliz. **B zeregineko** baliabide beraren esleipena **Sare-teknikaria** eremuaren **Funtzioa** atributuaren balioa erabiliz.


[!INCLUDE[footer-include](../includes/footer-banner.md)]