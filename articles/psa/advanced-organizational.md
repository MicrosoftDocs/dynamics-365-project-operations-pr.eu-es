---
title: Erakundearen unitateak
description: Gai honek entitate-unitate eta unitateei buruzko informazioa ematen du Dynamics 365 Project Service Automation-en.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/04/2019
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
ms.openlocfilehash: 454d9a4c4d139f493adf4604f8ba40a0211f0eec
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071148"
---
# <a name="organizational-units"></a>Erakundearen unitateak 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Dynamics 365 Project Service Automation, antolakuntza-unitate bat zerbitzu edo zerbitzu profesionalen enpresa bateko talde desberdina da, kostu tasak dituzten baliabide faktikoak erabiltzen dituena.

Hainbat praktika-arlo edo negozio-lerroetan baliabide teknikoak erabiltzen dituzten zerbitzu profesionalen enpresentzat, praktika-arlo edo negozio-lerro batean rol bat betetzearen kostua desberdina izan daiteke beste praktika-arlo edo negozio-lerro batean eginkizuna betetzeko. Kontzeptu antolakuntza unitateak agertoki horretan laguntzen du funtzio horiengatik kostu egitura desberdina duen sozietatearen banaketan rol fakturatzaileen multzoa taldekatzeko modua eskainiz.

## <a name="key-attributes-and-associations-of-organizational-units"></a>Erakundearen unitateen funtsezko atributu eta eta elkarteak

PSAn, PSAko erakundearen unitateak moneta zehatza eta kostu prezio-zerrenda zehatzak ditu.

Erakunde unitate bateko moneta kostuen jarraipena egiteko erabiltzen den lehen moneta da.

Kostuen prezio-zerrenda bat edo gehiago erantsi daitezke antolaketa unitate bakoitzari. PSAk mugak jartzen ditu erakunde unitate bati atxiki daitezkeen prezio-zerrendetan:

- Prezio-zerrendak erakunde unitatearen monetan egon behar du
- Prezio-zerrendek kostuen prezio-zerrendak izan behar dute

Gainera, baliabide entitatearen erakundearen unitate atributu bat dago. Baliabide bakoitzari erakundearen unitate eslei diezaiokezu.

## <a name="roles-of-organizational-units"></a>Erakundearen unitatearen funtzioak

Erakundearen unitateak bi funtzio betetzen ditu PSAn:

- **Kontratazio Unitatea** : salmenta irabaztea eta bezeroari lana eta zerbitzuak entregatzea kudeatzeaz arduratzen den enpresa-taldea edo zatiketa ordezkatzen duen antolakuntza-unitatea. Kontratazio unitateak identifikatzen du **Kontratazio Unitatea** eremua goiburuko ataleko goiburuko atalean **Abagunea** , **Eskaintza** , **Proiektuaren kontratua** , eta **Proiektua** orrietakoak.
- **Baliabide Unitatea** : baliabide bat dagokion edo esleitzen zaion unitate antolatzailea. Erakundearen unitate honek bere baliabideak eman ditzake laneko aitorpenetan (SOWs) eta unitate kontratatzailearen jabetzakoak diren eginkizunetarako.

> ![Kontratazio unitateak eta baliabide unitateak](media/advanced-1.png)

## <a name="organizational-unit-faqs"></a>Erakunde-unitatearen FAQak

Erakundearen unitate batzuei buruzko ohiko galdera ugariren erantzunak aurkituko dituzu hemen:

### <a name="how-is-the-organizational-unit-entity-in-psa-related-to-the-organization-entity-that-already-exists-in-dynamics-365"></a>Nola lotzen da PSAko Antolakuntza Unitateko entitatea Dynamics 365-en dagoeneko existitzen den Antolakuntza entitatearekin?

Erakundearen entitatea Microsoft Dynamics 365-ek Dynamics 365 instantzia global baten izena adierazten du. Izen hori normalean enpresa globalaren izena da.

Erakundearen unitatea erakundea enpresa globalean talde edo zatiketa bat da. Talde edo zatiketa honek funtzio eta kostu prezio-zerrenda bat dauka funtzio horientzat, eta funtzioak eta prezio-zerrendak enpresako beste talde edo zatiketa batzuen eginkizun eta prezio-zerrendak desberdinak dira.

PSA instalatzen denean, antolakuntza unitate lehenetsi bat sortzen da antolakuntzan oinarrituta. Dauden baliabide guztiak erakundearen unitate lehenetsian esleitzen dira. Active Directory-ko erabiltzaile edo baliabide berriak Dynamics 365-en inportatzen badira, erabiltzaileen inportazio prozesuak PSAko antolaketa unitate lehenetsiari esleitzen dizkio.
 
### <a name="how-does-the-organizational-unit-entity-differ-from-the-business-unit-entity"></a>Zertan desberdintzen da erakundearen unitateko entitatea negozio unitateko entitatearengandik?

Dynamics 365-en, Business Unit entitatea segurtasun eraikuntza da. Erabiltzaileen negozio unitate batekin elkartzeak erabiltzaileak sarbidea duen entitateak eta entitate erregistroak zehazten ditu. Erabiltzaileak entitate-erregistro horietarako dituen baimenak (Sortu, Irakurri, Idatzi, Ezabatu, Erantsi, Honi erantsi, Esleitu edo Partekatu) zehazten ditu.

Erakundearen unitate erakundeak enpresa talde edo zatiketa bat du, esleitutako langileentzako kostu tasak desberdinak dituena. Baliabide bat erakundearen unitatearekin elkartzeak zehazten du baliabidearen kostua proiektuaren konpromisoan.

Dynamics 365 ezartzen duzunean, optimizatu segurtasun baimena negozio unitateen hierarkiarako eta erabiltzaileak negozio unitateei esleitzeko. Esleitu negozio unitate berean erregistro multzo bera sartu behar duten erabiltzaile guztiei. Unitate antolatzaileak ez du eraginik segurtasun baimenean edo sarbidean.

#### <a name="example-of-organizational-units-and-business-units"></a>Erakunde unitateen eta negozio unitateen adibidea

Contoso, Ltd.-ek Microsoft teknologiaren praktika oparoa du. Dabid eta Aizpea biak C\# garatzaileak dira, baina Aizpea Gasteizen dago, Dabid Iruñekoa den bitartean. Proiektuen konpromiso gehienek Badiola Iruña eta Badiola Gasteizeko baliabideak behar dituzte, eta Dabid eta Aizpeak segurtasun maila bera eskatzen dute praktika arlo horretako proiektuetarako. Hala ere, Badiola Iruñeko garatzaileen kostua ezberdina da Badiola Gasteizeko garatzaileen kostua.

Hemen gertakari hau diseinatzeko modu ezin hobea da Dynamics 365 eta PSA erabiliz.

1. Sortu Microsoft teknologiaren praktika negozio unitate gisa eta lotu Dabid eta Aizpea berarekin. Horrela, bi langileek segurtasun maila berdina izan dezaketela bermatzen laguntzen duzu praktika arloko edozein proiektuetarako. Biek egiaztatu ahal izango dute aurrerapena eta denbora, gastuak eta zereginen eguneratzeak jakinarazi. 
2. Sortu bi antolakuntza unitate proiektuaren kostua behar bezala islatzen dela bermatzeko. 
3. Elkartu Aizpea Badiola Gasteizekin eta lotu Dabid Badiola Iruñearekin.
4. Esleitu kostu prezio-zerrenda egokiak erakunde biei. Horrela, Dabid eta Aizpea proiektuetan grabatutako kostuak zehatz-mehatz kontratatzen dituzu Badiola Gasteiz eta Badiola Iruñea arteko kostuen aldea.

### <a name="are-organizational-units-related-to-sales-territories-in-dynamics-365"></a>Dynamics 365-en salmenta lurraldeekin erlazionatuta daude antolakuntza unitateak?

Ez dago loturarik edo harremanik salmenten lurraldeen eta erakundearen unitateen artean. Salmenta-lurraldea normalean salmentak gertatzen diren eremu geografikoa da. Salmenta prezio-zerrenda salmenta-urralde bakoitzari lotuta egon daiteke.

Erakunde unitatea enpresako barne-talde edo zatiketa da, beste dibisio batzuei edo kanpoko bezeroei saltzen dituen funtzio multzo baten kostuak kontrolatzen dituena.

#### <a name="example-of-organizational-units-and-sales-territories"></a>Erakunde unitateen eta salmenta-lurraldeen adibidea

Badila, Ltd.-k bi garapen zentro ditu: Badiola Gasteiz eta Badiola Iruñea. Baliabideen kostuak asko dira bi garapen zentro horien artean.

Badiolak nazioarteko merkatu askotan saltzen ditu bere IT zerbitzuak, hala nola Latinoamerikan, Ipar Amerikan, Asia-Pazifikoan, Mendebaldeko Europan eta Ekialde Hurbilean. Proiektu bereko funtzioen fakturen tasak oso alda daitezke merkatu hauetan.

Badiola Gasteizek eta Badiola Iruñeak erakundearen unitate gisa eratu beharko lirateke, eta erakundearen unitate bakoitzak bere kostuen prezio-zerrenda izan beharko luke. Asia-Pazifikoa, Latinoamerika, Ipar Amerika, Mendebaldeko Europa eta Ekialde Hurbilean salmenta-lurralde gisa ezarri beharko lirateke, eta salmenta-lurralde bakoitzak bere salmenta prezio-zerrenda izan beharko luke.

### <a name="why-is-there-a-restriction-on-the-association-of-price-lists-with-organizational-units"></a>Zergatik dago murrizketarik prezio-zerrenden erakundearen unitateekin lotzeari dagokionez? 

Salmenten prezioak zerbitzuak saltzen diren gune geografiko edo merkatuetarako bakarra da. Enpresa baten barne-banaketak ez dute normalean zerbitzu mota bereko salmenten prezio propiorik izaten. Hala ere, barne-banaketak saltzen diren ondasunen kostuak (COGS) desberdinak dituzte, enplegatzen duten pertsonen trebetasunen eta eskualdeko lan-baldintzen arabera. Erakunde-unitateak enpresa baten barne-banaketa gisa eredutzen direnez, kostuen prezio-zerrendak soilik izan ditzakete.

### <a name="why-cant-we-associate-sales-price-lists-to-organizational-units"></a>Zergatik ezin ditugu salmenta prezio-zerrendak erakundearen unitateekin lotu?

PSAn, salmenten prezio-zerrendak bezeroekin eta salmenta-lurraldeekin lotu daitezke. Abagunea, Eskaintza, Proiektu-kontratua eta Proiektua bezalako erakunde transakzionalek bezeroaren kontura edo salmenta-lurraldeari atxikitako salmenten prezio-zerrendak erabiltzen dituzte proiektuaren konpromisoan fakturen tasak eta diru-sarrera potentzialak zehazteko.

Kostuen prezioen-zerrendak erakundearen unitateekin lotzen dira. Abagunea, Eskaintza, Proiektu-kontratua eta Proiektua bezalako erakunde transakzioek, kontratazio unitateari atxikitako kostuen prezio-zerrendak erabiltzen dituzte proiektuaren konpromisoari dagozkion kostuak zehazteko.

### <a name="are-organizational-units-hierarchical-in-psa"></a>Erakunde-unitateak hierarkikoak al dira PSAn?

Ez. PSAren oraingo oharrean, erakundearen unitateak ez dira hierarkikoak. Horrek esan nahi du ezin duzula:

- Konfiguratu eredua hierarkia bat zeharkatzen duen kostu-prezio lehenetsiak. 
- Sarreren edo kostuen berri eman erakundearen unitateen hierarkiaren maila desberdinetan.

### <a name="were-a-big-multinational-firm-with-a-complex-multilevel-hierarchy-of-cost-centers-divisions-and-billing-offices-how-can-we-make-the-best-use-of-the-organizational-unit-concept-in-this-version-of-the-project-service-app"></a>Multinazional enpresa handia gara kostu zentroen, zatiketen eta fakturazio bulegoen hierarkia konplexua eta askotarikoa. Nola egin dezakegu Project Service aplikazioaren bertsio honetan antolaketa unitatearen kontzeptuaren erabilerarik onena?

Kostu zentroak, zatiketak, fakturazio bulegoak, etab., Hierarkia konplexua baduzu, konfiguratu hierarkia horren hosto-nodoak antolakuntza unitate desberdin gisa.
Hurrengo adibidean hierarkia tipikoa agertzen da:

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
 
Zure hierarkia antzekoa bada, zerrenda lau gisa ezarri behar duzu hemen:
- Badiola Iruñea - SAP Praktika - Aholkulari Teknikoak 
- Badiola Iruñea - SAP Praktika - Aholkulari funtzionala       
- Badiola Iruñea - Microsoft Technology Aholkulari funtzionala 
- Badiola Iruñea - Microsoft Technology Aholkulari funtzionala 
- Badiola Gasteiz - SAP Praktika - Aholkulari Teknikoak  
- Badiola Gasteiz - SAP Praktika - Aholkulari funtzionala  
- Badiola Gasteiz - Microsoft Technology Aholkulari teknikoak 
- Badiola Gasteiz - Microsoft Technology Aholkulari funtzionala

### <a name="were-a-small-professional-services-company-that-operates-as-only-one-division-how-can-we-best-use-the-organizational-unit-concept-in-the-current-version-of-psa"></a>Zerbitzu profesionalean maila bakarrean lan egiten duen enpresa txiki bat gara. Nola erabil dezakegu erakundearen unitatearen kontzeptua PSAren egungo bertsioan?

Zure enpresak kostuen prezioen zerrenda bat duen unitate gisa funtzionatzen badu, ez duzu antolaketa unitaterik ezarri behar. PSA instalazioan zehar, Dynamics 365-ek antolakuntza unitate lehenetsi bat sortzen du erakundearen izen bera duena. Lehenespenez dauden baliabide guztiak erakundearen unitate lehenetsian esleitzen dira. Sistemak unitate antolatzaile bat aukeratu behar duen bakoitzean, unitate antolakuntza hau lehenespenez hautatzen da.

### <a name="when-a-project-is-created-from-a-quote-or-project-contract-line-the-default-contracting-unit-comes-from-the-quote-or-project-contract-if-a-project-is-created-before-sales-entities-such-as-quote-or-project-contract-what-is-the-default-contracting-unit"></a>Proiektua aurrekontuen edo proiektuaren kontratuaren lerrotik sortzen denean, kontratazio unitate lehenetsia aurrekontu edo proiektu kontratutik dator. Proiektu bat salmentako entitateen aurretik sortzen bada, aurrekontua edo proiektuaren kontratua, zein da kontratazio unitate lehenetsia?

Proiektua bere kabuz sortutakoan, proiektuaren kontratazio unitate lehenetsia sortzen duen erabiltzailea da. Erabiltzailea ere proiektu kudeatzaile lehenetsia da. Proiektua salmentako entitate batera mapatzen bada, aurrekontu edo proiektu kontratu gisa, proiektuaren kontratazio unitatea salmenta entitatean oinarritzen da. Kasu honetan, proiektuaren kalkuluak berriro kalkulatu litezke, izan ere, kostu-estimazioen aldaketak kalkulatzeko kostu-prezioen zerrenda erabiltzen da kontratazio-unitatea aldatzen bada. Salmenten prezioen zerrenda aldatuko diren salmenten kalkuluak kalkulatzeko erabiltzen da, proiektuaren prezioen zerrenda aurrekontuarekin sinkronizatzeko.

The **Kontratazio Unitatea** eta **Moneta** Proiektuko eremuak editatzeko blokeatuta daude, proiektuaren mapak egiten dituen salmenta-erakundean (aurrekontua edo proiektu kontratua) dituzten balioekin sinkronizatuta egon behar dutelako.