---
title: Proiektuaren salmenten jarraipena
description: Gai honek Project Operations-en proiektu bateko lan-sarreren aurka nola aurreratzen duten jakiteko informazioa eskaintzen du.
author: rumant
ms.date: 03/24/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 78d7bdaf9f5ca1757273cb81a1303befb0357ba547eb354097786fc3c38962b9
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6995566"
---
# <a name="project-sales-tracking"></a>Proiektuaren salmenten jarraipena

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations eskulanaren kalkuluen eta diru-sarreren jarraipena egiten du proiektuaren planeko eskakizun txikienean. Lan-sarreren kalkulua aurreikusitako ahaleginean eta proiektuaren planeko hosto nodo zeregin bakoitzari esleitutako baliabide generiko edo izendatuetan oinarritzen da. Proiektua hasten denean eta jendea proiektuko hainbat zereginen denboraren berri ematen hasten denean, lanaren benetako diru-sarrerak laburbiltzen dira eta horrek proiekzioen kalkulua hasten du.

## <a name="labor-revenue-tracking-view"></a>Laneko diru-sarreraren segimenduaren ikuspegia

**Proiektuak** orrialdean, **Jarraipena** fitxa, hauta dezakezu **Jarraipena** > **Kostua** irekitzeko **Kostuen jarraipena** ikuspegia. Edo, hauta dezakezu **Erabilera** > **Faktura-tasa** irekitzeko **Diru sarreren jarraipena** ikuspegia, proiektuaren planeko zeregin bakoitzaren lan sarreren aurrerapena erakusten duena. Ikuspegi honek zeregin batean gastatutako benetako lan-sarrerak zereginaren aurreikusitako lan-sarrerekin alderatzen ditu. Project Operations-ek formula hauek erabiltzen ditu lan-sarreren metrikak kalkulatzeko:

- **Aurreikusitako diru-sarrerak**: Hosto nodo zeregin bakoitzean baliabideen esleipen guztien salmenten balio estimatuak
- **Benetako diru-sarrerak**: Zereginean erregistratutako denboraren fakturaziorik gabeko salmenten guztizkoaren batura
- **Diru-sarreren% fakturagarria**: Benetako diru-sarrerak ÷ Diru-sarreren kalkulua amaitutakoan
- **Geratzen den dirud-sarrera**: Benetako aurreikuspena amaitutakoan - Benetako diru-sarrera
- **Aurreikusitako diru-sarrera amaitutakoan**: Geratzen den diru-sarrera + benetako diru-sarrera
- **Diru-sarreraren aldaera**: Aurreikusitako diru-sarrera - Kalkulatutako diru-sarrera amaitutakoan


> [!NOTE]
> Project Operations-ek laneko diru sarrerak soilik erakusten dituzte **Proiektua** orrialdean **Jarraipena** fitxa. Kontsumorako materialak eta gastuak kalkula eta jarrai daitezkeen arren, diru-sarrera horiek ez dira sartu **Jarraipena** fitxa. Fitxa hau laneko diru-sarrerak berriro proiektatzeko ahalegina berriro proiektatzeko diseinatuta dago.  
> Erakutsitako diru-sarrera guztiak proiektuaren kostu monetara bihurtzen dira. Proiektuaren kostu moneta proiektuan kontratatzeko unitatearen moneta da. Prezio finkoetarako, diru sarreren kopuruak **Lan-sarreren jarraipena** Ikuspegiak ez dira garrantzitsuak fakturatu gabeko salmenten datuak ez baitira denbora onartzen denean erregistratzen.
> Urtean erakusten diren salmenten balio estimatuak **Estimazioa** proiektuaren fitxak ezingo du aurreikusitako diru sarreren balioa gehitu **Jarraipena** fitxa. Desadostasun horren iturria bi arrazoi posibleengatik da:
><ol>
   ><li> <b>Aurrekontuak</b> fitxak salmenten monetan kalkulatutako diru-sarrerak erakusten ditu, eta <b>Jarraipena</b> fitxa kostuaren monetara bihurtutako aurreikusitako diru-sarrerak erakusten ditu. </li>
   ><li> Aurreikusitako salmentak kontratuan moneta bihurtzen direnean <b>Aurrekontuak</b> fitxan, proiektuaren monetara, bihurketak zehaztasun galera ekar dezaketen urratsak dakartza: </li>
><ol>
><li> Kontratuaren monetako salmenten zenbatekoa oinarrizko monetara bihurtzen da lehenik (1 bihurketa).</li>
><li> Oinarri-monetako salmenten zenbatekoa proiektuaren kostu-monetara bihurtzen da lehenik (2 bihurketa). </li>
></ol>
></ol>
> Moneta zehaztasuna bi urratsetan aplikatzen da, eta, ondorioz, proiektuaren monetan aurreikusitako diru-sarreren desbideraketa kontratuko monetan aurreikusitako salmentekiko.
   

## <a name="reprojecting-revenues-on-leaf-node-tasks"></a>Hosto nodoko zereginetan diru sarrerak berriro proiektatzea

Hosto nodoko zeregin bateko laneko diru-sarrerak ezin dira zuzenean berriro proiektatu **Jarraipena** fitxan **Proiektua** orrialdea. Hala ere, erabil dezakezu **Esfortzuaren jarraipena** zeregin batean geratzen den ahalegina berriro proiektatzeko. Horrek zereginean geratzen diren diru sarreren birkalkulatzea eragiten du. Jarraian hau nola funtzionatzen duen deskribatzen da.

1. Proiektu kudeatzaile batek zereginetan ahalegina berriro proiektatu dezake **Gainerako ahalegina** eremuaren kalkulu berriarekin gainerako ahalegina zereginean. Berriro proiektatzeak zereginaren ahaleginaren aurreikuspena amaitutakoan, garapenaren ehunekoa eta zeregin baten proiektatutako ahaleginaren bariantza berriro kalkulatzea eragiten du. EAC, kalkulua amaitutkoan (ETC) eta garapenaren ehunekoa ere berriro kalkulatzen dira eta ahaleginaren bariantzaren proiekzio berri bat sortzen dute.
2. Atazan geratzen den esfortzuaren balio berrian oinarrituta, sistemak gainerako sarrerak kalkulatzen ditu **Diru sarreren jarraipena** ikuspegia. Gainerako diru-sarrerak gainerako ahaleginaren arabera kalkulatzeko, sistemak lehenik eta behin zereginaren orduko batez besteko diru-sarrerak kalkulatzen ditu aurreikusitako diru-sarrera edo aurreikusitako ahalegin gisa. Aurreikusitako diru-sarrerak zeregineko baliabide-esleipen guztien diru-sarreren batura da. Orduko batez besteko diru-sarrerak atazan proiektatu berri den gainerako ahaleginaren gainerako diru-sarrerak kalkulatzeko erabiltzen da.
3. Hosto nodoaren zereginean zenbatetsitako diru-sarrerak eta diru-sarreren kontsumoaren ehunekoa berriro kalkulatzen dira.
4. Erro-nodora bideratutako laburpen-zereginen Amaitutakoan diru-sarreraren balioak berriro kalkulatzen dira.

## <a name="reprojecting-revenues-on-summary-tasks"></a>Laburpen-zereginetan diru sarrerak berriro proiektatzea

Laneko diru-sarrerak laburbildu edo edukiontzien zereginetan berriro proiekta ditzakezu. Alabaina, zuzenean birproiekta ditzakezu lanaren diru-sarrerak laburpen-proiektuaren zeregin batean **Jarraipena** fitxan **Proiektua** orrialdean. Hosto-nodoen zereginen antzera, laburpena eta edukiontzien zereginak birproiektatzeko erabil dezakezu **Esfortzuaren jarraipena** ikuspegia. Ikuspegi honetan, gainerako ahalegina laburpen-zeregin batean berriro proiekta dezakezu, laburpen-zereginean gainerako diru-sarreren birkalkulazioa eginez. Jarraian hau nola funtzionatzen duen deskribatzen da.

1. Proiektu kudeatzaile batek zereginetan ahalegina berriro proiektatu dezake **Gainerako ahalegina** eremuaren kalkulu berriarekin **Gainerako ahalegina** zereginean. Berriro proiektatzeak zereginaren aurreikuspena amaitutakoan, garapenaren ehunekoa eta zeregin baten proiektatutako ahaleginaren bariantza berriro kalkulatzea eragiten du. Laburpen zereginetan EAC, ETC eta garapenaren ehunekoa ere berriro kalkulatzen dira eta ahaleginaren bariantzaren proiekzio berri bat sortzen dute.
2. Atazan **Geratzen den esfortzua** eremuaren balio berrian oinarrituta, sistemak gainerako sarrerak kalkulatzen ditu **Diru-sarreren jarraipena** ikuspegia. Gainerako diru-sarrerak gainerako ahaleginaren arabera kalkulatzeko, sistemak lehenik eta behin zereginaren orduko batez besteko diru-sarrerak kalkulatzen ditu aurreikusitako diru-sarrera edo aurreikusitako ahalegin gisa. Aurreikusitako diru-sarrerak zeregineko baliabide-esleipen guztien diru-sarreren batura da. Orduko batez besteko diru-sarrerak atazan proiektatu berri den gainerako ahaleginaren diru-sarrerak kalkulatzeko erabiltzen da.
3. Laburpen-zereginean zenbatetsitako diru-sarrerak eta diru-sarreren kontsumoaren ehunekoak berriro kalkulatzen dira.
4. Amaitutako estimatutako diru-sarreren balio berria haurren zereginetara banatzen da, aurreikusitako diru-sarrerak zereginean zeuden proportzio berean.
5. Banako zeregin bakoitzaren aurreikusitako diru-sarrera amaitutakoan zereginetara jaitsitako zeregin berria kalkulatzen da. Balio horretan oinarrituta, kaltetutako seme-alabek hosto-nodoetaraino egiten dituzten atazek gainerako sarrera eta diru-sarreren kontsumoaren ehunekoa birkalkulatuko dute balio osoko diru-sarreren arabera. Horrek zereginaren diru-sarreraren bariantzarako beste proiekzio bat sortzen du. 
6. Erro-nodora bideratutako laburpen-zereginen Amaitutakoan diru-sarreraren balioak berriro kalkulatzen dira.


[!INCLUDE[footer-include](../includes/footer-banner.md)]

