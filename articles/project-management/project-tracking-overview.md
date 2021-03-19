---
title: Proiektuen jarraipenaren informazio orokorra
description: Gai honek proiektuaren garapenaren eta kostuen kontsumoaren jarraipena egiteari buruzko informazioa ematen du.
author: ruhercul
manager: AnnBe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 14094d603be2834dc66abff2ff1faf5e940b1ffa
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286593"
---
# <a name="project-tracking-overview"></a>Proiektuen jarraipenaren informazio orokorra

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Antolaketa eta garapena jarraitzeko beharra aldatu egiten da industriaren arabera. Zenbait industriak jarraipen zehatza egiten du; beste batzuek jarraipen orokorragoa egiten dute. Gai honek erakundearen eskakizunak betetzeko nola antolatu behar den erakusten du.

## <a name="effort-tracking-view"></a>Ahaleginen segimenduaren ikuspegia

**Esfortzuaren jarraipena** ikuspegia egutegiaren zereginen bilakaeraren jarraipena egiten du zeregin batean emandako benetako esfortzu-orduak atazaren aurreikusitako esfortzu-orduekin alderatuz. Dynamics 365 Project Operations-ek honako formula hauek erabiltzen ditu jarraipen-neurriak kalkulatzeko:

- **Garapenaren ehunekoa**: Orain arte egindako ahalegina ÷ Aurreikusitako kostua osatzen denerako (EAC) 
- **Burutzeko estimazioa (ETC)**: Aurreikusitako ahalegina - Orain arte egindako ahalegina 
- **EAC**: Geratzen den ahalegina + Orain arte egindako ahalegina 
- **Proiektatutako ahaleginaren bariantza**: Aurreikusitako ahalegina - EAC

Project Operations-ek zereginen bariantzaren bistaratzea erakusten du. EAC aurreikusitako ahalegina baino handiagoa bada, zereginak hasieran aurreikusitakoa baino denbora gehiago beharko duela aurreikusten da eta antolaketaren atzean dago. EAC aurreikusitako ahalegina baino gutxiago bada, zereginak hasieran aurreikusitakoa baino denbora gutxiago beharko duela aurreikusten da eta antolaketaren aurrean dago.

## <a name="reprojecting-effort"></a>Berriro proiektatzeko ahalegina

Proiektu-kudeatzaileek sarritan zereginen jatorrizko aurreikuspenak berrikusten dituzte. Proiektuaren birproiekzioak proiektu-kudeatzaileak proiektuaren egungo egoera ikusita duen kalkuluen pertzepzioa da. Hala ere, ez dugu gomendatzen proiektuen kudeatzaileek oinarrizko zenbakiak aldatzea. Proiektuaren oinarria denez proiektuaren antolaketaren eta kostuen ezarritako benetako jatorria eta proiektuko interes-talde guztiek onartu dute hori.

Proiektu-kudeatzaileak bi modutara birproiektatu ditzake zereginetako ahaleginak:

- Gainidatzi ETC lehenetsia zereginen benetako ahaleginaren beste kalkulu batekin. 
- Gainidatzi garapenaren ehuneko lehenetsia zereginen benetako garapenaren beste kalkulu batekin.

Ikuspegi bakoitzak zereginaren ETC, EAC, garapenaren ehunekoa eta zeregin baten proiektatutako ahaleginaren bariantza berriro kalkulatzea eragiten du. Laburpen zereginetan EAC, ETC eta garapenaren ehunekoa ere berriro kalkulatzen dira eta ahaleginaren bariantzaren proiekzio berri bat sortzen dute.

## <a name="reprojection-of-effort-on-summary-tasks"></a>Laburpen-zereginetan ahalegina berriro proiektatzea

Laburpen-zereginetan edo edukitzaile-zereginetan ahalegina berriro proiektatu daiteke. Erabiltzaileak laburpen-zereginetan gelditzen den ahalegina edo garapenaren ehunekoa erabiliz birproiektatzen duen kontuan izan gabe, honako kalkulu multzoa hasten da:

- Zeregineko EAC, ETC eta garapenaren ehunekoa kalkulatzen dira.
- EAC berria bigarren mailako zereginetan banatzen da jatorrizko zereginean zegoen EAC proportzio berean.
- Hosto-nodoen zereginetara jaitsitako zeregin indibidualetako EAC berria kalkulatzen da. 
- Berriro kalkulatzen dira hosto-nodoetan kaltetutako bigarren mailako zereginen ETC balioa eta garapenaren portzentajea EAC balioaren arabera. Horrek zereginaren ahaleginaren bariantzarako beste proiekzio bat sortzen du. 
- Erro-nodora bideratutako laburpen-zereginen EAC-ak berriro kalkulatzen dira.

### <a name="cost-tracking-view"></a>Kostuen jarraipenaren ikuspegia 

**Kostuen jarraipena** ikuspegiak zeregin batean gastatu diren kostu errealak zeregin batean aurreikusitako kostuekin alderatzen ditu. 

> [!NOTE]
> Ikuspegi honek lan-kostuak bakarrik erakusten ditu eta ez ditu gastuen kalkuluko gastuak barne hartzen. Project Operations-ek honako formula hauek erabiltzen ditu jarraipen-neurriak kalkulatzeko:

- **Kontsumitutako kostuaren ehunekoa**: Orain arte gastatutako kostua ÷ Aurreikusitako kostua osatzen denerako
- **Burutzeko kostua (CTC)**: Aurreikusitako kostua - Orain arte egindako kostua
- **EAC**: Geratzen den kostua + Unera arte gastatutako benetako kostua
- **Proiektatutako kostuaren bariantza**: Aurreikusitako kostua - EAC

Kostuaren bariantzaren proiekzioa erakusten da zereginean. EAC aurreikusitako kostua baino handiagoa bada, zereginak hasieran aurreikusitakoa baino kostu handiagoa beharko duela aurreikusten da. Beraz, aurrekontu gainditzeko joera erakusten du. EAC aurreikusitako kostua baino txikiagoa bada, zereginak hasieran aurreikusitakoa baino kostu txikiagoa beharko duela aurreikusten da. Beraz, aurrekontuaren azpitik gelditzeko joera erakusten du.

## <a name="project-managers-reprojection-of-cost"></a>Proiektu-kudeatzaileak egindako kostuaren birproiekzioa

Esfortzua berriro proiektatzen denean, CTC, EAC, kontsumitutako kostuaren ehunekoa eta proiektatutako kostuen bariantza berriro kalkulatuko dira **Kostuen jarraipena** ikuspegian.

## <a name="project-status-summary"></a>Proiektuaren egoeraren laburpena

**Ahaleginen jarraipena** eta **Kostuen jarraipena** ikuspegietako datuen jarraipenak proiektuaren erro-nodoaren, laburpen-zereginaren eta hosto-nodoaren zereginen mailan egondako garapena eta kostuen kontsumoa erakusten dute. **Egoera** atalak, **Proiektuaren entitatea** orrialdeakoak, proiektu-mailaren egoeraren laburpena erakusten du.

## <a name="status-summary-fields"></a>Egoeraren laburpen-eremuak

**Proiektuaren egoera orokorra** eremua editagarria den eremua da, eta proiektuaren egoera orokorra erakusten du. Kolore bidezko kodeketa erabiltzen du, hala nola berdea, horia eta gorria, arriskua handitzen dela adierazteko. **Oharrak** eremuak proiektu-kudeatzaileari egoerari buruzko iruzkin zehatzak sartzen uzten dio. **Egoera eguneratu da** eremua ez da editagarria eta balioa egoera azkenekoz noiz eguneratu zen adierazten duen denbora-zigilua da.

**Antolaketaren errendimendua** eta **Kostuen errendimendua** eremuak jarraipen-datatik ezartzen dira. Erro-nodoaren antolaketa eta kostuaren bariantza positiboak direnean **Ahaleginaren jarraipena** ikuspegian, eremu horiek **Aurreratua** gisa ezar ditzakezu. Erro-nukleoaren antolaketa eta kostuaren bariantza negatiboak direnean, **Atzeratuta** gisa ezar ditzakezu.


[!INCLUDE[footer-include](../includes/footer-banner.md)]