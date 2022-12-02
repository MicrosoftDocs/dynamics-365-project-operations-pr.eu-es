---
title: Erakundearen unitateak
description: Artikulu honek erakundearen unitateen kontzeptua deskribatzen du eta erakundearen unitateak nola sortu eta nola mantendu azaltzen du Microsoft Dynamics 365 Project Operations-en.
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
# <a name="organizational-units-overview"></a>Erakundearen unitatearen ikuspegi orokorra

Microsoft Dynamics 365 Project Operations-en, *erakundearen unitate* bat zerbitzu edo zerbitzu profesionalen enpresa bateko talde desberdina da, kostu tasak dituzten baliabide faktikoak erabiltzen dituena.

Hainbat praktika-arlo edo negozio-lerroetan baliabide teknikoak erabiltzen dituzten zerbitzu profesionalen enpresentzat, praktika-arlo edo negozio-lerro batean rol bat betetzearen kostua desberdina izan daiteke beste praktika-arlo batean eginkizuna betetzeko. Erakundearen unitatearen kontzeptuak agertoki horretan laguntzen du funtzio horiengatik kostu egitura desberdina duen enpresen banaketan funtzio fakturagarrien multzoa taldekatzeko modua eskainiz.

## <a name="the-concept-of-organizational-units-in-project-operations"></a>Erakundeen unitateen kontzeptua Project Operations-en

Project Operations-en, erakundearen unitateak moneta zehatza eta kostu prezio-zerrenda zehatzak ditu.

Erakunde unitate bateko moneta kostuen jarraipena egiteko erabiltzen den lehen moneta da.

Kostuen prezio-zerrenda bat edo gehiago erantsi daitezke antolaketa unitate bakoitzari. Project Operations-ek mugak jartzen ditu erakundearen unitate bati atxiki daitezkeen prezio-zerrendetan:

- Prezio-zerrendak erakunde unitatearen monetan egon behar du.
- Prezio-zerrendek kostuen prezio-zerrendak izan behar dute.

Gainera, baliabide entitatearen erakundearen unitate atributu bat dago. Baliabide bakoitzari erakundearen unitate eslei diezaiokezu.

### <a name="roles-of-organizational-units"></a>Erakundearen unitatearen funtzioak

Erakundearen unitateak bi funtzio betetzen ditu Project Operations-en:

- **Kontratazio Unitatea**: salmenta irabaztea eta bezeroari lana eta zerbitzuak entregatzea kudeatzeaz arduratzen den enpresa-taldea edo zatiketa ordezkatzen duen antolakuntza-unitatea. Kontratazio unitateak identifikatzen du **Kontratazio Unitatea** eremua goiburuko ataleko goiburuko atalean **Abagunea**, **Eskaintza**, **Proiektuaren kontratua**, eta **Proiektua** orrietakoak.
- **Baliabide Unitatea**: baliabide bat dagokion edo esleitzen zaion unitate antolatzailea. Erakundearen unitate honek bere baliabideak eman ditzake laneko aitorpenetan (SOWs) eta unitate kontratatzailearen jabetzakoak diren eginkizunetarako.

![Kontratazio unitateak eta baliabide unitateak.](media/OrgUnits.png)

### <a name="organizational-unit-faq"></a>Erakundearen unitateari buruz maiz egiten diren galderak

Erakundearen unitate batzuei buruzko ohiko galdera ugariren erantzunak aurkituko dituzu hemen:

#### <a name="how-is-the-organizational-unit-entity-in-project-operations-related-to-the-organization-entity-that-already-exists-in-dynamics-365"></a>Nola lotzen da Project Operations-eko erakundearen unitateko entitatea Dynamics 365-en dagoeneko existitzen den erakundearen entitatearekin?

Erakundearen entitatea Dynamics 365-ek Dynamics 365 instantzia global baten izena adierazten du. Izen hori normalean enpresa globalaren izena da.

Erakundearen unitatea erakundea enpresa globalean talde edo zatiketa bat da. Talde edo zatiketa honek funtzio eta kostu prezio-zerrenda bat dauka funtzio horientzat, eta funtzioak eta prezio-zerrendak enpresako beste talde edo zatiketa batzuen eginkizun eta prezio-zerrendak desberdinak dira.

Project Operations instalatzen denean, erakundearen unitate lehenetsi bat sortzen da antolakuntzan oinarrituta. Dauden baliabide guztiak erakundearen unitate lehenetsian esleitzen dira. Active Directory-ko erabiltzaile edo baliabide berriak Dynamics 365-en inportatzen badira, erabiltzaileen inportazio prozesuak Project Operations-eko erakundearen unitate lehenetsiari esleitzen dizkio.

#### <a name="how-does-the-organizational-unit-entity-differ-from-the-business-unit-entity"></a>Zertan desberdintzen da erakundearen unitateko entitatea negozio unitateko entitatearengandik?

Dynamics 365-en, Business Unit entitatea segurtasun eraikuntza da. Erabiltzaileen negozio unitate batekin elkartzeak erabiltzaileak sarbidea duen entitateak eta entitate erregistroak zehazten ditu. Erabiltzaileak entitate-erregistro horietarako dituen baimenak (Sortu, Irakurri, Idatzi, Ezabatu, Erantsi, Honi erantsi, Esleitu edo Partekatu) zehazten ditu.

Erakundearen unitate erakundeak enpresa talde edo zatiketa bat du, esleitutako langileentzako kostu tasak desberdinak dituena. Baliabide bat erakundearen unitatearekin elkartzeak zehazten du baliabidearen kostua proiektuaren konpromisoan.

Dynamics 365 ezartzen duzunean, optimizatu segurtasun baimena negozio unitateen hierarkiarako eta erabiltzaileak negozio unitateei esleitzeko. Esleitu negozio unitate berean erregistro multzo bera sartu behar duten erabiltzaile guztiei. Unitate antolatzaileak ez du eraginik segurtasun baimenean edo sarbidean.

**Erakundearen unitateen eta negozio-unitateen ereduak sortzean balizko diferentzia bat erakusten duen adibidea**

Contoso, Ltd.-ek Microsoft teknologiaren praktika oparoa du. Dabid eta Aizpea biak C\# garatzaileak dira, baina Aizpea Gasteizen dago, Dabid Iruñekoa den bitartean. Proiektuen konpromiso gehienek Contoso India eta Contoso AEB-ko baliabideak behar dituzte, eta Dabid eta Aizpeak segurtasun maila bera eskatzen dute praktika arlo horretako proiektuetarako. Hala ere, Badiola Iruñeko garatzaileen kostua ezberdina da Badiola Gasteizeko garatzaileen kostua.

Hemen gertakari hau diseinatzeko modu ezin hobea da Dynamics 365 eta Project Operations erabiliz.

1. Sortu Microsoft teknologiaren praktika negozio unitate gisa eta lotu Dabid eta Aizpea berarekin. Horrela, bi langileek segurtasun maila berdina izan dezaketela bermatzen laguntzen duzu praktika arloko edozein proiektuetarako. Biek egiaztatu ahal izango dute aurrerapena eta denbora, gastuak, materialen erabilera eta zereginen eguneratzeak jakinarazi.
2. Sortu bi antolakuntza unitate proiektuaren kostua behar bezala islatzen dela bermatzeko.
3. Elkartu Aizpea Contoso AEB-rekin eta lotu Dabid Contoso India-rekin.
4. Esleitu kostu prezio-zerrenda egokiak erakunde biei. Horrela, Dabid eta Aizpea proiektuetan grabatutako kostuak zehatz-mehatz kontratatzen dituzu Contoso AEB eta Contoso India arteko kostuen aldea.

#### <a name="are-organizational-units-related-to-sales-territories-in-dynamics-365"></a>Dynamics 365-en salmenta lurraldeekin erlazionatuta daude antolakuntza unitateak?

Ez dago loturarik edo harremanik salmenten lurraldeen eta erakundearen unitateen artean. Salmenta-lurraldea normalean salmentak gertatzen diren eremu geografikoa da. Salmenta prezio-zerrenda salmenta-urralde bakoitzari lotuta egon daiteke.

Erakunde unitatea enpresako barne-talde edo zatiketa da, beste dibisio batzuei edo kanpoko bezeroei saltzen dituen funtzio multzo baten kostuak kontrolatzen dituena.

**Erakundearen unitateen eta salmenta-lurraldeen ereduak sortzean balizko diferentzia bat erakusten duen adibidea**

Badila, Ltd.-k bi garapen zentro ditu: Badiola Gasteiz eta Badiola Iruñea. Baliabideen kostuak asko dira bi garapen zentro horien artean. Contoso-k nazioarteko merkatu askotan saltzen ditu bere informazioaren teknologia (IKT) zerbitzuak, hala nola Latinoamerikan, Ipar Amerikan, Asia-Pazifikoan, Mendebaldeko Europan eta Ekialde Hurbilean. Proiektu bereko funtzioen fakturen tasak oso alda daitezke merkatu hauetan. Badiola Gasteizek eta Badiola Iruñeak erakundearen unitate gisa eratu beharko lirateke, eta erakundearen unitate bakoitzak bere kostuen prezio-zerrenda izan beharko luke. Asia-Pazifikoa, Latinoamerika, Ipar Amerika, Mendebaldeko Europa eta Ekialde Hurbilean salmenta-lurralde gisa ezarri beharko lirateke, eta salmenta-lurralde bakoitzak bere salmenta prezio-zerrenda izan beharko luke.

#### <a name="why-is-there-a-restriction-on-the-association-of-price-lists-with-organizational-units"></a>Zergatik dago murrizketarik prezio-zerrenden erakundearen unitateekin lotzeari dagokionez?

Salmenten prezioak zerbitzuak saltzen diren gune geografiko edo merkatuetarako bakarra da. Enpresa baten barne-banaketak ez dute normalean zerbitzu mota bereko salmenten prezio propiorik izaten. Hala ere, barne-banaketak saltzen diren ondasunen kostuak (COGS) desberdinak dituzte, enplegatzen duten pertsonen trebetasunen eta eskualdeko lan-baldintzen arabera. Erakunde-unitateak enpresa baten barne-banaketa gisa eredutzen direnez, kostuen prezio-zerrendak soilik izan ditzakete.

#### <a name="why-cant-we-associate-sales-price-lists-with-organizational-units"></a>Zergatik ezin ditugu salmenta prezio-zerrendak erakundearen unitateekin lotu?

Project Operations-en, salmenten prezio-zerrendak bezeroekin eta salmenta-lurraldeekin lotu daitezke. Abagunea, Eskaintza, Proiektu-kontratua eta Proiektua bezalako erakunde transakzionalek bezeroaren kontura edo salmenta-lurraldeari atxikitako salmenten prezio-zerrendak erabiltzen dituzte proiektuaren konpromisoan fakturen tasak eta diru-sarrera potentzialak zehazteko.

Kostuen prezioen-zerrendak erakundearen unitateekin lotzen dira. Abagunea, Eskaintza, Proiektu-kontratua eta Proiektua bezalako erakunde transakzioek, kontratazio unitateari atxikitako kostuen prezio-zerrendak erabiltzen dituzte proiektuaren konpromisoari dagozkion kostuak zehazteko.

#### <a name="are-organizational-units-hierarchical-in-project-operations"></a>Erakunde-unitateak hierarkikoak al dira Project Operations-en?

Ez. Project Operations-en oraingo oharrean, erakundearen unitateak ez dira hierarkikoak. Horregatik, honako zeregin hauek ezin dituzu egin:

- Konfiguratu eredua hierarkia bat zeharkatzen duen kostu-prezio lehenetsiak sartzeko.
- Sarreren edo kostuen berri eman erakundearen unitateen hierarkiaren maila desberdinetan.

#### <a name="were-a-big-multinational-firm-that-has-a-complex-multilevel-hierarchy-of-cost-centers-divisions-and-billing-offices-how-can-we-best-use-the-concept-of-organizational-units-in-the-current-version-of-project-operations"></a>Multinazional enpresa handia gara kostu zentroen, zatiketen eta fakturazio bulegoen hierarkia konplexua eta askotarikoa. Nola erabil dezakegu erakundearen unitatearen kontzeptua Project Operations-en egungo bertsioan?

Kostu zentroak, zatiketak, fakturazio bulegoak, etab., Hierarkia konplexua baduzu, konfiguratu hierarkia horren hosto-nodoak antolakuntza unitate desberdin gisa.

Hurrengo adibidean hierarkia tipikoa agertzen da.

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

Zure hierarkia adibidearen antzekoa bada, zerrenda lau gisa ezarri behar duzu hemen:

- Badiola Iruñea - SAP Praktika - Aholkulari Teknikoak
- Badiola Iruñea - SAP Praktika - Aholkulari funtzionala
- Badiola Iruñea - Microsoft Technology Aholkulari funtzionala
- Badiola Iruñea - Microsoft Technology Aholkulari funtzionala
- Badiola Gasteiz - SAP Praktika - Aholkulari Teknikoak
- Badiola Gasteiz - SAP Praktika - Aholkulari funtzionala
- Badiola Gasteiz - Microsoft Technology Aholkulari teknikoak
- Badiola Gasteiz - Microsoft Technology Aholkulari funtzionala

#### <a name="were-a-small-professional-services-company-that-operates-as-only-one-division-how-can-we-best-use-the-concept-of-organizational-units-in-the-current-version-of-project-operations"></a>Zerbitzu profesionalean maila bakarrean lan egiten duen enpresa txiki bat gara. Nola erabil dezakegu erakundearen unitatearen kontzeptua Project Operations-en egungo bertsioan?

Zure enpresak kostuen prezioen zerrenda bat duen unitate gisa funtzionatzen badu, ez duzu antolaketa unitaterik ezarri behar. Project Operations-en instalazioan zehar, antolakuntza unitate lehenetsi bat sortzen du erakundearen izen bera duena. Lehenespenez dauden baliabide guztiak erakundearen unitate lehenetsian esleitzen dira. Sistemak unitate antolatzaile bat aukeratu behar duen bakoitzean, unitate antolakuntza hau lehenespenez hautatzen da.

#### <a name="when-a-project-is-created-from-a-quote-or-project-contract-line-the-default-contracting-unit-comes-from-the-quote-or-project-contract-what-is-the-default-contracting-unit-if-a-project-is-created-before-sales-entities-such-as-quote-or-project-contract"></a>Proiektua aurrekontuen edo proiektuaren kontratuaren lerrotik sortzen denean, kontratazio unitate lehenetsia aurrekontu edo proiektu kontratutik dator. Proiektu bat salmentako entitateen aurretik sortzen bada, aurrekontua edo proiektuaren kontratua, zein da kontratazio unitate lehenetsia?

Proiektua bere kabuz sortutakoan, proiektuaren kontratazio unitate lehenetsia sortzen duen erabiltzailea da. Erabiltzailea ere proiektu kudeatzaile lehenetsia da. Proiektua salmentako entitate batera mapatzen bada, aurrekontu edo proiektu kontratu gisa, proiektuaren kontratazio unitatea salmenta entitatean oinarritzen da. Kasu honetan, proiektuaren kalkuluak berriro kalkulatu litezke, izan ere, kostu-estimazioen aldaketak kalkulatzeko kostu-prezioen zerrenda erabiltzen da kontratazio-unitatea aldatzen bada. Salmenten prezioen zerrenda aldatuko diren salmenten kalkuluak kalkulatzeko erabiltzen da, proiektuaren prezioen zerrenda aurrekontuarekin sinkronizatzeko.

**Kontratazio Unitatea** eta **Moneta** Proiektuko eremuak editatzeko blokeatuta daude, proiektuaren mapak egiten dituen salmenta-erakundean (aurrekontua edo proiektu kontratua) dituzten balioekin sinkronizatuta egon behar dutelako.

## <a name="create-and-maintain-organizational-units-in-project-operations"></a>Project Operations-en erakundearen unitateak sortzea eta mantentzea

Jarraitu urrats hauek Project Operations-en erakundearen unitate bat sortzeko.

1. Joan **Ezarpenak \> Antolaketa-unitateak**.
2. Hautatu **Berria**.
3. **Orokorra** arean, **Izena** eremuan, adierazi erakundearen unitatearen izena. Ondoren, ezarri gainerako eremuak behar bezala.
4. Hautatu **Gorde**, erregistroa sortzeko, horrela editatzen jarraitu ahal izateko.
5. **Kostuen prezio-zerrendak** atalean, hautatu plus ikurra (**+**) prezio-zerrenda gehitzeko. **Kostua** testuinguru duten prezio-zerrendak soilik gehi ditzakezu hemen.
6. **Izena** eremuan, hautatu **Bilaketa** botoia eta hautatu erakundearen unitate honetan erabilgarri egotea nahi duzun prezio-zerrenda. Jarraitu behar diren prezio-zerrendak gehitzen.
7. Prezio-zerrendak gehitzeaz amaitutakoan, hautatu **Gorde** ikonoa orriko beheko eskuineko izkinan.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
