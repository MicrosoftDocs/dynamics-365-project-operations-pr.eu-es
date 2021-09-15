---
title: Onarpen multzoak
description: Gai honek onarpen multzoekin, eskaerekin eta eragiketa horien azpimultzoekin nola lan egin azaltzen du.
author: stsporen
manager: tfehr
ms.date: 08/10/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 1d9333033eb2b03966c6531d0fd6ad5b878acd93
ms.sourcegitcommit: 80aa1e8070f0cb4992ac408fc05bdffe47cee931
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "7323221"
---
# <a name="approval-sets"></a>Onarpen multzoak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Onarpenak taldearen onarpen eskaerak eragiketa azpimultzo txikiagoetan biltzen ditu. Multzo horri esker, onarpenak proiektuen arabera orden zehatz batean prozesatu daitezke eta berriro saiatzea eta sekuentziatzea ahalbidetzen du. Onarpen-eskaerak batera multzokatzeak homologazioen prozesuen fidagarritasuna eta trazabilitatea hobetzen ditu homologazio kopuru handietan.

Onarpen multzoek erlazionatutako erregistroen prozesatze egoera orokorra adierazten dute. Onarpen erregistroa onarpen multzoa erabiliz prozesatzen denean, erregistroa mugitzen da **Aurkeztua** hurrengora **Onartua**, eta jada ez dago onarpen multzoarekin lotuta. Erregistro batek huts egiten badu onarpenera aurkezten denean, erregistroa egoera berean geratzen da **Bidalita** eta onarpen multzoa huts egin duela markatzen da. Onarpen multzoak hutsaren errore mezua erregistratzen du.

## <a name="processing-approvals-and-approval-sets"></a>Onarpenak eta onarpen multzoak prozesatzea
Fitxategian prozesatzeko ilaran dauden onarpenak ikusgai daude **Onarpenak prozesatzen** ikuspegia. Sistemak sarrera guztiak hainbat aldiz prozesatzen ditu modu asinkronoan, aurreko saiakerak huts egiten badu baimena berriro saiatzea barne.

**Onarpena ezarri Bizitza** eremuak multzoa prozesatzeko geratzen den saiakera kopurua erregistratzen du huts egin duela markatu aurretik.

## <a name="failed-approvals-and-approval-sets"></a>Ezin izan dira ezarri onarpenak eta onarpen multzoak
**Hutsegitea onartu da** ikuspegia erabiltzailearen esku-hartzea eskatzen duten onarpen guztiak zerrendatzen ditu. Ireki lotutako onarpen multzoen erregistroak porrotaren zergatia identifikatzeko.
**Saiatu berriro** hautatuz gero onarpen multzoari bizitza osoko zenbaketa gehitzen dio, onarpen multzoa berriro egoera batera eramaten du **Prozesamendua**, eta gainerako erregistroak prozesatzen saiatzen da.

## <a name="configure-approval-sets"></a>Konfiguratu onarpen multzoak

### <a name="enable-the-approval-sets-feature"></a>Gaitu Onarpen multzoen eginbidea
Onarpen multzoa eginbidea gaitu aurretik, egiaztatu ez dagoela prozesatzen ari diren onarpenik.

- Joan **Proiektuaren parametroak** orrialdera eta hautatu **Ezaugarrien kontrola** > **Gaitu onarpen modernoak**.

### <a name="turn-off-the-approval-sets-feature"></a>Desaktibatu Onarpen multzoen eginbidea
Onarpen multzoa eginbidea desaktibatu aurretik, egiaztatu ez dagoela prozesatzen ari diren onarpenik.

- Joan **Proiektuaren parametroak** orrialdera eta hautatu **Ezaugarrien kontrola** > **Desgaitu onarpen modernoak**.

### <a name="configuring-the-asynchronous-threshold"></a>Atalasea sinkronoa konfiguratzea 
Onarpen multzoak sortzen direnean, prozesamendua bigarren plano batera pasatzen da onartutako hautatutako erregistro kopurua adierazitako atalasea gainditzen duenean. Erabili **Atalasea asinkronoa** onarpen prozesamendua sinkronikoki edo asinkronikoki exekutatu behar denean konfiguratzeko eremua. Hautatu balio hauetako bat:

  - Zero: eskaera guztiak modu asinkronoan prozesatu beharko lirateke. 
  - Zero baino handiagoak diren zenbakiak: onartutakoak modu asinkronoan prozesatzen dira aurkeztutako onarpen kopuruak balio hori gainditzen duenean.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
