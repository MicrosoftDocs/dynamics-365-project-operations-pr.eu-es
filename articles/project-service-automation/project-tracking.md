---
title: Proiektuen garapena eta kostuen kontsumoa
description: Gai honek proiektuaren garapenaren eta kostuen kontsumoaren jarraipena egiteari buruzko informazioa ematen du.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 0d742164-5469-421d-8917-63160a81f651
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8aa5814938129f30885d8161a7c86197ab013364
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748923"
---
# <a name="project-progress-and-cost-consumption"></a>Proiektuen garapena eta kostuen kontsumoa

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Antolaketa eta garapena jarraitzeko beharra aldatu egiten da industriaren arabera. Zenbait industriak jarraipen zehatza egiten du; beste batzuek, aldiz, jarraipen orokorragoa egiten dute. Gai honek erakundearen eskakizunak betetzeko nola antolatu behar den erakusten du.

## <a name="effort-tracking-view"></a>Ahaleginen segimenduaren ikuspegia

**Ahaleginen jarraipena** ikuspegiak antolaketako zereginen garapenaren jarraipena egiten du. Zeregin batean egin diren uneko ahalegin orduak eta zereginerako aurreikusitako esfortzu orduak konparatzen ditu. PSA-k honako formula hauek erabiltzen ditu jarraipen-neurriak kalkulatzeko:

- Garapenaren ehunekoa = Orain arte egindako egiazko ahalegina ÷ Zereginerako aurreikusitako ahalegina 
- Burutzeko estimazioa (ETC) = Aurreikusitako ahalegina - Orain arte egindako ahalegina 
- Burutzean egindako estimazioa (EAC) = Geratzen den ahalegina + Orain arte egindako ahalegina 
- Proiektatutako ahaleginaren bariantza = Aurreikusitako ahalegina - EAC

PSA-k zereginen bariantzaren bistaratzea erakusten du. EAC aurreikusitako ahalegina baino handiagoa bada, zereginak hasieran aurreikusitakoa baino denbora gehiago beharko duela aurreikusten da. Hori dela eta, atzeratuta dago. EAC aurreikusitako ahalegina baino txikiagoa bada, zereginak hasieran aurreikusitakoa baino denbora gutxiago beharko duela aurreikusten da. Hori dela eta, aurreratuta dago.

## <a name="re-projecting-effort"></a>Berriro proiektatzeko ahalegina

Ohikoa da proiektu-kudeatzaile batek zereginen jatorrizko kalkuluak berrikustea. Proiektuaren birproiekzioak proiektu-kudeatzaileak proiektuaren egungo egoera ikusita duen kalkuluen pertzepzioa da. Hala ere, ez dugu gomendatzen proiektu-kudeatzaileak oinarrizko zenbakiak aldatzea, proiektuaren oinarria baita proiektuaren antolaketaren eta kostuen ezarritako benetako jatorria eta proiektuko interes-talde guztiek onartu dute hori.

Proiektu-kudeatzaileak bi modutara birproiektatu ditzake zereginetako ahaleginak:

- Gainidatzi ETC lehenetsia zereginen benetako ahaleginaren beste kalkulu batekin. 
- Gainidatzi garapenaren ehuneko lehenetsia zereginen benetako garapenaren beste kalkulu batekin.

Planteamendu horietako bakoitzak zereginaren ETC, EAC eta garapenaren ehunekoa eta zeregin baten proiektatutako ahaleginaren bariantza berriro kalkulatzea eragiten du. Laburpen zereginetan EAC, ETC eta garapenaren ehunekoa ere berriro kalkulatzen dira eta ahaleginaren bariantzaren proiekzio berri bat sortzen dute.

## <a name="re-projection-of-effort-on-summary-tasks"></a>Laburpen-zereginetan ahalegina berriro proiektatzea

Laburpen-zereginetan edo edukitzaile-zereginetan ahalegina berriro proiektatu daiteke. Erabiltzaileak laburpen-zereginetan gelditzen den ahalegina edo garapenaren ehunekoa erabiliz birproiektatzen duen kontuan izan gabe, honako kalkulu multzoa hasten da:

- Zeregineko EAC, ETC eta garapenaren ehunekoa kalkulatzen dira.
- EAC berria bigarren mailako zereginetan banatzen da jatorrizko zereginean zegoen EAC proportzio berean.
- Hosto-nodoen zereginetara jaitsitako zeregin indibidualetako EAC berria kalkulatzen da. 
- Berriro kalkulatzen dira hosto-nodoetan kaltetutako bigarren mailako zereginen ETC balioa eta garapenaren portzentajea EAC balioaren arabera. Horrek zereginaren ahaleginaren bariantzarako beste proiekzio bat sortzen du. 
- Erro-nodora bideratutako laburpen-zereginen EAC-ak berriro kalkulatzen dira.

### <a name="cost-tracking-view"></a>Kostuen jarraipenaren ikuspegia 

**Kostuen jarraipena** ikuspegiak zeregin batean gastatu diren kostu errealak zeregin batean aurreikusitako kostuekin alderatzen ditu. 

> [!NOTE]
> Ikuspegi honek lan-kostuak bakarrik erakusten ditu eta ez ditu gastuen kalkuluko gastuak barne hartzen. 

PSA-k honako formula hauek erabiltzen ditu jarraipen-neurriak kalkulatzeko:

- Kontsumitutako kostuaren ehunekoa = Orain arte gastatutako kostua ÷ Zereginerako aurreikusitako kostua
- Burutzeko kostua (CTC) = Aurreikusitako kostua - Orain arte egindako kostua
- EAC = CTC + Orain arte gastatutako benetako kostua
- Proiektatutako kostuaren bariantza = Aurreikusitako kostua - EAC

Kostuaren bariantzaren proiekzioa erakusten da zereginean. EAC aurreikusitako kostua baino handiagoa bada, zereginak hasieran aurreikusitakoa baino kostu handiagoa beharko duela aurreikusten da. Beraz, aurrekontu gainditzeko joera erakusten du. EAC aurreikusitako kostua baino txikiagoa bada, zereginak hasieran aurreikusitakoa baino kostu txikiagoa beharko duela aurreikusten da. Beraz, aurrekontuaren azpitik gelditzeko joera erakusten du.

## <a name="project-managers-re-projection-of-cost"></a>Proiektu-kudeatzaileak egindako kostuaren birproiekzioa

Esfortzua berriro proiektatzen denean, CTC, EAC, kontsumitutako kostuaren ehunekoa eta proiektatutako kostuen bariantza berriro kalkulatuko dira **Kostuen jarraipena** ikuspegian.

## <a name="project-status-summary"></a>Proiektuaren egoeraren laburpena

**Ahaleginen jarraipena** eta **Kostuen jarraipena** ikuspegietako datuen jarraipenak proiektuaren erro-nodoaren, laburpen-zereginaren eta hosto-nodoaren zereginen mailan egondako garapena eta kostuen kontsumoa erakusten dute. **Egoera** atalak, **Proiektuaren entitatea** orrialdeakoak, proiektu-mailaren egoeraren laburpena erakusten du.

## <a name="status-summary-fields"></a>Egoeraren laburpen-eremuak

**Proiektuaren egoera orokorra** eremua editagarria den eremua da, eta proiektuaren egoera orokorra erakusten du. Kolore bidezko kodeketa erabiltzen du, hala nola berdea, horia eta gorria, arriskua handitzen dela adierazteko. **Oharrak** eremuak proiektu-kudeatzaileari egoerari buruzko iruzkin zehatzak sartzen uzten dio. **Egoera eguneratu da** eremua ez da editagarria eta balioa egoera azkenekoz noiz eguneratu zen adierazten duen denbora-zigilua da.

**Antolaketaren errendimendua** eta **Kostuen errendimendua** eremuak jarraipen-datatik ezartzen dira. Erro-nodoaren antolaketa eta kostuaren bariantza positiboak direnean **Ahaleginaren jarraipena** ikuspegian, eremu horiek **Aurreratua** gisa ezar ditzakezu. Erro-nukleoaren antolaketa eta kostuaren bariantza negatiboak direnean, **Atzeratuta** gisa ezar ditzakezu.
