---
title: Proiektuaren baliabideak
description: Gai honek proiektuaren baliabideei buruzko informazioa ematen du.
author: KimANelson
manager: AnnBe
ms.date: 09/14/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: f9352465f83abe19097945dd34eada365cd03b8f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748801"
---
# <a name="project-resourcing"></a>Proiektuaren baliabideak

[!include [banner](../includes/banner.md)]

Gai honek proiektuaren baliabideei buruzko informazioa ematen du.

Proiektuen kudeatzaileek eta baliabideen kudeatzaileek erronka bat proiektuaren plangintza fasean baliabideen esleipena da, non proiektuan lan egiteko baliabide zuzena zehaztu eta erreserbatu behar duten. Urtean Dynamics 365 Finance, Proiektuetarako baliabideen gaitasunak konpromiso jakin baterako edo konpromiso baten zati baterako gorde daitezkeen aldi baterako baliabide gisa tratatzen diren rolak definitzen uzten dizu. Baliabide mota honekin proiektuen kudeatzaileek eta baliabideen kudeatzaileek zeregin hauek bete ditzakete:

- Definitu eskatutako gaitasunak dituen eginkizuna, baliabideak parekatzea erraza izan dadin.
- Erabili rolak gordetako baliabideetan oinarritutako hasierako konpromiso programa definitzeko.
- Kostuak kalkulatu eta hasierako aurrekontua zehaztu, proiektu baterako eginkizun eta baliabideetan oinarrituta.
- Erabili rolak konpromiso bakoitzerako beharrezkoak diren baliabideen erreserbak zenbatesteko.
- Kalkulatu proiektu baten bizitza ziklo osorako beharrezkoak diren baliabide kopurua.
- Zirriborroa lanen banakako egitura (WBS), hasierako baliabideen esleipenak erabiliz.

[![Proiektuaren bizitza zikloa](./media/projectresourcing02-1024x812.jpg)](./media/projectresourcing02.jpg)

Proiektuaren plangintza aurrera doan heinean, aurreikusitako baliabideak langileekin hornitu daitezke. Proiektuaren kudeatzaileak atzera egin eta baliabideen erreserbak eguneratu ditzake proiektuaren edozein fasetan.

## <a name="set-up-project-resources"></a>Konfiguratu proiektuan baliabideak
Egutegia konfiguratu eta langile batekin edo langile batekin lotu behar duzu. Egutegia proiektua eta proiekturako gordetako baliabideen lanaldia antolatzeko erabiltzen da. Egutegia konfiguratzerakoan, proiektuen kudeatzaileek baliabideen berdinketa egin dezakete baliabideak optimizatzearen barruan. Egutegiaren ordutegian oinarrituta, baliabideetan murrizketak jar daitezke. Egutegia konfigura dezakezu **Egutegiak** orrialdea.

Langile bat proiektuaren baliabide gisa konfiguratzen duzunean, enpresan lan egiten duten langileen artean baliabideak konfiguratzen ari zarenetik hauta dezakezu. Bestela, zure erakundeko beste enpresa batzuetako langileak hauta ditzakezu. Langile horiek enpresen arteko baliabideak bezala ezagutzen dira.

Ondorengo prozedurek langile bat zure enpresan proiektuaren baliabide gisa nola konfiguratu eta enpresen arteko proiektuaren baliabide bat nola konfiguratu azaltzen dute.

### <a name="set-up-a-worker-as-a-project-resource"></a>Konfiguratu langilea proiektuaren baliabide gisa

1. Gainean **Langileak** orrialdean, **Langileak** zerrenda, hautatu proiektuaren baliabide gisa gehitzen ari zaren langilea eta ireki langilearen erregistroa.
2. Ekintza panelean, hautatu **Proiektua** &gt; **Konfigurazioa** &gt; **Proiektuaren konfigurazioa**.
3. Aukeratu egutegi bat eta itxi orria.

Baliabide baterako proiektu lehenetsiak ere zehaztu ditzakezu aurrez esleitzeko mota gisa. Aurrez esleipenak baliabideen kudeatzaileak edo proiektuaren kudeatzaileak baliabideak aldez aurretik zein proiektutan landuko dituen dakienean erabil daitezke. Aurretiazko esleipenak proiektuaren babesle edo bezero baten eskaeran oinarrituta ere egin daitezke. Proiektu bat aurrez esleitzeko, **Proiektuak esleitu** orrialdean, **Proiektuak** fitxan, **Gainerako proiektuak** zerrenda, hautatu proiektu egokia.

### <a name="set-up-an-intercompany-resource"></a>Konfiguratu enpresen arteko baliabide bat

Langilea enpresen arteko baliabide gisa konfiguratzen duzunean, konfigurazioa osatu behar duzu bai mailegu-enpresan bai mailegu-enpresan.

**Mailegu-enpresan**

1. Finantzetan, egiaztatu enpresa mailegu-emailea hautatuta dagoela eta, ondoren, osatu aurreko ataleko prozedura, "Konfiguratu langilea proiektuaren baliabide gisa."
2. **Konpainia arteko kontua** orrian, hautatu **Berria**.
3. **Pertsona juridikoaren IDa** eremuan, hautatu mailegu-enpresa. Bete gainerako eremuak egoki gisa, eta gero hautatu **Gorde**.
4. **Transferitzeko prezioa** orrian, hautatu **Berria**.
5. **Hartu legezko entitatea** eremuan, hautatu konpainia egokia.
6. Mailegu-enpresari atal honen hasieran sortu zenituen baliabideak soilik emateko **Baliabidea** eremuan, hautatu sortu duzun baliabidearen izena. Mailegu-enpresaren baliabide guztiak mailegu-enpresaren eskura jartzeko, utzi **Baliabidea** eremua hutsik.
7. Gainean **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdean, **Enpresa artekoa** fitxa, ezarri **Gaitu enpresen arteko baliabideen programazioa eta denbora-orriak** aukera **Bai**.

**Hartutako konpainian**

- Gainean **Baliabideen zerrenda** orrian, bilaketa-iragazkian, idatzi mailegu-enpresarentzat sortu duzun baliabidearen izena, izena mailegu-enpresaren baliabideen zerrendan sartuta dagoela egiaztatzeko.

## <a name="manage-resource-competencies"></a>Kudeatu baliabide-gaitasunak
Baliabideen gaitasunak baliabideen kudeaketaren funtsezko atala dira. Gaitasunak oinarri gisa erabil daitezke gaitasunen, hezkuntzaren, ziurtagirien eta proiektuaren esperientzia oreka zuzena duten baliabideak zehazteko. Informazio hau baliabide bakoitzerako konfiguratu eta erregularki eguneratu beharko zenuke. Modu honetan, gaitasunak maximizatu ditzakezu proiektuaren baliabideak esleitzean baliabide-gaitasun zehatzak parekatzen direnean.

[![Gaitasunen, ziurtagirien, hezkuntzaren eta proiektuaren esperientziaren adibideak](./media/projectresourcing06-1024x383.jpg)](./media/projectresourcing06.jpg)

Ondorengo prozedurek baliabide baterako konpetentzia batzuk nola konfiguratu azaltzen dute.

Langilearen konpetentziak konfiguratzeko, bai erabil dezakezu **Langileak** zerrenda Giza baliabideak edo **Baliabideak** zerrenda orria Proiektuen kudeaketan eta kontabilitatean. Ondorengo prozeduretarako, **Langileak** Giza baliabideak ataleko zerrenda erabiltzen da.

### <a name="set-up-competencies-certificates"></a>Konfiguratu gaitasunak: ziurtagiriak

1. Gainean **Langileak** zerrendaren orria, hautatu langileari ziurtagiriaren informazioa gehitzeko.
2. Ekintza panelean, **Langilea** fitxan, **Konpetentziak** taldea, hautatu **Ziurtagiriak**.
3. Hautatu **Berria**, eta gero, **Ziurtagiriaren mota** eremua, hautatu **PMP**.
4. **Hasiera data** eremua, hautatu **2015/10/01**, eta hautatu **Gorde**.

### <a name="set-up-competencies-skills"></a>Konfiguratu gaitasunak: gaitasunak

1. Gainean **Langileak** zerrendako orria, ziurtatu aurreko prozeduran erabili zenuen langilea oraindik hautatuta dagoela. Orduan, ekintza panelean, **Langilea** fitxan, **Konpetentziak** taldea, hautatu **Gaitasunak**.
2. Hautatu **Berria**.
3. **Trebetasuna** eremua, hautatu **Proiektu-kudeaketa**.
4. **Maila** eremua, hautatu **5 Aditua**.
5. **Mailaren data** eremua, hautatu **2014/01/14**.
6. **Urteetako esperientzia** eremua, sartu **10**.
7. Aukeratu **Gorde**, eta gero itxi orria.

## <a name="create-a-new-project"></a>Sortu proiektua
1. **Proiektuaren kudeaketa** orria, hautatu **Proiektu berria**, eta idatzi hurrengo balioak:

    - **Proiektu mota:** Denbora eta materiala
    - **Proiektuaren izena:** XYZ berritzea 2. fasea
    - **Proiektu taldea:** TM\_WIP
    - **Proiektuaren kontratua ID:** 00000002

2. Hautatu **Sortu proiektua**.

### <a name="assign-a-resource-to-a-project"></a>Esleitu baliabide bat proiektu bati

1. Gainean **Langileak** orrialdean, **Langileak** zerrenda, hautatu erregistroa langilearentzat aurretik konfiguratu gaitasunak horretarako, eta ireki langilearen erregistroa.
2. Ekintza panelean, **Proiektua** fitxan, **Konfigurazioa** taldea, hautatu **Esleitu proiektuak**.
3. Gainean **Baliabideak balioztatzeko proiektuaren esleipenak** orrialdean, **Proiektuak** fitxan, **Gehitu proiektua hautatutako proiektuei** eremua, iragazkia **XYZ berritzea 2. fasea** proiektua.
4. **Gainerako proiektuak** panelean, hautatu proiektu bat eta, ondoren, hautatu gezi botoia gehitzeko **Aukeratutako proiektuak** panela.

Baliabide batentzako kategoriak ere eska ditzakezu nahi duzun moduan. Kategoria mota bai da **Kostua** edo **Diru-sarrerak**. Kategoria mota zure erakundeak zehazten du. Baliabide batentzako kategoriarik esleitzen ez bada, Finantzak kostuen eta diru-sarreren orduen prezioen kategoria lehenetsia bilatzen du.

### <a name="set-up-project-resource-and-role-characteristics"></a>Ezarri proiektuaren baliabideen eta rolen ezaugarriak

Proiektu kudeatzaile batek proiektuaren baliabideen funtzionalitatea erabil dezake proiektuan beharrezkoak diren rolak sortzeko. Rolak erabil daitezke baliabideak erreserbatzen direnean berretsitako baliabideak oraindik ezezagunak badira. Eginkizunak aldi baterako gorde daitezke aurreikusitako baliabide gisa, proiektuaren plangintza faseak jarraitu ahal izateko.

[![Rol baten adibidea](./media/projectresourcing05.jpg)](./media/projectresourcing05.jpg) 

**Eszenatokia:** Contoso kontratatu zen onartutako proiektuen karta duen Denbora eta material proiektu bat osatzeko. Proiektu zuzendari gaztea proiektuaren esparrua osatzen ari da oraindik. Baliabideen kudeatzailea proiektu berrian lan egiteko gordetako baliabide zehatzak identifikatzen ari da. Proiektuaren izaera kritikoa dela eta, proiektuaren babesleak proiektu nagusiko zuzendaria eskatu zuen eginkizunetako bat izateko. Baliabideen kudeatzaileak baliabide berria eskuratu behar du eta sistemako rola definitu behar du, proiektuaren kudeatzaile juniorrak proiektuaren plangintza egitean baliabideen informazioa behar badu.

Ondorengo pausoek erakusten dute baliabideen kudeatzaileak proiektuaren arduradun nagusiaren eginkizuna nola konfigura dezakeen eta baliabideen ezaugarriak harekin lotzen dituen. Geroago, eginkizuna eskatutako baliabideen eskumenekin bat datozen baliabide erabilgarriak bilatzeko erabil daiteke.

1. **Konfigurazio-funtzioak** orria, hautatu **Berria**, eta idatzi hurrengo balioak:

    - **Rolaren IDa:** Proiektu zuzendari nagusia
    - **Deskribapena:** Proiektu zuzendari nagusia

2. Hautatu **Sortu**.
3. Aukeratu **Proiektu zuzendari nagusia** rola, eta hautatu **Ezaugarriak konfiguratu**.
4. **Ezaugarri mota** eremua, hautatu **Gaitasuna**.
5. **Erabilgarri dauden ezaugarriak** eremuan, sartu bilatu beharreko trebetasuna.
6. **Ezaugarrien mota** eremua, hautatu **Ziurtagiria**.
7. **Erabilgarri dauden ezaugarriak** eremuan, sartu bilatu beharreko ziurtagiri mota.

### <a name="assign-a-project-resource-to-a-project"></a>Esleitu proiektuaren baliabide bat proiektu bati

1. Gainean **Proiektu guztiak** orria, hautatu **XYZ berritzea 2. fasea** proiektua.
2. Gainean **Proiektu taldea eta programazioa** fitxa, hautatu **Gehitu**.
3. **Rola** eremua, hautatu **Taldekidea**.
4. Hautatu **Erreserbatu egutegia**.
5. Gainean **Baliabideen erabilgarritasuna** orrialdea, hautatu **Ikusi ezarpenak**.
6. Gainean **Doitu ikuspegiaren ezarpenak** orrian, sartu balio hauek:

    - **Data tartea ikusteko formatua:** Eguna
    - **Bistaratu erabilgarritasunaren deskribapenak:** Bai
    - **Gainerako edukiera bistaratu:** Bai

7. Baliabide-zerrendan, hautatu baliabidea.
8. Aukeratu **Liburu gogorra** eta **Edukiera osoa**.


### <a name="assign-a-resource-to-a-default-role"></a>Esleitu baliabidea lehenetsitako funtzioa

Proiektu edo baliabideen kudeatzaileek proiektu baterako gorde daitezkeen baliabideak sakondu ditzakete. Rol lehenetsia lehendik dagoen baliabide batekin edo eskuratu berri den baliabide batekin lotu dezakezu. Adibidez, Daniel kontratatu zutenean, esperientzia eta trebetasunak zituen Enpresa analista papera betetzeko. Baliabideen kudeatzaileak rol hau Danielen lehenetsitako rol gisa izendatu du. Hori dela eta, baliabideen zuzendariak Daniel gehitu zuen proiektuetan lan egiteko erabilgarri dauden negozio analista multzo batean.

Baliabideak erreserbatu bitartean, proiektuen arduradunek proiektuetan lan egiteko erabilgarri dauden rol baliabideak iragazi ditzakete. Informazio hori irizpide gisa erabil dezakete, baliabideen betetzean irizpide anitzeko erabakien analisia egiten dutenean. Iragazkiari beste baliabide batzuen ezaugarriak ere gehi ditzakete proiektu jakin baterako trebetasunak, hezkuntza eta esperientzia zehatzak dituzten baliabideak bilatzeko.

**Eszenatokia:** Onartutako proiektua hasi da, eta proiektuaren zuzendari nagusiaren eginkizuna planifikatutako baliabide gisa gorde da proiektuaren plangintza fasean. Baliabideen kudeatzaileak baliabide bat eskuratu du orain Senior proiektuaren kudeatzaile rola betetzeko.

1. Gainean **Baliabideen zerrenda** orrialdea, hautatu **Daniel Goldschmidt**.
2. **Baliabide-funtzioa** orria, hautatu **Berria**, eta idatzi hurrengo balioak:

    - **Eraginkorra:** Sartu uneko data.
    - **Iraungipena:** Sartu **Inoiz ez**.
    - **Funtzioa:** Idatzi **Proiektu zuzendari nagusia**.

3. Aukeratu **Gorde**, eta gero itxi orria.
4. Gainean **Konpetentziak** fitxa, gehitu **ProjectMgmt** trebetasuna eta **PMP** ziurtagiria.

## <a name="set-up-role-based-pricing"></a>Konfiguratu roletan oinarritutako prezioak
Kostu, salmenta eta transferentzia prezio guztiak eginkizunetarako konfigura daitezke.

1. Gainean **Salmenta prezioa (ordua)** orrialdea, hautatu **Berria**, eta sartu data eraginkorra.
2. **Rola** zutabean, hautatu rol bat.
3. **Prezioak** zutabean, sartu hautatutako baliabide rolaren prezioa.

## <a name="form-a-project-team"></a>Inprimakiaren proiektuaren taldea
Aurretik proiektu batean konfiguratutako eginkizunak erabiltzeko, proiektuaren kudeatzaileak eginkizunak proiektuarekin lotu behar ditu. Hainbat eginkizun esleitu daitezke proiektu baterako. Nahasmena ekiditeko, funtzio hauek automatikoki etiketatzen dira erreserbatu bitartean. Adibidez, proiektuaren zuzendariak hiru software ingeniari behar baditu, hiru Software ingeniari funtzio betetzen dituzte **software ingeniaria 1**, **software ingeniaria 2**, eta **software ingeniaria 3** haien etiketak automatikoki sortzen baitira. Aurretik rolaren ezaugarriak rolerako ezarri badira, iragazki gisa aplikatuko dira baliabide bat bilatzerakoan. Ezaugarri osagarriak gehi daitezke, bilaketa gehiago zehazteko beharrezkoak diren moduan.

Ikuspegi ezarpenak pertsonaliza daitezke, baliabideen erabilgarritasuna hobeto ikusteko. Ordubeteko, eguneroko, asteko, hileko, hiruhileko eta urteko erabilgarritasuna erakusteko aukerak daude. Baliabideetan eskuragarri eta geratzen den gaitasuna erakusteko aukera ere badago. Aukera hau erabilgarria da denbora kudeatzeko, jardueretarako edo baliabideen erabilgarritasunerako denbora librea kalkulatzen duzunean.

Proiektuaren kudeatzaileak orrialdeko rol bat hauta dezake eta, gero, eskakizunera egokitzen den baliabide erabilgarri bat badago, hautatu papera betetzeko baliabide bat gordetzea. Kontuan izan baliabideak ez direla zertan erreserbatu plangintza faseko une honetan. WBS bat sortzen duzunean, eginkizunak proiektuko langileekin ordezkatu ditzakezu. Rolak WBSn langileekin hornitutako baliabideekin ordezkatzen badira, baliabideen konfigurazioak proiektuaren taldeen zerrenda eta programazioa automatikoki eguneratuko ditu.

[![Eginkizunak eta benetako baliabideak biltzen dituen proiektu taldeen zerrenda](./media/projectresourcing03-1024x368.jpg)](./media/projectresourcing03.jpg) 

Proiektuaren kudeatzaileak proiektu baterako baliabide bat erreserbatzeko hainbat aukera ditu, adibidez **Gainerako gaitasuna**, **Edukiera osoa**, **Edukiera ehunekoa**, eta **Zehaztu orduak**. Erreserba aukera hauek edozein unetan bertan behera utzi daitezke baliabideen esleipenak aldatzen badira. Bi erreserba mota onartzen dira:

- **Liburu gogorra** - Baliabideen erreserba onartu eta baieztatu zen konpromisoan zehaztutako iraupenean lan egiteko.
- **Behin behineko erreserba** - Baliabideen erreserbak behin-behinean zen konpromisoan zehaztutako iraupenean lan egiteko.

Prozedura honetan azaltzen nola proiektuaren taldea sortu:

### <a name="create-a-project-team"></a>Sortu proiektuaren taldea

1. Gainean **Proiektu guztiak** zerrendaren orria, hautatu proiektu bat eta, ondoren, hautatu **Editatu**.
2. Gainean **Proiektu taldea eta programazioa** fitxan, **Egitarauaren amaiera data** eremuan, sartu programazioaren hasiera data gehi hilabete bat. Adibidez, ordutegia hasteko data 2017ko ekainaren 24a bada (2017/06/24), sartu **2017/07/24**.
3. Hautatu **Gehitu**.
4. **Gehitu eginkizunak proiektuari** panelean, **Rola** eremua, hautatu **Proiektu zuzendari nagusia**.
5. Aukeratu **Eskatutako gaitasunak**.
6. Gainean **Aukeratu ezaugarriak** orrialdean, lehenago zuzendari nagusiaren eginkizunerako zehaztutako ezaugarriak lehenespenez hautatzen dira. Hautatu **Ados**.
7. Gainean **Gehitu rolak proiektuari** orrialdean, **Baliabide kopurua** eremua, sartu **1**.
8. **Baliabidea** eremuan, bilaketak beharrezko gaitasunak dituzten baliabide guztiak erakusten ditu. Aukeratu **Daniel Goldschmidt** eta, ondoren, hautatu **Sortu**.
9. **Proiektua** orrian, hautatu **Gehitu**.
10. **Gehitu eginkizunak proiektuari** panelean, **Rola** eremua, hautatu **Taldekidea**. **Baliabide-kopurua** eremua, sartu **5**.
11. Hautatu **Sortu**.
12. Gainean **Proiektuak** orrialdea, hautatu **Baliabidea bete**.

## <a name="resource-capacity-synchronization"></a>Baliabide gaitasunaren sinkronizazioa
Baliabideak sinkronizatzeko prozesuei esker, egutegiaren eta oinarrizko egutegiaren informazioa proiektuaren baliabideen programazioan sartzen da. Egutegia aldatzen bada, prozesuek beharrezko eguneratzeak egiten dituzte proiektuaren baliabideen programazioan. Prozesuek errendimendua hobetzen ere laguntzen dute, egutegiaren baliabideen informazioa aldez aurretik sinkronizatuta dagoelako. Hori dela eta, baliabideak antolatzeko informazioaren eguneratzeak azkarrago gertatzen dira. Prozesuak multzo gisa antolatzea gomendatzen dizugu, aldi berean ordez. Bestela, norbaitek informazioa azkeneko aldiz sinkronizatu zeneko egun biak barne ahazteko arriskua dago. Data inklusiboak erabiltzen ez badira, hutsuneak gerta daitezke data sinkronizatzean.

![Egutegiaren sinkronizazioa](./media/projectresourcing04-1024x471.jpg)

### <a name="synchronize-resource-capacity-roll-ups"></a>Sinkronizatu baliabide-gaitasuna bateratzea

Sinkronizazio prozesua baliabideen egutegiko informazio guztia sinkronizatzeko diseinatuta dago. Informazio honek proiektuaren Baliabideen egutegiaren edukiera taulan egindako aldaketen inguruko oinarrizko egutegiko informazioa biltzen du. Proiektuan baliabide berriak gehitzen badira, sinkronizazioak eguneratutako egutegiko informazioa eskuragarri dagoela bermatzen laguntzen du. Sinkronizazio hau edozein unetan egin daiteke.

Gomendatzen dizugu erabiltzea sorta gisa. Aukerak eskuragarri daude edukiera erreserbak sinkronizatzean.

1. Aukeratu **Proiektuen kudeaketa eta kontabilitatea** &gt; **Aldizkakoa** &gt; **Edukiera sinkronizatzea** &gt; **Sinkronizatu baliabideen ahalmenak**.
2. Ezarri aukerak ondoko taulan bistaratzen dira.

    | Aukera      | Deskribapenak |
    |-------------|-------------|
    | Garai kodea | Aukeran hautatu Liburu nagusiaren data tarte kodea, baliabideen edukiera biltzeko sinkronizazio prozesuaren hasiera eta amaiera datak ezartzeko. |
    | Hasiera-data  | Idatzi baliabideen edukiera biltzeko prozesuen sinkronizazio prozesuaren hasiera data. |
    | Amaiera-data    | Idatzi baliabideen edukiera biltzeko prozesuen sinkronizazio prozesuaren amaiera data. |

[![Sinkronizazio-prozesua](./media/projectresourcing09.jpg)](./media/projectresourcing09.jpg)

## <a name="set-up-roles-on-wbs-templates"></a>Konfiguratu rolak WBS txantiloietan
Proiektuen kudeatzaileek WBS txantiloiak konfigura ditzakete, proiektu berrietarako WBS sortzen dutenean aplika ditzaketen. Proiektuen kudeatzaileek rolak gehi ditzakete txantiloia sortzen dutenean. Erabili prozedura hau WBS txantiloiari rol bat esleitzeko.

1. Aukeratu **Proiektuen kudeaketa eta kontabilitatea** &gt; **Konfigurazioa** &gt; **Proiektuak** &gt; **Lanen matxuren egitura txantiloiak**.
2. Aukeratu **Xehetasunak** hautatutako WBS txantiloia lortzeko.
3. Hautatu zeregin bat zerrendan, eta gero **Rola** eremuan, hautatu zereginari esleitzeko funtzioa.

### <a name="work-with-a-wbs"></a>Egin lan WBS

Sortu egin dezakezu WBS berria edo kopiatu WBS inprimakia existitzen den WBS txantiloia. Proiektu kudeatzaile batek baliabideak erraz kudea ditzake WBSko zeregin berriei rolak esleituz. Rolak ordezka daitezke baliabide bat eskuratu ondoren edo zereginean lan egiteko baieztatutako baliabide bat identifikatu ondoren. Malgutasun honi esker, proiektuen kudeatzaileek zeregin hauek bete ditzakegu:

- Identifikatu WBS lan paketeetarako beharrezkoak diren baliabide kopurua.
- Balioztatu proiektuaren kostuak.
- Aurretiazko aurrekontua zehaztu.
- Jardueraren iraupena kalkulatu, rol eta baliabideetan oinarrituta.
- Proiektuak kudeatzeko zenbait plan garatu, eskuragarri dagoen proiektuaren informazioan oinarrituta.

Aukera osagarriak gehitu dira WBSn, baliabideen funtzionalitatea hobeto erabiltzeko.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Aukera</th>
<th>Deskribapenak</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Baliabide-esleipenak</td>
<td>Ikusi esleitutako baliabideak, datak, ordu kopurua eta erreserba mota WBSn zereginetarako.</td>
</tr>
<tr class="even">
<td>Auto sortu taldea</td>
<td>Gehitu automatikoki aurreikusitako baliabideak ataza batekin lotutako rolak erabiliz. Finantzak automatikoki iradokitzen ditu planifikatutako baliabideak, roletan oinarritutako irizpide anitzeko erabakien analisia erabiliz. WBS batean zereginak egiteko rolak eta ahalegina (orduak) ezarri ondoren, eta egitura askatu ondoren, hautatu <strong>Auto taldea sortu</strong>. Aurreikusitako beharrezko baliabide kopurua gehitzen zaio WBSri eta <strong>Proiektuen eta taldeen programazioa</strong> fitxa.</td>
</tr>
<tr class="odd">
<td>Baliabidea (goitibehera zerrenda)</td>
<td>Gainean <strong>Baliabideen esleipena abiarazi</strong> orrialdean, hard-book edo soft-book baliabideak hauta ditzakezu, zehaztutako iraupenaren arabera. Ikuspegiaren ezarpenak doitu ditzakezu baliabideen jardueren iraupena ikusi eta ezartzeko. Lan pakete mailan baliabideak hauta eta esleitu ditzakezu aukera hauek erabiliz:
<ul>
<li><strong>Onartu</strong> - Egiaztatu zeregin bati esleitutako baliabidearen aldaketak.</li>
<li><strong>Ezeztatu</strong> - Ezeztatu zeregin bati esleitutako baliabidearen aldaketak.</li>
<li><strong>Esleitu automatikoki</strong> - Bat datorren eginkizuna duen langile baliabide erabilgarri bat automatikoki hautatzen da eta hautatutako ataza esleitzen zaio.</li>
</ul></td>
</tr>
</tbody>
</table>

1. Gainean **Proiektu guztiak** orria, hautatu **XYZ berritzea 2. fasea** proiektua.
2. Aukeratu **Plana** &gt; **Jarduerak** &gt; **Lanen matxuren egitura**.
3. Aukeratu **Berria** WBSari maila bateko jarduera hauek gehitzeko:

    - Hasi
    - Antolaketa
    - Exekutatzen
    - Monitorizatu eta kontrola
    - Itxi

4. Ezarri datak eta ahalegina (orduak), hurrengo ilustrazioan agertzen den moduan.

    [![Datak eta ahalegina zehaztea](./media/projectresourcing10.jpg)](./media/projectresourcing10.jpg)

5. Aukeratu **Hasi** ataza lerroa, eta gero, **Rola** eremua, hautatu **Proiektu zuzendari nagusia**.
6. Hautatu **Argitaratu**.
7. Lerro berean, **Baliabidea** eremua, hautatu **Daniel Goldschmidt** eta, ondoren, hautatu **Onartu**.
8. Aukeratu **Plangintza** ataza lerroa, eta gero, **Rola** eremua, hautatu **Enpresa analista**.
9. Aukeratu **Argitaratu** eta, ondoren, hautatu **Auto taldea sortu**.
10. Agertzen den mezuaren koadroa, hautatu **Bai**.
11. **Baliabidea** eremua, egiaztatu balioa dela **Enpresa analista 1**.
12. Hurrengorako **Enpresa analista 1** baliabidea, ireki bilaketa eta hautatu **Abiarazi baliabideen esleipenak**. Ondoren, hautatu langilea zereginerako.
13. Aukeratu **Soft esleitzeko** &gt; **Edukiera osoa**.

    > [!NOTE] 
    > Ez duzu ohartarazten zehaztutako baliabidea 2 dela, baliabide kopurua 1 izaten jarraitzen duelako.

14. Gainean **Lanen matxuren egitura** orrialdean, baliozkotu baliabideen esleipena WBSn eta hautatu **Gorde**.

## <a name="resource-fulfillment-for-planned-resources"></a>Aurreikusitako baliabideetarako baliabideak betetzea
Proiektu kudeatzaile batek proiektu baterako beharrezko baliabide rolak planifika ditzake. Baliabideen kudeatzaileak aurreikusitako baliabide hauek ikusiko ditu eskaeran **Baliabideen betetzea** orrialdean eta benetako baliabideak esleitu ditzake.

1. Gainean **Proiektu guztiak** orria, hautatu **XYZ berritzea 2. fasea** proiektua.
2. Hautatu **Proiektua**, eta gero hautatu **Editatu**.
3. Gainean **Proiektu taldea eta programazioa** fitxa, hautatu **Gehitu**.
4. **Gehitu rolak** Elkarrizketa koadroa, hautatu **Software garatzailea** rola.
5. Aukeratu **Sortu**, eta gero itxi proiektuaren orria.
6. Gainean **Baliabideen betetzea** orrialdea, hautatu **Software garatzailea 1** egiteko **XYZ Berritze proiektua 2. fasea** proiektua.
7. Hautatu langile bat, eta ondoren, hautatu **Esleitu**.
8. Egiaztatu lerro hori **Software garatzailea 1** kendu da **XYZ Berritze proiektua 2. fasea** proiektua.
9. Gainean **Proiektu taldea eta programazioa** fitxa, **XYZ berritzea 2. fasea** proiektua, egiaztatu aurreko urratsean hautatu zenuen langilea honela gehitu dela **Software garatzailea**.

## <a name="requests-for-project-resources"></a>Proiektuaren baliabideen eskaerak
Proiektuaren baliabideen antolaketarako funtzionaltasunak baliabideen kudeatzaileek konpromiso edo proiektuetan pertsonaleko baliabideak banatu ditzaten soilik. Funtzionalitate hau gaitzeko, burutu zeregin hauek edo egiaztatu egin direla:

- Konfiguratu zenbaki sekuentziak.
- Konfiguratu proiektuen kudeaketa eta kontabilitate lan-fluxuak.
- Gaitu baliabideen eskaera-fluxuak.

Aurreko zereginak amaitu ondoren, zeregin hauek bete ditzakezu nahi duzun moduan:

- Sortu baliabide eskaera bat gordetako langileen baliabide batetik.
- Monitorizatu baliabide-eskaerak.
- Baliabide-eskaerak bete.
- Eskatu baliabide pertsonal bat WBS bati.
- Erreserbatu baliabideak proiektu batera, pertsonaleko baliabiderik eskatu gabe.

## <a name="monitor-project-teams"></a>Proiektu taldeak kontrolatu
1. **Proiektu guztiak** orria, hautatu **Proiektuaren ID-a** esteka **XYZ Bertsio berritu fasea 2** proiektua.
2. Gainean **Proiektu taldea eta programazioa** FastTab, egiaztatu zerrendan agertzen diren proiektuaren baliabideak zuzenak direla.
