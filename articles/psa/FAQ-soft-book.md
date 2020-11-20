---
title: Baliabidearen behin behineko erreserba
description: Gai honek erreserben proiektuaren taldekideek behin-behinean nola antolatu edo programatzeko informazioa eskaintzen du.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 9/25/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.app:
- ProjectOperations
ms.openlocfilehash: af71ff9d60e237a9d1379b3ccd4c0d5ffce411e4
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122193"
---
# <a name="soft-book-a-resource"></a>Baliabidearen behin behineko erreserba

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Antolatu tentatively edo "soft liburua" baliabide taldeak proiektua erakusteko inprimatu nahi baliabidea proiektua bat esleitu. Baliabide baten ahalmena erabilgarri ez darabil soft bookings eta soft erreserbatuta taldeko kideak proiektua zereginak esleitu. Hala ere, soft erreserbatu ez darabil baliabide baten ahalmena, delako dezakezu still "disko liburua" baliabide-zereginak beste epean bera. Baliabide generikoak ezin dira erreserbatu, eta erreserba bigunek ezin dute bete eskakizun bat baliabide generiko baterako.

Bigun erreserbatutako proiektuen taldekideak **Taldea** fitxan zerrendatzen dira **Proiektua** orrian, eta bere erreserba bigunak erakusten dira **Bigun erreserbatutako orduak** zutabean **Izena duten taldekideak** ikuspegian. Soft erreserbatuta taldeko kideak antolaketa-panela atalean ere zerrendatzen dira. Delako dira soft erreserbatuta, antolaketa-panelan ez ditu erakutsi horiek baliabide baten ahalmena consumption edozein. **Kontziliazioa** fitxan soft erreserbatuta ordua erakutsi ez, helbidera da erakutsiko **Hedatutako erreserbak** eremua **Kontziliazioa** fitxan aurki daiteke antolaketa-panela. 

Xede proiektuaren inprimatu taldearen kide soft erreserbatutako bi modu daude: zuzenean antolaketa-panelan edo **Taldeak** fitxan taldeko kideak gehituz. 

## <a name="soft-book-from-the-schedule-board"></a>Erreserba leuna antolaketa-paneletik
Jarraitu hurrengo pausoak baliabide bat Schedule boardetik liburu bat biguntzeko. 

1. Ireki antolaketa-panela fitxa eta gero **Erreserba-eskakizunak** panelaren hautatu **Proiektua** fitxa.
2. Aurkitu nahi duzun soft liburua baliabide atalean proiektua. Zerrendan proiektu ugari badaude, hautatu **Proiektua** zutabe goiburua eta, ondoren, erabili iragazkia proiektu bat edo gehiago bilatzeko.
3. Hautatu proiektuan, sakatu ondoren, arrastatu eta ezabatu baliabideen ordua sareta atalean.
5. **Sortu Baliabideen Erreserba** panelan, doitu hasiera eta amaiera data, ezarri **Erreserbaren egoera** egoeratik **Biguna** egoerara eta, ondoren, ezarri orduak. 
6. Sakatu **Liburua**. Proiektuan lanean baliabidea orain erakusten du, **Taldeak** fitxan baliabide gisa proiekturako. **Taldekidearen izena** ikuspegian ikusiko duzu **Erreserbatuta ordu bigunak** zutabean soft erreserbatuta ordu.

> [!NOTE]
> Orain esleitzea soft **Antolaketa** fitxan zereginak erreserbatuta. **Kontziliazioa** fitxan, baliabidea erakusten du zeregin beren esleipena erlazionatutako erreserbatu bat deficit **Kontziliazioa** fitxa soilik kontuan disko bookings gisa. Disko-liburuarekin baliabidea **Hedatutako erreserbak** funtzioa erabil dezakezu baliabideak esleipenetan aurka bookings disko deficit eliminate. Beharko duzu eskuz bertan behera uzteko, baliabide-soft erreserbatu **Mantendu erreserbak** erabiliz.

## <a name="soft-book-on-the-team-tab"></a>Taldeko fitxan liburua soft

**Taldea** fitxan zuzenean taldeko kideak gehitu ahal ditzakezu, eta ondoren, aldatu erreseben egoera **Irmoa** egoeratik **Biguna** egoerara **Mantendu egoerak** egoerarekin. Horrela taldearen kide gehitzean, hori da beti result erreserbatu disko bateko guztirako baldintza kopuruak metodoa bat ere **Ez** gisa hautatzen ez.

Metodo hau erabili behar izan dezake bete urrats hauek.

1. **Proiektua** orrialdean **Taldea** fitxan, egin klik **Berria** aukeran.
2. Hautatu baliabide erreserbagarria, funtzioa eta noiztik eta noiz arte datetatik.
3. Hautatu esleipen bat metodoa bat **Ere** ez:
4. Sakatu **Gorde**. Ikusiko duzu, baliabide taldeak sareta eta orduak haien **Erreserba irmoko orduen** zutabean.
5. Mantendu baliabideen bookings **Mantendu erreserbak** sakatuz.
6. Antolaketa-panela irekitzen duenean, zabaldu baliabide bookings beren erakusteko. Ikusiko duzu, erreserbatu **Irmoa** gisa adierazita.
7. **Aldatu egoera** atalean erreserbatu, egin klik eskuineko botoiarekin, hautatu **Erreserba biguna** \> **Biguna**. Erreserba-egoera **Biguna** da.
8. Itxi ostean antolaketa-panela, ikusiko duzu dela baliabidea ordu-izan mugitu **Erreserbatutako ordu irmoak** fitxategitik **Erreserbatutako ordu bigunak** saretan **Taldea** fitxan, **Izena duten taldekideak** ikuspegia aldi nahi duzunean.

> [!NOTE]
> Kontuan izan baliabide bat gogor erreserbatzen baduzu talde batean eta zereginak esleitzen badizkiozu antolaketan, **erreserbak mantentzen** dituzunean egoera **Irmotik** **Bigunera** aldatzeko, baliabidearen zeregin-esleipenak mantenduko dituzula. Hala ere, **Kontziliazioa** fitxan, baliabidea izango erreserbatu deficiency gisa bookings disko soilik salmentekin alderatzen dituzten analisietarako esleipenetan erreserba kontziliazioa duzunean hartzen dira. **Erreserba hedatua** baliabidea **Kontziliazioa** funtzioan erabil dezakezu baliabideak esleipenetan aurka bookings disko defizit kentzeko. Beharko duzu eskuz bertan behera uzteko, baliabide-soft erreserbatu **Mantendu erreserbak** erabiliz.

Erreserbatuta disko taldearen kide soft erreserbatuta taldearen kide baliabide aldatzeko zereginak esleitu ahal izateko prest zaudenean, ondokoa egin:

1. Antolaketa-panelean, zabaldu baliabide erreserbak beren erakusteko. Ikusiko duzu, erreserbatu **Biguna** gisa erakutsita.
2. **Aldatu Egoera** atalean erreserbatu, egin klik eskuineko botoiarekin, hautatu **Erreserba irmoa** \> **Irmoa**. Erreserba-egoera **Irmoa** da.
3. Antolaketa-panela itxi ostean, itzuli proiektura eta ireki **Taldea** fitxa, eta ikusiko duzu baliabideen orduak mugitu direla **Erreserbatutako ordu bigunak** zutabetik **Erreserbatutako ordu irmoetara** zutabera **Taldea** fitxan **Izena duten taldekideak** ikuspeagian. Baliabidea ez ikusiko duten zereginak esleitu erakutsiko erreserbatu defizita **Kontziliazioa** fitxan bookings beren orain dira disko gisa.

