---
title: Onarpen multzoak
description: Artikulu honek onarpen-multzoekin, eskaerarekin eta eragiketa horien azpimultzoekin nola lan egin azaltzen du.
author: stsporen
ms.date: 02/01/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: ca205073edbce2b399aab3ae273d635c8af96765
ms.sourcegitcommit: b2d05f898daa552179d67fdf4c060c93a9c66bd1
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/16/2022
ms.locfileid: "9524901"
---
# <a name="approval-sets"></a>Onarpen multzoak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Onarpenak taldearen onarpen eskaerak eragiketa azpimultzo txikiagoetan biltzen ditu. Multzo horri esker, onarpenak proiektuen arabera orden zehatz batean prozesatu daitezke eta berriro saiatzea eta sekuentziatzea ahalbidetzen du. Onarpen-eskaerak batera multzokatzeak homologazioen prozesuen fidagarritasuna eta trazabilitatea hobetzen ditu homologazio kopuru handietan.

Onarpen multzoek erlazionatutako erregistroen prozesatze egoera orokorra adierazten dute. Onarpen erregistroa onarpen multzoa erabiliz prozesatzen denean, erregistroa mugitzen da **Aurkeztua** hurrengora **Onartua**, eta jada ez dago onarpen multzoarekin lotuta. Erregistro batek huts egiten badu onarpenera aurkezten denean, erregistroa egoera berean geratzen da **Bidalita** eta onarpen multzoa huts egin duela markatzen da. Onarpen multzoak hutsaren errore mezua erregistratzen du.

## <a name="processing-approvals-and-approval-sets"></a>Onarpenak eta onarpen multzoak prozesatzea
Fitxategian prozesatzeko ilaran dauden onarpenak ikusgai daude **Onarpenak prozesatzen** ikuspegia. Sistemak sarrera guztiak hainbat aldiz prozesatzen ditu modu asinkronoan, aurreko saiakerak huts egiten badu baimena berriro saiatzea barne.

**Onarpena ezarri Bizitza** eremuak multzoa prozesatzeko geratzen den saiakera kopurua erregistratzen du huts egin duela markatu aurretik.

Onarpen-multzoak a-n oinarritutako aldizkako aktibazioaren bidez prozesatzen dira **Hodei Fluxua** izendatua **Proiektu-zerbitzua - Behin eta berriz programatu proiektuak onartzeko multzoak**. Hau aurkitzen da **Irtenbidea** izendatua **Proiektuaren Eragiketak**. 

Ziurtatu fluxua aktibatuta dagoela hurrengo urratsak betez.

1. Administratzaile gisa, hasi saioa [flow.microsoft.com](https://powerautomate.microsoft.com).
2. Goiko eskuineko izkinan, aldatu erabiltzen duzun ingurunera Dynamics 365 Project Operations.
3. Hautatu **Irtenbideak** ingurunean instalatutako irtenbideak zerrendatzeko.
4. Irtenbideen zerrendan, hautatu **Proiektuaren Eragiketak**.
5. Aldatu iragazkia honetatik **Denak** to **Hodei Fluxuak**.
6. Egiaztatu hori **Proiektuen Zerbitzua - Behin eta berriz programatu proiektuak onartzeko multzoak** fluxua ezarrita dago **On**. Hala ez bada, hautatu fluxua eta, ondoren, hautatu **Piztu**.
7. Egiaztatu prozesaketa bost minuturo gertatzen dela berrikusiz **Sistema-lanak** zerrendan **Ezarpenak** zure Proiektu Eragiketen barruan Dataverse ingurunea.

## <a name="failed-approvals-and-approval-sets"></a>Ezin izan dira ezarri onarpenak eta onarpen multzoak
**Hutsegitea onartu da** ikuspegia erabiltzailearen esku-hartzea eskatzen duten onarpen guztiak zerrendatzen ditu. Ireki lotutako onarpen multzoen erregistroak porrotaren zergatia identifikatzeko.
**Saiatu berriro** hautatuz gero onarpen multzoari bizitza osoko zenbaketa gehitzen dio, onarpen multzoa berriro egoera batera eramaten du **Prozesamendua**, eta gainerako erregistroak prozesatzen saiatzen da.

## <a name="configure-approval-sets"></a>Konfiguratu onarpen multzoak

### <a name="enable-the-approval-sets-feature"></a>Gaitu Onarpen multzoen eginbidea
Onarpen multzoa eginbidea gaitu aurretik, egiaztatu ez dagoela prozesatzen ari diren onarpenik. Eginbide hau gaitu ondoren, ezin da desgaitu.

- Joan **Proiektuaren parametroak** orrialdera eta hautatu **Ezaugarrien kontrola** > **Gaitu onarpen modernoak**.

### <a name="configuring-the-asynchronous-threshold"></a>Atalasea sinkronoa konfiguratzea 
Onarpen multzoak sortzen direnean, prozesamendua bigarren plano batera pasatzen da onartutako hautatutako erregistro kopurua adierazitako atalasea gainditzen duenean. Erabili **Atalasea asinkronoa** onarpen prozesamendua sinkronikoki edo asinkronikoki exekutatu behar denean konfiguratzeko eremua. Hautatu balio hauetako bat:

  - Zero: eskaera guztiak modu asinkronoan prozesatu beharko lirateke. 
  - Zero baino handiagoak diren zenbakiak: onartutakoak modu asinkronoan prozesatzen dira aurkeztutako onarpen kopuruak balio hori gainditzen duenean.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
