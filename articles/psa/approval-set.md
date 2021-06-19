---
title: Onarpen multzoak
description: Gai honek onarpen multzoari, eskaerei eta eragiketa horien azpimultzoei buruzko informazioa eskaintzen du.
author: stsporen
manager: tfehr
ms.date: 05/28/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: ac73313420029ece740d0bdb9c21c7abaa9defc6
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116856"
---
# <a name="approval-sets"></a>Onarpen multzoak

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Onarpenak taldearen onarpen eskaerak eragiketa azpimultzo txikiagoetan biltzen ditu. Taldekatze honek Proiektuaren arabera onar ditzake onarpenak eta berriro saiatzea eta sekuentziatzea ahalbidetzen du. Multzokatzeak homologazioen prozesuen fidagarritasuna eta trazabilitatea hobetzen ditu homologazio kopuru handietan.

Onarpen multzoek erlazionatutako erregistroen prozesatze egoera orokorra adierazten dute. Onarpen erregistroa onarpen multzo bat erabiliz prozesatzen denean, erregistroa mugitzen da **Bidalita** aukeratik **Onartuta** aukerara, eta onarpen multzoarekin lotu gabe dago. Erregistro batek huts egiten badu onarpenera aurkezten denean, erregistroa egoera berean geratzen da **Bidalita** eta onarpen multzoa huts egin duela markatzen da. Onarpen multzoak hutsaren errore mezua erregistratzen du.

## <a name="processing-approvals-and-approval-sets"></a>Onarpenak eta onarpen multzoak prozesatzea
Fitxategian prozesatzeko ilaran dauden onarpenak ikusgai daude **Onarpenak prozesatzen** ikuspegia. Sistema sarrera guztiak hainbat aldiz modu asinkronoan prozesatzen saiatzen da, aurreko saiakerak huts egiten badu baimena berriro saiatzea barne.

**Onarpena ezarri Bizitza** eremuak multzoa prozesatzeko geratzen den saiakera kopurua erregistratzen du huts egin duela markatu aurretik.

## <a name="failed-approvals-and-approval-sets"></a>Ezin izan dira ezarri onarpenak eta onarpen multzoak
**Hutsegitea onartu da** ikuspegia erabiltzailearen esku-hartzea behar duten onarpen guztiak zerrendatzen ditu. Ireki lotutako onarpen multzoen erregistroak porrotaren zergatia identifikatzeko.
**Saiatu berriro** hautatuz gero onarpen multzoari bizitza osoko zenbaketa gehitzen dio, onarpen multzoa berriro egoera batera eramaten du **Prozesamendua**, eta gainerako erregistroak prozesatzen saiatzen da.

## <a name="configure-approval-sets"></a>Konfiguratu onarpen multzoak

###  <a name="enable-the-approval-sets-feature"></a>Gaitu Onarpen multzoen eginbidea
Onarpen multzoa eginbidea gaitu aurretik, egiaztatu ez dagoela prozesatzen ari diren onarpenik.

- Joan **Proiektuaren parametroak** orrialdera eta hautatu **Ezaugarrien kontrola** > **Gaitu onarpen modernoak**.

### <a name="turn-off-the-approval-sets-feature"></a>Desaktibatu Onarpen multzoen eginbidea
Onarpen multzoa eginbidea desaktibatu aurretik, egiaztatu ez dagoela prozesatzen ari diren onarpenik.

- Joan **Proiektuaren parametroak** orrialdera eta hautatu **Ezaugarrien kontrola** > **Desgaitu onarpen modernoak**.

### <a name="configuring-the-asynchronous-threshold"></a>Atalasea sinkronoa konfiguratzea 
Onarpen multzoak sortzen direnean, prozesamendua bigarren plano batera pasatzen da onartutako hautatutako erregistro kopurua adierazitako atalasea gainditzen duenean. Erabili **Atalasea asinkronoa** onarpen prozesamendua sinkronikoki edo asinkronikoki exekutatu behar denean konfiguratzeko eremua.
Baliozko balioak dira:

  - Zero: eskaera guztiak modu asinkronoan prozesatu beharko lirateke. 
  - Zero baino handiagoak diren zenbakiak: onartutakoak modu asinkronoan prozesatzen dira aurkeztutako onarpen kopuruak balio hori gainditzen duenean.

[!INCLUDE[footer-include](../includes/footer-banner.md)]