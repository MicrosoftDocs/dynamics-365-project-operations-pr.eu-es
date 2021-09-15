---
title: 2021eko azaroko azpikontratazioaren sarbide esklusiboa argitalpena
description: Gai honek 2021eko urriko sarbide goiztiarraren bertsioaren parte diren Project Operations azpikontratatzeko gaitasunen ikuspegi orokorra eskaintzen du.
author: rumant
ms.date: 08/02/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 21ec8355487b5e69fc5b68b11dca029e6dc04f3c
ms.sourcegitcommit: c7f891adb5c81654c01d00c6b39beed403058eb1
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/14/2021
ms.locfileid: "7383680"
---
# <a name="subcontracting-in-october-2021-early-access-release"></a>2021eko azaroko azpikontratazioaren sarbide esklusiboa argitalpena

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Gai honek 2021eko urriko sarbide goiztiarraren bertsioaren parte diren Dynamics 365 Project Operations azpikontratatzeko gaitasunen ikuspegi orokorra eskaintzen du. Ezaugarri multzo hau ez dago ekoizteko edo zuzeneko inguruneetarako prest, beraz funtzio hauek sarbide goiztiarrean egongo dira funtzio multzo osoa kaleratu arte. Biziki gomendatzen dugu ez erabiltzea azpikontratazioen ezaugarriak zuzeneko produkzio eszenatokietarako, aurrebista bandera kendu arte. 

Ondorengo zerrendan 2021eko urriko sarbide goiztiarreko bertsioan gaur egun erabilgarri dagoenaren eskema ematen da:

1. Proiektuaren kudeatzaileak azpikontrata sortzen du saltzaile batekin. Berez, saltzailearen erregistroari atxikitako prezioen zerrendak azpikontratatzeko erabiltzen dira. Saltzailearen kontuak **Saltzailea** edo **Hornitzailea** motako erlazioa du.

2. Proiektuaren zuzendariak erosketa guztiak azpikontratako lineako elementu gisa sailka ditzake. Azpikontratazio lineak denbora, gastu edo produktuetarako izan daitezke. Azpikontratazio lerro transakzio klaseak zehazten du zertarako den linea.

3. Saltzailearen kontu kudeatzaileak eta proiektuaren kudeatzaileak azpikontrataren bidez errepika dezakete. Prezioa doi dezakezu azpikontratuan esleitu diren erosketaren prezio-zerrendetan.

4. Prozesuaren une honetan edo geroago, azpikontratazio lerroa denbora bada, saltzailearen kontu kudeatzaileak azpikontratazio lerro bakoitzarekin saltzailearen kontaktuak lotzen ditu. Elkarte honek informazioa ematen dio azpikontratuan lanean ari den proiektuaren zuzendariari. Kontaktu bat azpikontratazio lerro batekin lotzen denean saltzaileak, sistemak automatikoki erreserbatzeko baliabide bat sortzen du kontaktuarekin, erreserbatzeko baliabide bat existitzen ez bada.

5. Azpikontratazio lerro bakoitzeko fakturazio metodoa izan daiteke **Prezio finkoa** edo **Denbora eta materiala**. Prezio finkoaren azpikontratazio lerroetan, mugarrietan oinarritutako fakturen egutegia konfiguratuta dago.

Orokorrean deskribatutako negozio-prozesuaren fluxu-eko gainerako urratsak ez daude erabilgarri. Funtzionalitate berria gehitzen den neurrian, gai hau eguneratu egingo da. 

Ondorengo ilustrazioak Azpikontratazioko Sarbide Goiztiarreko bertsioa adierazten du amaierako negozioaren prozesuarekin alderatuta.

![Azpikontratazio prozesuaren fluxua](../media/SubcontractingEAFlow.png)  


## <a name="quantity-based-and-work-based-subcontract-lines-early-access-release"></a>Kopuruan oinarritutako eta lanean oinarritutako azpikontrata lerroak sarreraren argitalpen bizkorra
2021eko urriko Early Access bertsioan, kantitatean oinarritutako azpikontrata lerroak soilik onartzen dira. Horrek esan nahi du azpikontratazio lerro bat saltzaileari denbora, gastuak edo materialak erosteko erabil daitekeela, baina ez lan osoa. Horrek esan nahi du azpikontratazio lerro batean erositako kantitatea (denbora unitateak, gastuak edo material kantitatea) azpikontratazio lerro batean sistemako edozein proiektuetan erabil daitekeela.



[!INCLUDE[footer-include](../../includes/footer-banner.md)]
