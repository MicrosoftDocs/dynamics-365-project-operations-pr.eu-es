---
title: Proiektuaren kostuaren segimendua
description: Gai honek Project Operations-en proiektu bateko lanaren kostuaren eta gastuaren aurka nola aurreratzen duten jakiteko informazioa eskaintzen du.
author: rumant
ms.date: 03/22/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: f724ee29728a363c58ed0e69087f4c18be89ea2d
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8591435"
---
# <a name="labor-cost-tracking-on-projects"></a>Proiektuetako lan-kostuen segimendua

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations eskulanaren kalkuluen eta gastuaren jarraipena egiten du proiektuaren planeko eskakizun txikienean. Lanaren kostuaren kalkulu finantzarioa aurreikusitako ahaleginean eta proiektuaren planeko hosto nodo zeregin bakoitzari esleitutako baliabide generiko edo izendatuetan oinarritzen da. Proiektua hasten denean eta jendea proiektuko hainbat zereginen denboraren berri ematen hasten denean, lanaren benetako gastuak laburbiltzen dira eta horrek proiekzioen kalkulua hasten du.

## <a name="labor-cost-tracking-view"></a>Lanaren kostuen jarraipenaren ikuspegia

**Proiektuak** orrialdean, **Jarraipena** fitxa, hauta dezakezu **Jarraipena** > **Kostua** irekitzeko **Kostuen jarraipena** ikusi eta ikusi lan bakoitzaren gastuaren aurrerapena proiektuaren planean. Ikuspegi honek zeregin batean gastatutako benetako lanaren kostuaren zereginaren aurreikusitako lanaren kostuarekin alderatzen ditu. Project Operations-ek formula hauek erabiltzen ditu lanaren kostuen metrikak kalkulatzeko:

- **Aurreikusitako kostua**: Hosto nodo zeregin bakoitzean baliabideen esleipen guztien salmenten kostu estimatuak
- **Benetako kostua**: Zereginean erregistratutako denboraren kostuaren guztizkoaren batura
- **Kostuen kontsumoaren ehunekoa**: Benetako kostua ÷ Kostuaren estimazioa amaitutakoan
- **Geratzen den kostua**: Kostuaren estimazioa amaitutakoan - Benetako kostua
- **Kostua amaitutakoan**: Geratzen den kostua + Benetako kostua
- **Kostuaren bariantza**: Aurreikusitako kostua - Kostuaren estimazioa amaitutakoan

Zeregin bakoitzak kostuaren bariantzaren proiekzioa erakusten du zereginean. Osatutako kostuaren aurrekontua aurreikusitako kostua baino handiagoa bada, zereginak aurrekontua gaindituko duela aurreikusten da. Osatutako kostuaren aurrekontua aurreikusitako kostua baino txikiagoa bada, zereginak aurrekontuaren azpitik amaituko dela aurreikusten da.

>[!NOTE]
> Project Operations-ek laneko kostuak soilik erakusten dituzte **Proiektua** orrialdean **Jarraipena** fitxa. Kontsumorako materialak eta gastuak kalkula eta jarrai daitezkeen arren, kostu horiek ez dira sartu **Jarraipena** fitxa. Fitxa hau laneko kostuak berriro proiektatzeko ahalegina berriro proiektatzeko diseinatuta dago.
Erakutsitako kostu kopuru guztiak proiektuaren kostuaren monetara bihurtzen dira kostuaren tasa zehazteko erabilitako proiektuaren kostuaren monetara. Proiektuaren kostu moneta proiektuan kontratatzeko unitatearen moneta da. Urtean erakusten diren kostuen balio estimatuak **Aurrekontuak** fitxan **Proiektua** orrialdeak agian ez du aurreikusitako kostua gehituko **Jarraipena** fitxa. Desadostasun horren arrazoia kalkulatutako kostua nola laburbiltzen den ezberdintasunengatik da **Aurrekontuak** sarearen eta aurreikusitako kostua nola kalkulatzen den **Jarraipena** sareta. 
>
> - **Aurrekontuen fitxa** kalkulatutako kostua prezioen zerrendako kostu tasaren moneta bera erabiliz kalkulatzen du. Orduan, prezio zerrendako monetan kalkulatutako kostua proiektuaren kostu monetan kalkulatutako kostu bihurtzen da. Proiektuaren monetan kalkulatutako kostua 2 hamartarrera biribilduta agertzen da. Bihurketa honen unean uneko moneta zehaztasuna ez da aplikatzen. 
> - **Jarraipena** fitxan, aurreikusitako kostuen kalkuluak zertxobait desberdina den kalkulu ordena jarraitzen du, moneta zehaztasuna bi etapatan aplikatzea eskatzen duena: 
   ><ol>
   ><li>Oinarri-monetako kostuaren zenbatekoa oinarrizko monetara bihurtzen da lehenik (1 bihurketa).</li>
   ><li>Oinarri-monetako kostuaren zenbatekoa proiektuaren kostu-monetara bihurtzen da lehenik (2 bihurketa). </li>
   ></ol>
   >Moneta zehaztasuna bi urratsetan aplikatzen da aurreikusitako kostua lortzeko (**Jarraipena** fitxa) zenbatetsitako kostutik (**Denbora mailakatua** ikuspegia **Aurrekontuak** fitxa). 
   
## <a name="reprojecting-costs-on-leaf-node-tasks"></a>Hosto nodoko zereginetan kostuak berriro proiektatzea

Hosto nodoko zeregin bateko laneko kostuak ezin dira zuzenean berriro proiektatu **Jarraipena** fitxan **Proiektua** orrialdea. Hala ere, erabil dezakezu **Esfortzuaren jarraipena** zeregin batean geratzen den ahalegina berriro proiektatzeko. Horrek zereginean geratzen diren kostuaren birkalkulatzea eragiten du. Jarraian hau nola funtzionatzen duen deskribatzen da.

1. Proiektu kudeatzaile batek zereginetan ahalegina berriro proiektatu dezake **Gainerako ahalegina** eremuaren kalkulu berriarekin gainerako ahalegina zereginean. Berriro proiektatzeak zereginaren ahaleginaren aurreikuspena amaitutakoan, garapenaren ehunekoa eta zeregin baten proiektatutako ahaleginaren bariantza berriro kalkulatzea eragiten du. EAC, kalkulua amaitutkoan (ETC) eta garapenaren ehunekoa ere berriro kalkulatzen dira eta ahaleginaren bariantzaren proiekzio berri bat sortzen dute.
2. Atazan geratzen den esfortzuaren balio berrian oinarrituta, sistemak gainerako kostuak kalkulatzen ditu **Kostuaren jarraipena** ikuspegia. Gainerako kostuak gainerako ahaleginaren arabera kalkulatzeko, sistemak lehenik eta behin zereginaren orduko batez besteko kostuak kalkulatzen ditu aurreikusitako kostua edo aurreikusitako ahalegin gisa. Aurreikusitako kostuak zeregineko baliabide-esleipen guztien kostuaren batura da. Orduko batez besteko kostuak atazan proiektatu berri den gainerako ahaleginaren gainerako kostuak kalkulatzeko erabiltzen da.
3. Hosto nodoaren zereginean kostuak eta kostuaren kontsumoaren ehunekoa berriro kalkulatzen dira.
4. Erro-nodora bideratutako laburpen-zereginen Amaitutakoan kostuaren balioak berriro kalkulatzen dira.

## <a name="reprojecting-costs-on-summary-tasks"></a>Laburpen-zereginetan kostuak berriro proiektatzea

Laneko kostuak laburbildu edo edukiontzien zereginetan berriro proiekta ditzakezu. Alabaina, zuzenean birproiekta ditzakezu lanaren kostuak laburpen-proiektuaren zeregin batean **Jarraipena** fitxan **Proiektua** orrialdean. Hosto-nodoen zereginen antzera, laburpena eta edukiontzien zereginak birproiektatzeko erabil dezakezu **Esfortzuaren jarraipena** ikuspegia. Ikuspegi honetan, gainerako ahalegina laburpen-zeregin batean berriro proiekta dezakezu, laburpen-zereginean gainerako kostuen birkalkulazioa eginez. Jarraian hau nola funtzionatzen duen deskribatzen da.

1. Proiektu kudeatzaile batek laburpen-zereginetan ahalegina berriro proiektatu dezake gainerako ahaleginaren kalkulu berriarekin gainerako ahalegina zereginean. Eguneratzen honek laburpen-zereginaren aurreikuspena amaitutakoan, garapenaren ehunekoa eta zeregin baten proiektatutako ahaleginaren bariantza berriro kalkulatzea eragiten du. Laburpen zereginetan EAC, ETC eta garapenaren ehunekoa ere berriro kalkulatzen dira eta ahaleginaren bariantzaren proiekzio berri bat sortzen dute.
2. Laburpen-zereginean geratzen den esfortzuaren balio berrian oinarrituta, sistemak gainerako kostuak kalkulatzen ditu **Kostuaren jarraipena** ikuspegia. Gainerako kostuak gainerako ahaleginaren arabera kalkulatzeko, sistemak lehenik eta behin laburpen-zereginaren orduko batez besteko kostuak kalkulatzen ditu aurreikusitako kostua edo aurreikusitako ahalegin gisa. Orduko batez besteko kostuak laburpen-atazan proiektatu berri den gainerako ahaleginaren gainerako kostuak kalkulatzeko erabiltzen da.
3. Laburpen-zereginean kostuak eta kostuaren kontsumoaren ehunekoa berriro kalkulatzen dira.
4. Amaitutako kostu berria haurren zereginetara banatzen da, aurreikusitako kostuak zereginean zeuden proportzio berean.
5. Banako zeregin bakoitzaren kostu berria amaitutakoan zereginetara jaitsitako zeregin berria kalkulatzen da. Balio horretan oinarrituta, kaltetutako seme-alabek hosto-nodoetaraino egiten dituzten atazek gainerako kostua eta kostuaren kontsumoaren ehunekoa birkalkulatuko dute balio osoko kostuaren arabera. Balio horrek zereginaren kostu-bariantzarako beste proiekzio bat sortzen du. 


**Kostuen errendimendua** eremua jarraipen datuetatik ezar daiteke. Fitxategian erro nodoaren kostuaren bariantza denean **Kostuen jarraipena** ikuspegia negatiboa da, eremu hau ezar dezakezu **Aurrekontuaren arabera**. Erro nodoaren kostu bariantza positiboa denean, balioa ezarri dezakezu **Aurrekontuaren gainetik**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
