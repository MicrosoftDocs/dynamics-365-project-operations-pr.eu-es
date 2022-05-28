---
title: Denbora-sarrerak luzatzea
description: Gai honetan garatzaileek denbora sartzeko kontrola nola luzatu dezaketen buruzko informazioa ematen da.
author: stsporen
ms.date: 01/27/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 6b91aecd76950d2bd37192d634c80ea98d08034e
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8582971"
---
# <a name="extending-time-entries"></a>Denbora-sarrerak luzatzea

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations-ek denbora sartzeko kontrol pertsonalizagarria luzagarria da. Kontrol honek eginbide hauk ditu:

- Sartu denbora astean horizontalean
- Eguneko, errenkadako edo asteko guztizkoak
- Kopiatu errenkadak edo asteak
- Denbora sarrera HH bidez: mm edo HH:hh (automatikoki HH:hh bihurtzen da)
- Inportatu zereginetatik, erreserbetatik edo hitzorduetatik

Denbora sarrerak luzatzea posible da bi eremutan:
- [Gehitu denbora pertsonalizatutako sarrera zure erabilerarako](#add)
- [Pertsonalizatu asteroko denbora-sarreraren kontrola](#customize)

## <a name="add-custom-time-entries-for-your-own-use"></a><a name="add"></a>Gehitu denbora pertsonalizatutako sarrera zure erabilerarako

Denbora-sarrerak agertoki anitzetan erabilitako oinarrizko entitatea dira. 2020ko apirilaren 1ean, TESAren oinarrizko irtenbidea aurkeztu zen. TESAk eskaintzen du **Ezarpenak** entitatea eta berria **Denbora sartzeko erabiltzailea** segurtasun-funtzio. Eremu berriak, **msdyn_start** eta **msdyn_end** erlazio zuzena dutenak **msdyn_duration**, ere sartu ziren. Entitate berriak, segurtasun-funtzio, eta eremuek produktuaren arteko denborarekiko ikuspegi bateratuagoa ahalbidetzen dute.


### <a name="time-source-entity"></a>Denboraren iturburuko entitatea
| Eremua | Deskribapena | 
|-------|------------|
| Eman izena  | Denbora sorkuntzan hautapen balio gisa erabilitako denbora iturriaren sarreraren izena. |
| Denbora iturri lehenetsia [Denbora iturria: isdefault] | Berez, denbora iturri bakarra markatu daiteke denbora lehenetsian. Horri esker, sarrerak denbora-iturri lehenetsi daitezke, zehazten ez bada. |
|Denbora iturri mota [Denbora iturria: sourcetype] | Iturri mota denbora iturria aplikazio batekin elkartzea ahalbidetzen duen aukera da (Time Entry Source Type). Microsoft-ek 190.000.000 baino balio handiagoak gordetzen dituela.|


### <a name="time-entries-and-the-time-source-entity"></a>Denbora-sarrerak eta denbora-iturburuaren entitatea
Denbora-sarrera bakoitza denbora-iturburu erregistro batekin lotzen da. Erregistro honek zehazten du zein aplikazio prozesatu behar duten denbora-sarrera eta nola.

Denbora-sarrerak hasierako, amaierako eta iraupenarekin lotuta dauden denbora-blokeak dira.

Logikak denbora sartzeko erregistroa automatikoki eguneratuko du egoera hauetan:

- Hurrengo hiru eremuetatik bi ematen badira, hirugarrena automatikoki kalkulatuko da: 

    - **msdyn_start**
    - **msdyn_end**
    - **msdyn_duration**

- The **msdyn_start** eta **msdyn_end** eremuek ordu-eremua ezagutzen dute.
- Denbora-sarrerak soilik sortutakoarekin **msdyn_date** eta **msdyn_duration** zehaztutako gauerdian hasiko da. **msdyn_start** eta **msdyn_end** eremuak eguneratu egingo dira.

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

1. Gehitu eremu pertsonalizatua **Sortu azkarra** elkarrizketa-koadroa.
2. Konfiguratu sareta pertsonalizatutako eremua erakusteko.
3. Gehitu eremu pertsonalizatua **Errenkadak editatzea** edo **Denbora-sarrera editatzea** orrialdea, dagokion moduan.

Ziurtatu eremu berriak beharrezko balioztatzeak dituela **Errenkadak editatzea** edo **Denbora-sarrera editatzea** orrialdea. Zeregin honen zati gisa, blokeatu eremua, denbora-sarreraren egoeraren arabera.

Eremu pertsonalizatu bat gehitzen duzunean **Denbora sarrera** sareta eta, ondoren, denbora-sarrerak zuzenean sarean sortu, sarrera horien eremu pertsonalizatua automatikoki ezartzen da errenkadarekin bat etor dadin. 

### <a name="add-the-custom-field-to-the-quick-create-dialog-box"></a>Gehitu eremu pertsonalizatua Sortu azkarreko elkarrizketa-koadroan
Gehitu eremu pertsonalizatua **Sortu azkarra: Sortu denbora sarrera** elkarrizketa-koadroa. Orduan, erabiltzaileek balio bat sar dezakete denbora hautatuz gehituz gero **Berria**.

### <a name="configure-the-grid-to-show-the-custom-field"></a>Konfiguratu sareta pertsonalizatutako eremua erakusteko
Bi modu daude eremu pertsonalizatu bat gehitzeko **Asteroko denbora sarrera** sareta.

- Pertsonalizatu **Nire asteko denbora-sarrerak** ikusi eta gehitu eremu pertsonalizatua. Eremu pertsonalizatuaren posizioa eta tamaina zehaztu ditzakezu sarean, ikuspegiko propietateak editatuz.
- Sortu ordua sartzeko ikuspegi pertsonalizatu berri bat eta ezarri ikuspegi lehenetsi gisa. Ikuspegi honek eduki behar du **Deskribapena** eta **Kanpoko iruzkinak** sareak sartzea nahi dituzun zutabeez gain eremuak. Sarearen posizioa, tamaina eta ordena lehenetsia zehaztu ditzakezu ikuspegiko propietateak editatuz. Ondoren, konfiguratu ikuspegi horretarako kontrol pertsonalizatua **Denbora-sarreraren sareta** kontrola izan dadin. Gehitu kontrola ikuspegiari eta hautatu **Weba**, **·**, eta **Tableta**. Ondoren, konfiguratu parametroak **Asteroko denbora sarrera** sareta. Ezarri **Hasiera data** eremura **msdyn\_ data**, ezarri **Iraupena** eremura **msdyn\_ iraupena**, eta ezarri **Egoera** eremura **msdyn\_ sarrera-egoera**. The **Irakurtzeko soilik egoera zerrenda** eremuan ezarrita dago **192350002 (onartua)**, **(Bidalketa)**, edo **192350004 (Deialdia eskatu da)**.

### <a name="add-the-custom-field-to-the-appropriate-edit-page"></a>Gehitu eremu pertsonalizatua dagokion edizio-orrian
Ordu-sarrera edo denbora-sarrera errenkada bat editatzeko erabiltzen diren orrialdeak azpian aurki daitezke **Formak**. The **Editatu sarrera** sareko botoiak irekitzen du **Editatu sarrera** orrialdea, eta **Editatu errenkada** botoiak irekitzen du **Errenkadak editatzea** orrialdea. Orrialde hauek edita ditzakezu, eremu pertsonalizatuak izan ditzaten.

Bi aukerak kutxaz kanpoko iragazki batzuk kentzen ditu **Proiektua** eta **Proiektuaren zeregina** entitateak, entitateen bilaketa-ikuspegi guztiak ikusgai egon daitezen. Laukitik kanpo, bilaketa-ikuspegi garrantzitsuak bakarrik ikus daitezke.

Eremu pertsonalizaturako orri egokia zehaztu behar duzu. Seguruenik, eremua sarera gehitu baduzu, joan beharko litzateke **Errenkadak editatzea** Denbora-sarreren errenkada osoari aplikatzen zaizkion eremuetarako erabiltzen den orrialdea. Eremu pertsonalizatuak egunero errenkadan balio esklusibo bat badu (adibidez, amaierako eremu pertsonalizatua bada), eremuan joan beharko luke.**Denbora-sarrera editatzea** orrialdea.

Eremu pertsonalizatua orri batean gehitzeko, arrastatu a **Eremua** elementua orrialdeko posizio egokian jarri eta, ondoren, ezarri bere propietateak.

### <a name="add-new-option-set-values"></a>Gehitu beste aukera multzoen balio batzuk
Kutxaz kanpoko eremu batean aukera multzo balioak gehitzeko, jarraitu urrats hauek.

1. Ireki eremuaren edizio orria, eta, ondoren, azpian **Mota**, hautatu **Editatu** aukera multzo-ren ondoan.
2. Gehitu etiketa pertsonalizatua eta kolorea dituena beste aukera bat. Ordua sartzeko egoera berri bat gehitu nahi baduzu, kutxaz kanpoko eremuari izena emango zaio **Sarrera Egoera**.

### <a name="designate-a-new-time-entry-status-as-read-only"></a>Izendatu denbora-sarreraren egoera bat irakurtzeko soilik
Denbora-sarreraren egoera berria irakurtzeko bakarrik izendatzeko, gehitu denbora-sarrerako balio berria **Irakurtzeko soilik egoera-zerrenda** propietateari. Ziurtatu zenbakia gehitzen duzula, ez etiketa. Ordua sartzeko saretaren zati editagarria blokeatuko da orain egoera berria duten errenkadetan. Ezartzeko **Irakurtzeko soilik egoera zerrenda** jabetza ezberdina ezberdinentzat **Denbora Sarrera** ikuspegiak, gehitu **Denbora sarrera** sarea ikuspegi batean **Kontrol pertsonalizatuak** atalean, eta konfiguratu parametroak dagokion moduan.

Ondoren, gehitu negozio-arauak eremu guztiak blokeatzeko **Errenkadak editatzea** eta **Denbora-sarrera editatzea** orrialdeak. Orrialde hauetako negozio-arauetara sartzeko, ireki orrialde bakoitzeko inprimaki-editore, eta hautatu **Enpresa-arauak**. Lehendik dauden negozioaren arauetan egoera gehitu dezakezu baldintzara, edo beste negozioaren arau bat gehitu dezakezu egoera berrian.

### <a name="add-custom-validation-rules"></a>Gehitu balidazio-arau pertsonalizatuak
Bi baliozkotze-arau mota gehi ditzakezu **Asteroko denbora sarrera** sareko esperientzia:

- Orrialdeetan funtzionatzen duten bezeroen alboko negozio-arauak
- Denbora-sarreren eguneratze guztietan aplikatzen diren zerbitzariaren alboko pluginen baliozkotzeak

#### <a name="client-side-business-rules"></a>Bezeroaren aldetik negozio-arauak
Erabili negozioaren arauak eremuak blokeatzeko eta desblokeatzeko, eremuetan balio lehenetsiak sartzeko eta uneko sarrera erregistratik soilik informazioa eskatzen duten balidazioak definitzeko. Orrialde baten negozio-arauetara sartzeko, ireki inprimaki-editore eta, ondoren, hautatu **Enpresa-arauak**. Lehendik dauden negozioaren arauak editatu edo beste negozioaren arau batzuk gehitu ditzakezu.

#### <a name="server-side-plug-in-validations"></a>Zerbitzariaren alboko pluginen baliozkotzeak
Denbora sarrera-erregistro bakarrean eskuragarri dagoena baino testuinguru gehiago behar duten balidazioetarako erabili behar dituzu plug-in-en balioztapenak. Sareko lineako eguneraketetan exekutatu nahi dituzun baliozkotzeetarako ere erabili beharko zenuke. Balidazioak osatzeko, sortu plug-in pertsonalizatu bat **Denbora Sarrera** entitatea.

### <a name="limits"></a>Mugak
Gaur egun, **Denbora sarrera** sareak 500 errenkadako tamaina-muga du. 500 errenkada baino gehiago badaude, gehiegizko errenkadak ez dira erakutsiko. Ez dago tamaina muga hori handitzeko modurik.

### <a name="copying-time-entries"></a>Denbora-sarrerak kopiatzea
Erabili ikuspegia **Kopiatu denbora sartzeko zutabeak** denbora sartzean kopiatu beharreko eremuen zerrenda definitzeko. **Data** eta **Iraupena** derrigorrezko eremuak dira eta ez dira bistatik kendu behar.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
