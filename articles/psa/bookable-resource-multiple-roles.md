---
title: Kalkulatu proiektuaren salmentak eta kostuak, erreserbatu daitekeen baliabide batek proiektu bateko eginkizun ugari betetzen dituenean
description: Gai honetan prezioen dimentsioak proiektu bateko eginkizun ugari betetzen dituen baliabide baten prezioei eta kostuei buruzko estimazioak onartzeko nola erabil daitekeen azaltzen da.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 67e24156e960b9b09cf92f7f0cd77f6c74a982b8
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5145028"
---
# <a name="estimate-project-sales-and-costs-when-a-bookable-resource-fills-multiple-roles-for-a-project"></a>Kalkulatu proiektuaren salmentak eta kostuak, erreserbatu daitekeen baliabide batek proiektu bateko eginkizun ugari betetzen dituenean 

[!include [banner](../includes/psa-now-project-operations.md)]

Proiektuetan oinarritutako enpresek baliabide baten beharra izaten dute proiektu batean eginkizun ugari egiteko. Eginkizun horietako bakoitzaren prezioak eta kostuak desberdinak izan litezke; horrek esan nahi du baliabide berdinak proiektuan izandako denborak finantza-estimazio desberdina lor dezakeela eginkizun bakoitzaren fakturaren eta kostuen tasen arabera. Project Service Automation-ek izendatutako baliabiderako taldekideen erregistroan dauden balioak konfiguratzea ahalbidetzen du eta taldekideari esleitutako zeregin bakoitzean gainidatziak egiteko aukera ematen du.

Ondorengo adibidean azaltzen da nola balio horren gainidazte soilak baliabide batek proiektu batean funtzio anitz izatea kostuen eta fakturen tasa desberdinekin.

## <a name="create-tasks"></a>Sortu zereginak
Sortu 40 orduko bi proiektuetako zereginak, A zeregina eta B zeregina. Aukeratu A zeregina B zereginaren aurreko gisa.

## <a name="set-up-role-and-organization-unit-for-a-generic-project-team-member"></a>Konfiguratu proiektuko talde-kide orokor baten Funtzioa eta Antolaketa-unitatea

1. **Antolaketa** orrian, hautatu A zereginaren **Zeregina** errenkada. 
2. **Baliabideak** eremuan, hautatu **Sortu** goitibeherako zerrendan.
3. **Talde-kidearen sorrera azkarra** orrian, zehaztu zeregin hori egin dezakeen talde-kide orokorraren atributuak.
4. Hautatu funtzio eta antolaketa-unitate egokia, eta hautatu **Gorde eta itxi**. Talde-kide orokor bat sortu eta zeregin horri esleitzen zaio. 

Errepikatu B zereginaren urrats horiek eta ziurtatu B zereginean sortutako talde-kide orokorreko funtzioa eta antolaketa-unitatea eta A zereginarenak desberdinak direla. 

## <a name="set-up-role-and-organization-unit-for-a-project-task"></a>Konfiguratu proiektu-zereginaren funtzioa eta antolaketa-unitatea

1. A zeregina sortu ondoren, hautatu zeregina eta, ondoren, hautatu **Editatu zeregina**.
2. **Zereginaren xehetasunak** orrian, aurkitu **Funtzioa** eta **Antolaketa-unitatea** eremuak, gehitu zeregin hori egiteko behar den baliabide bat gehitzeko. 

  > [!NOTE]
  > Project Service Automation demo-datuak erabiliz agertoki hau osatzen ari bazara, hautatu funtzioaren **Aholkularitza-arduraduna**, eta **Fabrikam US** antolaketa-unitate gisa.

3. Hautatu B zeregina eta, ondoren, hautatu **Editatu zeregina**.
4. **Zereginaren xehetasunak** orrian, aurkitu **Funtzioa** eta **Antolaketa-unitatea** eremuak, gehitu zeregin hori egiteko behar den baliabide bat gehitzeko. Ziurtatu fitxategiko balioak **Funtzioa** eta **Antolakuntza-unitatea** eremuak desberdinak dira B ataza egiteko A ataza balioekin alderatuta. 

  > [!NOTE]
  > Project Service Automation demo-datuak erabiliz agertoki hau osatzen ari bazara, hautatu funtzioaren **Sare-teknikaria**, eta **Fabrikam US** antolaketa-unitate gisa.

5. Gorde eta itxi **Zereginaren xehetasunak** orria. 

## <a name="team-member-and-estimates-behavior"></a>Taldekidea eta portaera kalkulatzen du 

1. **Zereginaren xehetasunak** orrian, **Talde-kidea** atalean, hautatu bi talde-kide orokor eta hautatu **Sortu eskakizunak**. 
2. Hautatu **Aholkularitza-arduraduna** eginbidearen talde-kidea eta, ondoren, hautatu **Erreserbatu**. Antolaketa-panelak eskakizun horretarako baliabide bat irekitzen eta erreserbatzen du.
3. Hautatu **Sare-teknikaria** eginbidearen talde-kidea eta, ondoren, hautatu **Erreserbatu**. Antolaketa-panelak eskakizun horretako baliabide bera irekitzen eta erreserbatzen du.

### <a name="team-member-grid"></a>Talde-kideen sareta 
**Talde-kidea** saretan, ikusi talde-kideen bi erregistro orokor ezabatu egin direla eta baliabide bat ordezkatu dela. **Funtzioa** eta **Antolaketa-unitatea** eremuetako balioen multzo lehenetsia erakusten duen baliabidearen balio multzo bat dago.
Talde-kideen erregistro horren errenkada zabaltzen duzunean, bi zeregin horietako zeregin desberdinak ikus ditzakezu talde-kideen erregistroan. Zereginen errenkada bakoitzak **Funtzioa** eta **Antolaketa-unitatea** funtzioen balio zehatzak ditu. 

### <a name="estimates-grid"></a>Aurreikuspenen sareta 
**Aurreikuspenak** sarera nabigatzen duzunean, baliabide beraren bi zereginek prezio desberdinak dituztela ohartuko zara.
A zeregineko baliabidearen esleipena **Aholkularitza-arduraduna** eremuaren **Funtzioa** atributuaren balioa erabiliz. B zeregineko baliabide beraren esleipena **Sare-teknikaria** eremuaren **Funtzioa** atributuaren balioa erabiliz.



[!INCLUDE[footer-include](../includes/footer-banner.md)]