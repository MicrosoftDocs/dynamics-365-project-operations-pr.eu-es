---
title: Onarpen multzoak
description: Artikulu honetan, eragiketa horien onarpen-multzoekin, eskabideekin eta azpikonjuntekin nola lan egin azaltzen da.
author: stsporen
ms.date: 02/01/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 5e030c1aa4a41b428a0f4541fd204a7a3deaba08
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8918067"
---
# <a name="approval-sets"></a>Onarpen multzoak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Onarpenak taldearen onarpen eskaerak eragiketa azpimultzo txikiagoetan biltzen ditu. Multzo horri esker, onarpenak proiektuen arabera orden zehatz batean prozesatu daitezke eta berriro saiatzea eta sekuentziatzea ahalbidetzen du. Onarpen-eskaerak batera multzokatzeak homologazioen prozesuen fidagarritasuna eta trazabilitatea hobetzen ditu homologazio kopuru handietan.

Onarpen multzoek erlazionatutako erregistroen prozesatze egoera orokorra adierazten dute. Onarpen erregistroa onarpen multzoa erabiliz prozesatzen denean, erregistroa mugitzen da **Aurkeztua** hurrengora **Onartua**, eta jada ez dago onarpen multzoarekin lotuta. Erregistro batek huts egiten badu onarpenera aurkezten denean, erregistroa egoera berean geratzen da **Bidalita** eta onarpen multzoa huts egin duela markatzen da. Onarpen multzoak hutsaren errore mezua erregistratzen du.

## <a name="processing-approvals-and-approval-sets"></a>Onarpenak eta onarpen multzoak prozesatzea
Fitxategian prozesatzeko ilaran dauden onarpenak ikusgai daude **Onarpenak prozesatzen** ikuspegia. Sistemak sarrera guztiak hainbat aldiz prozesatzen ditu modu asinkronoan, aurreko saiakerak huts egiten badu baimena berriro saiatzea barne.

**Onarpena ezarri Bizitza** eremuak multzoa prozesatzeko geratzen den saiakera kopurua erregistratzen du huts egin duela markatu aurretik.

Onarpen-multzoak Project Service - Recurrently Schedule Project Approval Sets izeneko **hodei-fluxu batean** oinarritutako aldizkako **aktibazioaren bidez prozesatzen dira**. Hori proiektu-eragiketak **izeneko soluzioan** **·**. 

Ziurtatu fluxua aktibatuta dagoela hurrengo urratsak osatuz.

1. Administratzaile gisa, hasi saioa [flow.microsoft.com](https://powerautomate.microsoft.com).
2. Goiko eskuineko izkinan, aldatu ingurua Dynamics 365 Project Operations.
3. Ingurunean instalatutako soluzioak zerrendatzeko konponbideak **hautatu**.
4. Konponbideen zerrendan, aukeratu **proiektu-eragiketak**.
5. Aldatu Guztien **iragazkia** **hodeian**.
6. Egiazta ezazu proiektu-zerbitzuaren fluxua **– Proiektuak onartzeko** aldian behin programatzea aktibatuta **dagoela**. Hala ez bada, fluxua hautatu eta, ondoren, **aktibatu**.
7. Egiazta ezazu prozesamendua bost minuturo gertatzen dela, Project Operations **inguruneko konfigurazio-eremuko** sistemaren **lan-zerrenda** berrikusiz Dataverse.

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
