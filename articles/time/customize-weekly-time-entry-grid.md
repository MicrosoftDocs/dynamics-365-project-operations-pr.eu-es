---
title: Denbora-sarrerak luzatzea
description: Artikulu honetan, garatzaileek denbora-sarreraren kontrola nola handitu dezaketen erakusten da.
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
Denbora-sarrera bakoitza denbora-iturburu erregistro batekin lotzen da. Erregistro horrek zehazten du zer aplikazio prozesatu behar diren denbora-sarreran eta nola.

Denbora-sarrerak hasierako, amaierako eta iraupenarekin lotuta dauden denbora-blokeak dira.

Logikak denbora sartzeko erregistroa automatikoki eguneratuko du egoera hauetan:

- Hurrengo hiru eremuetatik bi ematen badira, hirugarrena automatikoki kalkulatuko da: 

    - **msdyn_start**
    - **msdyn_end**
    - **msdyn_duration**

- **msdyn_start eta** msdyn_end **zelaiak** ordu-eremuaren jakitun dira.
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

1. Gaineratu eremu pertsonalizatua elkarrizketa-koadro **azkarrari**.
2. Konfiguratu sareta pertsonalizatutako eremua erakusteko.
3. Gaineratu eremu pertsonalizatua ordu-sarrerako edizio-orrira **·**, dagokionaren **arabera.**

Ziurtatu eremu berriak beharrezko balidazioak dituela ordu-sarrerako edizio-orrian **·** **.** Lan horren parte gisa, zelaia blokeatu egiten du, denbora-sarreraren egoeraren arabera.

Denbora-sarrerako **laukiari** eremu pertsonalizatu bat gehitzen zaionean eta, ondoren, laukian zuzenean denbora-sarrerak sortzen direnean, sarrera horietarako eremu pertsonalizatua automatikoki ezartzen da ilararekin bat etor dadin. 

### <a name="add-the-custom-field-to-the-quick-create-dialog-box"></a>Elkarrizketa-koadroari eremu pertsonalizatua gehitzea
Gaineratu eremu pertsonalizatua **elkarrizketa-koadroari: Denbora-sarrera** sortzea. Orduan, erabiltzaileek balio bat sar dezakete denbora hautatuz gehituz gero **Berria**.

### <a name="configure-the-grid-to-show-the-custom-field"></a>Konfiguratu sareta pertsonalizatutako eremua erakusteko
Astean zehar sartzeko laukiari **eremu pertsonalizatu** bat gehitzeko bi modu daude.

- Ikus ezazu **nire asteko denbora-sarrerak** eta eman eremu pertsonalizatua. Laukian eremu pertsonalizatuaren kokaera eta tamaina zehaztu ditzakezu, ikusmenaren propietateak argitaratuz.
- Denbora pertsonalizatuaren beste bista bat sortzen du, eta aurrez zehaztutako ikusmena bezain establizkala. Ikustaldi honek kanpoko deskribapen **- eta** iruzkin-eremuak izan **behar ditu**, baita laukiak izatea nahi duen zutabeak ere. Laukiaren kokaera, tamaina eta ordena aurrez zehaztua zehaztu ditzakezu, ikusmenaren propietateak argitaratuz. Ondoren, konfiguratu ikuspegi horretarako kontrol pertsonalizatua **Denbora-sarreraren sareta** kontrola izan dadin. Gaineratu kontrol hori bistan eta hautatu Web, Telefono eta **Tabletarako**.**·** **·** Jarraian, konfiguratu asteko sarrera-laukirako **parametroak**. **Msdyn date-n** **\_ hasierako data** ezarri, msdyn **duration-en** **Duration\_ zelaia ezarri** eta msdyn **entrystatus-en** Status **\_ zelaia** ezarri. Irakurketa-zerrendaren eremua **192350002 (Onartua),** **192350003 (Bidalia) edo** 192350004 (Eskatutako erretiratzea) **ezartzen** da.**·**

### <a name="add-the-custom-field-to-the-appropriate-edit-page"></a>Eremu pertsonalizatua edizio-orri egokira gehitzea
Denbora-sarrera bat edo denbora-sarrera ilara bat editatzeko erabiltzen diren orriak formularioetan **aurki** daitezke. Editar sarrera **botoiak Editar sarrera** orrialdea **ireki** eta Editar fila **botoiak edizio** orrialdea ireki du **.** Orri hauek editatu ditzakezu, eremu pertsonalizatuak izan daitezen.

Project **eta** Project Task erakundeetan erabiltzeko prest dauden **iragazki batzuk kendu dituzte bi aukera horiek**, erakundeak bilatzeko ikuspegi guztiak ikusgai egon daitezen. Laukitik kanpo, bilaketa-ikuspegi garrantzitsuak bakarrik ikus daitezke.

Eremu pertsonalizaturako orrialde egokia zehaztu behar du. Litekeena da, zelaia laukian gehituz gero, denbora-sarrera osoari aplikatzen zaizkion zelaietarako erabiltzen den ilara-orrira **joan** beharko lukeela. Eremu pertsonalizatuak balio bakarra badu ilaran egunero (adibidez, amaiera-ordurako eremu pertsonalizatua bada), denbora-sarreraren edizio-orrira **joan** behar du.

Eremu pertsonalizatua orri bati gehitzeko, eraman elementu **bat** orrialdearen posizio egokira eta, ondoren, bere propietateak ezarri.

### <a name="add-new-option-set-values"></a>Gehitu beste aukera multzoen balio batzuk
Erabiltzeko prest dauden zelai batera aukera-balioak gehitzeko, jarraitu pauso hauek.

1. Orria entzun Orria entzun **2019ko** **edizioaren orrialdea**.
2. Gehitu etiketa pertsonalizatua eta kolorea dituena beste aukera bat. Ordu-sarrera berri bat gehitu nahi baduzu, erabiltzeko prest dagoen eremuari sarrera-estatua **deritzo**.

### <a name="designate-a-new-time-entry-status-as-read-only"></a>Izendatu denbora-sarreraren egoera bat irakurtzeko soilik
Denbora-sarreraren egoera berria irakurtzeko bakarrik izendatzeko, gehitu denbora-sarrerako balio berria **Irakurtzeko soilik egoera-zerrenda** propietateari. Ziurtatu zenbakia gehitu behar duzula, ez etiketa. Denbora sarrerako laukiaren zati editagarria blokeatuko da orain egoera berria duten lerroentzat. Denbora-sarrerako **bista desberdinetarako** irakurketa-egoeraren **zerrenda modu desberdinean ezartzeko**, gaineratu ordu-sarrerako **laukiari** ikustaldi baten kontrol pertsonalizatuak **atalean**, eta konfigura itztu parametroak, dagokionaren arabera.

Jarraian, negozio arauak gaineratu, ordu-sarrerako **edizio** eta **ilarako** esparru guztiak blokeatzeko. Orri hauen negozio-arauak eskuratu ahal izateko, ireki orri bakoitzaren inprimaki-editorea eta, ondoren, negozio-arauak **aukeratzea**. Lehendik dauden negozioaren arauetan egoera gehitu dezakezu baldintzara, edo beste negozioaren arau bat gehitu dezakezu egoera berrian.

### <a name="add-custom-validation-rules"></a>Gehitu balidazio-arau pertsonalizatuak
Asteko sarrera-laukiaren **esperientziarako** bi balidazio-arau mota erans ditzakezu:

- Bezeroaren aldeko negozio-arauak, orrietan funtzionatzen dutenak
- Zerbitzariaren aldeko plug-in balidazioak, garai guztietako sarrera-eguneratzeei aplikatzen zaizkienak

#### <a name="client-side-business-rules"></a>Bezeroaren aldeko negozio-arauak
Erabili negozioaren arauak eremuak blokeatzeko eta desblokeatzeko, eremuetan balio lehenetsiak sartzeko eta uneko sarrera erregistratik soilik informazioa eskatzen duten balidazioak definitzeko. Orri bateko negozio-arauak eskuratu ahal izateko, ireki inprimaki-editorea eta, ondoren, negozio-arauak **aukeratu**. Lehendik dauden negozioaren arauak editatu edo beste negozioaren arau batzuk gehitu ditzakezu.

#### <a name="server-side-plug-in-validations"></a>Zerbitzariaren aldeko plug-in balidazioak
Plug-in balidazioak erabili behar ditu denbora-sarrerako erregistro bakar batean eskuragarri dagoena baino testuinguru handiagoa behar duen edozein balidaziotazio egiteko. Laukian lineako eguneratzeetan egin nahi duen edozein balidaziotarako ere erabili behar ditu. Balidazioak osatzeko, Time Entry **erakundean osagarri pertsonalizatua sortzen du**.

### <a name="limits"></a>Mugak
Gaur egun, **denbora sartzeko** laukiak 500 lerroko muga du. 500 lerro baino gehiago baldin badaude, ez dira soberan dauden lerroak erakutsiko. Ez tamaina-muga hori handitzeko modurik.

### <a name="copying-time-entries"></a>Denbora-sarrerak kopiatzea
Erabili ikuspegia **Kopiatu denbora sartzeko zutabeak** denbora sartzean kopiatu beharreko eremuen zerrenda definitzeko. **Data** eta **Iraupena** derrigorrezko eremuak dira eta ez dira bistatik kendu behar.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
