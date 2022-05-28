---
title: Proformako fakturak
description: Gai honek Proformako fakturen inguruko informazioa eskaintzen du Project Operations-en.
author: rumant
ms.date: 04/05/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: e20ea17691c592493a790fb38451b35db03416be
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8600037"
---
# <a name="proforma-invoices"></a>Proformako fakturak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Proformako fakturak fakturak egitea erabilgarria da proiektuen kudeatzaileei bigarren onespen maila ematen dielako bezeroei fakturak sortu aurretik. Lehen onarpen maila proiektuko kideek bidaltzen dituzten denbora-, gastu- eta material-sarrerak onartzen direnean amaitzen da. Baieztatutako proforma fakturak eskuragarri daude Project Operations-en Proiektuen Kontabilitate moduluan. Proiektuaren kontulariek eguneratze osagarriak egin ditzakete, hala nola salmenten gaineko zerga, kontabilitatea eta fakturen diseinua.


## <a name="creating-project-invoices"></a>Sortu proiektuaren fakturak

Proiektuen fakturak banan-banan edo guztiak batera sor daitezke. Eskuz sor ditzakezu edo lasterbide automatizatuetan sor daitezke.

### <a name="manually-create-project-invoices"></a>Eskuz sortutako proiektuaren fakturak 

**Proiektuen kontratuak** zerrenda-orritik, proiektu-fakturak banan-banan sor ditzakezu proiektu-kontratu bakoitzeko, edo fakturak denak batera sor ditzakezu hainbat proiekturako.

Jarraitu urrats hau proiektu-kontratu jakin baterako faktura sortzeko.

- **Proiektuen kontratuak** zerrenda-orrian, ireki proiektu-kontratua eta ondoren hautatu **Sortu faktura**.

    Faktura sortzen da **Fakturatzeko prest** egoera daukaten hautatutako proiektu-kontratuaren transakzio guztientzat. Transakzio horien artean daude denbora, gastuak, materialak, mugarriak eta fakturatu gabeko beste salmenta aldizkari lerro batzuk.

Jarraitu urrats hauei fakturak denak batera sortzeko.

1. **Proiektuen kontratuak** zerrenda-orria, hautatu faktura bat sortu behar dituzun proiektu kontratu bat edo gehiago eta, ondoren, hautatu **Sortu proiektu-Fakturak**.

    Abisu mezu batek fakturak sortu aurretik atzerapen bat egon daitekeela jakinarazten dizu. Prozesua ere erakusten da.

2. Hautatu **Ados** mezu-koadroa ixteko.

    Faktura sortzen da **Fakturatzeko prest** egoera daukaten proiektu-kontratuaren transakzio guztientzat. Transakzio horien artean daude denbora, gastuak, materialak, mugarriak eta fakturatu gabeko beste salmenta aldizkari lerro batzuk.

3. Sortzen diren fakturak ikusteko, joan **Salmentak** \> **Fakturazioa** \> **Fakturak** atalera. Proiektu-kontratu bakoitzeko faktura bat ikusiko duzu.

### <a name="set-up-automated-creation-of-project-invoices"></a>Konfiguratu proiektu-fakturak automatikoki sortzea 

Jarraitu urrats hauei exekutatutako faktura automatikoa konfiguratzeko.

1. Joan **Ezarpenak** \> **Lan sortak** atalera.
2. Sortu lan-sortat eta eman izen hau: **Project eragiketek fakturak sortzea**. Lan-sortaren izenak "Fakturak sortu" terminoa izan behar du.
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
 
### <a name="edit-a-draft-invoice"></a>Editatu fakturaren zirriborroa

Proiektuen fakturaren zirriborroa sortzen duzunean, fakturazioan sartu behar dira denbora-, gastu- eta material erabileraren sarrerak onartu zirenean sortu gabeko salmenta transakzio guztiak. Doikuntza hauek egin ditzakezu faktura oraindik zirriborro fasean dagoen bitartean:

- Ezabatu edo editatu fakturaren linearen xehetasunak.
- Editatu eta doitu kantitatea eta fakturazio mota.

Aukeratu **Berretsi** faktura berresteko. Berretsi ekintza norabide bakarreko ekintza da. Hautatzen duzunean **Berretsi**, sistemak faktura irakurtzeko bakarrik egiten du eta fakturazioaren lineako xehetasunetatik fakturatutako salmenta errealak sortzen ditu. Fakturen linearen xehetasunak fakturatu gabeko salmenten benetako erreferentzia izanez gero, sistemak fakturatu gabeko salmenten benetako itzulketa ere itzuliko du. (Denbora- edo gastu-sarreratik sortu den edozein fakturaren lerroko xehetasunek fakturatu gabeko salmenten erreferentzia izango dute.) Liburu nagusiaren integrazio-sistemek berraztertze hau erabil dezakete martxan dagoen proiektuaren (WIP) alderantzizko kontabilitaterako.

> [!NOTE]
> Berretsitako proformako fakturak eta erlazionatutako erregistroak (adibidez, faktura lerroak eta faktura lerroaren xehetasunak) ezin dira editatu edo ezabatu. 

### <a name="correct-a-confirmed-invoice"></a>Zuzendu berretsitako faktura

Berretsitako fakturak editatu daitezke (zuzenduta). Berretsitako faktura zuzentzen duzunean, faktura zuzentzaileen zirriborro berria sortzen da. Jatorrizko fakturatik transakzio eta kantitate guztiak berraztertu nahi dituzulako hipotesiarekin, faktura zuzentzaile honek jatorrizko fakturaren transakzio guztiak barne hartzen ditu, eta bertan dauden kantitate guztiak 0 (zero) dira.

Transakzioren bat zuzentzen ez bada, faktura zuzentzailearen zirriborrotik kendu dezakezu. Kantitate partziala soilik alderantzikatu edo itzuli nahi baduzu, editatu dezakezu **Kopurua** eremuan, lerroaren xehetasunean. Fakturen lerroaren xehetasuna irekitzen baduzu, fakturaren jatorrizko kantitatea ikus dezakezu. Uneko fakturaren kantitatea editatu ahal izango duzu, fakturaren jatorrizko kantitatea baino gutxiago edo gehiago izan dadin.

Faktura zuzentzailea baieztatzen duzunean, fakturatutako jatorrizko salmenten benetakoa alderantzikatu egiten da eta fakturatutako salmenta erreal berria sortzen da. Kantitatea murriztuko balitz, aldaketak fakturatu gabeko salmenta berriak ere sortuko ditu. Adibidez, fakturatutako jatorrizko salmenta zortzi orduz izan bazenuen eta faktura zuzentzailearen linearen xehetasunak sei orduko kantitatera murriztu badu, jatorrizko fakturatutako salmenta-lerroa alderantzikatuko da eta bi berri sortuko dira:

- Fakturatutako salmentak sei orduz fakturatu dira.
- Bete gabeko salmentak benetako gainerako bi orduetan. Transakzio hau beranduago fakturatu daiteke edo kargagabea izan daiteke, bezeroarekin izandako negoziazioen arabera.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
