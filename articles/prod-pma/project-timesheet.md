---
title: Proiektuaren orrialde mugikorretarako aplikazioa
description: Artikulu honek honi buruzko informazioa eskaintzen du Microsoft Dynamics 365 Project Timesheet mugikorretarako aplikazioa. Project Timesheet aplikazio mugikorrak erabiltzaileei gailu mugikorrean proiektuen fitxak aurkezteko eta onartzeko aukera ematen die.
author: abruer
ms.date: 06/29/2022
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: johnmichalak
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 10
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 730ed36841d07df60e8a8f343126209f0edcc593
ms.sourcegitcommit: 5c971b15295046b3c92ff6638dd1352129f1c390
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 07/01/2022
ms.locfileid: "9110960"
---
# <a name="project-timesheet-mobile-application"></a>Proiektuaren orrialde mugikorretarako aplikazioa

[!include [banner](../includes/banner.md)]

## <a name="overview"></a>Informazio orokorra

The Microsoft Dynamics 365 Project Timesheet mugikorretarako aplikazioak erabiltzaileei gailu mugikorrean (iPhone edo Android). Mugikorretarako aplikazio honek Dynamics 365 Finance proiektuaren kudeaketa eta kontabilitate eremuan dagoen denbora-orriaren funtzionaltasuna azaleratzen du. Erabiltzaileen produktibitatea eta eraginkortasuna hobetzen laguntzen du, eta proiektuen kronogramak garaiz sartzea eta onartzea ahalbidetzen du.

## <a name="download-and-install-the-mobile-app"></a>Deskargatu eta instalatu mugikorreko aplikazioa

Deskargatu eta instalatu Microsoft Dynamics 365 Project Timesheet mugikorretarako aplikazioa Android edo iPhone gailuko mugikor dendatik.

## <a name="enable-the-app"></a>Gaitu aplikazioa 

Finantzetan, Project Timesheet mugikorretarako aplikazioa gaituta egon behar da. Funtzionalitatea gaitzeko, joan hona: **Proiektuen kudeaketa eta kontabilitate parametroak \> Denbora-orria** eta hautatu **Gaitu Microsoft Dynamics 365 Project Timesheet** parametroa.

### <a name="resolve-sign-in-issues"></a>Ebatzi saioa hasteko arazoak

**Arazoa:** Project Timesheet Mobile aplikazioan saioa hastean, erabiltzaileek errore-mezu bat jasotzen dute, non "aplikaziora ezin dutela sartu" esaten duena.2bc50526-cdc3-4e36-a970-c284c34cbd6e maizter horretan.

**Arazoa:** Project Timesheet Mobile aplikazioan saioa hastean, erabiltzaileek adibide hauetako baten antza duen errore bat jasotzen dute:

- "AADSTS50020: identitate-hornitzailearen '[erabiltzaile izena]' erabiltzaile-kontua'https://sts.windows.net/ [aplikazioaren id]' ez dago maizterrean '[errente ID]' eta ezin da atzitu maizter horretako '[app id]' aplikaziora."
- "Hautatutako erabiltzaile-kontua ez dago maizterrean '[errente ID]' eta ezin da atzitu maizter horretako '[app id]' aplikaziora."

**Azalpena:** Arazo hauek egindako aldaketa batek eragindakoak dira Azure Active Directory (Azure AD) 2022ko maiatzean eta kanpoko erabiltzaileei lotuta dago. Aldaketa hau finantza- eta eragiketa-aplikazioetan egin ez denez, plataformaren edo aplikazioaren edozein bertsiotako bezeroei eragin diezaieke.

**Konponketa:** Kanpoko erabiltzaile guztiak maizterra gonbidatu behar dira bidez Azure AD. Informazio gehiagorako, ikus [Gonbidatu erabiltzaileak Azure Active Directory B2B lankidetza](/power-platform/admin/invite-users-azure-active-directory-b2b-collaboration).

## <a name="sign-in-to-the-app"></a>Saio hasi aplikazioa

1.  Hasi aplikazioa zure mugikorreko gailuan.

2.  Idatzi zure finantza URL-a.

3.  Saioa hasten duzun lehen aldian, zure erabiltzaile izena eta pasahitza eskatuko zaizu. Idatzi kredentzialak.

4. Zure enpresa lehenetsian saioa hasiko zara.

## <a name="submit-a-project-timesheet"></a>Bidali proiektuaren fitxa

Proiektuaren denbora-orria sortu eta bidali dezakezu aplikazioan. Denbora-orri berri bat aurreko orri bateko informazioan, gordetako lerroetan edo proiektuen esleipenetan oinarritu dezakezu. Ordezkari gisa izendatuta bazaude, beste langile baten ordu-orria ere sar dezakezu. Ordezkari gisa ordu-orria sortzeko, hautatu **Menua** botoia eta, ondoren, hautatu baliabide-izen bat.

Denbora-orriaren orriak ordu-orrialderako denbora-orri berria sortuko du, uneko datan oinarrituta. Lan-astea bistaratuko da. Denbora-orriaren epeak hainbat aste hartzen baditu, laneko beste aste bat hauta dezakezu laneko asteko fitxetan.
Uneko dataren ordu orria badago, bistaratuko da. Denbora-orri berri bat denbora-orri desberdin batean sortu behar baduzu, hautatu **Menua** botoia eta hautatu **Ordutegi berria**.

Proiektuaren informazioa sar dezakezu klik eginez **Gehitu denbora** ekintza edo **Kopiatu denbora** ekintza. **Kopiatu denbora** ekintzak proiektuaren lerroaren informazioa kopiatuko du, baina ez orduak. **Kopiatu denbora** menuak aukera hauek ditu:

- **Kopiatu lehendik dagoen ordu-orritik** - Kopiatu denbora-orriaren lerroak lehendik dagoen ordu-orri batetik.

- **Kopiatu gogokoenetik** - Sortu denbora-orriaren lerro berriak gogoko gisa hautatu dituzun ordu-orrien ezarpenak erabiliz.

- **Kopiatu zereginetik** - Sortu ordu-lerro berriak esleitutako proiektuetatik.

Bistaratzen den proiektuaren informazioa fitxategian definitu dituzun parametro mugikorren menpe dago **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea.

**Pertsona juridikoa** eremuan, hautatu proiektuko lana burutu duzun pertsona juridikoa. **Pertsona juridikoa** eremua eskuragarri dago enpresen arteko orri orriaren laguntza gaituta badago zure entitate juridikoarentzat.

Aukeratu proiektuarekin lotutako bezeroa denbora-orriarentzat. Hasierako oharra egiteko Android, bezeroaren sarrera ez da onartzen, lehenik proiektua hautatu behar baituzu. Lehenengo proiektua hautatu baduzu, **Bezeroa** eremua automatikoki betetzen da.

urtean **Proiektua** eremuan, hautatu denbora sartzen ari zaren proiektua. **Bezeroa** eremua automatikoki betetzen da.

Bezeroen eta proiektuen bilaketek bezeroen eta proiektuen artean bilaketak egitea ahalbidetzen dute.

Aukeratu informazioa **Kategoria**, **Jarduera**, **Linearen jabetza**, **Salmenten gaineko zerga taldea**, eta **Artikuluen salmenten gaineko zergaren taldea** eremuak behar bezala. Eremu hauek gainidatz daitezke.

**Linearen jabetza** eremuak balio lehenetsia ezarriko du, proiektuaren kudeaketa eta kontabilitate parametroetan oinarrituta. Proiektu / kategoria eta kategoria / baliabide parametroak gaituta daudenean, **Linearen jabetza** balioa baliozkotze honetarako definitu duzun balio lehenetsian ezarriko da. Proiektu/kategoria eta kategoria/baliabide parametroak gaituta ez daudenean, **Lerroaren jabetza** balioa lehenetsiko da **Gaitu lerro-propietate lehenetsia** eremuan **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea. **Linearen jabetza** balioa gainidatz daiteke.

Aukeratu egun bat denbora gehitzeko. Idatzi egunero lan egin duzun ordu kopurua.

Sartzen ari zaren orduei buruzko iruzkinak gehitzeko, egin klik **Gehitu iruzkinak**, eta, ondoren, sartu iruzkinak barne-audientzia baterako, bezero-publiko baterako edo bietarako.
Barne iruzkinak proiektuaren arduradunek ikusi ahal izango dituzte. Bezeroen iruzkinak fakturetan daude.

Lerroa gogoko gisa gordetzeko, hautatu kontrol laukia eta egin klik **Gorde gogoko gisa**.

Finantza-dimentsioa eta eranskinen laguntza ez daude mugikorreko aplikazioan.

Jarrai ezazu proiektuaren lerroak gehitzen zure denbora-orria osatzeko behar duzun moduan.

Egin klik **Bidali** denbora-orria onarpen-lanera bidaltzeko.

## <a name="review-timesheets"></a>Berrikusi denbora-orriak

Berrikusi behar diren ordu-orrien zerrenda eskuragarri dago menuan. Aukera hau lan-fluxuen onartzaile izendatu zaituztenean bakarrik dago erabilgarri. Goiburukoa eta lineako onarpena onartzen dira. Linea maila onartzeak onartzeko lerro bat edo gehiago markatzeko aukera eskaintzen du. Ordutegiaren informazioa berrikusi ondoren, egin klik **Onartu**, **Ordezkaria**, edo **Itzuli** lan-fluxuarekin jarraitzeko.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
