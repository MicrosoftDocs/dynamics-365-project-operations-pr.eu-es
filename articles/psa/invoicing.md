---
title: Fakturak egin Project Service Automation-en
description: Gai honek fakturak egiteari buruzko informazioa ematen du.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 08/03/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: f8107a660f9993c7b6a32d69047a81fb7e0abef8
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071100"
---
# <a name="invoicing-in-project-service-automation"></a>Fakturak egin Project Service Automation-en

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Dynamics 365 Project Service Automation-en fakturak egitea erabilgarria da proiektuen kudeatzaileei bigarren onespen maila ematen dielako bezeroei fakturak sortu aurretik. Lehen onarpen maila proiektuko kideek bidaltzen dituzten denbora- eta gastu-sarrerak onartzen direnean amaitzen da.

PSA ez dago diseinatuta bezeroaren aurrean fakturak sortzeko, arrazoi hauengatik:

- Ez du zerga informaziorik.
- Ezin ditu beste monetak fakturazio-moneta bihurtu behar bezala konfiguratutako kanbio-tasak erabiliz.
- Ezin ditu fakturak behar bezala formatu inprimatu ahal izateko.

Horren ordez, finantza- edo kontabilitate-sistema erabil dezakezu PSAn sortzen diren fakturen proposamenetatik informazioa erabiltzen duten bezeroei zuzendutako fakturak sortzeko.

## <a name="creating-project-invoices-in-psa"></a>Sortu proiektuaren fakturak PSAn

Proiektuen fakturak banan-banan edo guztiak batera sor daitezke. Eskuz sor ditzakezu edo lasterbide automatizatuetan sor daitezke.

### <a name="manually-create-project-invoices-in-psa"></a>Eskuz sortutako proiektuaren fakturak PSAn

**Proiektuen kontratuak** zerrenda-orritik, proiektu-fakturak banan-banan sor ditzakezu proiektu-kontratu bakoitzeko, edo fakturak denak batera sor ditzakezu hainbat proiekturako.

Jarraitu urrats hau proiektu-kontratu jakin baterako faktura sortzeko.

- **Proiektuen kontratuak** zerrenda-orrian, ireki proiektu-kontratua eta ondoren hautatu **Sortu faktura**.

    ![Proiektu-fakturak sortzea proiektu jakin bateko kontratuetarako](media/CreateProjectInvoicesOneByOne.png)

    Faktura sortzen da **Fakturatzeko prest** egoera daukaten hautatutako proiektu-kontratuaren transakzio guztientzat. Eragiketa horien artean, denbora, gastuak, mugak eta produktuetan oinarritutako kontratuaren lerroak daude.

Jarraitu urrats hauei fakturak denak batera sortzeko.

1. **Proiektuen kontratuak** zerrenda-orria, hautatu faktura bat sortu behar dituzun proiektu kontratu bat edo gehiago eta, ondoren, hautatu **Sortu proiektu-Fakturak**.

    ![Sortu proiektuaren fakturak denak batera](media/CreateProjectInvoicesBulk.png)

    Abisu mezu batek fakturak sortu aurretik atzerapen bat egon daitekeela jakinarazten dizu. Prozesua ere erakusten da.

2. Hautatu **Ados** mezu-koadroa ixteko.

    Faktura sortzen da **Fakturatzeko prest** egoera daukaten proiektu-kontratuaren transakzio guztientzat. Eragiketa horien artean, denbora, gastuak, mugak eta produktuetan oinarritutako kontratuaren lerroak daude.

3. Sortzen diren fakturak ikusteko, joan **Salmentak** \> **Fakturazioa** \> **Fakturak** atalera. Proiektu-kontratu bakoitzeko faktura bat ikusiko duzu.

### <a name="set-up-automated-creation-of-project-invoices-in-psa"></a>Konfiguratu proiektu-fakturak automatikoki sortzea PSAn

Jarraitu urrats hauei PSAn exekutatutako faktura automatikoa konfiguratzeko.

1. Joan **Project Service** \> **Ezarpenak** \> **Lan-sortak** atalera.
2. Sortu lan-sortat eta eman izen hau: **PSA fakturak sortu**. Lan-sortaren izenak "Fakturak sortu" terminoa izan behar du.
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
> Project Service Automation-en fakturazio sorta fakturen egutegien arabera konfiguratutako proiektuen kontratu lerroetarako bakarrik exekutatzen da. Prezio finkoko fakturazio metodoa duen kontratu-lerroak mugarriak konfiguratu behar ditu. Ordua eta materiala fakturatzeko metodoa duen proiektu-kontratuen lerroak fakturen egitaraua finkatuko du. Gaian agertzen da fakturazio-maiztasunak ezartzeko informazioa aurrekontu-lerro batean oinarritutako proiektuaren testuinguruan, [Aurrekontuak eta aurrekontu ildoak](basic-quote-lines.md#invoice-schedule). Gauza bera gertatzen da proiektuan oinarritutako kontratu lerroan.      
 
### <a name="edit-a-draft-psa-invoice"></a>Editatu PSAren fakturaren zirriborroa

Proiektuen fakturaren zirriborroa sortzen duzunean, fakturazioan sartu behar dira denbora- eta gastu-sarrerak onartu zirenean sortu gabeko salmenta transakzio guztiak. Doikuntza hauek egin ditzakezu faktura oraindik zirriborro fasean dagoen bitartean:

- Ezabatu edo editatu fakturaren linearen xehetasunak.
- Editatu eta doitu kantitatea eta fakturazio mota.
- Fakturan transakzio gisa denbora, gastua eta tasak zuzenean gehitu. Ezaugarri hau erabil dezakezu faktura-lerroa transakzio-klase horiek baimentzen dituen kontratu-lerrora esleituta badago.

Aukeratu **Berretsi** faktura berresteko. Berretsi ekintza norabide bakarreko ekintza da. Hautatzen duzunean **Berretsi** , sistemak faktura irakurtzeko bakarrik egiten du eta fakturazioaren lineako xehetasunetatik fakturatutako salmenta errealak sortzen ditu. Fakturen linearen xehetasunak fakturatu gabeko salmenten benetako erreferentzia izanez gero, sistemak fakturatu gabeko salmenten benetako itzulketa ere itzuliko du. (Denbora- edo gastu-sarreratik sortu den edozein fakturaren lerroko xehetasunek fakturatu gabeko salmenten erreferentzia izango dute.) Liburu nagusiaren integrazio-sistemek berraztertze hau erabil dezakete martxan dagoen proiektuaren (WIP) alderantzizko kontabilitaterako.

### <a name="correct-a-confirmed-psa-invoice"></a>Zuzendu berretsitako PSAren faktura

Berretsitako PSAren fakturak editatu daitezke (zuzenduta). Berretsitako faktura zuzentzen duzunean, faktura zuzentzaileen zirriborro berria sortzen da. Jatorrizko fakturatik transakzio eta kantitate guztiak berraztertu nahi dituzulako hipotesiarekin, faktura zuzentzaile honek jatorrizko fakturaren transakzio guztiak barne hartzen ditu, eta bertan dauden kantitate guztiak 0 (zero) dira.

Transakzioren bat zuzentzen ez bada, faktura zuzentzailearen zirriborrotik kendu dezakezu. Kantitate partziala soilik alderantzikatu edo itzuli nahi baduzu, editatu dezakezu **Kopurua** eremuan, lerroaren xehetasunean. Fakturen lerroaren xehetasuna irekitzen baduzu, fakturaren jatorrizko kantitatea ikus dezakezu. Uneko fakturaren kantitatea editatu ahal izango duzu, fakturaren jatorrizko kantitatea baino gutxiago edo gehiago izan dadin.

Faktura zuzentzailea baieztatzen duzunean, fakturatutako jatorrizko salmenten benetakoa alderantzikatu egiten da eta fakturatutako salmenta erreal berria sortzen da. Kantitatea murriztuko balitz, aldaketak fakturatu gabeko salmenta berriak ere sortuko ditu. Adibidez, fakturatutako jatorrizko salmentak zortzi orduz izan bazituen eta fakturaren zuzentzaileen linearen xehetasunak sei orduko kantitatera murriztu badu, PSAk jatorrizko fakturatutako salmenta-lerroa alderantzikatu eta bi berri sortzen ditu:

- Fakturatutako salmentak sei orduz fakturatu dira.
- Bete gabeko salmentak benetako gainerako bi orduetan. Transakzio hau beranduago fakturatu daiteke edo kargagabea izan daiteke, bezeroarekin izandako negoziazioen arabera.
