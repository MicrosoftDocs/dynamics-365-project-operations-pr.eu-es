---
title: Sortu proiektu-txantiloiak
description: Nola sortu proiektu-txantiloia Project Service-n
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 07/19/2022
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
ms.reviewer: johnmichalak
ms.openlocfilehash: 8159e0390441e5029f9beb0228cffcbc4d683479
ms.sourcegitcommit: 278740b352f1ed9618ee5c79597c8f449984d6f4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 07/19/2022
ms.locfileid: "9177410"
---
# <a name="create-a-project-template-project-service"></a>Nola sortu proiektu-txantiloia (Project Service)

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

Proiektua duzu ordu gorde txantiloiak enpresaren erregularki bids projects moten antzeko baduzu. Funtzio multzo eta estimatua proiektua mota ordu estandarra eskaintzen dute. Kontu buruentzako eta proiektua kudeatzaileak sor dezakezu projects oinarrituta proiektua txantiloi bat, edo txantiloia kopiatu eta hauetako euren egin dute.  
  
## <a name="components-of-project-template"></a>Proiektua txantiloiaren osagaiak
 Txantiloi proiektua hiru osagai zikloek dituzte:  
  
- **Lan egin diren kanpaina-xehatzea egitura**: lana diren kanpaina-xehatzea egitura proiektua txantiloian proiektuan bai elementuak multzo da. Sortu zeregin bat hierarkia, zeregin, zehaztu antolaketa atributu, ez diren menpekotasunak ezarri eta Gantt, datu guztiak ikusiko funtzioak erlazionatu. Aplikazioko txantiloiak proiektua egitura diren kanpaina-xehatzea lan ere laguntza zeregin moduak bakoitza. Ez dago proiektua txantiloi bat eta proiektua bat arteko aldea ez lan-antolaketa sortzen dituzunean.  
  
- **Proiektua estimates**: Proiektua estimates txantiloiak aplikazioan era berean lan duten projects ez bezala, kasuetan izan ezik, prezio-zerrenda lortzeko kostua defaulting eta prezioak salmenta beti dira lehenetsia kostua eta salmentak prezio-zerrendak zehaztutako [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] parametroak. Funtzionalitate gainerako proiektua bat bai berdina da.  
  
- **Proiektu-taldearen trebakuntza**: proiektu-txantiloirako proiektua taldeak sortzean, ezin duzu erreserbatu izendun baliabiderik txantiloian. Erabil dezakezu **Sortu Proiektua Taldearen** orokorra baliabide multzo bat sortu behar diren kanpaina-xehatzea egitura lan egin atalean. Ere zehaztu dezakezu beharrezko trebakuntza eta proficiencies baliabide orokorra. Ezin duzu ordezko bookable baliabide bat proiektua txantiloiak duen baliabide orokorra.  

## <a name="create-a-project-template-from-an-existing-project"></a>Sortu proiektuaren txantiloi bat lehendik dagoen proiektu batetik
Sor ditzakezu proiektua bat txantiloietatik hurrengo modu hauek daude:

- **Lanaren banaketa-egitura** : Proiektu batetik eratorritako txantiloi bateko lanaren banaketa-egitura batek zeregin eta menpekotasun guztiak kopiatuko ditu. Sortzen diren lanak proiektuaren txantiloia sortzen denean proiektu-taldeari gehitzen zaizkion talde-kide generikoetan oinarrituta egongo dira.
- **Proiektuaren aurrekontuak** : Lehendik dagoen proiektu batetik proiektu txantiloia sortzen denean, iturburuko proiektuaren estimazioak proiektuaren txantiloian kopiatzen dira.
- **Proiektuko taldekideak** : Lehendik dagoen proiektu batetik txantiloi bat sortzen denean, izendatutako taldekide guztiak erakundearen baliabide generikoarekin ordezkatzen dira. Kargu-izen eta rol guztiak mantentzen dira.

## <a name="create-a-project-from-a-template"></a>Sortu proiektua txantiloitik  
 Sor ditzakezu proiektua bat txantiloietatik hurrengo modu hauek daude:  
  
-   Eskaintzatik proiektua bat sortzeko, proiektu-txantiloi bat aukera dezakezu proiektua bizkor sortzeko inprimakian.  
  
-   Sakatuz proiektua bat sortzean **Berria Proiektua**, proiektua inprimakian bistaratzen erregistroa gorde aurretik. Bertatik, saka dezakezu **txantiloi bat Aukeratu** eremu aurretik zehaztutako proiektua txantiloiak erakundean zerrendatik hautatu.  
  
-   Sakatu **Sortu proiektua txantiloi batetik** **Proiektu-txantiloia** orrian, txantiloitik proiektu bat sortzeko.  
  
## <a name="copying-components-of-a-template-to-a-project"></a>Txantiloiko osagaiak proiektuan kopiatzea  
 Aplikaziora proiektua bat txantiloi bat osagaiak kopiatzen dituzunean daude gauza buruzko jakin behar duzu.  
  
 **Lan egin diren kanpaina-xehatzea egitura kopiatzen**: kopiatzen Duzunean lan diren kanpaina-xehatzea egitura proiektua txantiloi batetik proiektuan txantiloia baino proiektua beste egutegi bat badu, proiektua, egutegi batetik lanorduekin lan egin aplikatuko zereginak antolaketan. Antolaketa backing proiektua egutegiarekin egokitzen. Similarly, lana diren kanpaina-xehatzea egitura, zeregina lehen ez ditu irauten proiektua, hasiera-data, beraz gainerako, zeregina hierarkia eta iraupena-txantiloia lan diren kanpaina-xehatzea egitura zehazten menpekotasunak oinarrituta eguneratzen da.  
  
 **Proiektua estimates kopiatzen**: kopiatzen Dituzunean proiektua dagozkionak lineak zehar, prezio-zerrendak karpeetako zure proiektua kostua prezio-zerrenda eta salmenta-prezio-zerrendako bezero-unitatea oinarrituta. Unitate-kostua eta prezioak salmenta batetik erlazionatutako entitate salmenta projects, prezio-zerrendak horiek zehazten dituzte.  
  
 **Taldeak proiektua kopiatzen**: Denean duzu kopiatu proiektua talde-txantiloiaren proiektua bat, baliabideak orokorra dira kopiatzen zehar, bai eta trebakuntza proficiencies txantiloian zehaztuta. Baliabide orokorra esleipenetan proiektua txantiloi bai ere mantenduko dira.  
  
### <a name="see-also"></a>Ikusi baita ere  
 [Proiektu-kudeatzailearen gida](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
