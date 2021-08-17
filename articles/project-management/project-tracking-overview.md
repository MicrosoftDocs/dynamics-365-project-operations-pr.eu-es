---
title: Proiektuko ahaleginaren segimendua
description: Gai honek proiektuaren ahaleginaren eta lanaren garapenaren jarraipena egiteari buruzko informazioa ematen du.
author: ruhercul
ms.date: 03/22/2021
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.custom: intro-internal
ms.openlocfilehash: 0df357eaf662816107fbc1777ebae030c93bd199756e78a1c3d59155dc64d38f
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6993946"
---
# <a name="project-effort-tracking"></a>Proiektuko ahaleginaren segimendua

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Antolaketa eta garapena jarraitzeko beharra aldatu egiten da industriaren arabera. Zenbait industriak jarraipen zehatza egiten du; beste batzuek jarraipen orokorragoa egiten dute. Gai honek erakundearen eskakizunak betetzeko nola antolatu behar den erakusten du.

## <a name="effort-tracking-view"></a>Ahaleginen segimenduaren ikuspegia

**Esfortzuaren jarraipena** ikuspegia egutegiaren zereginen bilakaeraren jarraipena egiten du zeregin batean emandako benetako esfortzu-orduak atazaren aurreikusitako esfortzu-orduekin alderatuz. Dynamics 365 Project Operations-ek honako formula hauek erabiltzen ditu jarraipen-neurriak kalkulatzeko:

- **Garapenaren ehunekoa**: Orain arte egindako ahalegina ÷ Aurreikusitako kostua osatzen denerako (EAC) 
- **Geratzen den ahalegina** Aurreikusitako ahalegina osatzen denerako - Orain arte egindako ahalegina 
- **EAC**: Geratzen den ahalegina + Orain arte egindako ahalegina 
- **Proiektatutako ahaleginaren bariantza**: Aurreikusitako ahalegina - EAC

Project Operations-ek zereginen bariantzaren bistaratzea erakusten du. EAC aurreikusitako ahalegina baino handiagoa bada, zereginak hasieran aurreikusitakoa baino denbora gehiago beharko duela aurreikusten da eta antolaketaren atzean dago. EAC aurreikusitako ahalegina baino gutxiago bada, zereginak hasieran aurreikusitakoa baino denbora gutxiago beharko duela aurreikusten da eta antolaketaren aurrean dago.

## <a name="reprojecting-effort-on-leaf-node-tasks"></a>Hosto nodoko zereginetan ahalegina berriro proiektatzea

Proiektu-kudeatzaileek sarritan zereginen jatorrizko aurreikuspenak berrikusten dituzte. Proiektuaren birproiekzioak proiektu-kudeatzaileak proiektuaren egungo egoera ikusita duen kalkuluen pertzepzioa da. Hala ere, ez dugu gomendatzen proiektuaren kudeatzaileek aurreikusitako ahalegin zenbakiak aldatzea. Hau da, proiektuaren aurreikusitako ahalegina proiektuaren egutegiaren eta kostuen kalkulurako ezarritako egiaren iturria dela eta proiektuko eragile guztiek ados jarri direlako.

Proiektu kudeatzaile batek zereginetan ahalegina berriro proiektatu dezake **Geratzen den ahalegina** lehenetsia kalkulu berriarekin gainerako ahalegina zereginean. Eguneratzen honek zereginaren aurreikuspena amaitutakoan, garapenaren ehunekoa eta zeregin baten proiektatutako ahaleginaren bariantza berriro kalkulatzea eragiten du. Laburpen zereginetan EAC, ETC eta garapenaren ehunekoa ere berriro kalkulatzen dira eta ahaleginaren bariantzaren proiekzio berri bat sortzen dute.

## <a name="reprojection-of-effort-on-summary-tasks"></a>Laburpen-zereginetan ahalegina berriro proiektatzea

Laburpen-zereginetan edo edukitzaile-zereginetan ahalegina berriro proiektatu daiteke. Proiektuen kudeatzaileek laburpen zereginetan gainerako ahalegina egunera dezakete. Gainerako ahalegina eguneratzeak honako kalkulu multzoa eragiten du aplikazioan:

- Zeregineko EAC eta garapenaren ehunekoa kalkulatzen dira.
- EAC berria bigarren mailako zereginetan banatzen da jatorrizko zereginean zegoen EAC proportzio berean.
- Hosto-nodoen zereginetara jaitsitako zeregin indibidualetako EAC berria kalkulatzen da. 
- Berriro kalkulatzen dira hosto-nodoetan kaltetutako bigarren mailako zereginen geratzen den ahaleginaren balioa eta garapenaren portzentajea EAC balioaren arabera. Horrek zereginaren ahaleginaren bariantzarako beste proiekzio bat sortzen du. 
- Erro-nodora bideratutako laburpen-zereginen EAC-ak berriro kalkulatzen dira.


## <a name="project-status-summary"></a>Proiektuaren egoeraren laburpena

**Ahaleginen jarraipena** eta **Kostuen jarraipena** ikuspegietako datuen jarraipenak proiektuaren erro-nodoaren, laburpen-zereginaren eta hosto-nodoaren zereginen mailan egondako garapena eta kostuen kontsumoa erakusten dute. **Egoera** atalak, **Proiektuaren entitatea** orrialdeakoak, proiektu-mailaren egoeraren laburpena erakusten du.

## <a name="status-summary-fields"></a>Egoeraren laburpen-eremuak

**Proiektuaren egoera orokorra** eremua editagarria den eremua da, eta proiektuaren egoera orokorra erakusten du. Kolore bidezko kodeketa erabiltzen du, hala nola berdea, horia eta gorria, arriskua handitzen dela adierazteko. **Oharrak** eremuak proiektu-kudeatzaileari egoerari buruzko iruzkin zehatzak sartzen uzten dio. **Egoera eguneratu da** eremua ez da editagarria eta balioa egoera azkenekoz noiz eguneratu zen adierazten duen denbora-zigilua da.

**Antolaketaren errendimendua** eta **Kostuen errendimendua** eremuak jarraipen-datatik ezartzen dira. Erro-nodoaren antolaketa eta kostuaren bariantza positiboak direnean **Ahaleginaren jarraipena** ikuspegian, eremu horiek **Aurreratua** gisa ezar ditzakezu. Erro-nukleoaren antolaketa eta kostuaren bariantza negatiboak direnean, **Atzeratuta** gisa ezar ditzakezu.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
