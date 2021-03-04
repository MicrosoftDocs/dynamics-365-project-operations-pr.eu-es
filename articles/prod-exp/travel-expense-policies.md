---
title: Konfiguratu gastu-gidalerroak
description: Zure langileek Microsoft Dynamics 365 Finance-ko gastuen txostenak eta bidaia-eskaerak sartu eta bidaltzerakoan jarraitu behar dituzten gastu-politikak konfigura ditzakezu.
author: suvaidya
manager: AnnBe
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysPolicyListPage, TrvPolicyRule
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: ab99c0ec769eb2e0914fc7d993f83d20e2c327f6
ms.sourcegitcommit: 9f31b33ed6e7f1b49200a407913201a1337f3401
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 01/14/2021
ms.locfileid: "4960682"
---
# <a name="set-up-expense-policies"></a>Konfiguratu gastu-gidalerroak

Zure langileek txostenak eta bidaia-eskaerak sartu eta bidaltzerakoan jarraitu behar dituzten gastu-politikak defini ditzakezu.         
Gastu politikak ezartzeak gastuak modu eraginkorrean kudeatzen lagun zaitzake.         

Adibidez, New Yorkeko hoteletako gastuei buruzko politika bat ezar dezakezu, gaueko gastuak ezin dituela USD 250 baino gehiago adierazi.       
Langile batek gastuen txostena edo bidaiaren eskaera aurkezten badu gelaren tarifak zenbateko hori gainditzen duenean, sistemak horren berri emango dio        
Langileak gastuaren polizaren zenbatekoa gainditu duela. Langileak zu jasotzean jasoko duen mezua konfigura dezakezu        
Politika definitu.      
        
Hiru politika mota defini ditzakezu:         
        
- Abisua: Langileak gastuen txostena edo bidaia eskaera aurkezteko aukera ematen du baina gastua onartzaile guztientzat eta        
  geroago salatzeko.        

- Errorea: Langileari gastua berrikusteko eskatzen dio politika betetzeko, gastuen txostena edo bidaia eskaera bidali aurretik.       
 
 - Justifikazioa: Langileak edo zuzendariak polizaren zenbatekoa gainditu izanaren justifikazioa sartzeko eskatzen du, gastuen txostena edo bidaia eskaera aurkeztu aurretik.        

## <a name="policy-tips"></a>Politika aholkuak
Hona hemen gastuak kudeatzeko politika berriak sortzen lagun zaitzaketen iradokizun batzuk. 
* Gidalerroak indarrean daudenean, horrek esan nahi du gidalerroek ez dutela eragina izango gastua gertatu den egunaren ondorengo datarekin sortzen bada. Adibidez, gaur 50 $ gehieneko otorduen gastua betearazteko politika berri bat sortzen ari bazara, atzotik sartutako lehendik dauden gastuak ez dira politika honen aurka egiaztatuko.
* Zehaztu daitekeen gastu-kategoria baterako politika sortzerakoan, kontuan hartu gastu-lerro motarako baldintza bat gehitzea. Baliteke ordainagiria eskatzea bezalako politika batzuek ez dute zentzurik zerrendatutako lerroetan eta goiburuaren lerroan edo zehaztu gabeko lerroan soilik aplikatu behar dira. 
* Gastuak kudeatzeko gidalerroak jatorrizko entitatearen arabera ebaluatzen dira lehenespenez. Enpresen arteko eszenatokietan, helburuko entitatearekin (mailegu-entitatea) ebaluatzeko politika ezarri dezakezu. Helburuko entitatearen aurkako gidalerroak exekutatzeko, aktibatu "Pertsona juridiko mailegu-hartzailearekiko Gastuen politika ebaluatzea" funtzioan **Ezaugarrien kudeaketa** lan eremua.

## <a name="when-to-evaluate-policies"></a>Noiz ebaluatu politikak

Gastua kudeatzeko parametroetan, aukera bat dago gastuak kudeatzeko politikak ebaluatzeko lerro bat gordetzen denean edo gastuen txostena aurkezten denean. Lerro bat noiz gordetzen den ebaluatzea aukeratzen baduzu, horrela erabiltzaileek lehenago ikusiko dute zer egin behar duten beren gastuen txostena aldi berean osatzeko. Bestela, gidalerroen ebaluazioa atzeratu eta denbora aurrez dezakezu amaieran baliozkotatzen bada, lan-fluxura bidalitakoan.
