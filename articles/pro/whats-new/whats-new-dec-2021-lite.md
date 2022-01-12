---
title: 2021eko abenduko berriak - Project Operations lite inplementatzea
description: Gai honek Project Operations lite inplementazioaren 2021eko abenduko bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 12/09/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 0432e2d4970c352e91cca589987bbdace57c6eaf
ms.sourcegitcommit: 9d20e7738cce195d344f5925a115741a1ce3ca36
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/21/2021
ms.locfileid: "7942962"
---
# <a name="whats-new-december-2021---project-operations-lite-deployment"></a>2021eko abenduko berriak - Project Operations lite inplementatzea

_Honi aplikatzen zaio: Oinarrizko inplementazioa: kudeatu proformako fakturak_

Gai hau Microsoft-en osagai eta bertsio hauei dagokie Dynamics 365 Project Operations:

- Proiektuaren Eragiketak a Dataverse ingurunearen bertsioa 4.27.0.195, 4.27.0.242


## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

### <a name="subcontract-management"></a>Azpikontratuen kudeaketa 

- [Proiektuko taldekideak azpikontratatzea](../subcontracting/subcontracting-project-team-members.md) : Proiektu-zuzendari batek taldekide izendun edo generikoak sor ditzake azpikontratuekin eta azpikontratu-lerroekin, langileen eta estimazioan eragina izateko.
- [Proiektuko taldekideentzako azpikontratazio aukerak](../subcontracting/subcon-options.md) : Proiektuko taldekideen izendun edo generikoen langileen aukerak egitean, proiektuaren kudeatzaileak dauden azpikontratuak berrikus ditzake edo proiektuko taldekide bat edo gehiagorentzat azpikontratu berriak sor ditzake. 
- [Azpikontratatutako baliabideen esleipenen kostuen estimazioa](../subcontracting/costing-subcon-ra.md) : Proiektuaren kostuen estimazioak azpikontratatutako baliabideen esleipenak hartuko ditu kontuan eta azpikontratuei lotutako erosketa-prezio-zerrendak erabiliz egingo du kostua. 
- [Konfiguratu Schedule Board lan-kontratuko langileak eta azpikontratatutako gaitasuna erakusteko](../subcontracting/configure-sb-subcon.md) : Ordutegi-taula Project Operations-en orain konfigura daiteke kontratu-langileen baliabideak eta azpikontratatutako gaitasuna langileekin batera bilatzeko eta iradokitzeko. Konfigurazio hau proiektu-eskakizun zehatz baterako langileen testuinguruan baliabideak bilatzean edo proiektu-eskakizun baten testuingurutik kanpo bilatzean aplika daiteke.
- [Proiektu bat lan-kontratuko langileekin eta azpikontratatutako gaitasunarekin hornitzea](../subcontracting/staffing-cw.md) : Kontratupeko langileak ordutegi batzordeko esperientziak aprobetxatuz proiektuetan erreserbatu daitezke.
- [Azpikontratatutako osagaien proiektuetan denbora, gastuak eta materialaren erabilera erregistratzea](../subcontracting/recording-subcon-actuals.md) : Kontratuko langileek denbora eta gastuak erregistra ditzakete, eta proiektuko taldekideek proiektu batean azpikontratu bat erabiliz erositako materialen erabilera ere erregistra dezakete. Honen ondorioz, erositako ahalmena edo materialak erabiltzen dituzten proiektuetan kostu zehatzak erregistratuko dira.
- [Azpikontratu batean estatu-trantsizioak](../subcontracting/subcon-states.md) : Azpikontratuak saltzailearekin negoziazioa osatzeko berretsi daitezke, itxi egin daitezke entrega amaitu dela adierazteko, edo bertan behera utzi daitezke hornitzailearekin kontratua amaitzea adierazteko entrega amaitu aurretik.

### <a name="task-planning"></a>Zereginen Plangintza
- Sistema-administratzaileentzako arazoen konponketa hobetua. Erabiltzaile batek proiektu bat ireki ezin duenean, administratzaileak lizentziekin lotutako akatsak berrikus ditzake Weberako Project-etik sortutako akatsak.[Proiektua antolatzeko erregistroak](../../project-management/schedule-api-logs.md).
- [Erabili zereginen zerrendak Microsoft Project-en weberako](https://support.microsoft.com/en-us/office/use-task-checklists-in-microsoft-project-for-the-web-c69bcf73-5c75-4ad3-9893-6d6f92360e9c). Weberako Microsoft Project-en, zeregin bati kontrol-zerrenda bat gehi diezaiokezu elementu zehatzen jarraipena egiteko.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

| **Ezaugarrien eremua** | **Erreferentzia-zenbakia** | **Kalitatearen eguneratzea** |
| --- | --- | --- |
| Antolaketa eta jarraipena | 2392596 | Schedule APIek orain eguneratzeak onartzen dituzte **Ahaleginak geratzen dira**, **amaituta**, eta **% Osatu** eremuak. |
| Antolaketa eta jarraipena | 2478497 | Programatu APIak **Jardueraren zenbakia** eta **Zereginaren IDa** eremuak hutsik egon daitezke sarreran, sistemak zenbakiketa automatizatua erabiliz beteko dituelako.|
| Denbora eta gastua | 2468135 | Onarpen-saioen kopurua bost izatetik hirura murrizten da. |
| Denbora eta gastua | 2468188 | Erregistroko testuak gehienezko luzera gainditzen zuen arazoa konpondu da **ohar-testua** ren atributua **oharpena** entitate. |
