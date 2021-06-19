---
title: Pertsonalizatu asteroko denbora-sarrera
description: Gai honek erakundearen praktikak onartzen dituzten negozioaren arau pertsonalizatuak inplementatzeko moduari buruzko informazioa ematen du.
author: stsporen
ms.custom:
- dyn365-projectservice
ms.date: 07/09/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: c117e06e7a5c57c7f9b70d1380f450c0ea97cd12
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6013021"
---
# <a name="customize-weekly-time-entry"></a>Pertsonalizatu asteroko denbora-sarrera 

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Microsoft Dynamics 365 Project Service Automation aplikazioaren 3.3 bertsioan, Microsoft-ek sareta modernoa sartu zuen proiektuen baliabideak azkar sar daitezen aste baterako. Asteko denbora-sarreraren sareak sarrera guztira erakutsi ditzake dataren, errenkadaren edo astearen arabera. Baliabideek asteko denbora-sarreren kopiak egin ditzakete eta baita aurreko asteetakoen kopiatze masiboa ere. Sistemaren pertsonalizatzaileek ikuspegia pertsonaliza dezakete eremuak gehituz, bilaketa beste entitate batzuetara gehituz eta negozioaren arau pertsonalizatuak aplikatuz, beren erakundearen praktikak onartzeko.

Denbora-sarrera eta asteko denbora-sareta berria gunearen maparen bidez atzitzen dira. Lehengo PSA bertsioetako denbora-sarrera pertsonalizatua ez zen hedagarria asteko denbora-sarrera hedagarriarekin ordezkatu da, eta baita ordezko egoera batekin irakurketzeko soilik den saretan eta egutegian. Aldaketa hori dela eta, erabiltzaileek denbora sartu dezakete astero.

## <a name="page-layout"></a>Orriaren diseinua
Asteko denbora-sarrera sareta berria kontrol pertsonalizatua da, eta tresna-barra bat eta bi atal nagusi ditu: **Neurriak** eta **Iraupena**. Tresna-barrak denbora-sarreraren saretarako kontrol pertsonalizatu honetarako bakarrik aplikatzen den botoia du. Aldiz, orriaren goiko aldeko ekintza-paneleko botoiak denbora-sarrerak onartzen dituen hiru kontrol motei aplikatzen zaizkie: asteko denbora-sarreraren kontrola, irakurtzeko soilik kontrola eta egutegiaren kontrola.

### <a name="dimensions"></a>Neurriak
**Neurriak** sekzioak, zutabeetako izenburuak diren neurrian, denboraren aurka sartu daitezkeen dimentsio guztiak erakusten ditu. Hauek dira onartzen diren neurri integratuak:

- Proiektua
- Proiektuaren zeregina
- Funtzioa
- Mota
- Sarreraren egoera

**Neurriak** sekzioak ez du lineako edizioa onartzen. Sekzio honek eremu pertsonalizatuak asteroko denbora-sarreraren saretan gehitzeko aukera ematen duen ikuspegiaren babesa du. Eremu pertsonalizatuak gehitzeari buruzko informazioa eskuratzeko, ikusi "Hedagarritasuna" atala gai honetan aurrerago.

### <a name="duration"></a>Iraupena
Iraupena sekzioak asteko egunak zutabeetako goiburu gisa erakusten ditu. Sekzio honek lineako edizioa ahalbidetzen du. Neurri egokiak dituen denbora-sarreraren errenkada bat sortu ondoren, erabiltzaileek azkar sar dezakete linean neurri horietan igarotzen duten denbora.

## <a name="create-a-new-time-entry"></a>Sortu beste denbora-sarrera bat
Beste denbora-sarrera bat sartzeko denbora-sarreraren saretan, hautatu **Berria**. **Denbora-sarreraren sorrera bizkorra** elkarrizketa-koadroa agertuko da. Elkarrizketa-koadro horretan, erabiltzaileek denbora-sarreraren data aukeratu dezakete, eta, ondoren, **Proiektua**, **Proiektuaren zeregina**, **Funtzioa**, eta **Iraupena** neurrietarako datuak idatzi ditzakete minutu, ordu edo egunetan **h**, **m**, edo **d**, zenbakiarekin batera. Erabiltzaileek kanpokoekin partekatu daitezkeen denbora-sarreraren deskribapenak eta iruzkinak ere sar ditzakete. Erabiltzaileek aldaketak gordetzean, neurrietan sartu dituzten balioak **Neurriak** sekzioan agertzen dira. **Iraupena** eremuan idatzi duten iraupenari buruzko informazioa denbora-sarrera sortu zen datan agertzen da.

Sistemaren ikuspegiek bilatze-eremuak babesten dituzte. Adibidez, erabiltzaile bat proiektu batean sartu ondoren, **Proiektuaren zeregina** eremuan **Kopia** ikuspegi gisa ezarrita dago lehenespenez. Erabiltzaile bati esleitu ez zaizkion zereginetarako denbora-sarrerak sortzeko, hautatu **Aldatu ikuspegia** bilaketaren elkarrizketa-koadroan eta, ondoren, hautatu **Proiektu aktiboko zeregin guztiak** ikuspegia.

## <a name="edit-a-time-entry"></a>Editatu denbora-sarrera
Denbora-sarrera orrialdeko eremu batzuetako xehetasunak, adibidez **Deskribapena** eta **Kanpoko iruzkinak**, ez dira asteroko denbora-sarreraren saretan agertzen. Horren ordez, xehetasun osagarri horiek dituen hiruki adierazle txiki bat agertzen da iraupen-gelaxkan. Hautatu gelaxka eta, ondoren, hautatu **Editatu xehetasunak** aukera **Edizio bizkorra** panelean datuak ikusteko. Asteko denbora-sarrerako denbora-sarearen zati ez den denbora-sarrera jakin baterako editatu edo eguneratzeko, erabiltzaileek **Edizio bizkorra** panela ireki behar dute.

## <a name="copy-a-time-entry-row"></a>Kopiatu denbora-sarreraren errenkada bat
Lehenengo denbora-sarreraren errenkada sortu ondoren, erabiltzaileek **Kopiatu errenkada** aukera dezakete errenkada osoa errenkada berri batean kopiatzeko. Errenkada bat modu horretan kopiatzean, neurriak eta iraupenak ere kopiatzen dira. Erabiltzaileek **Editatu errenkada** ere aukera dezakete neurrien balioak eta iraupenen linean eguneratzeko **Iraupena** sekzioan.

## <a name="open-a-time-entry"></a>Ireki denbora-sarrera
Eremu garrantzitsuenetan sarrera egokiak eta azkarrak onartzeko, asteko denbora-sarreraren saretak hautatutako neurrien eta denboraren iraupenaren azpimultzoa erakusten du. Denbora-sarrera bakarraren xehetasun guztiak ikusteko, **Editatu sarrera** atalean, hautatu **Ireki**.

## <a name="submit-a-time-entry"></a>Bidali denbora-sarrera bat
Erabiltzaileek denbora-sarrera bakar bat edo denbora-sarreren talde bat bidal dezakete gelaxka bloke bat edo denbora-sarrera errenkada oso bat aukeratuz eta, ondoren, **Bidali** hautatuta. Bidalitako denbora-sarrerak onesteko zain dauden sarrera gisa agertzen dira onartzailearen **Onespena** orrian. Denbora-sarrerak bidali ondoren, ezin dira editatu.

## <a name="recall-a-time-entry"></a>Berreskuratu denbora-sarrera bat
Bidali dituzun denbora-sarrerak berreskura ditzakezu. Denbora-sarrera bakarra, denbora-arreren bloke bat edo denbora-sarreren errenkada oso bat berreskuratu dezakezu. Berreskuratutako denbora-sarrerak eskuragarri daude editatzeko baliabideetarako.

## <a name="time-entry-status"></a>Denbora-sarreraren egoera
Denbora-sarrera berriei automatikoki esleitzen zaie **Zirriborroa** egoera. Denbora-sarrera bidaltzen denean, **Bidalita** egoerara eguneratzen da. Bidalitako denbora-sarrera onartzen denean, **Onartuta** egoerara eguneratzen da. Denbora-sarrera onartzen ez bada, **Itzulia** egoera eguneratuko da, eta sarrera eskuragarri egongo da zuzentzeko eta berriz bidaltzeko. **Zirriborroa** egoera duten denbora-sarrerak soilik ezaba daitezke.

## <a name="view-rejection-comments"></a>Ikusi baztertze-iruzkinak
Onartzaile batek denbora-sarrera bat baztertzen duenean, onartzaileak baztertze-iruzkinak gehitu ditzake baliabideak baztertzearen zergatia uler dezan. Denbora-sarrera baten baztertze-iruzkinak ikusteko, hautatu **Ireki sarrera**. Baztertze-iruzkinak kronologian erakutsiko dira. Kronologian, baliabideak baztertze-iruzkinei erantzun diezaiekete sarrera berriro bidali aurretik.

## <a name="copy-week"></a>Kopiatu astea
Zenbait denbora-sarrera sortu ondoren, erabiltzaileek **Kopiatu astea** aukera dezakete denbora-sarrera gehigarriak gehitzeko modu masiboan. **Kopiatu** elkarrizketa-koadroa agertuko da. **Aldi honetatik** sekzioan, erabili **Hasiera data** eta **Amaiera Data** eremuak denbora-sarrerak kopiatu behar diren data-tartea zehazteko. **Aldira** atalean, **Hasiera data** eremuan, zehaztu zein datarako sortu nahi dituzun sarrerak. Ondoren, hautatu **Kopiatu**. "Amera" aldian zehaztutako datarako, "Hasiera" aldian dagokion asteko egunerako denbora-sarreren kopia sortzen da. Adibidez, asteleheneko pasa den asteko denbora-sarrera "amaiera" aldian zehazten den asteko astelehenean kopiatzen da.

## <a name="import"></a>Inportatu
Oinarrizko prozesu bera erreserbetatik, zereginetatik eta trukeetatik inportatzeko erabiltzen da. Erabiltzaileek erreserbak inportatzen diren tokiko data-tartea zehaztu dezakete. Ondoren, modu esplizituan hautatu behar dituzte zirriborroen denbora-sarreretan kopiatu beharko liratekeen erreserbak. Aurreko bertsioan, iradokitako denbora-sarrerak saretan eta egutegian agertu ziren eta saioa berritzean galdu ziren.

## <a name="extensibility"></a>Hedagarritasuna
### <a name="add-custom-fields-that-have-lookups-to-other-entities"></a>Gehitu bilaketak dituzten eremu pertsonalizatuak beste entitateetan
Asteko denbora-sarrera saretan eremu pertsonalizatua gehitzeko hiru urrats nagusi daude.

1.  Gehitu pertsonalizatutako eremua sorrera bizkorreko elkarrizketa-koadroan.
2.  Konfiguratu sareta pertsonalizatutako eremua erakusteko.
3.  Gehitu eremu pertsonalizatua errenkadaren zeregin-fluxura edo gelaxka editatzeko zeregin-fluxura, hala badagokio.

Ziurtatu eremu berriak behar beharrezko balidazioak dituela errenkadan edo gelaxka editatzeko zeregin-fluxuan. Urrats honen zati gisa, eremua blokeatu behar duzu, denbora-sarreraren egoeran oinarrituta.

#### <a name="add-the-custom-field-to-the-quick-create-dialog-box"></a>Gehitu pertsonalizatutako eremua sorrera bizkorreko elkarrizketa-koadroan
Eremu pertsonalizatua gehitu behar duzu Sortu denboraren-sarreraren sorrera bizkorra elkarrizketa-koadroan. erabiltzaileek horren balioa sar dezaten denbora-sarrerak gehitzen dituztenean **Berria** botoia erabiliz.

#### <a name="configure-the-grid-to-show-the-custom-field"></a>Konfiguratu sareta pertsonalizatutako eremua erakusteko
Asteko denbora-sarrera saretan eremu pertsonalizatua gehitzeko bi modu daude. Lehen aukera, **Nire asteko denbora-sarrerak** ikuspegia pertsonalizatzea da eta gehitu eremu pertsonalizatua bertara. Saretako eremu pertsonalizatuaren posizioa eta tamaina aukeratu ditzakezu ikuspegian propietateak editatuz.

Bigarren aukera denbora-sarrera pertsonalizatuaren beste ikuspegi bat sortzea eta ikuspegi lehenetsi gisa ezartzea da. Ikuspegi horrek **Deskribapena** eta **Kanpoko iruzkinak** eremuak eduki beharko lituzke, saretan eduki nahi dituzun zutabeez gain. Saretako posizioa, tamaina eta multzoaren hurrenkera lehenetsia aukeratu ditzakezu ikuspegian propietateak editatuz. Ondoren, konfiguratu ikuspegi horretarako kontrol pertsonalizatua **Denbora-sarreraren sareta** kontrola izan dadin. Gehitu kontrol hori ikuspegian, eta hautatu web, telefono eta tabletetarako. Ondoren, konfiguratu asteako denbora-sarrerako saretako parametroak. Ezar ezazu **Hasiera data** eremua **msdyn_date** gisa, ezarri **Iraupena** eremua **msdyn_duration** gisa eta ezarri **Egoera** eremua **msdyn_entrystatus** gisa. Ikuspegi lehenetsirako, **Irakurtzeko soilik den egoera-zerrenda** eremua **192350002,192350003,192350004** gisa dago ezarrita, **Errenkada editatzeko zeregin-fluxua** eremuan **msdyn_timeentryrowedit** gisa eta **Gelaxka editatzeko zeregin-fluxua** eremuan **msdyn_timeentryedit** gisa. Eremu hauek pertsonaliza ditzakezu irakurtzeko soilik egoera gehitzeko edo kentzeko, edo zereginetan oinarritutako egoera (TBX) bat erabil dezakezu errenkada edo gelaxka editatzeko. Eremu hauek balio estatiko batera lotu beharko lirateke.

#### <a name="add-the-custom-field-to-the-appropriate-edit-task-flow"></a>Gehitu eremu pertsonalizatua editatzeko zeregin-fluxu egokira
Editatzeko erabiltzen diren TBX orriak **Prozesuak** atalean daude. Lehenetsitako orriak honako hauek dira: **Project Service - Denbora-sarreraren errenkadaren edizioa** eta **Project Service - Denbora-sarreraren edizioa**. Orrialde lehenetsi hauek edita ditzakezu edo TBX orrialde pertsonalizatuak sor ditzakezu.

> [!NOTE] 
> Bi aukerek integratutako iragazki batzuk kenduko dituzte **Proiektua** eta **Proiektuaren zeregina** entitateetan, entitateen bilaketa ikuspegi guztiak ikusgai egon daitezen. Laukitik kanpo, bilaketa-ikuspegi garrantzitsuak bakarrik ikus daitezke.

Eremu pertsonalizatuetarako zeregin-fluxu egokia zehaztu behar duzu. Seguruenik, eremua saretan gehitzen baduzu, denbora-sarrerako errenkada osora aplikatzen diren eremuetarako erabiltzen den errenkadako zeregin-fluxuan joan beharko litzateke. Eremu pertsonalizatuak egunero balio esklusiboa badu, adibidez, eremu pertsonalizatua **Amaiera ordua** aukerarako,zeregin-fluxuaren edizioa gelaxkan sartu beharko litzateke.

Eremu pertsonalizatua zeregin-fluxu batean gehitzeko, arrastatu **Eremua** elementua orrialdeko kokapen egokian eta, ondoren, ezarri bere propietateak. Ezar ezazu **Iturria** jabetza **Denbora-sarrera** gisa, eta ezarri **Datu-eremua** propietatea eremu pertsonalizaturako. **Eremua** propietateak TBX orrian agertzen den bistaren izena zehazten du. Eremuan egindako aldaketak gordetzeko, sakatu **Aplikatu**. Orriari egindako aldaketak gordetzeko, sakatu **Eguneratu**.

Horren ordez TBX orrialde pertsonalizatu bat erabiltzeko, sortu beste prozesu bat. Ezarri kategoria **Negozio-prozesuaren fluxua** gisa, ezarri entitatea **Denbora-sarrera** gisa eta zehaztu negozio-prozesu mota **Exekutatu prozesua zeregin-fluxu gisa** bezala. **Propietateak** aukeran, **Orriaren izena** propietatea orrialdearen bistaratzeko izenean ezarri behar da. Gehitu eremu garrantzitsu guztiak TBX orrialdean. Gorde eta aktibatu prozesua eta, ondoren, eguneratu zeregin-fluxuari dagokion kontrol pertsonalizatuaren propietatea **Izena** baliora prozesuan.

### <a name="add-new-option-set-values"></a>Gehitu beste aukera multzoen balio batzuk
Aukera multzoaren balioak integratutako eremu batean gehitzeko, ireki eremuaren edizio orria eta, ondoren, **Mota** atalean, hautatu **Editatu** aukera aukera multzoaren ondoan. Ondoren, gehitu etiketa pertsonalizatua eta kolorea dituena beste aukera bat. Denbora-sarreraren beste egoera bat gehitu nahi baduzu, integratutako eremuak **Sarreraren egoera** du izena, ez **Egoera**.

### <a name="designate-a-new-time-entry-status-as-read-only"></a>Izendatu denbora-sarreraren egoera bat irakurtzeko soilik
Denbora-sarreraren egoera berria irakurtzeko bakarrik izendatzeko, gehitu denbora-sarrerako balio berria (kopurua, ez etiketa) **Irakurtzeko soilik egoera-zerrenda** propietateari. Denbora-sarreraren saretaren zati editagarria blokeatuta egongo da egoera berria duten errenkadetarako.
Ondoren, gehitu negozioaren arauak eremu guztiak blokeatzeko **Denbora-sarreraren errenkadaren edizioa** eta **Denbora-sarreraren edizioa** TBX orrietan. Orrialde hauetako negozioaren arauak atzitu ditzakezu orrirako negozio-prozesuaren fluxu editorea irekiz eta, ondoren, **Negozioaren arauak** hautatuz. Lehendik dauden negozioaren arauetan egoera gehitu dezakezu baldintzara, edo beste negozioaren arau bat gehitu dezakezu egoera berrian.

### <a name="add-custom-validation-rules"></a>Gehitu balidazio-arau pertsonalizatuak
Asteko denbora-sarrerako saretaren egoera gehitzeko bi balidazio-arau mota daude: •   Elkarrizketa-koadro azkarretan eta TBX orrietan lan egiten duten bezeroen alboko negozioaren arauak •   Denbora-sarreren eguneratze guztiei aplikatzen zaizkien zerbitzariaren alboko plugin balioztapenak.

#### <a name="business-rules"></a>Negozioaren arauak
Erabili negozioaren arauak eremuak blokeatzeko eta desblokeatzeko, eremuetan balio lehenetsiak sartzeko eta uneko sarrera erregistratik soilik informazioa eskatzen duten balidazioak definitzeko. TBX orrialde bateko negozioaren arauak atzitu ditzakezu orrirako negozio-prozesuaren fluxu editorea irekiz eta, ondoren, **Negozioaren arauak** hautatuz. Lehendik dauden negozioaren arauak editatu edo beste negozioaren arau batzuk gehitu ditzakezu. Balidazio pertsonalizatuagoak lortzeko, negozioaren araua erabil dezakezu JavaScript exekutatzeko.

#### <a name="plug-in-validations"></a>Plugin-en balidazioak
Plugin-en balidazioak erabili beharko zenituzke denbora-sarrera erregistro bakarrean eskuragarri dagoen testuingurua baino gehiago behar duten balidazioetarako edo saretako lineako eguneratzeetan exekutatu nahi dituzun balidazioetarako. Balidazioa osatzeko, sortu plugin pertsonalizatua **Denbora-sarrera** erakundean.

> [!IMPORTANT] 
> Gaur egun, TBX orrietan ezagutzen den arazo batek erabiltzaileei informazioa zuzentzea eta berriro "Eginda" aukeratzea galarazten die eguneratzeak pluginen balioztapena huts egiten duenean. Konponbide gisa, konfiguratu negozioaren arauen balidazioa egoera hori ahalik eta gehien saihesteko.


[!INCLUDE[footer-include](../includes/footer-banner.md)]