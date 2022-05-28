---
title: Erakundearen unitateak
description: Gai honek antolakuntza-unitateen kontzeptua deskribatzen du eta Microsoft-en antolakuntza-unitateak nola sortu eta nola mantendu azaltzen du Dynamics 365 Project Operations.
author: rumant
ms.date: 1/31/2022
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
ms.reviewer: johnmichalak
ms.openlocfilehash: 9a8c503dc6286f40c80ed9b7a8a04974ff7e50b4
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8581361"
---
# <a name="organizational-units-overview"></a>Antolaketa-unitateen ikuspegi orokorra

Microsoft-en Dynamics 365 Project Operations, an *antolakuntza-unitatea* kostu-tasa duten baliabide fakturagarriak erabiltzen dituen zerbitzu profesionalen enpresa bateko talde edo dibisio bereizia da.

Praktika-eremu edo negozio-lerro desberdinetan baliabide teknikoak erabiltzen dituzten zerbitzu profesionalen enpresentzat, rol bat betetzeko kostua alda daiteke, eginkizuna betetzen den praktika-eremuaren edo negozio-lerroaren arabera. Eszenatoki honetan, antolakuntza-unitateen kontzeptuak faktura daitezkeen rol multzo bat taldekatzeko modu bat eskaintzen du rol horietarako kostu-egitura desberdina duen enpresa baten dibisio batean.

## <a name="the-concept-of-organizational-units-in-project-operations"></a>Antolaketa-unitateen kontzeptua Proiektu Eragiketetan

Proiektuen Eragiketetan, antolakuntza-unitate batek moneta zehatz bat eta kostu-prezio-zerrenda zehatzak ditu.

Erakunde unitate bateko moneta kostuen jarraipena egiteko erabiltzen den lehen moneta da.

Kostuen prezio-zerrenda bat edo gehiago erantsi daitezke antolaketa unitate bakoitzari. Project Operations-ek honako muga hauek jartzen ditu antolakuntza-unitate bati atxiki daitezkeen prezio-zerrendei:

- Prezio-zerrendek antolakuntza-unitatearen moneta izan behar dute.
- Prezio-zerrendek kostu-prezio-zerrendak izan behar dute.

Horrez gain, Baliabide entitateak antolakuntza-unitaterako atributu bat barne hartzen du. Baliabide bakoitzari erakundearen unitate eslei diezaiokezu.

### <a name="roles-of-organizational-units"></a>Erakundearen unitatearen funtzioak

Antolaketa-unitateak bi eginkizun betetzen ditu Proiektuaren Eragiketetan:

- **Kontratazio Unitatea**: salmenta irabaztea eta bezeroari lana eta zerbitzuak entregatzea kudeatzeaz arduratzen den enpresa-taldea edo zatiketa ordezkatzen duen antolakuntza-unitatea. Kontratazio unitateak identifikatzen du **Kontratazio Unitatea** eremua goiburuko ataleko goiburuko atalean **Abagunea**, **Eskaintza**, **Proiektuaren kontratua**, eta **Proiektua** orrietakoak.
- **Baliabide Unitatea**: baliabide bat dagokion edo esleitzen zaion unitate antolatzailea. Erakundearen unitate honek bere baliabideak eman ditzake laneko aitorpenetan (SOWs) eta unitate kontratatzailearen jabetzakoak diren eginkizunetarako.

![Kontratazio unitateak eta baliabide unitateak.](media/OrgUnits.png)

### <a name="organizational-unit-faq"></a>Antolakuntza-unitatearen maiz galderak

Erakundearen unitate batzuei buruzko ohiko galdera ugariren erantzunak aurkituko dituzu hemen:

#### <a name="how-is-the-organizational-unit-entity-in-project-operations-related-to-the-organization-entity-that-already-exists-in-dynamics-365"></a>Nola dago erlazionatuta Project Operations-en Antolakuntza Unitatearen entitatea Dynamics 365-en dagoeneko existitzen den Antolakuntza-entitatearekin?

Dynamics 365eko Antolakuntza entitateak Dynamics 365 instantzia global baten izena adierazten du. Izen hori normalean enpresa globalaren izena da.

Erakundearen unitatea erakundea enpresa globalean talde edo zatiketa bat da. Talde edo zatiketa honek funtzio eta kostu prezio-zerrenda bat dauka funtzio horientzat, eta funtzioak eta prezio-zerrendak enpresako beste talde edo zatiketa batzuen eginkizun eta prezio-zerrendak desberdinak dira.

Project Operations instalatzen denean, lehenetsitako antolakuntza-unitate bat sortzen da erakundean oinarrituta. Dauden baliabide guztiak erakundearen unitate lehenetsian esleitzen dira. Dynamics 365-era Active Directory-ren erabiltzaile edo baliabide berriren bat inportatzen bada, erabiltzailearen inportazio-prozesuak Project Operations-eko antolakuntza-unitate lehenetsiari esleitzen ditu.

#### <a name="how-does-the-organizational-unit-entity-differ-from-the-business-unit-entity"></a>Zertan desberdintzen da Antolakuntza Unitateko entitatea Negozio Unitateko entitatetik?

Dynamics 365-en, Business Unit entitatea segurtasun eraikuntza da. Erabiltzaileen negozio unitate batekin elkartzeak erabiltzaileak sarbidea duen entitateak eta entitate erregistroak zehazten ditu. Erabiltzaileak entitate-erregistro horietarako dituen baimenak (Sortu, Irakurri, Idatzi, Ezabatu, Erantsi, Honi erantsi, Esleitu edo Partekatu) zehazten ditu.

Erakundearen unitate erakundeak enpresa talde edo zatiketa bat du, esleitutako langileentzako kostu tasak desberdinak dituena. Baliabide bat erakundearen unitatearekin elkartzeak zehazten du baliabidearen kostua proiektuaren konpromisoan.

Dynamics 365 ezartzen duzunean, optimizatu segurtasun baimena negozio unitateen hierarkiarako eta erabiltzaileak negozio unitateei esleitzeko. Esleitu negozio unitate berean erregistro multzo bera sartu behar duten erabiltzaile guztiei. Unitate antolatzaileak ez du eraginik segurtasun baimenean edo sarbidean.

**Antolaketa-unitateen eta negozio-unitateen modelizazioan balizko diferentzia bat erakusten duen adibidea**

Contoso, Ltd.-ek Microsoft teknologiaren praktika oparoa du. Dabid eta Aizpea biak C\# garatzaileak dira, baina Aizpea Gasteizen dago, Dabid Iruñekoa den bitartean. Proiektuko konpromiso gehienek Contoso Indiako eta Contoso AEBetako baliabideak behar dituzte, eta Prakash eta Tricia-k segurtasun-sarbide maila bera behar dute praktika-eremu honetako proiektuetarako. Hala ere, Badiola Iruñeko garatzaileen kostua ezberdina da Badiola Gasteizeko garatzaileen kostua.

Hona hemen eszenatoki honetarako diseinatzeko modu ezin hobea Dynamics 365 eta Project Operations erabiliz.

1. Sortu Microsoft teknologiaren praktika negozio unitate gisa eta lotu Dabid eta Aizpea berarekin. Horrela, bi langileek praktika-eremu horretako edozein proiektutarako segurtasun-sarbide-maila bera dutela ziurtatzen laguntzen duzu. Biek aurrerapena egiaztatu ahal izango dute eta denbora, gastuak, materialaren erabilera eta zereginen eguneraketak jakinarazi ahal izango dituzte.
2. Sortu bi antolamendu-unitate, proiektuaren kostua behar bezala islatzen dela ziurtatzeko.
3. Lotu Tricia Contoso AEBrekin eta Prakash Contoso Indiarekin.
4. Esleitu kostu prezio-zerrenda egokiak erakunde biei. Modu honetan, Prakash eta Tricia-ren proiektuan erregistratzen diren kostuek Contoso AEB eta Contoso Indiaren arteko kostuen aldea zehatz-mehatz islatzen dutela ziurtatzen duzu.

#### <a name="are-organizational-units-related-to-sales-territories-in-dynamics-365"></a>Dynamics 365-en salmenta lurraldeekin erlazionatuta daude antolakuntza unitateak?

Ez dago loturarik edo harremanik salmenten lurraldeen eta erakundearen unitateen artean. Salmenta-lurraldea normalean salmentak gertatzen diren eremu geografikoa da. Salmenta prezio-zerrenda salmenta-urralde bakoitzari lotuta egon daiteke.

Erakunde unitatea enpresako barne-talde edo zatiketa da, beste dibisio batzuei edo kanpoko bezeroei saltzen dituen funtzio multzo baten kostuak kontrolatzen dituena.

**Antolakuntza-unitateen eta salmenta-lurraldeen modelizazioan balizko diferentzia bat erakusten duen adibidea**

Badila, Ltd.-k bi garapen zentro ditu: Badiola Gasteiz eta Badiola Iruñea. Baliabideen kostua oso desberdina da bi garapen zentro horien artean. Contoso-ek bere informazio teknologia (IT) zerbitzuak nazioarteko merkatu askotan saltzen ditu, hala nola Latinoamerikan, Ipar Amerikan, Asia-Pazifikoan, Mendebaldeko Europan eta Ekialde Hurbilean. Proiektu bereko funtzioen fakturen tasak oso alda daitezke merkatu hauetan. Badiola Gasteizek eta Badiola Iruñeak erakundearen unitate gisa eratu beharko lirateke, eta erakundearen unitate bakoitzak bere kostuen prezio-zerrenda izan beharko luke. Asia-Pazifikoa, Latinoamerika, Ipar Amerika, Mendebaldeko Europa eta Ekialde Hurbilean salmenta-lurralde gisa ezarri beharko lirateke, eta salmenta-lurralde bakoitzak bere salmenta prezio-zerrenda izan beharko luke.

#### <a name="why-is-there-a-restriction-on-the-association-of-price-lists-with-organizational-units"></a>Zergatik dago murrizketarik prezio-zerrenden erakundearen unitateekin lotzeari dagokionez?

Salmenten prezioak zerbitzuak saltzen diren gune geografiko edo merkatuetarako bakarra da. Enpresa baten barne-banaketak ez dute normalean zerbitzu mota bereko salmenten prezio propiorik izaten. Hala ere, barne-banaketak saltzen diren ondasunen kostuak (COGS) desberdinak dituzte, enplegatzen duten pertsonen trebetasunen eta eskualdeko lan-baldintzen arabera. Erakunde-unitateak enpresa baten barne-banaketa gisa eredutzen direnez, kostuen prezio-zerrendak soilik izan ditzakete.

#### <a name="why-cant-we-associate-sales-price-lists-with-organizational-units"></a>Zergatik ezin ditugu salmenten prezioen zerrendak antolakuntza-unitateekin lotu?

Project Operations-en, salmenta-prezioen zerrendak bezeroekin eta salmenta-lurraldeekin lotu daitezke. Transakzio-entitateek, hala nola, Aukera, Aurrekontua, Proiektuaren Kontratua eta Proiektua bezeroen kontuari edo salmenta-lurraldeari atxikitako salmenta-prezio zerrendak erabiltzen dituzte faktura-tasak eta proiektuaren konpromisorako diru-sarrera potentzialak zehazteko.

Kostuen prezioen-zerrendak erakundearen unitateekin lotzen dira. Transakzio-entitateek, hala nola, Aukera, Aurrekontua, Proiektuaren Kontratua eta Proiektua, kontratazio-unitateari atxikitako kostu-prezio zerrendak erabiltzen dituzte proiektu-konpromiso baten kostuak zehazteko.

#### <a name="are-organizational-units-hierarchical-in-project-operations"></a>Antolakuntza-unitateak hierarkizatuta al daude Proiektu Eragiketetan?

Ez. Project Operations-en oraingo bertsioan, antolakuntza-unitateak ez dira hierarkizatuak. Hori dela eta, ezin dituzu zeregin hauek egin:

- Konfiguratu hierarkia batetik gora doan kostu-prezio lehenetsiak sartzeko eredua.
- Antolakuntza-unitateen hierarkiaren maila ezberdinetan bildutako diru-sarreren edo kostuen berri eman.

#### <a name="were-a-big-multinational-firm-that-has-a-complex-multilevel-hierarchy-of-cost-centers-divisions-and-billing-offices-how-can-we-best-use-the-concept-of-organizational-units-in-the-current-version-of-project-operations"></a>Enpresa multinazional handi bat gara, kostu zentroen, dibisioen eta fakturazio bulegoen maila anitzeko hierarkia konplexua duena. Nola erabil dezakegu hobekien antolakuntza-unitateen kontzeptua Project Operations-en egungo bertsioan?

Kostu-zentroen, dibisioen, fakturazio-bulegoen eta abarren hierarkia konplexu bat duzunean, konfiguratu hierarkia horren hosto-nodoak antolakuntza-unitate ezberdin gisa.

Hurrengo adibidean hierarkia tipiko bat erakusten da.

**Badiola Iruñea**

- SAP praktika

    - Aholkulari Teknikoak
    - Aholkularitza funtzionalak

- Microsoft Teknologia Praktika

    - Aholkulari Teknikoak
    - Aholkularitza funtzionalak

**Contoso US**

- SAP praktika

    - Aholkulari Teknikoak
    - Aholkularitza funtzionalak

- Microsoft Teknologia Praktika

    - Aholkulari Teknikoak
    - Aholkularitza funtzionalak

Zure hierarkiak adibide honen antza badu, zerrenda lau gisa konfiguratu behar duzu, hemen erakusten den moduan:

- Badiola Iruñea - SAP Praktika - Aholkulari Teknikoak
- Badiola Iruñea - SAP Praktika - Aholkulari funtzionala
- Badiola Iruñea - Microsoft Technology Aholkulari funtzionala
- Badiola Iruñea - Microsoft Technology Aholkulari funtzionala
- Badiola Gasteiz - SAP Praktika - Aholkulari Teknikoak
- Badiola Gasteiz - SAP Praktika - Aholkulari funtzionala
- Badiola Gasteiz - Microsoft Technology Aholkulari teknikoak
- Badiola Gasteiz - Microsoft Technology Aholkulari funtzionala

#### <a name="were-a-small-professional-services-company-that-operates-as-only-one-division-how-can-we-best-use-the-concept-of-organizational-units-in-the-current-version-of-project-operations"></a>Zerbitzu profesionalean maila bakarrean lan egiten duen enpresa txiki bat gara. Nola erabil dezakegu hobekien antolakuntza-unitateen kontzeptua Project Operations-en egungo bertsioan?

Zure enpresak kostuen prezioen zerrenda bat duen unitate gisa funtzionatzen badu, ez duzu antolaketa unitaterik ezarri behar. Project Operations instalazioak erakundearen izen bera duen lehenetsitako antolakuntza-unitate bat sortzen du. Lehenespenez dauden baliabide guztiak erakundearen unitate lehenetsian esleitzen dira. Sistemak unitate antolatzaile bat aukeratu behar duen bakoitzean, unitate antolakuntza hau lehenespenez hautatzen da.

#### <a name="when-a-project-is-created-from-a-quote-or-project-contract-line-the-default-contracting-unit-comes-from-the-quote-or-project-contract-what-is-the-default-contracting-unit-if-a-project-is-created-before-sales-entities-such-as-quote-or-project-contract"></a>Proiektua aurrekontuen edo proiektuaren kontratuaren lerrotik sortzen denean, kontratazio unitate lehenetsia aurrekontu edo proiektu kontratutik dator. Zein da kontratazio-unitate lehenetsia proiektu bat salmenta-entitateen aurretik sortzen bada, hala nola, Aurrekontua edo Proiektuaren Kontratua?

Proiektua bere kabuz sortutakoan, proiektuaren kontratazio unitate lehenetsia sortzen duen erabiltzailea da. Erabiltzailea ere proiektu kudeatzaile lehenetsia da. Proiektua salmenta-entitate batekin mapatzen bada, hala nola aurrekontu edo proiektu-kontratu batean, proiektuaren kontratazio-unitatea salmenta-entitatean oinarritzen da. Kasu honetan, proiektuaren kalkuluak berriro kalkulatu litezke, izan ere, kostu-estimazioen aldaketak kalkulatzeko kostu-prezioen zerrenda erabiltzen da kontratazio-unitatea aldatzen bada. Salmenten prezioen zerrenda aldatuko diren salmenten estimazioak kalkulatzeko erabiltzen da, aurrekontuaren proiektuko prezioen zerrendarekin sinkronizatu daitezen.

The **Kontratazio Unitatea** eta **Moneta** proiektuaren eremuak editatzeko blokeatuta daude, proiektua mapatzen den salmenta-entitatearen (aurrekontua edo proiektuaren kontratua) balioekin sinkronizatuta egon behar dutelako.

## <a name="create-and-maintain-organizational-units-in-project-operations"></a>Proiektu Eragiketetan antolakuntza-unitateak sortzea eta mantentzea

Project Operations-en antolakuntza-unitate bat sortzeko, jarraitu urrats hauek.

1. Joan **Ezarpenak \> Antolaketa Unitateak**.
2. Hautatu **Berria**.
3. urtean **Orokorra** eremuan, in **Izena** eremuan, idatzi antolakuntza-unitatearen izena. Ondoren, ezarri gainerako eremuak behar bezala.
4. Hautatu **Gorde** erregistroa sortzeko, editatzen jarraitu ahal izateko.
5. Azpian **Kostu Prezio Zerrendak**, hautatu plus ikurra (**+**) prezioen zerrenda gehitzeko. Hau duten prezioen zerrendak bakarrik gehi ditzakezu **Kostua** testuingurua hemen.
6. urtean **Izena** eremua, hautatu **Bilatu** botoia eta hautatu antolaketa-unitatearen eskura jarri nahi duzun prezio-zerrenda. Jarraitu prezioen zerrendak gehitzen behar bezala.
7. Prezio-zerrendak gehitzen amaitutakoan, hautatu **Gorde** orriaren behe-eskuineko izkinan.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
