---
title: Denbora-sarrerak luzatzea
description: Artikulu honetan garatzaileek denbora sartzeko kontrola nola luzatu dezaketen buruzko informazioa ematen da.
author: stsporen
ms.date: 01/27/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 7ed501af3fb2059ab3c3ab6f6c957fe518595d55
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8914755"
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
Denbora-sarrera bakoitza denbora-iturburu erregistro batekin lotzen da. Erregistro honek zehazten du nola eta zein aplikaziotan prozesatu behar duten denbora sarrera.

Denbora-sarrerak hasierako, amaierako eta iraupenarekin lotuta dauden denbora-blokeak dira.

Logikak denbora sartzeko erregistroa automatikoki eguneratuko du egoera hauetan:

- Hurrengo hiru eremuetatik bi ematen badira, hirugarrena automatikoki kalkulatuko da: 

    - **msdyn_start**
    - **msdyn_end**
    - **msdyn_duration**

- **msdyn_start** eta **msdyn_end** eremuek ordu-eremua ezagutzen dute.
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

1. Gehitu pertsonalizatutako eremua **sorrera bizkorreko** elkarrizketa-koadroan.
2. Konfiguratu sareta pertsonalizatutako eremua erakusteko.
3. Gehitu eremu pertsonalizatua **errenkada editatu** edo **denbora-sarrera editatu** orrian, egoki den moduan.

Ziurtatu eremu berriak behar beharrezko balidazioak dituela **errenkada editatu** edo **denbora-sarrera editatu** orrian. Zeregin honen zati gisa, eremua blokeatu behar duzu, denbora-sarreraren egoeran oinarrituta.

Eremu pertsonalizatu bat gehitzen duzunean **Denbora sarrera** sareta eta, ondoren, denbora-sarrerak zuzenean sarean sortu, sarrera horien eremu pertsonalizatua automatikoki ezartzen da errenkadarekin bat etor dadin. 

### <a name="add-the-custom-field-to-the-quick-create-dialog-box"></a>Gehitu pertsonalizatutako eremua sorrera bizkorreko elkarrizketa-koadroan
Gehitu eremu pertsonalizatua **Sorrera azkarra: sortu denboraren-sarrera** elkarrizketa-koadroan. Orduan, erabiltzaileek balio bat sar dezakete denbora hautatuz gehituz gero **Berria**.

### <a name="configure-the-grid-to-show-the-custom-field"></a>Konfiguratu sareta pertsonalizatutako eremua erakusteko
**Asteko denbora-sarrera** saretan eremu pertsonalizatua gehitzeko bi modu daude.

- Pertsonalizatu **Nire asteko denbora-sarrerak** ikuspegia pertsonaliza dezakezu eta gehitu eremu pertsonalizatua bertara. Saretako eremu pertsonalizatuaren posizioa eta tamaina zehaztu ditzakezu ikuspegian propietateak editatuz.
- Sortu denbora-sarrera pertsonalizatuaren beste ikuspegi bat sortu eta ikuspegi lehenetsi gisa ezarri. Ikuspegi horrek **Deskribapena** eta **Kanpoko iruzkinak** eremuak eduki beharko lituzke, saretan eduki nahi dituzun zutabeez gain. Saretako posizioa, tamaina eta multzoaren hurrenkera lehenetsia zehaztu ditzakezu ikuspegian propietateak editatuz. Ondoren, konfiguratu ikuspegi horretarako kontrol pertsonalizatua **Denbora-sarreraren sareta** kontrola izan dadin. Gehitu kontrol hori ikuspegian, eta hautatu **Web**, **telefono**, eta **tableta**. Ondoren, konfiguratu **asteroko denbora-sarrerako** saretako parametroak. Ezarri **hasiera data** eremua **msdyn\_date** gisa, ezarri **Iraupena** eremua **msdyn\_duration** gisa eta ezarri **Egoera** eremua **msdyn\_entrystatus** gisa. **Irakurtzeko soilik egoera-zerrenda** eremua ezarrita dago **192350002 (onartua)**, **192350003 (Bidalketa)**, edo **192350004 (Berriz eskatutakoa)** gisa.

### <a name="add-the-custom-field-to-the-appropriate-edit-page"></a>Gehitu eremu pertsonalizatua editatzeko orri egokira
Ordu-sarrera edo denbora-sarrera errenkada bat editatzeko erabiltzen diren orriak aurki daitezke **Inprimakiak** atalean. **Editatu sarrera** saretako botoiak irekitzen du **Editatu sarrera** orrialdea, eta **Editatu errenkada** botoiak irekitzen du **Errenkadak editatzea** orrialdea. Orrialde hauek edita ditzakezu, eremu pertsonalizatuak izan ditzaten.

Bi aukerek integratutako iragazki batzuk kentzen dituzte **Proiektua** eta **Proiektuaren zeregina** entitateetan, entitateen bilaketa ikuspegi guztiak ikusgai egon daitezen. Laukitik kanpo, bilaketa-ikuspegi garrantzitsuak bakarrik ikus daitezke.

Eremu pertsonalizatuetarako orri egokia zehaztu behar duzu. Seguruenik, eremua saretan gehitzen baduzu, denbora-sarrerako errenkada osora aplikatzen diren eremuetarako erabiltzen den **editatu errenkada** orrian joan beharko litzateke. Eremu pertsonalizatuak egunero balio esklusiboa badu errenkadan (adibidez, eremu pertsonalizatua Amaiera ordua aukerarako), **denbora sarrera editatu** orrian sartu beharko litzateke.

Eremu pertsonalizatua orri batean gehitzeko, arrastatu **Eremua** elementua orrialdeko kokapen egokian eta, ondoren, ezarri bere propietateak.

### <a name="add-new-option-set-values"></a>Gehitu beste aukera multzoen balio batzuk
Aukera multzoaren balioak erabiltzeko prest dagoen eremua gehitzeko, jarraitu urrats hauek.

1. Ireki eremuaren edizio orria eta, ondoren, **Mota** atalean, hautatu **Editatu** aukera aukera multzoaren ondoan.
2. Gehitu etiketa pertsonalizatua eta kolorea dituena beste aukera bat. Denbora-sarreraren beste egoera bat gehitu nahi baduzu, integratutako eremuak **Sarreraren egoera** du izena.

### <a name="designate-a-new-time-entry-status-as-read-only"></a>Izendatu denbora-sarreraren egoera bat irakurtzeko soilik
Denbora-sarreraren egoera berria irakurtzeko bakarrik izendatzeko, gehitu denbora-sarrerako balio berria **Irakurtzeko soilik egoera-zerrenda** propietateari. Ziurtatu zenbakia gehitzea, ez etiketa. Denbora-sarreraren saretaren zati editagarria blokeatuta egongo da egoera berria duten errenkadetarako. Ezartzeko **Irakurtzeko soilik egoera-zerrenda** jabetza ezberdina ezberdinentzat **Denbora Sarrera** ikuspegiak, gehitu **Denbora sarrera** sarea ikuspegi batean **Kontrol pertsonalizatuak** atalean, eta konfiguratu parametroak dagokion moduan.

Ondoren, gehitu negozioaren arauak eremu guztiak blokeatzeko **Errenkadaren edizioa** eta **Denbora-sarreraren edizioa** orrietan. Orrialde hauetako negozioaren arauak atzitu ditzakezu orrirako inprimaki-editorea irekiz eta, ondoren, **Negozioaren arauak** hautatuz. Lehendik dauden negozioaren arauetan egoera gehitu dezakezu baldintzara, edo beste negozioaren arau bat gehitu dezakezu egoera berrian.

### <a name="add-custom-validation-rules"></a>Gehitu balidazio-arau pertsonalizatuak
**Asteko denbora sartzeko** sareta esperientzian gehitu ditzakezun bi balioztatze arau mota daude:

- Orrialdeetan funtzionatzen duten bezeroen alboko negozio-arauak
- Zerbitzariaren aldeko pluginen balioztapenak, sarrera eguneratze guztiei aplikatzen zaizkienak

#### <a name="client-side-business-rules"></a>Bezeroaren aldetik negozio-arauak
Erabili negozioaren arauak eremuak blokeatzeko eta desblokeatzeko, eremuetan balio lehenetsiak sartzeko eta uneko sarrera erregistratik soilik informazioa eskatzen duten balidazioak definitzeko. Orrialde hauetako negozioaren arauak atzitu ditzakezu orrirako inprimaki-editorea irekiz eta, ondoren, **Negozioaren arauak** hautatuz. Lehendik dauden negozioaren arauak editatu edo beste negozioaren arau batzuk gehitu ditzakezu.

#### <a name="server-side-plug-in-validations"></a>Zerbitzariaren aldeko plugin-en baliozkotzeak
Erabili plugin-en balidazioak denbora-sarrera erregistro bakarrean eskuragarri dagoen testuingurua baino gehiago behar duten balidazioetarako. Sareko lineako eguneraketetan exekutatu nahi dituzun baliozkotzeetarako ere erabili beharko zenuke. Balidazioak osatzeko, sortu plugin pertsonalizatua **Denbora-sarrera** erakundean.

### <a name="limits"></a>Mugak
Gaur egun, **Denbora sarrera** sareak 500 errenkadako tamaina-muga du. 500 errenkada baino gehiago badaude, gehiegizko errenkadak ez dira erakutsiko. Ez dago tamaina muga hori handitzeko modurik.

### <a name="copying-time-entries"></a>Denbora-sarrerak kopiatzea
Erabili ikuspegia **Kopiatu denbora sartzeko zutabeak** denbora sartzean kopiatu beharreko eremuen zerrenda definitzeko. **Data** eta **Iraupena** derrigorrezko eremuak dira eta ez dira bistatik kendu behar.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
