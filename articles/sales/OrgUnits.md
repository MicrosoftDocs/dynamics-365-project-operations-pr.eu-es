---
title: Erakundearen unitateak
description: Artikulu honetan antolaketa unitateen kontzeptua deskribatzen da eta Microsoften antolaketa-unitateak nola sortu eta mantendu azaltzen da Dynamics 365 Project Operations.
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
ms.openlocfilehash: a20a37b61db68d70869a11e10bef5d30c422b1eb
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8921609"
---
# <a name="organizational-units-overview"></a>Antolaketa-unitateen laburpena

Microsoften Dynamics 365 Project Operations, antolaketa-unitate *bat* beste talde edo zatiketa bat da zerbitzu profesionaletako enpresa batean, eta kostu-tasak dituzten baliabide fakturagarriak erabiltzen ditu.

Hainbat arlotan edo negozio-lerrotan baliabide teknikoak erabiltzen dituzten zerbitzu profesionaletako enpresentzat, rol bat betetzeko kostua aldatu egin daiteke, rola betetzen den praktika-arloaren edo negozio-lerroaren arabera. Egoera horretan, antolaketa-unitateen kontzeptuak rol fakturagarrien multzo bat rol horietarako kostu desberdineko egitura duen enpresa baten banaketan taldekatzeko modu bat ematen laguntzen du.

## <a name="the-concept-of-organizational-units-in-project-operations"></a>Antolaketa-unitateen kontzeptua proiektu-eragiketetan

Proiektu-eragiketetan, antolaketa-unitate batek txanpon espezifiko bat eta kostu espezifikoko prezioen zerrendak ditu.

Erakunde unitate bateko moneta kostuen jarraipena egiteko erabiltzen den lehen moneta da.

Kostuen prezio-zerrenda bat edo gehiago erantsi daitezke antolaketa unitate bakoitzari. Project Operations-ek honako muga hauek ezartzen ditu antolaketa-unitate bati erantsi ahal zaizkion prezio-zerrendetan:

- Prezio-zerrendek antolakuntza-unitateko monetan egon behar dute.
- Prezioen zerrendek kostu-prezioen zerrenda izan behar dute.

Gainera, Resource erakundeak antolakuntza unitatearentzako atributu bat ere badu. Baliabide bakoitzari erakundearen unitate eslei diezaiokezu.

### <a name="roles-of-organizational-units"></a>Erakundearen unitatearen funtzioak

Antolaketa-unitateak bi eginkizun betetzen ditu proiektu-eragiketetan:

- **Kontratazio Unitatea**: salmenta irabaztea eta bezeroari lana eta zerbitzuak entregatzea kudeatzeaz arduratzen den enpresa-taldea edo zatiketa ordezkatzen duen antolakuntza-unitatea. Kontratazio unitateak identifikatzen du **Kontratazio Unitatea** eremua goiburuko ataleko goiburuko atalean **Abagunea**, **Eskaintza**, **Proiektuaren kontratua**, eta **Proiektua** orrietakoak.
- **Baliabide Unitatea**: baliabide bat dagokion edo esleitzen zaion unitate antolatzailea. Erakundearen unitate honek bere baliabideak eman ditzake laneko aitorpenetan (SOWs) eta unitate kontratatzailearen jabetzakoak diren eginkizunetarako.

![Kontratazio unitateak eta baliabide unitateak.](media/OrgUnits.png)

### <a name="organizational-unit-faq"></a>Antolaketa-unitateari buruzko ohiko galderak

Erakundearen unitate batzuei buruzko ohiko galdera ugariren erantzunak aurkituko dituzu hemen:

#### <a name="how-is-the-organizational-unit-entity-in-project-operations-related-to-the-organization-entity-that-already-exists-in-dynamics-365"></a>Nola lotzen da erakundea proiektu-eragiketetako antolaketa-unitatea Dynamics 365-en dagoen erakunde antolakuntzarekin?

Dynamics 365 erakundeak Dynamics 365 instantzia global baten izena ordezkatzen du. Izen hori normalean enpresa globalaren izena da.

Erakundearen unitatea erakundea enpresa globalean talde edo zatiketa bat da. Talde edo zatiketa honek funtzio eta kostu prezio-zerrenda bat dauka funtzio horientzat, eta funtzioak eta prezio-zerrendak enpresako beste talde edo zatiketa batzuen eginkizun eta prezio-zerrendak desberdinak dira.

Project Operations instalatzen denean, antolaketan oinarritutako antolaketa-unitate aurredeterminatu bat sortzen da. Dauden baliabide guztiak erakundearen unitate lehenetsian esleitzen dira. Erabiltzaile berriak edo Active Directory-ren Dynamics 365-en baliabide berriak inportatzen badira, erabiltzaileen inportazio-prozesua proiektu-eragiketetan aurrez zehaztutako antolaketa-unitateari esleitzen dizkio.

#### <a name="how-does-the-organizational-unit-entity-differ-from-the-business-unit-entity"></a>Zertan bereizten da Negozio Unitateko Erakundearen Antolakuntza Unitateko erakundea?

Dynamics 365-en, Business Unit entitatea segurtasun eraikuntza da. Erabiltzaileen negozio unitate batekin elkartzeak erabiltzaileak sarbidea duen entitateak eta entitate erregistroak zehazten ditu. Erabiltzaileak entitate-erregistro horietarako dituen baimenak (Sortu, Irakurri, Idatzi, Ezabatu, Erantsi, Honi erantsi, Esleitu edo Partekatu) zehazten ditu.

Erakundearen unitate erakundeak enpresa talde edo zatiketa bat du, esleitutako langileentzako kostu tasak desberdinak dituena. Baliabide bat erakundearen unitatearekin elkartzeak zehazten du baliabidearen kostua proiektuaren konpromisoan.

Dynamics 365 ezartzen duzunean, optimizatu segurtasun baimena negozio unitateen hierarkiarako eta erabiltzaileak negozio unitateei esleitzeko. Esleitu negozio unitate berean erregistro multzo bera sartu behar duten erabiltzaile guztiei. Unitate antolatzaileak ez du eraginik segurtasun baimenean edo sarbidean.

**Antolamendu-unitateen eta negozio-unitateen modelatzean alde potentziala erakusten duen adibidea**

Contoso, Ltd.-ek Microsoft teknologiaren praktika oparoa du. Dabid eta Aizpea biak C\# garatzaileak dira, baina Aizpea Gasteizen dago, Dabid Iruñekoa den bitartean. Proiektu-konpromiso gehienek Contoso Indiako eta Contoso Estatu Batuetako baliabideak behar dituzte, eta Prakashek eta Triciak segurtasun-maila bera eskatzen dute praktika-arlo horretako proiektuetarako. Hala ere, Badiola Iruñeko garatzaileen kostua ezberdina da Badiola Gasteizeko garatzaileen kostua.

Dynamics 365 eta Project Operations-en bidez eszenatoki honetarako diseinatzeko modu ezin hobea da.

1. Sortu Microsoft teknologiaren praktika negozio unitate gisa eta lotu Dabid eta Aizpea berarekin. Horrela, bi langileek praktika-eremu horretan edozein proiektutara segurtasun-maila bera izatea bermatzen laguntzen du. Biek aurrerapena egiaztatu ahal izango dute, eta denbora, gastuak, materialaren erabilera eta zereginen eguneratzeak jakinarazi ahal izango dituzte.
2. Bi antolaketa-unitate sortzen ditu, proiektuaren kostua behar bezala islatzen dela bermatzeko.
3. Trizia Contoso Estatu Batuekin eta Prakash Contoso Indiarekin lotzen ditu.
4. Esleitu kostu prezio-zerrenda egokiak erakunde biei. Horrela, Prakash eta Tricia proiektuetan jasotzen diren kostuek Contoso Estatu Batuen eta Contoso la Indiaren arteko kostuen arteko aldea zehaztasunez islatzen dutela bermatzen laguntzen duzu.

#### <a name="are-organizational-units-related-to-sales-territories-in-dynamics-365"></a>Dynamics 365-en salmenta lurraldeekin erlazionatuta daude antolakuntza unitateak?

Ez dago loturarik edo harremanik salmenten lurraldeen eta erakundearen unitateen artean. Salmenta-lurraldea normalean salmentak gertatzen diren eremu geografikoa da. Salmenta prezio-zerrenda salmenta-urralde bakoitzari lotuta egon daiteke.

Erakunde unitatea enpresako barne-talde edo zatiketa da, beste dibisio batzuei edo kanpoko bezeroei saltzen dituen funtzio multzo baten kostuak kontrolatzen dituena.

**Antolamendu-unitateen eta salmenta-lurraldeen modelatzean alde potentziala erakusten duen adibidea**

Badila, Ltd.-k bi garapen zentro ditu: Badiola Gasteiz eta Badiola Iruñea. Baliabideen kostua oso ezberdina da bi garapen-zentro horien artean. Contosok informazioaren teknologia zerbitzuak (TI) saltzen ditu nazioarteko merkatu askotan, hala nola Latinoamerikan, Ipar Amerikan, Asia-Pazifikoan, Mendebaldeko Europan eta Ekialde Ertainean. Proiektu bereko funtzioen fakturen tasak oso alda daitezke merkatu hauetan. Badiola Gasteizek eta Badiola Iruñeak erakundearen unitate gisa eratu beharko lirateke, eta erakundearen unitate bakoitzak bere kostuen prezio-zerrenda izan beharko luke. Asia-Pazifikoa, Latinoamerika, Ipar Amerika, Mendebaldeko Europa eta Ekialde Hurbilean salmenta-lurralde gisa ezarri beharko lirateke, eta salmenta-lurralde bakoitzak bere salmenta prezio-zerrenda izan beharko luke.

#### <a name="why-is-there-a-restriction-on-the-association-of-price-lists-with-organizational-units"></a>Zergatik dago murrizketarik prezio-zerrenden erakundearen unitateekin lotzeari dagokionez?

Salmenten prezioak zerbitzuak saltzen diren gune geografiko edo merkatuetarako bakarra da. Enpresa baten barne-banaketak ez dute normalean zerbitzu mota bereko salmenten prezio propiorik izaten. Hala ere, barne-banaketak saltzen diren ondasunen kostuak (COGS) desberdinak dituzte, enplegatzen duten pertsonen trebetasunen eta eskualdeko lan-baldintzen arabera. Erakunde-unitateak enpresa baten barne-banaketa gisa eredutzen direnez, kostuen prezio-zerrendak soilik izan ditzakete.

#### <a name="why-cant-we-associate-sales-price-lists-with-organizational-units"></a>Zergatik ezin ditugu salmenta-prezioen zerrendak antolaketa-unitateekin lotu?

Proiektu-eragiketetan, salmenta-prezioen zerrendak bezeroekin eta salmenta-lurraldeekin lotu daitezke. Aukera, Kotizazioa, Proiektu Kontratua eta Proiektua bezalako erakunde transakzionalek bezeroaren kontura edo salmenten lurraldera atxikitzen diren salmenta-prezioen zerrendak erabiltzen dituzte, fakturazio-tasak eta proiektua kontratatzeko diru-sarrera potentzialak zehazteko.

Kostuen prezioen-zerrendak erakundearen unitateekin lotzen dira. Aukera, Kotizazioa, Proiektu Kontratua eta Proiektua bezalako erakunde transakzionalek kontratazio-unitateari erantsitako kostu-prezioen zerrendak erabiltzen dituzte proiektu-konpromiso baten kostuak zehazteko.

#### <a name="are-organizational-units-hierarchical-in-project-operations"></a>Antolaketa-unitateak hierarkikoak al dira proiektu-eragiketetan?

Ez. Project Operations-en egungo bertsioan, antolakuntza unitateak ez dira hierarkikoak. Beraz, ezin ditu honako lan hauek egin:

- Konfiguratu patroi bat, hierarkia bat zeharkatzen duen kostu-prezio predeterminatuak sartzeko.
- Ea adierazten dituen antolaketa-unitatearen hierarkiaren maila desberdinetan metatzen diren diru-sarrerak edo kostuak.

#### <a name="were-a-big-multinational-firm-that-has-a-complex-multilevel-hierarchy-of-cost-centers-divisions-and-billing-offices-how-can-we-best-use-the-concept-of-organizational-units-in-the-current-version-of-project-operations"></a>Enpresa multinazional handi bat gara, kostu-, dibisio- eta fakturazio-bulegoen hierarkia konplexua eta multinibela duena. Nola erabil dezakegu hobeto antolakuntza-unitateen kontzeptua Project Operations-en egungo bertsioan?

Kostu-zentroen, dibisioen, fakturazio-bulegoen eta abarren hierarkia konplexua duzunean, konfigura itz ezazu hierarkia horren orri nodoak antolaketa-unitate desberdin gisa.

Hurrengo adibidean hierarkia tipiko bat agertzen da.

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

Bere hierarkia adibide honen antzekoa bada, zerrenda lau gisa konfiguratu behar du, hemen agertzen den bezala:

- Badiola Iruñea - SAP Praktika - Aholkulari Teknikoak
- Badiola Iruñea - SAP Praktika - Aholkulari funtzionala
- Badiola Iruñea - Microsoft Technology Aholkulari funtzionala
- Badiola Iruñea - Microsoft Technology Aholkulari funtzionala
- Badiola Gasteiz - SAP Praktika - Aholkulari Teknikoak
- Badiola Gasteiz - SAP Praktika - Aholkulari funtzionala
- Badiola Gasteiz - Microsoft Technology Aholkulari teknikoak
- Badiola Gasteiz - Microsoft Technology Aholkulari funtzionala

#### <a name="were-a-small-professional-services-company-that-operates-as-only-one-division-how-can-we-best-use-the-concept-of-organizational-units-in-the-current-version-of-project-operations"></a>Zerbitzu profesionalean maila bakarrean lan egiten duen enpresa txiki bat gara. Nola erabil dezakegu hobeto antolakuntza-unitateen kontzeptua Project Operations-en egungo bertsioan?

Zure enpresak kostuen prezioen zerrenda bat duen unitate gisa funtzionatzen badu, ez duzu antolaketa unitaterik ezarri behar. Proiektu-eragiketak instalatzeak aurrez zehaztutako antolaketa-unitate bat sortzen du, erakundearen izen bera duena. Lehenespenez dauden baliabide guztiak erakundearen unitate lehenetsian esleitzen dira. Sistemak unitate antolatzaile bat aukeratu behar duen bakoitzean, unitate antolakuntza hau lehenespenez hautatzen da.

#### <a name="when-a-project-is-created-from-a-quote-or-project-contract-line-the-default-contracting-unit-comes-from-the-quote-or-project-contract-what-is-the-default-contracting-unit-if-a-project-is-created-before-sales-entities-such-as-quote-or-project-contract"></a>Proiektua aurrekontuen edo proiektuaren kontratuaren lerrotik sortzen denean, kontratazio unitate lehenetsia aurrekontu edo proiektu kontratutik dator. Zein da aurrez zehaztutako kontratazio-unitatea, Quote edo Project Contract bezalako salmenta-erakundeak baino lehenago proiektu bat sortzen bada?

Proiektua bere kabuz sortutakoan, proiektuaren kontratazio unitate lehenetsia sortzen duen erabiltzailea da. Erabiltzailea ere proiektu kudeatzaile lehenetsia da. Proiektua salmenta-erakunde bati esleitzen bazaio, hala nola kotizazio bati edo proiektu-kontratu bati, proiektuaren kontratazio-unitatea salmenta-erakundean oinarritzen da. Kasu honetan, proiektuaren kalkuluak berriro kalkulatu litezke, izan ere, kostu-estimazioen aldaketak kalkulatzeko kostu-prezioen zerrenda erabiltzen da kontratazio-unitatea aldatzen bada. Salmenta-prezioen zerrenda aldatuko diren salmenten zenbatespenak kalkulatzeko erabiltzen da, kotizazio-proiektuaren prezioen zerrendarekin sinkronizatuta egon daitezen.

**Proiektuaren kontratazio- eta** diru-unitatearen **arloak** blokeatuta daude ediziorako, proiektua esleitu zaion salmenta-erakundearen baloreekin sinkronizatuta egon behar baitute(aurrekontua edo proiektu-kontratua).

## <a name="create-and-maintain-organizational-units-in-project-operations"></a>Proiektu-eragiketetan antolaketa-unitateak sortzea eta mantentzea

Proiektu-eragiketetan antolaketa-unitate bat sortzeko, jarraitu urrats horiek.

1. **Ikusi Konfigurazioko antolaketa-unitateak \>**.
2. Hautatu **Berria**.
3. **Arlo Orokorrean**, izenaren **arloan**, izen bat idatzi antolaketa-unitaterako. Ondoren, gainerako eremuak behar den moduan ezarri.
4. Hautatu **gorde** erregistroa sortzeko eta argitaratzen jarraitu ahal izateko.
5. Kostu-zerrendetan **·**, aukeratu zeinurik handiena (**+**) prezio-zerrenda bat eransteko. Kostu-testuingurua **duten** prezioen zerrendak bakarrik erantsi ditzakezu hemen.
6. Izena zelaian **, aukeratu** Bilatu **botoia eta aukeratu antolakuntza-unitatearen eskura jarri nahi duzun prezio-zerrenda bat.** Jarraitu prezio-zerrendak behar den neurrian gehitzen.
7. Prezio-zerrendak gehitzen amaitzen dituzunean, aukeratu **gorde** orriaren beheko eskuineko izkinan.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
