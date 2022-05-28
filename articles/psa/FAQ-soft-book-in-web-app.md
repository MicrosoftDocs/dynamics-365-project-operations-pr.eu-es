---
title: Nola egin dezaket "erreserba leuna" baliabideetan 2.x aplikazioaren bertsioan?
description: Artikulu honetan azaltzen nola soft liburua proiektua taldekideak Project Service batekin.
author: JohnPBurrows
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: 472529c146fbb5e7a4540676c880cabd4ab1a32b
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8585179"
---
# <a name="how-do-i-soft-book-resources-in-the-web-app-project-service-app-v2x"></a>Nola egin dezaket "soft liburua" baliabideak aplikazioko web aplikazioa (Project Service aplikazioa v2.x)?

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1.x-2.x](../includes/cc-applies-to-psa-app-1x-2x.md)]

Antolatu tentatively edo "soft liburua" baliabide taldeak proiektua erakusteko inprimatu nahi baliabidea proiektua bat esleitu. Soft bookings ez darabil baliabide baten ahalmena erabilgarri. Soft erreserbatuta taldeko kideak ezin zaizkie objektuak esleitu proiektua zereginak. Egoera Disko Erreserbatuta eta Mota Committed Commit baliabideak soilik zereginak (assuming nahikoa disko erreserbatu ordu esleipena ahalegina estaltzen duten) bati eslei dakizkioke.

Soft erreserbatuta proiektua taldekideak erakutsi Taldeko Kide saretan lanorduekin beren soft erreserbatuta Soft Liburua zutabean agertzen dena. Horiek ere adieraztea antolaketa board atalean. Berriro, ez dute ahalmena consumption edozein adierazteko soft erreserbatu baliabide baten ahalmena darabil ez du.

Hiru era daude soft liburua Project Service bertsio proiektua inprimatu taldearen kide 2.x. Soft liburua dezakezu antolaketa board, batekin baliatu Mantentzen Bookings edo lehenespenez sortu baliabide orokorra. Metodo horiek azpiko deskribatzen dira.

## <a name="soft-book-with-the-schedule-board"></a>Soft-honekin antolaketa board liburua

Soft-liburu antolaketa board honekin jarraitu prozedura honetan: 
1. Ireki antolaketa-panela.
2. Hautatu Proiektua fitxa Erreserba-eskakizunak panelaren antolaketa-panelaren behealdean.
3. Aurkitu nahi duzun soft liburua baliabide atalean proiektua. Hainbat projects baduzu, sakatu Proiektua zutabe-goiburuan eta ondoren erabili iragazkia proiektua zure bilatzeko.
4. Proiektuan, sakatu ondoren, arrastatu eta ezabatu baliabideen ordua sareta atalean.
5. Bertan irekitzen du Baliabide Booking Sortu eskuineko panela. Doitzeko hasiera- eta amaiera-data, hautatu Booking Egoera Soft gisa eta ezarri ordutan. 
6. Sakatu Liburuan.
7. Berriro, proiektuan lanean baliabidea orain erakutsiko Soft Liburua zutabean soft booked lanorduekin taldearen kide gisa.

Kontuan izan ezin diozu ahal izateko, lan-diren kanpaina-xehatzea egitura (WBS) zereginak baliabide disko izan behar bezala esleitu nahi dizkiozun taldea atalean erreserbatuta.

## <a name="soft-book-using-the-maintain-bookings-feature"></a>Soft-liburua Mantentzen Bookings eginbidea erabiliz

Erreserba leuna Mantendu erreserbarekin prozedura honi jarraitzen dio:
1. Taldearen kide saretan, Sakatu Berria.
2. Hautatu batetik /, bookable baliabide-funtzioak.
3. Hautatu esleipen bat metodoa bat Ere ez:
- Ahalmen osoa
- Ehuneko ahalmena
- Orduka, banatu modu uniformean
- Orduka, ordainketa goiztiarra
4. Sakatu Gorde. Ikusiko duzu, baliabide taldeak sareta eta orduak haien Disko gisa adierazita.
5. Mantendu baliabideen bookings Mantentzen Bookings sakatuz.
6. Antolaketa board irekitzen duenean, zabaldu baliabide bookings beren erakusteko. Ikusiko duzu, erreserbatu Disko gisa adierazita.
7. Aldatu Egoera atalean erreserbatu, egin klik eskuineko botoiarekin, hautatu Liburua Soft eta Soft ondoren. Erreserba-egoera Leuna da.
8. Itxi ostean antolaketa board, ikusiko duzu duzun baliabide-orduak aldatu Disko batetik Soft taldearen kide saretan.
Duzun disko baliabide taldearen inprimatu erreserbatutako eta, ondoren, esleitu ahal izateko, WBS, erabiltzean zereginak mantentzen bookings aldatu Disko egoera Soft oharra, bertan esleipenetan, ataletik ezabatuko baliabidearen, zereginak erreserbatuta baliabideak disko soilik eslei t gisa galdetuko.

## <a name="soft-book-by-creating-a-generic-resource"></a>Soft-orokorra baliabide sortuz liburua

Orokorra baliabide taldearen kide sortzeko, antolaketa board edo Baliabide-Eskaera osatu eta mota aldatuz gero, erreserbatu zehar soft erreserbatu bat sor dezakezu.
Hori egiteko, erabili prozedura hau:

1. Proiektuan WBS, lanean esleitu funtzioak zereginak orokorra taldekideak-sortu nahi duzun.
2. Sakatu Sortu proiektu-taldea.
3. Proiektua taldearen kide saretan, hautatu baliabidea orokorra eta sakatu Liburua.
4. Antolaketa-board, hautatu nahi duzun erreserbatutako baliabidea.
5. Sortu Baliabideen Booking antolaketa board panelean, atalean aldatu Booking Egoera Soft.
6. Sakatu Liburua edo Liburua eta Irten.

Itxi ostean antolaketa board, ikusiko duzu, hautatutako baliabideen lanorduekin Soft erreserbatuta taldera gehitu, lehendabizi esleitutako ordu. Ere ikusiko duzu den baliabide orokorra egoerarik taldearen atalean soft erreserbatuta taldearen kide zereginak esleituta dauden adierazle gisa.

Erreserbatuta disko taldearen kide soft erreserbatuta taldearen kide baliabide aldatzeko zereginak esleitu ahal izateko prest zaudenean, ondokoa egin:

1. Baliabidearen hautatu eta sakatu Bookings Mantentzeko.
2. Antolaketa board irekitzen duenean, zabaldu baliabide bookings beren erakusteko. Ikusiko duzu, erreserbatu Soft gisa ezarrita.
3. Aldatu Egoera atalean erreserbatu, egin klik eskuineko botoiarekin, hautatu Liburua Gogorra eta Gogorra ondoren. Erreserba-egoera Gogorra da.
4. Itxi ostean antolaketa board, ikusiko duzu duzun baliabide-orduak aldatu Disko batetik Gogorra taldearen kide saretan. Baliteke orain esleitzen baliabidea zereginak (emandako erreserbatuta disko ordu eta esleipena zereginaren ahalegina ordu arteko lerrokatzea da). Oharra duzun duzu ondoren elementu #3. urratsak, baliabide orokorra fulfilment urratsak disko, soft erreserbatuta bookable baliabidea egoera aldatzen duzunean, orokorra taldeko kide da kendu taldetik.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
