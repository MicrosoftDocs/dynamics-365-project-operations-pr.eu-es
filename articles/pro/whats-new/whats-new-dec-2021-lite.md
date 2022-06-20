---
title: 2021eko abenduko berrikuntzak - Project Operations lite-ren inplementazioa
description: Artikulu honetan, Project Operations lite-ren ezarpenaren 2021eko abenduko bertsioan eskuragarri dauden kalitate-eguneratzeei buruzko informazioa ematen da.
author: sigitac
ms.date: 12/09/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 301acc5be76fb0318d6298820b62ae5bb05efac3
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8914065"
---
# <a name="whats-new-december-2021---project-operations-lite-deployment"></a>2021eko abenduko berrikuntzak - Project Operations lite-ren inplementazioa

_Honi aplikatzen zaio: Oinarrizko inplementazioa: kudeatu proformako fakturak_

Artikulu hau Microsoft-en osagai eta bertsio hauei aplikatzen zaie Dynamics 365 Project Operations:

- Proiektuaren Eragiketak a Dataverse ingurunearen bertsioa 4.27.0.195, 4.27.0.242, 4.27.0.244


## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

### <a name="subcontract-management"></a>Azpikontratuen kudeaketa 

- [Proiektuko taldeko kideen](../subcontracting/subcontracting-project-team-members.md) azpikontratazioa: proiektu-kudeatzaile batek azpikontratuekin eta azpikontratazio-lerroekin izendatutako taldeko kideak edo generikoak sor ditzake, langileen hornidurari eta zenbatespenari erasan ahal izateko.
- [Proiektuko taldeko kideentzako](../subcontracting/subcon-options.md) azpikontratazio-aukerak: Proiektuko lantaldeko kide izendatuak edo generikoak diren langileentzako langileak hornitzeko erabakiak hartzean, proiektuaren gerenteak dauden azpikontratuak berrikusi edo azpikontratu berriak sortu ditzake proiektuko taldekide batentzat edo gehiagorentzat. 
- [Azpikontratatutako baliabideen esleipenen](../subcontracting/costing-subcon-ra.md) kostuen zenbatespena: Proiektuaren kostuen zenbatespenak kontuan hartuko ditu azpikontratatutako baliabideen esleipenak, eta azpikontratuekin lotutako erosketa-prezioen zerrendak erabiliz kostatuko dira. 
- [Konfiguratu programazio-taula kontratatutako langileak eta azpikontratatutako gaitasuna](../subcontracting/configure-sb-subcon.md) erakusteko: Proiektu-eragiketetako programazio-taula orain konfiguratu daiteke baliabide erreserbagarrien kontratatutako langile-mota eta azpikontratatutako gaitasuna, langileekin batera, bilatu eta iradokitzeko. Konfigurazio hori aplika daiteke proiektuaren baldintza zehatz baterako langileak hornitzearen testuinguruan baliabideak bilatzen direnean edo proiektuaren baldintza baten testuingurutik kanpo bilatzen denean.
- [Langile kontratatuak eta azpikontratatutako gaitasuna](../subcontracting/staffing-cw.md) dituen proiektu baterako langile-zuzkidura: Kontratatutako langileak proiektuetan gorde daitezke, programazio-batzordearen esperientziak aprobetxatuz.
- [Azpikontratatutako osagaietarako](../subcontracting/recording-subcon-actuals.md) proiektuetan denbora, gastuak eta materialen erabilera erregistratzea: kontratatutako langileek denbora eta gastuak erregistratu ditzakete, eta proiektuko lantaldeko kideek ere erregistratu dezakete erositako materialen erabilera, azpikontratu bat erabiliz proiektu batean. Hori, erositako gaitasuna edo materialak erabiltzen dituzten proiektuetan behar diren kostuen erregistroan gertatuko da.
- [Azpikontratu](../subcontracting/subcon-states.md) bateko estatu-transizioak: Azpikontratuak berretsi ahal izango dira hornitzailearekin negoziazioa osatzeko, entrega amaitu dela adierazteko itxi edo ezeztatzeko, hornitzailearekin kontratua amaitu dela adierazteko, entrega amaitu baino lehen.

### <a name="task-planning"></a>Zereginen plangintza
- Sistema-administratzaileentzako arazoen konponketa hobetua. Erabiltzaile batek proiektu bat ireki ezin duenean, administratzaileak Project-ek Project-en programazio-erregistroetan [sortutako lizentziarekin zerikusirik ez duten akatsak](../../project-management/schedule-api-logs.md) berrikusi ditzake.
- [Erabil zaitez Microsoft Project-en webgunerako](https://support.microsoft.com/en-us/office/use-task-checklists-in-microsoft-project-for-the-web-c69bcf73-5c75-4ad3-9893-6d6f92360e9c) lanak egiaztatzeko zerrendak. Weberako Microsoft Project-en, zeregin bati kontrol-zerrenda bat gehi diezaiokezu elementu zehatzen jarraipena egiteko.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

| **Ezaugarrien eremua** | **Erreferentzia-zenbakia** | **Kalitatearen eguneratzea** |
| --- | --- | --- |
| Antolaketa eta jarraipena | 2392596 | Schedule APIek orain eguneratzeak onartzen dituzte **Ahaleginak geratzen dira**, **amaituta**, eta **% Osatu** eremuak. |
| Antolaketa eta jarraipena | 2478497 | Jarduera-kopurua **eta** ID lan-eremuak **zuri** egon daitezke sarreran, sistemak zenbaki automatizatuaren bidez beteko dituelako.|
| Denbora eta gastua | 2468135 | Onarpen-saioen kopurua bost izatetik hirura murrizten da. |
| Denbora eta gastua | 2468188 | Arazoa erregistro-testuarekin zuzendu da, idatzohar-erakundearen notetext **atributuan** **gehieneko luzera gainditzen** baitzuen. |
