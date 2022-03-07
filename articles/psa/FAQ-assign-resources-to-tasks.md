---
title: Esleitu baliabide bat zeregin bati
description: Gai honek proiektuaren baliabideak zereginei esleitzeari buruzko informazioa ematen du.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 9/27/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 3f96344b917f088f1d5782c5cee1d84f1aff47bc1bad7c8f6b33307d1df340fa
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6987646"
---
# <a name="assign-a-resource-to-a-task"></a>Esleitu baliabide bat zeregin bati

[!include [banner](../includes/psa-now-project-operations.md)]

Baliabide bat hiru modutan eslei daiteke Microsoft Dynamics 365 Project Service Automation-en.

## <a name="book-a-resource-as-a-team-member-and-then-assign-the-resource-to-a-task"></a>Erreserbatu baliabidea taldearen kide gisa eta esleitu baliabidea zereginari

Proiektu-taldeari baliabide bat gehi diezaiokezu eta baliabidea zereginetan eslei dezakezu proiektuaren antolaketan.

1. **Taldekidea** fitxan, gehitu taldekide berria hautatuta **Berria**. 

2. **Taldekidea sorrera bizkorra** panela irekitzen da, hautatu baliabide erreserbagarriaren izena eta funtzio bat ezarri. 

    Hautatu baliabide erreserbagarrirako ondorengo esleipen metodo bat:

    - **Gaitasun osoa** aukerarekin baliabidearen ahalmena osoa zehaztutako liburu batetik eta data.
    - **Ehunekoaren gaitasuna** aukerak baliabidearen ahalmenaren ehuneko batean erreserbatzen du baliabidea zehaztutako daten artean.
    - **Orduak berdin banatu** aukerak epe jakin batean zehaztatutako orduak erreserbatzen ditu, zehaztatutako hasiera- eta amaiera-daten artean berdin banatuz, egunen arabera.
    - **Aurreikusitako orduaren arabera** ordu jakin baterako erreserbatzen du baliabidea, egunean ordu jakin batzuk zehaztutako datetan.
    - Ez hautatu **Bat ere ez** baliabidea taldean gehitzen duelako, baina ez du sortzen edozein bookings absorb baliabidearen ahalmena.

3. Zeregin baten **Antolaketa** saretan, hautatu, **Baliabidea** ikonoa baliabide gelaxkan **Taldekideak** aukeran, eta, ondoren, hautatu gehitu duzun taldekidea. 

> [!NOTE]
> **Taldekidea** eta **Kontziliazioa** fitxetan, baliabideak erakusten ditu erreserbatuta orduak zein esleitutako orduak. Orduak berdinak izan behar dira, baina ez da behar beharrezkoa, erreserbak eta esleipenak ez daudelako estu batera. **Kontziliazioa** fitxak xehetasunak ematen ditu ezberdinak direnean, adibidez, baliabide bati erreserbatu dituzunak baina ordu gehiago esleitzen dizkiozunean. Behar izanez gero, informazioa zuzendu dezakezu baliabidearen erreserba luzatzeko edo esleipena aldatzeko.

## <a name="create-a-generic-team-member-through-task-assignment"></a>Sortu zeregin-esleipenaren bidez taldeko kide orokor bat

Zereginen esleipenen bidez taldekide generikoa sortzean, leku-marka edo baliabide generikoa sortzen duzu, izena duen baliabidearen ezaugarriak azaltzen dituena, zereginetan lan egin nahi duzun horrenak. Zuk ondoren, sortu eskakizuna (edo eskakizunaren bidez eskaera eskaera bidali) izena duen baliabidea bilatzeko eta erreserbatzeko balio duena.

1. **Antolaketa** saretan zeregin batean, hautatu **Baliabidea** ikonoa baliabide gelaxkan.

2. Idatzi leku-marka baliabide izena gisa erabiltzeko. Adibidez, programaren kudeatzailea.

3. Hautatu **Sortu**, eta **Sorrera bizkorra proiektuaren taldekidea** eremuan, ezarri baliabide generikoaren funtzioa.

4. Jarrai dezakezu esleitzen zereginak leku-marka baliabide honi baliabidea zereginaren **Baliabide hautatzailea** eremuan hautatuz **Taldekideak** atalean zerrendatuta daude.

5. Noiz egin ari bertan orokorra baliabidea esleitu hautatu orokorra baliabide- **Taldearen** fitxan eta, gero, hautatu **Sortu Eskakizun** baliabide eskakizun baliabide orokorra sortzeko.

6. Hautatu **Liburua** baliabide orokorra. Bilatu eta erreserbatutako baliabide benetako antolaketa board ondoren, erabil dezakezu. Baliabide kudeatzailea arabera betetze-eskakizun hautatuta bidali dezakezu ere.

7. Baliabidea orokorra baliabide named beteta dagoenean, orokorra baliabide-taldetik kendu eta orokorra baliabide esleitutako zeregina orokorra baliabide baliabide eskakizun beteta baliabidea named esleitzen zaizkio.

## <a name="assign-a-named-resource-from-the-list-of-all-bookable-resources"></a>Esleitu izena duen baliabidea baliabide erreserbagarrien zerrendatik

Bilaketa-koadroa, **Baliabide hautatzailea** eremukoa, erabil dezakezu baliabide erreserbagarri guztiak bilatu eta zeregin bat esleitzeko.

Horrela esleitutako baliabideak erreserbatu gabe taldeari gehitzen zaizkio. Hau da taldekide bat gehitzea eta Inor metodo gisa hautatzearen berdina da. Baliabidea **Taldea** eta **Kontziliazioa** fitxetan agertzen da, esleipen eta erreserba defizita duten baliabide gisa. Erreserbatutako horiek erabilgarritasuna beren erabili nahi izanez gero.

1. **Antolaketa** saretan zeregin batean, hautatu **Baliabidea** ikonoa baliabide gelaxkan.

2. Hasiera-izen bat idazten. Bilaketaren emaitzak **Beste baliabideak** ataleko **Baliabide hautatzailea** eremuan bistaratzen dira.

3. Hautatu zereginari esleitu nahi diozun balabidea.



[!INCLUDE[footer-include](../includes/footer-banner.md)]