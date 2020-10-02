---
title: Konfiguratu fakturak automatikoko sortzeko aukera
description: Gai honek beroari buruzko informazioa eskaintzen du, fakturak automatikoki sortzeko sistema konfiguratzeko.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 764fd4568619e4f5676ee3cbf7fce14ffb069548
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898111"
---
# <a name="configure-automated-invoice-creation"></a>Konfiguratu fakturak automatikoko sortzeko aukera

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Bete urrats hauek Project eragiketetan faktura automatikoa exekutatzeko.

1. Joan **Ezarpenak** \> **Lan sortak** atalera.
2. Sortu lan-sortat eta eman izen hau: **Project eragiketek fakturak sortzea**. Lan-sortaren izenak "Sortu fakturak" terminoa izan behar du.
3. **Lan mota** eremuan, hautatu **Bat ere ez** aukera. Berez, **Maiztasuna egunero** eta **Aktibatuta dago** aukerak ezarrita daude **Bai** aukerarekin.
4. Hautatu **Lan-fluxua exekutatu**. **Begiratu erregistroa** elkarrizketa-koadroan, hiru lan-fluxu ikusiko dituzu:

    - ProcessRunCaller
    - ProcessRunner
    - UpdateRoleUtilization

5. Hautatu **ProcessRunCaller** eta gero hautatu **Gehitu**.
6. Berrespenaren hurrengo elkarrizketa-koadroan, hautatu **Ados**. **Lo** lan-fluxuaren ondoren dator **Prozesua** lan-fluxua.

    Aukeratu ere egin dezakezu **ProcessRunner** 5. urratsean. Ondoren, hautatzen duzunean **Ados** aukera, **Prozesua** lan-fluxuaren ondoren dator **Lo** lan-fluxua.

**ProcessRunCaller** eta **ProcessRunner** lan-fluxuek fakturak sortzen dituzte. **ProcessRunCaller** lan-fluxuak **ProcessRunner** lan-fluxuari deitzen dio. **ProcessRunner** fakturak benetan sortzen dituen lan-fluxua da. Fakturak sortu behar diren kontraturen lerro guztietatik igarotzen da eta fakturak sortzen ditu lerro horietarako. Fakturak eratu behar diren kontratuaren lerroak zehazteko, lanpostuak kontratuaren lerroen fakturazio datak aztertzen ditu. Kontratu bakarreko kontratuaren lerroek fakturaren iraupen-data bera badute, transakzioak bi faktura-lerro dituen faktura batean elkartzen dira. Fakturak sortzeko transakziorik ez badago, lanak fakturaren sorrera saltatzen du.

**ProcessRunner** exekutatzen amaitu denean, **ProcessRunCaller** lan-fluxuari deitzen dio, amaiera-ordua ematen du eta itxita dago. **ProcessRunCaller** lan-fluxuak, ondoren, zehaztutako amaiera-ordutik 24 orduz iraungo duen tenporizadorea hasten du. Tenporizadorearen amaieran, **ProcessRunCaller** lan-fluxua itxita dago.

Lan-sortaren prozesua lan errepikaria da. Prozesu-sorta hau askotan exekutatzen bada, lanaren zenbait kasu sortzen dira eta akatsak sor daitezke. Hori dela eta, prozesu-sorta behin bakarrik hasi beharko zenuke eta exekutatzen gelditzen bada bakarrik berrabiarazi beharko zenuke.

> [!NOTE]
> Sortako fakturazioa fakturen egutegien arabera konfiguratutako proiektuen kontratu lerroetarako bakarrik exekutatzen da. Prezio finkoko fakturazio metodoa duen kontratu-lerroak mugarriak konfiguratu behar ditu. Ordua eta materiala fakturatzeko metodoa duen proiektu-kontratuen lerroak fakturen egitaraua finkatuko du. Gauza bera gertatzen da proiektuan oinarritutako kontratu lerroan.     
