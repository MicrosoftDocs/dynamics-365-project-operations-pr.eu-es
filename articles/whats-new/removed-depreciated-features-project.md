---
title: Eginbide kendu edo zaharkituta daude Dynamics 365 Project Operations
description: Gai honek ezabatu diren edo kentzeko aurreikusita dauden eginbideak deskribatzen ditu Dynamics 365 Project Operations.
author: sigitac
ms.date: 03/16/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 61bb84b94274762636eb8532f09634db1109e969
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8601555"
---
# <a name="removed-or-deprecated-features-in-dynamics-365-project-operations"></a>Eginbide kendu edo zaharkituta daude Dynamics 365 Project Operations

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea eta produkzioan oinarritutako eszenatokien proiektuaren eragiketak_

Gai honek ezabatu diren edo kentzeko aurreikusita dauden eginbideak deskribatzen ditu Dynamics 365 Project Operations.

- *Kendu* eginbidea dagoeneko ez dago eskuragarri produktuan.
- *Zaharkitua* funtzioa ez dago garapen aktiboan eta baliteke etorkizuneko eguneratze batean ezabatzea.

Zerrenda honek zure planifikaziorako kentze eta amortizazio hauek kontuan hartzen lagunduko dizu.

> [!NOTE]
> Finantza eta Operazioen aplikazioetako objektuei buruzko informazio zehatza helbidean aurki daiteke [**Erreferentzia teknikoko txostenak**](/dynamics/s-e/global/axtechrefrep_61). Txosten hauen bertsio desberdinak konparatu ditzakezu Finantza eta Operazioen aplikazioen bertsio bakoitzean aldatu edo kendu diren objektuei buruz jakiteko.

## <a name="features-removed-or-deprecated-in-the-project-operations-march-2022-release"></a>Eginbideak kendu edo zaharkituta geratu dira Project Operations 2022ko martxoko bertsioan

### <a name="project-management-and-accounting-always-create-adjustment-transaction-parameter"></a>Proiektuen kudeaketa eta kontabilitatea "Sortu beti doikuntza transakzioa" parametroa

| &nbsp; | &nbsp; |
|--------|--------|
| **Deuseztatzeko / kentzeko arrazoia** | Egokitzapen-transakzioak behar dira auditoretza helburuetarako. Zaharkitu ondoren, parametro hau ezkutatu egingo da. Sistemak doikuntza-transakzioak sortuko ditu beti, parametroa ezarrita dagoenean une honetan egiten duen bezala **Bai**. |
| **Beste ezaugarri batek ordezkatu?** | No |
| **Kaltetutako produktu eremuak** | Aplikazioa |
| **Inplementazio-aukera** | Ekoizpen/hornitutako eszenatokietarako Proiektu Eragiketak |
| **Egoera** | Zaharkituta: 2023ko martxoaren 1erako, parametroa ezkutatuko dugu eta sistemaren portaera aldatuko dugu, doikuntza-transakzioak beti sortu daitezen. |

### <a name="project-management-and-accounting-use-adjustment-date-as-new-project-date-parameter"></a>Proiektuen kudeaketa eta kontabilitatea "Erabili doikuntza-data proiektuaren data berri gisa" parametroa

| &nbsp; | &nbsp; |
|--------|--------|
| **Deuseztatzeko / kentzeko arrazoia** | Parametro hau hasiera batean aldi fiskal bat ixten zenean doikuntzak egiteko erabili zen. Hala ere, jada ez da beharrezkoa, transakzioaren kontabilitate-data irekita dagoen epearen lehen datara alda daitekeelako, konfiguratuta badago. Proiektuaren data ez da aldatu behar, transakzioa gertatu zeneko data adierazten baitu. |
| **Beste ezaugarri batek ordezkatu?** | No |
| **Kaltetutako produktu eremuak** | Aplikazioa |
| **Inplementazio-aukera** | Ekoizpen/hornitutako eszenatokietarako Proiektu Eragiketak |
| **Egoera** | Zaharkituta: 2023ko martxoaren 1erako, parametroa ezkutatuko dugu eta sistemaren portaera aldatuko dugu, doikuntzetan proiektuaren data inoiz aldatu ez dadin. |

### <a name="resource-request-workflow-in-project-operations-for-stockedproduction-based-scenarios"></a>Baliabideak eskatzeko lan-fluxua Project Operations-en hornitutako/produkzioan oinarritutako eszenatokietarako

| &nbsp; | &nbsp; |
|--------|--------|
| **Deuseztatzeko / kentzeko arrazoia** | Zaharkituta dago erabilera eta transakzio bolumenaren mugak direlako. |
| **Beste ezaugarri batek ordezkatu?** | No |
| **Kaltetutako produktu eremuak** | Aplikazioa |
| **Inplementazio-aukera** | Ekoizpen/hornitutako eszenatokietarako Proiektu Eragiketak |
| **Egoera** | Zaharkituta: 2023ko martxoaren 1erako, proiekturako baliabideak eskatzeko aukera desgaituko dugu lan-fluxua erabiliz. |

### <a name="project-invoice-proposal-page-without-header-and-lines-views"></a>Proiektuaren faktura-proposamenaren orria Goiburua eta Lerroak ikuspegirik gabe

| &nbsp; | &nbsp; |
|--------|--------|
| **Deuseztatzeko / kentzeko arrazoia** | Zaharkituta geratu da orrialdearekin batera sartutako hobekuntzengatik **Erabili Proiektuaren faktura-proposamena eta fakturen egunkari-inprimakiak Goiburua eta Lerroak ikuspegiarekin** funtzio-gakoa. |
| **Beste ezaugarri batek ordezkatu?** | Yes |
| **Kaltetutako produktu eremuak** | Aplikazioa |
| **Inplementazio-aukera** | Ekoizpen/hornitutako eszenatokietarako Proiektu Eragiketak; Proiektuaren Eragiketak baliabide/hornitu gabeko eszenatokietarako |
| **Egoera** | Zaharkituta: 2023ko martxoaren 1erako, lehenago (oinarrizko) orria desaktibatu eta aktibatu egingo dugu.**Erabili Proiektuaren faktura-proposamena eta fakturen egunkari-inprimakiak Goiburua eta Lerroak ikuspegiarekin** funtzio-tekla lehenespenez. |

## <a name="features-removed-or-deprecated-in-the-project-operations-december-2021-release"></a>Eginbideak kendu edo zaharkituta geratu dira Project Operations 2021eko abenduko bertsioan

### <a name="collaboration-workspaces"></a>Lankidetzako lan guneak

[Sortu edo estekatu lankidetza lan-espazio bat (Proiektua)](/dynamicsax-2012/appuser-itpro/create-or-link-to-a-collaboration-workspace-project)

| &nbsp; | &nbsp; |
|--------|--------|
| **Deuseztatzeko / kentzeko arrazoia** | Zaharkituta dago erabilera txikia duelako. Baliabide edo hornituta ez dauden agertokietarako Project Operations erabiltzen duten bezeroek aprobetxa dezakete [Bulegoko taldeekin lankidetza](../project-management/collaboration-groups.md). |
| **Beste ezaugarri batek ordezkatu?** | No |
| **Kaltetutako produktu eremuak** | Aplikazioa  |
| **Inplementazio-aukera** | Ekoizpen/hornitutako eszenatokietarako Proiektu Eragiketak |
| **Egoera** | Zaharkituta: 2022ko abenduaren 1erako, Lankidetzako lan-eremuak ez onartzea aurreikusi dugu. |
