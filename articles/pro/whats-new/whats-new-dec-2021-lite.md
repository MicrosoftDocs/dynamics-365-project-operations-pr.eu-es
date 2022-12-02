---
title: Zer berri 2021eko abendua - Project Operations lite/ren inplementazioa
description: Gai honek informazioa eskaintzen du 2022ko abenduaren Project Operations inplementazio arinaren bertsioan eskuragarri dauden kalitate-eguneratzeei buruz.
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
# <a name="whats-new-december-2021---project-operations-lite-deployment"></a>Zer berri 2021eko abendua - Project Operations lite/ren inplementazioa

_Honi aplikatzen zaio: Oinarrizko inplementazioa: kudeatu proformako fakturak_

Gai hau Microsoft Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

- Project Operations 4.27.0.195, 4.27.0.242, 4.27.0.244 bertsioko Dataverse ingurunean


## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

### <a name="subcontract-management"></a>Azpikontratatuen kudeaketa 

- [Proiektuko taldekideak azpikontratatzea](../subcontracting/subcontracting-project-team-members.md): Proiektu-zuzendari batek taldekide izendun edo generikoak sor ditzake azpikontratuekin eta azpikontratazio-lerroekin, langileen eta estimazioan eragina izateko.
- [Proiektuko taldekideentzako azpikontratazio aukerak](../subcontracting/subcon-options.md): Proiektu-taldekideen izendun edo generikoen langileen aukerak egitean, proiektuaren kudeatzaileak lehendik dauden azpikontratuak berrikus ditzake edo proiektu-taldekide bat edo gehiagorentzat azpikontratu berriak sor ditzake. 
- [Azpikontratatutako baliabideen esleipenen kostuen estimazioa](../subcontracting/costing-subcon-ra.md): Proiektuaren kostuen zenbatespenak azpikontratatutako baliabideen esleipenak hartuko ditu kontuan eta azpikontratuei lotutako erosketa-prezio-zerrendak erabiliz egingo du kostua. 
- [Konfiguratu Schedule Board lan-kontratuko langileak eta azpikontratatutako gaitasuna erakusteko](../subcontracting/configure-sb-subcon.md): Ordutegi-taula Project Operations-en orain konfigura daiteke langileekin batera erreserba daitezkeen baliabideak eta azpikontratatutako edukiera kontratudun langile motak bilatzeko eta iradokitzeko. Konfigurazio hau proiektuaren eskakizun zehatz baterako langileen testuinguruan baliabideak bilatzean edo proiektuaren eskakizun baten testuingurutik kanpo bilatzean aplika daiteke.
- [Proiektu bat lan-kontratudun langileekin eta azpikontratatutako gaitasunarekin hornitzea](../subcontracting/staffing-cw.md): Kontratupeko langileak ordutegi batzordeko esperientziak aprobetxatuz proiektuetan erreserbatu daitezke.
- [Azpikontratatutako osagaien proiektuetan denbora, gastuak eta materialaren erabilera erregistratzea](../subcontracting/recording-subcon-actuals.md): Kontratuko langileek denbora eta gastuak erregistra ditzakete, eta proiektuko taldekideek proiektu batean azpikontratu bat erabiliz erositako materialen erabilera ere erregistra dezakete. Honen ondorioz, erositako ahalmena edo materialak erabiltzen dituzten proiektuetan kostu zehatzak erregistratuko dira.
- [Azpikontratu batean estatu-trantsizioak](../subcontracting/subcon-states.md): Azpikontratuak saltzailearekin negoziazioa amaitzeko berretsi daitezke, itxi egin daitezke entrega amaitu dela adierazteko, edo bertan behera utzi saltzailearekin kontratua amaitu baino lehen entregatu aurretik.

### <a name="task-planning"></a>Zeregina antolatu
- Arazoak konpontzeko eginbide hobetua sistema-administratzaileentzat. Erabiltzaile batek proiektu bat ireki ezin duenean, administratzaileak lizentziekin lotutako akatsak berrikus ditzake Project for the web-etik sortutako akatsak [Proiektua antolatzeko erregistroak](../../project-management/schedule-api-logs.md) atalean.
- [Erabili zereginen zerrendak Microsoft Project for the web-en](https://support.microsoft.com/en-us/office/use-task-checklists-in-microsoft-project-for-the-web-c69bcf73-5c75-4ad3-9893-6d6f92360e9c). Microsoft Project for the web-en, zeregin bati kontrol-zerrenda bat gehi diezaiokezu elementu zehatzen jarraipena egiteko.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

| **Ezaugarrien eremua** | **Erreferentzia-zenbakia** | **Kalitatearen eguneratzea** |
| --- | --- | --- |
| Antolaketa eta jarraipena | 2392596 | Antolaketa APIek orain eguneratzeak onartzen dituzte **Geratzen den ahalegina**, **Osatutako ahalegina**, eta **% Osatuta** eremuetan. |
| Antolaketa eta jarraipena | 2478497 | **Jardueraren zenbakia** eta **Zereginaren IDa** antolaketa APIen eremuak hutsik egon daitezke sarreran, sistemak beteko dituelako zenbakikuntza automatizatua erabiliz.|
| Denbora eta gastua | 2468135 | Onarpen-saioen kopurua bostetik hirura murrizten da. |
| Denbora eta gastua | 2468188 | Erregistroko testuak gehienezko luzera gainditzen zuen arazoa konpondu da **ohar-testua** atributuan **Oharra** entitatean. |
