---
title: Azpikontratuen kudeaketa Project Operations-en
description: Gai honek amaierako azpikontrata kudeatzeko prozesuaren ikuspegi orokorra eskaintzen du tipikoki proiektuetan oinarritutako erakundeetan.
author: rumant
ms.date: 09/14/2022
ms.topic: overview
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: b2e4518f77b2099f9818ea56623be9efb20b01f4
ms.sourcegitcommit: 08eb3be9eda44e9446c43ed9b6aefd58d77927c5
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/15/2022
ms.locfileid: "9522310"
---
# <a name="subcontract-management-in-project-operations"></a>Azpikontratuen kudeaketa Project Operations-en


_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Gai honek amaierako azpikontrata kudeatzeko prozesuaren ikuspegi orokorra eskaintzen du proiektuetan oinarritutako erakundeetan. Zerbitzuetarako azpikontratazioak normalean hurrengo diagraman agertzen den negozio-prozesuaren fluxu jarraitzen du.

![Azpikontratazio prozesuaren fluxua](../media/SubcontractingProcessFlow.png)

Hurrengo zerrendak hornitzen du azpikontratazio prozesuaren urratsez urrats deskribapena.

1. Proiektuaren kudeatzaileak azpikontrata sortzen du saltzaile batekin. Berez, saltzailearen erregistroari atxikitako prezioen zerrendak azpikontratatzeko erabiltzen dira. Saltzailearen kontuak **Saltzailea** edo **Hornitzailea** motako erlazioa du.
2. Proiektuaren zuzendariak erosketa guztiak azpikontratako lineako elementu gisa sailka ditzake. Azpikontratazio lineak denbora, gastu edo produktuetarako izan daitezke. Azpikontratazio lerro transakzio klaseak zehazten du zertarako den linea.
3. Saltzailearen kontu kudeatzaileak eta proiektuaren kudeatzaileak azpikontrataren bidez errepika dezakete. Prezioa doi dezakezu azpikontratuan esleitu diren erosketaren prezio-zerrendetan.
4. Prozesuaren une honetan edo geroago, azpikontratazio lerroa denbora bada, saltzailearen kontu kudeatzaileak azpikontratazio lerro bakoitzarekin saltzailearen kontaktuak lotzen ditu. Elkarte honek informazioa ematen dio azpikontratuan lanean ari den proiektuaren zuzendariari. Kontaktu bat azpikontratazio lerro batekin lotzen denean saltzaileak, sistemak automatikoki erreserbatzeko baliabide bat sortzen du kontaktuarekin, erreserbatzeko baliabide bat existitzen ez bada.
5. Azpikontratazio lerro bakoitzeko fakturazio metodoa izan daiteke **Prezio finkoa** edo **Denbora eta materiala**. Prezio finkoaren azpikontratazio lerroetan, mugarrietan oinarritutako fakturen egutegia konfiguratuta dago.
6.  Azpikontratua ezarri eta negoziazioa amaitu ondoren, berretsi egingo da. Baieztatutako azpikontratuak ezin dira editatu, baina aldaketak gertatzen badira, azpikontrata "berriro ireki daiteke editatzeko", eta horrek egoera ezartzen du **Baieztatuta** itzuli **Zirriborroa** eta negoziazioa berriro ireki daiteke. 
7.  Proiektu batean taldekide generikoa sortzerakoan, taldekidea azpikontrata lerro batekin lotu daiteke. Horrek azpikontratatzeko gaitasuna duen taldekide generikoa lantzeko beharra adierazten du.
8.  Izendatutako taldekideak proiektuan zuzenean sor daitezke edo baliabideak antolatzeko esperientziak erabiliz erreserbatuz sor daitezke. Izendatutako proiektuko taldekide bat kontratupeko langilea bada, posible da azpikontratazio lerro batekin lotzea. Honek eskuragarri dagoen edukiera azpikontratazio lerro batean marraztuko du.
9.  Azpikontratatutako baliabideek denbora, gastuak eta materialaren erabilera erregistratu ditzakete proiektuetan eta proiektuetako zereginetan, eta, ondoren, onartzeko. Langileen antzekoa da. Denbora grabatzen duenean, kontratupeko langileak azpikontrata eta azpikontrata lerro jakin bat hauta dezake.
10. Onartu ondoren, azpikontratuek onartutako denborak proiektuaren kostuen fakturak erregistratuko ditu, kontratupeko langilearen erosketa-prezioaren edo proiektuan betetzen duten funtzioaren arabera.
11. Saltzailearen fakturak eta saltzailearen fakturen ildoak sisteman erregistratu daitezke saltzailearen baliabideek edo saltzaileak entregatutako produktuek egindako lana egiteko. Saltzailearen faktura-lerroek proiektu baterako eta transakzio klaseko denbora, gastu, produktu / material, mugarri edo kuota zehatzak izan behar dute. Aukeran, saltzailearen faktura lerroek azpikontratazio lerro bat erreferentzia dezakete.
12. Sistemak automatikoki lotuko ditu azpikontratazio lerroarekin eta proiektuarekin bat datozen kostuen faktore guztiak saltzailearen fakturarekin. Honek 3 norabideko partida eta egiaztapen prozesua erraztuko du.
13. Proiektuaren kudeatzaileak, ondoren, automatikoki bat datozen proiektuaren datuak berrikusi ditzake, proiektuaren beste kostuen datuak kendu edo gehi ditzake eta egiaztapen prozesua osa dezake.
14. Lerro guztietan egiaztapen prozesua osatzeak saltzailearen faktura honela markatuko du **Ordainketarako prest**. Etapa honetan, saltzailearen faktura eta lerroak Kontabilitate edo Ordaintzeko sistema batera transferi daitezke saltzaileari ordainketa prozesatzeko. Aurretik erregistratutako proiektuaren kostuak alderantzikatu egingo dira eta saltzailearen faktura-lerroaren benetako kostuak proiektuan erregistratuko dira.

## <a name="quantity-based-subcontract-lines-and-work-based-subcontract-lines"></a>Kopuruan oinarritutako azpikontrata lerroak eta lanean oinarritutako azpikontrata lerroak

Azpikontratuaren lerroak kantitatean oinarritutakoa edo lanean oinarritutakoa. 

Azpikontratazio lerro bat denean **kantitatean oinarrituta**, azpikontrata lerroan denboran, gastuetan edo materialean erosten den kantitatea edozein proiektutan erabil daiteke.

Azpikontratazio lerro bat denean **lanean oinarrituta**, azpikontrata lerroak proiektuaren planeko nodo batek irudikatzen duen lan multzo batera mapatzen du. Azpikontratazio lerroaren balioa lan hori emateko beharrezkoak diren osagai guztien batura da. Hauek azpikontrata lerroaren xehetasun gisa modelatzen dira eta denbora, gastu edo materialen bilketa izan daitezke. Lanean oinarritutako azpikontratazio lerro baterako, azpikontratazio lerroa proiektu bakar bati ere eskaintzen zaio. Azpikontratazio mota hauek oraingoz ez dituzte onartzen Project Operations-ek.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]

