---
title: Denbora-sarrerak luzatzea
description: Gai honetan garatzaileek denbora sartzeko kontrola nola luzatu dezaketen buruzko informazioa ematen da.
author: stsporen
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 93f411ad7c86beefcc35e7799a03987dacdcd62b
ms.sourcegitcommit: 5a29adce48133e09f051929e8544d6c2c93c025d
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/02/2020
ms.locfileid: "3930865"
---
# <a name="extending-time-entries"></a>Denbora-sarrerak luzatzea

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations-ek denbora sartzeko kontrol pertsonalizagarria luzagarria du. Kontrol honek eginbide hauk ditu:

- Sartu denbora astean horizontalean
- Eguneko, errenkadako edo asteko guztizkoak
- Kopiatu errenkadak edo asteak
- Denbora sarrera HH bidez: mm edo HH:hh (automatikoki HH:hh bihurtzen da)
- Inportatu zereginetatik, erreserbetatik edo hitzorduetatik

Denbora sarrerak luzatzea posible da bi eremutan:
- [Gehitu denbora pertsonalizatutako sarrera zure erabilerarako](#add)
- [Pertsonalizatu asteroko denbora-sarreraren kontrola](#customize)

## <a name="add-custom-time-entries-for-your-own-use"></a><a name="add"></a>Gehitu denbora pertsonalizatutako sarrera zure erabilerarako.

Denbora-sarrerak agertoki anitzetarako erabiltzeko diseinatutako entitate nagusia dira. 2020ko apirilaren 1ean, TESA core irtenbidea aurkeztu zen, eta horrek eskaintzen du **Ezarpenak** entitatea eta berria **Denbora sartzeko erabiltzailea** segurtasun-funtzio. Eremu berriak, **msdyn_start** eta **msdyn_end** erlazio zuzena dutenak **msdyn_duration**, ere sartu ziren. Entitate berriak, segurtasun-funtzio, eta eremuek produktuaren arteko denborarekiko ikuspegi bateratuagoa ahalbidetzen dute.


### <a name="time-source-entity"></a>Denboraren iturburuko entitatea
| Eremua | Deskribapena | 
|-------|------------|
| Izena  | Denbora sorkuntzan hautapen balio gisa erabilitako denbora iturriaren sarreraren izena. |
| Denbora iturri lehenetsia [Denbora iturria: isdefault] | Berez, denbora iturri bakarra markatu daiteke denbora iturri lehenetsian. Gaitasun horri esker, sarrerak denbora-iturri lehenetsi daitezke, zehazten ez bada. |
|Denbora iturri mota [Denbora iturria: sourcetype] | Iturri mota denbora iturria aplikazio batekin elkartzea ahalbidetzen duen aukera da (Time Entry Source Type). Aukera multzo honi balio osagarriak gehituko zaizkio aplikazio osagarriak gehitu ahala. Kontuan izan Microsoftek 190.000.000 baino balio handiagoak gordetzen dituela.|


### <a name="time-entries-and-the-time-source-entity"></a>Denbora-sarrerak eta Time Source Entity
Denbora-sarrera bakoitza denbora-iturburu erregistro batekin lotzen da. Erregistro honek zehazten du nola eta zein aplikaziotan prozesatu behar duten denbora sarrera.

Denbora-sarrerak hasierako, amaierako eta iraupenarekin lotuta dauden denbora-blokeak dira.

Logikak denbora sartzeko erregistroa automatikoki eguneratuko du egoera hauetan:

- Hurrengo hiru eremuetatik bi ematen badira, hirugarrena automatikoki kalkulatuko da 

    - **msdyn_start**
    - **msdyn_end**
    - **msdyn_duration**

- Eremuak, **msdyn_start** eta **msdyn_end** ordu-eremua ezagutzen dute.
- Denbora-sarrerak soilik sortutakoarekin **msdyn_date** eta **msdyn_duration** zehaztutako gauerdian hasiko da, eta **msdyn_start** eta **msdyn_end** eguneratu egingo da.

#### <a name="time-entry-types"></a>Denbora-sarrera motak

Denbora sartzeko erregistroek lotutako aplikazioa aurkezteko fluxuan portaera definitzen duen mota lotua dute.

|Etiketa | Balioa|
|-----|-----|
|Atsedenean   |192,355,000|
|Bidaia | 192,355,001|
|Aparteko orduak   | 192,354,320|
|Lana   | 192,350,000|
|Laneko huts-egitea    | 192,350,001|
|Opor-eguna   | 192,350,002|



## <a name="customize-the-weekly-time-entry-control"></a><a name="customize"></a>Pertsonalizatu asteroko denbora-sarreraren kontrola
Garatzaileek eremu eta bilaketak gehi ditzakete beste entitate batzuetara eta negozio arau pertsonalizatuak ezar ditzakete beren negozio eszenatokiei laguntzeko.

### <a name="add-custom-fields-with-lookups-to-other-entities"></a>Gehitu bilaketak dituzten eremu pertsonalizatuak beste entitateetan
Asteko denbora-sarrera saretan eremu pertsonalizatua gehitzeko hiru urrats nagusi daude.

- Gehitu pertsonalizatutako eremua sorrera bizkorreko elkarrizketa-koadroan.
- Konfiguratu sareta pertsonalizatutako eremua erakusteko.
- Gehitu eremu pertsonalizatua errenkadaren zeregin-fluxura edo gelaxka editatzeko zeregin-fluxura.

Ziurtatu eremu berriak behar beharrezko balidazioak dituela errenkadan edo gelaxka editatzeko zeregin-fluxuan. Urrats honen zati gisa, eremua blokeatu behar duzu, denbora-sarreraren egoeran oinarrituta.

#### <a name="add-the-custom-field-to-the-quick-create-dialog-box"></a>Gehitu pertsonalizatutako eremua sorrera bizkorreko elkarrizketa-koadroan
Eremu pertsonalizatua gehitu behar duzu **Sortu denboraren-sarreraren sorrera bizkorra** elkarrizketa-koadroan. Orduan, erabiltzaileek balio bat sar dezakete denbora hautatuz gehituz gero **Berria**.

#### <a name="configure-the-grid-to-show-the-custom-field"></a>Konfiguratu sareta pertsonalizatutako eremua erakusteko
Asteko denbora-sarrera saretan eremu pertsonalizatua gehitzeko bi modu daude:

  - Pertsonalizatu ikuspegia eta gehitu eremu pertsonalizatua
  - Sortu denbora-sarrera pertsonalizatu lehenetsi bat 


**Pertsonalizatu ikuspegia eta gehitu eremu pertsonalizatua**

**Nire asteko denbora-sarrerak** ikuspegia pertsonaliza dezakezu eta gehitu eremu pertsonalizatua bertara. Saretako eremu pertsonalizatuaren posizioa eta tamaina aukeratu ditzakezu ikuspegian propietateak editatuz.

**Sortu denbora-sarrera pertsonalizatu lehenetsi bat** 

Ikuspegi horrek **Deskribapena** eta **Kanpoko iruzkinak** eremuak eduki beharko lituzke, saretan eduki nahi dituzun zutabeez gain. 

1. Aukeratu posizioa, tamaina eta multzoaren hurrenkera lehenetsia ikuspegian propietateak editatuz. 
2. Konfiguratu ikuspegi horretarako kontrol pertsonalizatua **Denbora-sarreraren sareta** kontrola izan dadin. 
3. Gehitu kontrol hori ikuspegian, eta hautatu web, telefono eta tabletetarako. 
4. Konfiguratu asteako denbora-sarrerako saretako parametroak. Ezar ezazu **Hasiera data**eremua **msdyn_date** gisa, ezarri **Iraupena** eremua **msdyn_duration** gisa eta ezarri **Egoera** eremua **msdyn_entrystatus** gisa. 
5. Ikuspegi lehenetsirako, **Irakurtzeko soilik den egoera-zerrenda** eremua **192350002,192350003,192350004** gisa dago ezarrita, **Errenkada editatzeko zeregin-fluxua** eremuan **msdyn_timeentryrowedit** gisa eta **Gelaxka editatzeko zeregin-fluxua** eremuan **msdyn_timeentryedit** gisa. 
6. Eremu hauek pertsonaliza ditzakezu irakurtzeko soilik egoera gehitzeko edo kentzeko, edo zereginetan oinarritutako egoera (TBX) bat erabil dezakezu errenkada edo gelaxka editatzeko. Eremu hauek balio estatiko batera lotu beharko lirateke.


> [!NOTE] 
> Bi aukerek integratutako iragazki batzuk kenduko dituzte **Proiektua** eta **Proiektuaren zeregina** entitateetan, entitateen bilaketa ikuspegi guztiak ikusgai egon daitezen. Laukitik kanpo, bilaketa-ikuspegi garrantzitsuak bakarrik ikus daitezke.
Eremu pertsonalizatuetarako zeregin-fluxu egokia zehaztu behar duzu. Seguruenik, eremua saretan gehitzen baduzu, denbora-sarrerako errenkada osora aplikatzen diren eremuetarako erabiltzen den errenkadako zeregin-fluxuan joan beharko litzateke. Eremu pertsonalizatuak egunero balio esklusiboa badu, adibidez, eremu pertsonalizatua **Amaiera ordua** aukerarako,zeregin-fluxuaren edizioa gelaxkan sartu beharko litzateke.

Eremu pertsonalizatua zeregin-fluxu batean gehitzeko, arrastatu **Eremua** elementua orrialdeko kokapen egokian eta, ondoren, ezarri eremuaren propietateak. Ezar ezazu **Iturria** jabetza **Denbora-sarrera** gisa, eta ezarri **Datu-eremua** propietatea eremu pertsonalizaturako. **Eremua** propietateak TBX orrian agertzen den bistaren izena zehazten du. Hautatu **Aplikatu** aldaketak eremuan gordetzeko eta, ondoren, hautatu **Eguneratu** aldaketak orrian gordetzeko.

Horren ordez TBX orrialde pertsonalizatu bat erabiltzeko, sortu beste prozesu bat. Ezarri kategoria **Negozio-prozesuaren fluxua** gisa, ezarri entitatea **Denbora-sarrera** gisa eta zehaztu negozio-prozesu mota **Exekutatu prozesua zeregin-fluxu gisa** bezala. **Propietateak** aukeran, **Orriaren izena** propietatea orrialdearen bistaratzeko izenean ezarri behar da. Gehitu eremu garrantzitsu guztiak TBX orrialdean. Gorde eta aktibatu prozesua eta, ondoren, eguneratu zeregin-fluxuari dagokion kontrol pertsonalizatuaren propietatea **Izena** baliora prozesuan.

### <a name="add-new-option-set-values"></a>Gehitu beste aukera multzoen balio batzuk
Aukera multzoaren balioak integratutako eremu batean gehitzeko, ireki eremuaren edizio orria eta, ondoren, **Mota** atalean, hautatu **Editatu** aukera aukera multzoaren ondoan. Ondoren, gehitu etiketa pertsonalizatua eta kolorea dituena beste aukera bat. Denbora-sarreraren beste egoera bat gehitu nahi baduzu, integratutako eremuak **Sarreraren egoera** du izena, ez **Egoera**.

### <a name="designate-a-new-time-entry-status-as-read-only"></a>Izendatu denbora-sarreraren egoera bat irakurtzeko soilik
Denbora-sarreraren egoera berria irakurtzeko bakarrik izendatzeko, gehitu denbora-sarrerako balio berria **Irakurtzeko soilik egoera-zerrenda** propietateari. Denbora-sarreraren saretaren zati editagarria blokeatuta egongo da egoera berria duten errenkadetarako.
Ondoren, gehitu negozioaren arauak eremu guztiak blokeatzeko **Denbora-sarreraren errenkadaren edizioa** eta **Denbora-sarreraren edizioa** TBX orrietan. Orrialde hauetako negozioaren arauak atzitu ditzakezu orrirako negozio-prozesuaren fluxu editorea irekiz eta, ondoren, **Negozioaren arauak** hautatuz. Lehendik dauden negozioaren arauetan egoera gehitu dezakezu baldintzara, edo beste negozioaren arau bat gehitu dezakezu egoera berrian.

### <a name="add-custom-validation-rules"></a>Gehitu balidazio-arau pertsonalizatuak
Bi asteko denbora sartzeko sareta esperientzian gehitu ditzakezun bi balioztatze arau mota daude:

- Elkarrizketa koadroetan eta TBX orrietan azkar funtzionatzen duten bezeroaren aldeko negozio arauak.
- Zerbitzariaren aldeko pluginen balioztapenak, sarrera eguneratze guztiei aplikatzen zaizkienak.

#### <a name="business-rules"></a>Negozioaren arauak
Erabili negozioaren arauak eremuak blokeatzeko eta desblokeatzeko, eremuetan balio lehenetsiak sartzeko eta uneko sarrera erregistratik soilik informazioa eskatzen duten balidazioak definitzeko. TBX orrialde bateko negozioaren arauak atzitu ditzakezu orrirako negozio-prozesuaren fluxu editorea irekiz eta, ondoren, **Negozioaren arauak** hautatuz. Lehendik dauden negozioaren arauak editatu edo beste negozioaren arau batzuk gehitu ditzakezu. Balidazio pertsonalizatuagoak lortzeko, negozioaren araua erabil dezakezu JavaScript exekutatzeko.

#### <a name="plug-in-validations"></a>Plugin-en balidazioak
Plugin-en balidazioak erabili beharko zenituzke denbora-sarrera erregistro bakarrean eskuragarri dagoen testuingurua baino gehiago behar duten balidazioetarako edo saretako lineako eguneratzeetan exekutatu nahi dituzun balidazioetarako. Balidazioa osatzeko, sortu plugin pertsonalizatua **Denbora-sarrera** erakundean.
