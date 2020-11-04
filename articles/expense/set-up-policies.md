---
title: Gastuen politikak zehaztu
description: Zure langileek gastuen txostenak eta bidaia-eskaerak sartu eta bidaltzerakoan jarraitu behar dituzten gastu-politikak defini ditzakezu.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 30b3a0e1547ca7043b1433da2b4ebf02f2b473a1
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071106"
---
# <a name="define-expense-policies"></a>Gastuen politikak zehaztu

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Zure langileek txostenak eta bidaia-eskaerak sartu eta bidaltzerakoan jarraitu behar dituzten gastu-politikak defini ditzakezu.         
Gastu politikak ezartzeak gastuak modu eraginkorrean kudeatzen lagun zaitzake.         

Adibidez, New Yorkeko hoteletako gastuei buruzko politika bat ezar dezakezu, gaueko gastuak ezin dituela USD 250 baino gehiago adierazi.       
Langile batek gastuen txostena edo bidaiaren eskaera aurkezten badu gelaren tarifak zenbateko hori gainditzen duenean, sistemak horren berri emango dio         
Langileak gastuaren polizaren zenbatekoa gainditu duela. Langileak zu jasotzean jasoko duen mezua konfigura dezakezu        
Politika definitu.      
        
Hiru politika mota defini ditzakezu:         
        
- **Abisua** : Langileak gastuen txostena edo bidaia eskaera aurkezteko aukera ematen du baina gastua onartzaile guztientzat eta         
  geroago salatzeko.        

- **Errorea** : Langileari gastua berrikusteko eskatzen dio politika betetzeko, gastuen txostena edo bidaia eskaera bidali aurretik.        
 
 - **Justifikazioa** : Langileak edo zuzendariak polizaren zenbatekoa gainditu izanaren justifikazioa sartzeko eskatzen du, gastuen txostena edo bidaia eskaera aurkeztu aurretik.        

## <a name="policy-tips"></a>Politika aholkuak
Hona hemen gastuak kudeatzeko politika berriak sortzen lagun zaitzaketen iradokizun batzuk: 

- Gidalerroak indarrean daudenean, horrek esan nahi du gidalerroek ez dutela eragina izango gastua gertatu den egunaren ondorengo datarekin sortzen bada. Adibidez, politika berri bat sortzen duzu gaur 50 $ gehieneko otorduen gastua betearazteko. Atzotik hasita sartutako gastuak ez dira politika honen aurka egiaztatuko.
- Zehaztu daitekeen gastu-kategoria baterako politika sortzerakoan, kontuan hartu gastu-lerro motarako baldintza bat gehitzea. Politika batzuek, hala nola ordainagiria eskatzeak, agian ez dute zentzurik banakako lerroetan. Egoera horretan, politika goiburuaren lerroan edo zehaztu gabeko lerroan soilik aplikatzen da. 
- Gastuak kudeatzeko gidalerroak jatorrizko entitatearen arabera ebaluatzen dira lehenespenez. Enpresen arteko eszenatokietan, helburuko entitatearekin (mailegu-entitatea) ebaluatzeko politika ezarri dezakezu. Helburuko entitatearen aurkako gidalerroak exekutatzeko, aktibatu **Pertsona juridiko mailegu-hartzailearekiko Gastuen politika ebaluatzea** funtzioan **Ezaugarrien kudeaketa** lan eremua.

## <a name="when-to-evaluate-policies"></a>Noiz ebaluatu politikak

Gastua kudeatzeko parametroetan, gastuak kudeatzeko politikak ebaluatzea hauta dezakezu lerro bat gordetzen denean edo gastuen txostena aurkezten denean. Lerro bat noiz gordetzen den ebaluatzea aukeratzen baduzu, erabiltzaileek lehenago ikusiko dute zer egin behar duten beren gastuen txostena aldi berean osatzeko. Bestela, gidalerroen ebaluazioa atzeratu eta denbora aurrez dezakezu amaieran baliozkotuz, lan-fluxura bidalitakoan.
