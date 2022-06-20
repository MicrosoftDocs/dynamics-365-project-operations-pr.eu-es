---
title: Sari Federalen kontsulten gastuen egutegia
description: Artikulu honek Sari Federalen Kontsultaren Gastuen Egitarauari buruzko informazioa eskaintzen du.
author: velofog
ms.date: 04/2/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: PSNProjSEFAinquiry
audience: Application User
ms.devlang: ''
ms.reviewer: johnmichalak
ms.tgt_pltfrm: ''
ms.custom: ''
ms.search.region: Global
ms.search.industry: public sector
ms.author: andchoi
ms.search.validFrom: 2020-4-01
ms.dyn365.ops.version: 10.0.11
ms.openlocfilehash: 00f9e97b9a6b3e8fe5e9cf9143e670612869b84c
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8916641"
---
# <a name="schedule-of-expenditures-of-federal-awards-inquiry"></a>Sari Federalen kontsulten gastuen egutegia

[!include [banner](../includes/banner.md)]

A-133 Bulegoko Kudeaketa eta Aurrekontuen Zirkularrak dioenez, funts federalak jasotzen dituzten agentziek ikuskaritza-eskakizunak betetzen dituzte, auditoria bakarra izenarekin ere ezagutzen direnak. Ikuskaritza prozesua beka federalen sarreren eta gastuen berri emateko erabiltzen da behin eta berriz. Ikuskaritza txosten bakarraren zati batek Sari Federalen Gastuen Egitaraua (SEFA) barne hartzen du.

Sari Federalen Gastuen Ordutegiak kontsultak barne hartzen ditu Etxe Laguntza Federalaren Katalogoa (CFDA) izenburua eta zenbakia, diru-laguntzaren zenbakia, diru-laguntzaren urtea, funtsak ematen dituen agentzia federalaren izena eta txartelaren izena. entitatearen bidez. Kontsulta epe zehatz baterako da. Normalean, epe hori finantza egoeraren aldiaren berdina da, hau da, urte fiskal.

Kontsultak hautatutako data tartean proiekzio datak dituzten laguntzak biltzen ditu. **Laguntzailea** kontsultaren zutabean, bekaren bezeroa edo, igarotako beka lortzeko, agentzia emailea agertzen da. Diru-laguntza emateko, **Pass-through agentzia** zutabeak beka bezeroa erakusten du. Diru-laguntza ematen ez bada, **Pass-through agentzia** zutabea hutsik geratuko da.

## <a name="set-up-the-cfda-clusters"></a>Konfiguratu CFDA klusterrak

CFDA zenbakiekin lotu daitezkeen CFDA klusterrak konfiguratu behar dituzu Sari Federalen Gastuen Egutegia kontsultan.

1. Joan **Proiektuen kudeaketa eta kontabilitatea\> Konfigurazioa\> Diru-laguntzak\> Barne Laguntza Federaleko klusterren katalogoa**.
2. Hautatu **Berria** CFDA klusterra sortzeko.
3. Idatzi klusterraren izena.
4. Aldaketak gordetzeko, sakatu **Gorde**.

## <a name="set-up-cfda-numbers"></a>Konfiguratu CFDA zenbakiak

CFDA zenbakiekin lotu daitezkeen CFDA klusterrak diru-laguntzetan gehi daitezke eta konfiguratu behar dituzu Sari Federalen Gastuen Egutegia kontsultan.

1. Joan **Proiektuen kudeaketa eta kontabilitatea \> Konfigurazioa \> Diru-laguntzak \> Barne Laguntza Federaleko zenbakien katalogoa**.
2. Hautatu **Berria** CFDA zenbaki bat sortzeko.
3. **Zenbakia** zutabean, idatzi CFDA zenbakia.
4. Sakatu **Fitxa** gakoa.
5. **Azalpena** zutabean, idatzi CFDA izenburua.
6. Sakatu **Fitxa** gakoa.
7. Aukerakoa: **Programa klusterra** eremuan, gehitu dagokion CFDA klusterra.
8. Aldaketak gordetzeko, sakatu **Gorde**.

## <a name="set-up-grants-to-report-for-the-schedule-of-expenditures-of-federal-awards-inquiry"></a>Ezarri diru-laguntzak Sari Federalen Gastuen Egutegia kontsultatzeko

1. Joan **Proiektuen kudeaketa eta kontabilitatea \> Diru-laguntzak \> Diru-laguntzak**, eta hautatu lehendik dagoen dirulaguntza.
2. **Konfigurazioa** FastTab fitxategian **Barne Laguntza Federalaren Katalogoa** eremuan, esleitu CFDA zenbakia. Bekaren CFDA zenbakiak CFDA klusterra zehazten du txostenak egiteko.
3. **Harremanetarako informazioa** FastTab-en, idatzi emailearen informazioa urrats hauek jarraituz:

    1. **Eman bezeroari** eremuan, sartu bekaren erantzule den bezeroa. Lehendik dagoen beka baterako, baliteke informazio hori jada sartzea.
    2. Adierazi bekaren bezeroa finantzatzailea den. Bekaren bezeroa finantzatzailea bada, utzi **Pasabidea** kontrol laukia garbitu da. Beste bezero bat finantzatzailea bada, eta diru-laguntza bezeroa dirua gastatzeaz eta jarraitzeaz arduratzen bada, hautatu **Pasabidea** kontrol-laukia.

4. Aukeratu baduzu **Pasabidea** markatu aurreko urratseko kontrol laukia **Laguntzailea** eremuan, idatzi beka eman duen bezeroa. Laguntza-agentzia eta beka-bezeroa ezin dira bezero bera izan.

Hona hemen igarotako beka baten adibidea:

Gobernu federalak estatu baterako azpiegitura proiektua finantzatu zuen. Gobernu federalak dirua eman zion estatuari gastatzeko. Kasu honetan, gobernu federala da laguntza-agentzia, eta estatua beka-bezeroa da.

> [!NOTE] 
> Ezaugarria lehen aldiz aktibatzen duzunean, hasierako CFDA zenbakiak diru-laguntzetan dauden zenbakiak erabiliz sartuko dira.

## <a name="exclude-grants-from-sefa-reporting-based-on-the-grant-type"></a>Baztertu diru-laguntzak SEFA txostenetik diru-laguntza motaren arabera

1. Joan **Proiektuen kudeaketa eta kontabilitatea \> Konfigurazioa \> Diru-laguntzak \> Beka motak**.
2. **Informazio lehenetsia** FastTab-en, hautatu **Sari Federalen Gastuen Ordutegitik kanpo utzi** kontrol-laukia.
3. Aldaketak gordetzeko, sakatu **Gorde**.

## <a name="run-the-schedule-of-expenditures-of-federal-awards-inquiry"></a>Exekutatu Sari Federalen kontsulten gastuen egutegia

1. Joan **Proiektuen kudeaketa eta kontabilitatea \> Kontsultak eta txostenak \> Beka kontsulta \> Sari Federalen Gastuen Egitaraua**.
2. **Parametroak** sekzioan, ondorengo pausoak jarraitu:

    1. **Data tartea** eremuan, hautatu data tartearen kodea. Bestela, **Datatik aurrera** eta **Orain arte** eremuak, zehaztu data tartea.
    2. Aukerakoa: kontsultan diru-sarrera gisa fakturatutako transakzioak soilik sartzeko, ezarri **Sartu fakturatutako diru-sarrerak soilik** aukera **Bai**.

## <a name="columns"></a>Zutabeak

Sari Federalen Gastuen Ordutegiak kontsultak honako zutabe hauek ditu:

- Barne Laguntza Federalaren klusterren katalogoa
- Laguntzailea
- Pasabide-agentzia
- Eman izena
- Eman IDa
- Diru-laguntza eskaeraren IDa
- Barne Laguntza Federalaren katalogoa
- Agiriak
- Gastuak


[!INCLUDE[footer-include](../includes/footer-banner.md)]