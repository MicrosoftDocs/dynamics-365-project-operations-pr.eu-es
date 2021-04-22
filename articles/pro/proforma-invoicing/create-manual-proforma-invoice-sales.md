---
title: Proiektuko fakturen proforma
description: Gai honek Proforma proiektuaren fakturen inguruko informazioa eskaintzen du Project Operations-en.
author: rumant
manager: Annbe
ms.date: 04/06/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d08e2b0422a991aa4c98ae5d1e0f60aa0eb9daa6
ms.sourcegitcommit: ca0fc078d1a12484eca193fe051b8442c0559db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/07/2021
ms.locfileid: "5867161"
---
# <a name="proforma-project-pnvoices"></a>Proiektuko fakturen proforma

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proformako proiektu-fakturak fakturak egitea erabilgarria da proiektuen kudeatzaileei bigarren onespen maila ematen dielako bezeroei fakturak sortu aurretik. Lehen onarpen maila proiektuko kideek bidaltzen dituzten denbora-, gastu- eta material-sarrerak onartzen direnean amaitzen da.

Dynamics 365 Project Operations Lite Deployment ez dago bezeroari begira fakturak sortzeko diseinatuta. Ondorengo zerrendan fakturak zergatik ezin diren sortu erakusten da:

- Ez dauka zerga informaziorik.
- Ezin dira beste monetak fakturazio monetara bihurtu.
- Inprimatzeko fakturak ezin dira zuzen formateatu.

Horren ordez, finantza- edo kontabilitate-sistema erabil dezakezu sortutako fakturen proposamenetatik informazioa erabiltzen duten bezeroei zuzendutako fakturak sortzeko.

## <a name="creating-project-invoices"></a>Sortu proiektuaren fakturak

Proiektuen fakturak banan-banan edo guztiak batera sor daitezke. Eskuz sor ditzakezu edo lasterbide automatizatuetan sor daitezke.

### <a name="manually-create-project-invoices"></a>Eskuz sortutako proiektuaren fakturak 

**Proiektuen kontratuak** zerrenda-orrian, proiektu-fakturak banan-banan sor ditzakezu proiektu-kontratu bakoitzeko, edo fakturak denak batera sor ditzakezu hainbat proiekturako.

   - Proiektu-kontratu jakin baten faktura bat sortzeko, **Proiektuen kontratuak** zerrenda-orrian, ireki proiektu-kontratu bat eta hautatu **Sortu faktura**.

   Faktura sortzen da **Fakturatzeko prest** egoera daukaten hautatutako proiektu-kontratuaren transakzio guztientzat. Transakzio horien artean daude denbora, gastuak, materialak, mugarriak, produktuetan oinarritutako kontratu lerroak eta baieztatu daitezkeen fakturaziorik gabeko salmenta aldizkari lerroak.

Fakturak sortaka sortzeko:

1. **Proiektuen kontratuak** zerrenda-orrian, hautatu faktura bat sortu behar dituzun proiektu kontratu bat edo gehiago eta, ondoren, hautatu **Sortu proiektu-Fakturak**.
2. Abisu mezu batek fakturak sortu aurretik atzerapen bat egon daitekeela jakinarazten dizu. Prozesua ere erakusten da. Hautatu **Ados** mezu-koadroa ixteko.

   Faktura sortzen da **Fakturatzeko prest** egoera daukaten proiektu-kontratuaren transakzio guztientzat. Transakzio horien artean daude denbora, gastuak, materialak, mugarriak, produktuetan oinarritutako kontratu lerroak eta baieztatu daitezkeen fakturaziorik gabeko salmenta aldizkari lerroak.

3. Ikusi sortzen diren fakturak **Salmentak** \> **Fakturazioa** \> **Fakturak** atalean. Proiektu-kontratu bakoitzeko faktura bat ikusiko duzu.

### <a name="set-up-automated-creation-of-project-invoices"></a>Konfiguratu proiektu-fakturak automatikoki sortzea 

Jarraitu urrats hauei exekutatutako faktura automatikoa konfiguratzeko.

1. Joan **Ezarpenak** \> **Lan sortak** atalera.
2. Sortu lan-sortat eta eman izen hau: **Project eragiketek fakturak sortzea**. Lan-sortaren izenak "Fakturak sortu" terminoa izan behar du.
3. **Lan mota** eremuan, hautatu **Bat ere ez** aukera. Berez, **Maiztasuna egunero** eta **Aktibatuta dago** aukerak ezarrita daude **Bai** aukerarekin.
4. Hautatu **Lan-fluxua exekutatu**. **Begiratu erregistroa** elkarrizketa-koadroan, lan-fluxu hauek ikusiko dituzu:

    - ProcessRunCaller
    - Prozesuaren exekuzioak
    - Eguneratu funtzioen erabilera

5. Hautatu **ProcessRunCaller** eta gero hautatu **Gehitu**.
6. Berrespenaren hurrengo elkarrizketa-koadroan, hautatu **Ados**. **Lo** lan-fluxuaren ondoren dator **Prozesua** lan-fluxua.

    Aukeratu ere egin dezakezu **ProcessRunner** 5. urratsean. Ondoren, hautatzen duzunean **Ados** aukera, **Prozesua** lan-fluxuaren ondoren dator **Lo** lan-fluxua.

**ProcessRunCaller** eta **ProcessRunner** lan-fluxuek fakturak sortzen dituzte. **ProcessRunCaller** lan-fluxuak **ProcessRunner** lan-fluxuari deitzen dio. **ProcessRunner** fakturak sortzen dituen lan-fluxua da. Lan-fluxu hau fakturak sortu behar diren kontraturen lerro guztietatik igarotzen da eta fakturak sortzen ditu. Fakturak eratu behar diren kontratuaren lerroak zehazteko, lan-fluxuak kontratuaren lerroen fakturazio datak aztertzen ditu. Kontratu bakarreko kontratuaren lerroek fakturaren iraupen-data bera badute, transakzioak bi faktura-lerro dituen faktura batean elkartzen dira. Fakturak sortzeko transakziorik ez badago, ez da fakturarik sortzen.

**ProcessRunner** exekutatzen amaitu denean, **ProcessRunCaller** lan-fluxuari deitzen dio, amaiera-ordua ematen du eta itxita dago. **ProcessRunCaller** lan-fluxuak, ondoren, zehaztutako amaiera-ordutik 24 orduz iraungo duen tenporizadorea hasten du. Tenporizadorearen amaieran, **ProcessRunCaller** lan-fluxua itxita dago.

Lan-sortaren prozesua lan errepikaria da. Prozesu-sorta hau askotan exekutatzen bada, lanaren zenbait kasu sortzen dira eta akatsak sor daitezke. Arazokoak konpontzeko, hasi prozesu-sorta behin bakarrik eta exekutatzen gelditzen bada bakarrik berrabiarazi beharko zenuke.

> [!NOTE]
> Sortako fakturazioa fakturen egutegien arabera konfiguratutako proiektuen kontratu lerroetarako bakarrik exekutatzen da. Prezio finkoko fakturazio metodoa duen kontratu-lerroak mugarriak konfiguratu behar ditu. Ordua eta materiala fakturatzeko metodoa duen proiektu-kontratuen lerroak fakturen egitaraua finkatuko du. Gauza bera gertatzen da proiektuan oinarritutako kontratu lerroan.      
 
### <a name="edit-a-draft-invoice"></a>Editatu fakturaren zirriborroa

Proiektuen fakturaren zirriborroa sortzen duzunean, fakturazioan sartu behar dira denbora- eta gastu-sarrerak onartu zirenean sortu gabeko salmenta transakzio guztiak. Doikuntza hauek egin ditzakezu faktura oraindik zirriborro fasean dagoen bitartean:

- Ezabatu edo editatu fakturaren linearen xehetasunak.
- Editatu eta doitu kantitatea eta fakturazio mota.
- Fakturan transakzio gisa denbora, gastua, materiala eta tasak zuzenean gehitu. Ezaugarri hau erabil dezakezu faktura-lerroa transakzio-klase horiek baimentzen dituen kontratu-lerrora esleituta badago.

Aukeratu **Berretsi** faktura berresteko. Ekintza norabide bakarreko ekintza da. Hautatzen duzunean **Berretsi**, faktura irakurtzeko bakarrik egiten du eta fakturazioaren lineako xehetasunetatik fakturatutako salmenta errealak sortzen ditu. Fakturen linearen xehetasunak fakturatu gabeko salmenten benetako erreferentzia izanez gero, fakturatu gabeko salmenten benetako itzulketa egingo da. Denbora, gastu edo material erabileraren sarreratik sortutako faktura lerroaren xehetasunak fakturatu gabeko salmenten benetako erreferentzia izango du. Liburu nagusien integrazio sistemek alderantzikapen hori erabil dezakete egiten ari diren proiektuak (WIP) alderantzikatzeko kontabilitate helburuetarako.

### <a name="correct-a-confirmed-invoice"></a>Zuzendu berretsitako faktura

Berretsitako fakturak editatu daitezke. Berretsitako faktura zuzentzen duzunean, faktura zuzentzaileen zirriborro berria sortzen da. Jatorrizko fakturatik transakzio eta kantitate guztiak berraztertu nahi dituzulako hipotesiarekin, faktura zuzentzaile honek jatorrizko fakturaren transakzio guztiak barne hartzen ditu, eta bertan dauden kantitate guztiak 0 dira.

Transakzioren bat zuzentzen ez bada, faktura zuzentzailearen zirriborrotik kendu dezakezu. Kantitate partziala soilik alderantzikatu edo itzuli nahi baduzu, editatu dezakezu **Kopurua** eremuan, lerroaren xehetasunean. Fakturen lerroaren xehetasuna irekitzen baduzu, fakturaren jatorrizko kantitatea ikus dezakezu. Uneko fakturaren kantitatea editatu ahal izango duzu, fakturaren jatorrizko kantitatea baino gutxiago edo gehiago izan dadin.

Faktura zuzentzailea baieztatzen duzunean, fakturatutako jatorrizko salmenten benetakoa alderantzikatu egiten da eta fakturatutako salmenta erreal berria sortzen da. Kantitatea murriztuko balitz, aldaketak fakturatu gabeko salmenta berriak sortuko ditu. Adibidez, fakturatutako jatorrizko salmenta zortzi orduz izan bazenuen eta faktura zuzentzailearen linearen xehetasunak sei orduko kantitatera murriztu badu, jatorrizko fakturatutako salmenta-lerroa alderantzikatuko da eta bi berri sortuko dira:

- Fakturatutako salmentak sei orduz fakturatu dira.
- Bete gabeko salmentak benetako gainerako bi orduetan. Transakzio hau geroago fakturatu daiteke edo kargagabea izan daiteke, bezeroarekin izandako negoziazioen arabera.



[!INCLUDE[footer-include](../../includes/footer-banner.md)]
