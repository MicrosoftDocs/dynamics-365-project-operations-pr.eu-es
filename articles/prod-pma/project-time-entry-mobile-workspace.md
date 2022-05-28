---
title: Proiektuaren denbora sartzeko mugikorreko lan eremua
description: Gai hori emateko informazioa buruz Proiektuaren denbora-sarreran mugikorreko laneko area. Laneko espazio honi esker, erabiltzaileek proiektu baten aurka sartu eta denbora aurrez dezakete beren gailu mugikorra erabiliz.
author: Yowelle
ms.date: 12/01/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: johnmichalak
ms.custom: 272101
ms.assetid: 4505f021-b9bb-4b87-be24-6bf0bd88ee60
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: Version 1611
ms.search.validFrom: 2016-11-30
ms.openlocfilehash: 64a80d931332a4d6edfcd175d7168a7815ddca38
ms.sourcegitcommit: 2c2a5a11d446adec2f21030ab77a053d7e2da28e
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/04/2022
ms.locfileid: "8683891"
---
# <a name="project-time-entry-mobile-workspace"></a>Proiektuaren denbora sartzeko mugikorreko lan eremua

[!include [banner](../includes/banner.md)]

Gai horrek informazioa ematen du **Proiektuaren sarrerako ordua** buruz mugikorreko lan-eremua. Laneko espazio honi esker, erabiltzaileek proiektu baten aurka sartu eta denbora aurrez dezakete beren gailu mugikorra erabiliz.

Mugikorretarako lan-espazio hau Dynamics 365 Unified Ops mugikorretarako aplikazioarekin erabiltzeko pentsatuta dago. 

## <a name="overview"></a>Informazio orokorra
Eguneroko lanaren barruan, proiektuaren baliabideak tokian tokiko edo bidaiatzaileak izan ohi dira. **Proiektuaren denbora sarrera** mugikorreko lan-eremuak erabiltzaileei aukeratutako gailu mugikorrean fakturatzeko edo fakturaziorik gabeko denbora sartzeko aukera ematen die. Hori dela eta, proiektuaren baliabideek denbora-sarrerak noiznahi eta nonnahi grabatu ditzakete. Jadanik grabatutako denbora-sarrerak ere ikus ditzakete. 

Zehazki, **Proiektuaren denbora sarrera** mugikorreko laneko eremuan, erabiltzaileek zeregin hauek egin ditzakete:

-   Aukeratutako edozein datarako, sartu zeregin zehatz batean emandako ordu kopurua.
-   Bilatu proiektuaren izenaren edo bezeroaren arabera denbora sartzeko proiektua aurkitzeko.
-   Zehaztu igarotako denboraren kategoria eta jarduera.
-   Grabatu denbora proiektuaren fakturagarritzat edo ez fakturatzeko moduan.
-   Sar ezazu kanpoko edo barneko iruzkinak.

## <a name="prerequisites"></a>Aurrebaldintzak
Aurrebaldintzak desberdinak dira, bertsioaren arabera Microsoft Dynamics 365 zure erakundean inplementatu dena.

### <a name="prerequisites-if-you-use-dynamics-365-finance"></a>Dynamics 365 Finance erabiltzen baduzu aurrebaldintzak
Finantzak zure erakundean hedatu badira, sistemaren administratzaileak argitaratu beharko du **Proiektuaren denbora sarrera** mugikorreko lan eremua. Argibideak lortzeko, ikusi [Argitaratu mugikorreko lan eremua](/dynamics365/fin-ops-core/dev-itpro/mobile-apps/publish-mobile-workspace).

### <a name="prerequisites-if-you-use-version-1611-with-platform-update-3-or-later"></a>Aurrebaldintzak 1611 bertsioa Plataformako 3. eguneratzearekin edo berriagoarekin erabiltzen baduzu
Plataformaren 3. eguneratzearekin edo berriagoarekin 1611 bertsioa zure erakundean hedatu bada, sistemaren administratzaileak honako baldintza hauek bete beharko ditu. 

<table>
<thead>
<tr class="header">
<th>Aurrebaldintza</th>
<th>Funtzioa</th>
<th>Deskribapenak</th>
</tr>
</thead>
<tbody>
<tr class="odd">

<td>Ezarri KB 4018050.</td>
<td>Sistemaren administratzailea</td>
<td>KB 4018050 fitxategia duen X ++ eguneratze edo metadatuen zuzenketa zuzena da <strong>Proiektuaren denbora sarrera</strong> mugikorreko lan eremua. KB 4018050 ezartzeko, zure sistemaren administratzaileak urrats hauek jarraitu behar ditu.
<ol>
<li><a href="/dynamics365/fin-ops-core/dev-itpro/migration-upgrade/download-hotfix-lcs">Deskargatu metadatuen zuzenketa Microsoft Dynamics Lifecycle Services (LCS)</a>.</li>
<li><a href="/dynamics365/fin-ops-core/dev-itpro/migration-upgrade/install-metadata-hotfix-package">Instalatu metadatuen zuzenketa zuzena</a>.</li>
<li><a href="/dynamics365/fin-ops-core/dev-itpro/deployment/create-apply-deployable-package">Sortu pakete inplementagarri bat</a> horrek dauka <strong>ApplicationSuite</strong> eta <strong>ProjectMobile</strong> modeloak eta, ondoren, pakete inplementagarria LCS-ra igo.</li>
<li><a href="/dynamics365/fin-ops-core/dev-itpro/deployment/apply-deployable-package-system">Aplikatu pakete inplementagarria</a>.</li>

</ol></td>
</tr>
<tr class="even">
<td>Argitaratu <strong>Proiektuaren denbora-sarrera</strong> mugikorreko lan-eremua.</td>
<td>Sistemaren administratzailea</td>
<td>Ikusi <a href="/dynamics365/fin-ops-core/dev-itpro/mobile-apps/publish-mobile-workspace">Argitaratu mugikorreko lan eremua</a>.</td>
</tr>
</tbody>
</table>

## <a name="download-and-install-the-mobile-app"></a>Deskargatu eta instalatu mugikorreko aplikazioa

Deskargatu eta instalatu Finantza eta Operazioak mugikorreko aplikazioa:

-   [Hurrengorako Android telefonoak](https://go.microsoft.com/fwlink/?linkid=850662)
-   [iPhone-tarako](https://go.microsoft.com/fwlink/?linkid=850663)

## <a name="sign-in-to-the-mobile-app"></a>Saio hasi mugikorreko aplikazioa
1.  Hasi aplikazioa zure mugikorreko gailuan.
2.  Idatzi zure Dynamics 365 URL.
3.  Saioa hasten duzun lehen aldian, zure erabiltzaile izena eta pasahitza eskatuko zaizu. Idatzi kredentzialak.
4.  Saioa hasi ondoren, zure enpresarako erabilgarri dauden lan-eremuak agertzen dira. Kontuan izan zure sistemaren administratzaileak gero laneko espazio berri bat argitaratzen badu, mugikorretarako laneko espazioak berritu beharko dituzula.

[![Tira freskatzeko.](./media/pull-to-refresh-list-of-workspaces-183x300.png)](./media/pull-to-refresh-list-of-workspaces.png)

## <a name="enter-time-by-using-the-project-time-entry-mobile-workspace"></a>Idatzi denbora Project time entry mobile area erabilita
1.  Zure gailu mugikorrean, hautatu **Proiektuaren denbora sarrera** lan eremua.
2.  Hautatu **Denbora-sarrera**. Uneko asteko egutegiaren datak agertzen dira.
3.  Aukeratutako data baterako, hautatu **Ekintzak** &gt; **Sarrera berria**.
4.  Idatzi zenbakia orduena erregistratzeko.
5.  Aukeratu proiektua denbora sarrerako. Zerrenda batek zure aplikazioan konexiorik gabe erabiltzeko kargatutako proiektuak erakusten ditu. Berez, 50 elementu kargatzen dira, baina garatzaile batek zenbaki hori alda dezake. Informazio gehiagorako, ikusi [Mugikorreko plataforma](/dynamics365/fin-ops-core/dev-itpro/mobile-apps/mobile-app-home-page).
6.  Zure proiektua zerrendan ez badago, hautatu **Bilatu**. Bilatu izenaren arabera edo aldatu proiektuaren izenaren edo bezeroaren arabera.
7.  Hautatu kategoria bat. Zerrenda batek zure aplikazioan konexiorik gabe erabiltzeko kargatutako kategoriak erakusten ditu. Berez, 50 elementu kargatzen dira, baina garatzaile batek zenbaki hori alda dezake. Informazio gehiagorako, ikusi [Mugikorreko plataforma](/dynamics365/fin-ops-core/dev-itpro/mobile-apps/mobile-app-home-page).
8.  Zure kategoria zerrendan ez badago, hautatu **Bilatu**. Bilatu kategorien arabera edo aldatu bilaketa kategoriaren izenaren arabera.
9.  Hautatu jarduera. Zerrenda batek zure aplikazioan konexiorik gabe erabiltzeko kargatutako jarduerak erakusten ditu. Berez, 50 elementu kargatzen dira, baina garatzaile batek zenbaki hori alda dezake. Informazio gehiagorako, ikusi [Mugikorreko plataforma](/dynamics365/fin-ops-core/dev-itpro/mobile-apps/mobile-app-home-page).
10. Zure jarduera zerrendan ez badago, hautatu **Bilatu**. Bilatu jardueraren zenbakiaren arabera edo aldatu helburuaren arabera.

11. Aukeratu lerroaren jabetza.
12. Hautazkoa: Idatzi edozein kanpoko eta barneko iruzkinak.
13. Hautatu **Eginda**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]