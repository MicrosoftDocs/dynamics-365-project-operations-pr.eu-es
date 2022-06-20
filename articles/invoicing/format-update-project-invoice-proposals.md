---
title: Kudeatu proiektuaren faktura-proposamenak
description: Artikulu honek bezeroei begira dauden fakturak prozesatzeari buruzko xehetasunak eskaintzen ditu Project Operations-ekin baliabideetan edo hornituta ez dauden agertokietarako.
author: sigitac
ms.date: 04/12/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: ef6003499f1372a51d7d1606db6f5bf9722a369d
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8927819"
---
# <a name="manage-project-invoice-proposals"></a>Kudeatu proiektuaren faktura-proposamenak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Proiektuen faktura proposamenak fakturazio sailak prozesatu ditzake bi baldintza hauek betetzen direnean:

  - Proiektuaren kudeatzaileak proforma faktura berresten du Microsoft Dataverse-n.
  - Proforma fakturan sartzen diren fakturatu gabeko denbora eta material salmenta transakzio guztiak Dynamics 365 **Project Operations-en integrazioa** aldizkaria erabiliz argitaratzen dira.

Erabili urrats hauek Dynamics 365 Finance-en proiektuaren faktura-proposamena osatzeko.

1. Berrikusi fakturazioari buruzko informazioa denbora eta material transakzioetarako eta bidali **Project Operations-en integrazioa** aldizkaria.
2. Berrikusi fakturazio informazioa prezio finkoko fakturazio mugarrietarako.
3. Berrikusi eta eman formatua proiektuen fakturen proposamena.
4. Argitaratu eta inprimatu proiektuaren fakturak.

## <a name="manage-billing-information-in-the-project-operations-integration-journal"></a>Kudeatu fakturazio informazioa Project Operations Integration aldizkarian

Dataverse-n sortutako proiektuaren benetako datuak Finance-n argitaratzen ditu Proiektu-kontulariak. Integrazio-aldizkariarekin lan egiteari buruzko informazio gehiago lortzeko, ikusi [Project Operations-en Integrazio aldizkaria](../project-accounting/project-operations-integration-journal.md).

Kostuen fakturak eta fakturatu gabeko salmenten errealitateak Integrazio aldizkarian gehitzen dira lerro bereizi gisa:

  - Unitatearen kostuaren prezioa eta kostuaren zenbatekoa, proiektuaren kostuaren benetako lehenetsitako kostuaren transakzioan Dataverse-n.
  - Fakturarik gabeko salmenta transakzioko salmenta unitateko prezioa eta salmenten zenbatekoa fakturatutako fakturatutako salmenten transakzioaren lehenetsitakoak dira Dataverse-n.

### <a name="billing-sales-tax"></a>Fakturazio salmenten gaineko zerga

Fakturazioaren salmenten gaineko zergaren kalkulua **Fakturazio salmenten gaineko zerga taldea** eta **Fakturazio elementuen salmenten gaineko zerga taldea** eremuko konbinazioa fakturatu gabeko salmenten erregistroan **Proiektuen eragiketen integrazioa** aldizkari lerroa. Sistemak lehenetsitako eremuko balio hauek ezarpenetan oinarrituta daude **Finantzak** fitxan **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea.

- **Salmenten gaineko zerga taldearen metodoa** fakturazio salmenten gaineko zerga taldearen lehenetsitako logika zehazten du:
  
  - **Proiektua**: Proiektuaren fakturazio salmenten gaineko zerga taldea lehenetsiko du beti. Proiektu baten fakturazio lehenetsitako salmenten gaineko zerga taldea berrikusi edo alda dezakezu hautatuta **Erakutsi lehenetsitako kontabilitatea** **Proiektu guztiak** orrialdean.
  - **Proiektuaren kontratua**: Proiektuaren kontratuko fakturazio salmenten gaineko zerga taldea lehenetsiko du beti. Proiektuaren kontratu baten lehenetsitako salmenten gaineko zerga taldea berrikusi edo alda dezakezu hautatuta **Erakutsi lehenetsitako kontabilitatea** **Proiektuaren kontraktuak** orrialdean.
  - **Bezeroa**: Bezeroaren fakturazio salmenten gaineko zerga taldea lehenetsiko du beti.
  - **Bilatu**: Goiko entitate guztietan bilatuko du eta eskuragarri dagoen lehen balioa hautatuko du. Bilaketa ikurrarekin hasten da **Proiektua** entitatea, **Proiektuaren kontratua** entitatea, eta azkenik **Bezeroa** entitatea.

- **Elementuen salmenten gaineko zerga taldearen metodoa** fakturazio-elementuen salmenten gaineko zerga taldearen lehenetsitako logika zehazten du:
  
  - Denbora, gastu eta kuoten transakzio moten kasuan, fakturazio elementuen salmenten gaineko zerga taldeak lehenetsitakoa izango da beti **Proiektuaren kategoria** entitatea.
  - Transakzio material motetarako, fakturazio elementuen salmenten gaineko zerga taldeak lehenetsitakoa da **Elementuen salmenten gaineko zergaren taldearen metodoa** **Proiektuen kudeaketa eta kontabilitate parametroak** ezartzean. Artikuluaren zenbakiak elementuen salmenten gaineko zergaren taldea lehenetsi du **Kaleratutako produktua** entitatean. Kategoriak elementuen salmenten gaineko zergaren taldea lehenetsi du **Proiektuaren kategoria** entitatean.

### <a name="financial-dimensions"></a>Finantza-dimentsioak

Urtean fakturatu gabeko salmenten erregistroen dimentsio ekonomikoak **Project Operations-en integrazioa** aldizkariaren lehenetsia **Proiektua** entitatea. Finantza dimentsioak berrikusi eta doitu ditzakezu **Zenbatekoak banatu** hautatuta. Integrazio aldizkaria argitaratu ondoren fakturatu gabeko salmenten erregistroaren dimentsio ekonomikoak aldatu behar badituzu baina Proforma faktura baieztatu aurretik, joan **Proiektu guztiak** > **Kudeatu** > **Argitaratutako transakzioak** aukerara, hautatu transakzioa eta, ondoren, hautatu **Prozesua** > **Doitu kontabilitatea**.

### <a name="exchange-rates"></a>Kanbio-tasak

Fakturatu gabeko transakzioaren moneta Dataverse-n Finance-n transakzio moneta gisa erabiltzen da eta konpainiaren kontabilitate moneta bihurtzen da Finantzan definitutako kanbio tasak erabiliz.


## <a name="manage-the-financial-attributes-of-billing-milestones"></a>Kudeatu fakturazio mugarrien finantza atributuak 

Prezio finkoko fakturazio metodoa erabiliz proiektuen kontratu lineak fakturatzen dira [Prezio finkoaren mugarriak](../sales/invoice-schedules-contract-line.md#create-a-fixed-price-invoice-schedule-for-a-contract-line). Proiektuaren kontulariak Finantzako fakturazio mugarriak berrikus ditzake, joan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** > **Kudeatu** > **Kontuko transakzioak** aukerara.

### <a name="billing-sales-tax"></a>Fakturazio salmenten gaineko zerga

**Salmenten gaineko zerga taldea** eta **Artikuluen salmenten gaineko zergaren taldea** ezarpenetako balio lehenetsiak fakturazio mugarri berria sortzen denean Dataverse-n. Sistemak lehenetsitako eremuko balio horiek ezarpenetan oinarrituta daude **Finantzak** fitxan **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea.

- **Salmenten gaineko zerga taldearen metodoa** eremuak **Fakturazio-salmenten gaineko zerga taldea** eremuaren lehenetsitako logika zehazten du:

    - **Proiektua**: proiektuaren fakturazio salmenten gaineko zerga taldea lehenetsiko du beti. Proiektu baten lehenetsitako salmenten gaineko zerga taldea berrikusi edo alda dezakezu hautatuta **Erakutsi lehenetsitako kontabilitatea** **Proiektu guztiak** orrialdean.
    - **Proiektuaren kontratua**: proiektuaren kontratuko fakturazio salmenten gaineko zerga taldea lehenetsiko du beti. Proiektuaren kontratu baten lehenetsitako salmenten gaineko zerga taldea berrikusi edo alda dezakezu hautatuta **Erakutsi lehenetsitako kontabilitatea** **Proiektuaren kontraktuak** orrialdean.
    - **Bezeroa**: bezeroaren fakturazio salmenten gaineko zerga taldea lehenetsiko du beti.
    - **Bilatu**: goiko entitate guztietan bilatuko du eta eskuragarri dagoen lehen balioa hautatuko du. Bilaketa ikurrarekin hasten da **Proiektua** entitatea, **Proiektuaren kontratua** entitatea, eta **Bezeroa** entitatea.

- **Prezio finkoaren mugarriaren salmenten gaineko zerga taldea** fitxategian balio lehenetsi gisa erabiltzen da **Artikuluen salmenten gaineko zergaren taldea** fakturazio mugarriaren eremua. Kontulariak balio hori berrikusi eta alda dezake **Kontuko transakzioak** orrialdea. Sistemak kontuko transakzioaren balioa erabiltzen du proiektuaren faktura proposamen lerro bat sortzerakoan.
 

### <a name="financial-dimensions"></a>Finantza-dimentsioak

Prezio finkoko fakturazio mugarriaren lehenetsitako finantza dimentsioak Proiektuaren kontratu lerroetan ezartzen dira. Joan **Proiektuen kontratuak** > **Erakutsi lehenetsitako kontabilitatea** eta **Kontratuaren lerroak** fitxa, hautatu **prezioaren kontratuaren lerroa** aukerara, ezarri lehenetsi gisa erabili nahi dituzun finantza dimentsioen balioak.

Proiektuaren kontulariak salmenten gaineko zergaren eta finantza dimentsioen informazioa alda dezake fakturen mugarrietan, proiektuaren faktura proposamena sortu arte.


## <a name="create-project-invoice-proposals"></a>Sortu proiektuaren faktura-proposamenak

Proiektuen faktura proposamenak berrikus daitezke **Proiektuen kudeaketa eta kontabilitatea** modulura **Proiektuaren fakturak** > **Proiektuen faktura proposamenak** aukerara joanda.

Proiektuaren faktura proposamenaren goiburua Finantzan sortzen da Proforma faktura baieztatzen denean Dataverse-n. Erraz uztartzeko, sistemak Proiektuaren faktura proposamenaren zenbakia Finantzetan Proforma fakturaren IDaren zenbaki berean ezartzen du Dataverse-n. Proformaren fakturak ez direnez zertan sortu diren ordena berean baieztatzen, Finantzako Proiektuaren faktura proposamenen zenbaki sekuentziak zenbaki baxu eta altuagoetarako aldaketak baimendu behar ditu. Konfiguratu zenbaki sekuentziak urrats hauek erabiliz:

1. Finance-n, joan **Erakundearen administrazioa** > **Zenbaki sekuentziak** > **Zenbaki sekuentziak**.
2. **Eremua** iragazkian, hautatu **Proiektuak**.
3. **Erreferentzia** iragazkian, hautatu **Faktura proposamena**.
4. Erabili **Enpresa** eremua pertsona juridiko bakoitza Project Operations Dataverse integrazioa gaituta.
5. Ireki **Zenbakien sekuentziaren xehetasunak** eta **Orokorra** fitxan ezarri:

    - **Baimendu erabiltzaile aldaketak: zenbaki txikiago batera** = **Bai**
    - **Baimendu erabiltzaile aldaketak: zenbaki handiago batera** = **Bai**

Proiektuen faktura proposamenen lerroak sistemak aldizkako prozesua erabiliz gehitzen ditu **Inportatu taulako taulatik** (**Proiektuen kudeaketa eta kontabilitatea** > **Aldizkakoa** > **Proiektu Operations-en integrazioa** > **Inportatu taulako taulatik**). Prozesua eskuz exekuta daiteke edo aldian aldiko antolaketa erabiliz. Sistemak ez ditu lerroak gehituko faktura proposamenaren dokumentuan lerro guztiak fakturatzeko prest egon arte. Denbora eta material transakzioak fakturatzeko prest daude **Project Operations-en integrazioa** aldizkaria.

## <a name="format-and-print-invoice-proposals"></a>Eman formatua eta inprimatu fakturen proposamenak

Proiektuaren kontulariak proiektuaren fakturen inprimaketa pertsonaliza dezake **Faktura proposamena formateatu** orria eta inprimatzeko kudeaketa gaitasunak.

### <a name="format-invoice-proposals"></a>Eman formatua fakturen proposamenei

**Eman formatua faktura proposamenei** orrialdeak pertsonalizatutako multzokatze transakzioak bezeroaren proiektuaren fakturan bistaratzeko aukera ematen du.

1. **Proiektuaren faktura proposamena** orrialdean, hautatu **Inprimatu** > **Eman formatua faktura proposamenei**.
2. Aukeratu **Berria** proiektuaren faktura inprimatzeko taldekatze berria sortzeko.
3. **Xehetasuna / Laburpena** eremuan, hautatu taldekatze honetarako aukerak:

    - Aukeratu **Xehetasuna** bezeroaren fakturaren transakzio datuak inprimatzeko.
    - Aukeratu **Laburpena** bezeroaren fakturaren transakzioaren laburpena inprimatzeko.

> [!NOTE]
> **Xehetasuna/Laburpena** eremuko hautapenak, **Eman formatua faktura proposamenari** orrialdean, fitxategian hautatutako aukera gainidazten du **Fakturaren formatua** eremuan **Faktura proposamenak** orrian faktura zehatza edo laburpen faktura inprimatzeko.

- Aukeratu atalean sartu beharreko transakzio lerroak **Eskuragarri dauden transakzioak** fitxa eta hautatu **Sartu transakzioak** **Aukeratutako transakzioak** fitxara eramateko.
- Aukeratu **Mugitu gora** eta **Mugitu behera** ordena aldatzeko.
- Aukeratu **Inprimatzeko aurrebista** formateatutako faktura aurreikusteko.

### <a name="print-management"></a>Inprimatze-kudeaketa

Inprimatze kudeaketak txosten fitxategi desberdinak erabiltzen ditu fakturaren inprimatzeko, helmugak zehazteko eta orri-oina pertsonalizatzeko. Inprimatze kudeaketa modulu mailan konfigura daiteke, hala ere ezarpen horiek bezero, kontratu edo faktura proposamen zehatz baterako gainidatz daitezke. Funtzio honetara sartzeko **Proiektuaren faktura proposamena** orrialdean, hautatu **Inprimatu** > **Inprimatze-kudeaketa**.

Inprimatze kudeaketa konfigurazioa zuhaitz ikuspegi gisa bistaratzen da, non nodo maila bakoitzak doitzeko dauden dokumentuak bistaratzen ditu. Inprimaketa pertsonalizatuak esleitu ditzakezu moduluan, bezeroan, kontratuan edo faktura proposamenaren dokumentu mailan. Jatorrizko dokumentuaren inprimaketa aldatzeko, zabaldu nahi duzun nodoa eta hautatu **Elementu originala**. **Txosten formatua** eremuan, hautatu inprimatzeko erabiliko den txosten formatua. Txosten formatu pertsonalizatuak erabil ditzakezu [Negozioaren dokumentu-kudeaketaren esparrua](/dynamics365/fin-ops-core/dev-itpro/analytics/er-business-document-management) erabiliz.

## <a name="post-invoice-proposals"></a>Argitaratu fakturen proposamenak

Faktura berrikusi eta editatu ondoren, eta faktura proposamenen lerroak asebetetzen direnean, egiaztatu fakturen guztizkoak eta salmenten gaineko zerga. **Xehetasunak** taldean, hautatu **Guztira** eta, ondoren, hautatu **Argitaratu** faktura argitaratzeko.

Argitaratu aurretik faktura ikusteko, garbitu **Argitaratzen** kontrol-laukia. **Proforma** fakturan inprimatuko da lagin-faktura dela adierazteko. Faktura inprimatzeko, hautatu **Inprimatu faktura** kontrol-laukia.

Horrez gain, **Faktura proposamena** orrialdean, fakturen proposamenak aldian-aldian lan eginez ere bidal daitezke, **Faktura proposamenak bidali**. Lan hau aurkitzeko, joan **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkakoa** > **Proiektuaren fakturak** > **Faktura-proposamenak bidali** aukerara.

Orrialde honetan argitaratzeko prest dauden faktura proposamen guztiak agertzen dira. Faktura proposamenak bidaltzeko programatu dezakezu **Sorta** hautatuta. Ezarri **Sortaka prozesatzeko parametroa** **Bai** gisa, eta ezarri sortaka prozesatzeko errepikapena **Errepikapena** hautatuta.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
