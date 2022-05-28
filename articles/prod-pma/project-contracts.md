---
title: Proiektu-kontratuak
description: Gai honek proiektu mota eta finantzaketa iturri desberdinetarako sor ditzakezun proiektuen kontratuen adibideak eta kontratuak eta fakturak bezeroen fakturak nola kudeatu ditzakezu.
author: Yowelle
ms.date: 11/03/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectContractsListPage, ProjProjectsListPage
audience: Application User, IT Pro
ms.reviewer: johnmichalak
ms.custom: 23561
ms.assetid: bfd18d9b-d9a6-4e21-bc95-bf4af45f617f
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 8cfc5183ce28574d865389eba72cafd3528741cc
ms.sourcegitcommit: 2c2a5a11d446adec2f21030ab77a053d7e2da28e
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/04/2022
ms.locfileid: "8683477"
---
# <a name="project-contracts"></a>Proiektu-kontratuak

[!include [banner](../includes/banner.md)]

Artikulu honek proiektu mota eta finantzaketa iturri desberdinetarako sor ditzakezun proiektuen kontratuen adibideak eta kontratuak eta fakturak bezeroen fakturak nola kudeatu ditzakezu.

Proiektu kontratu baterako sortzen duzun proiektu motak proiektuaren bezeroei fakturatzeko erabiltzen den metodoa zehazten du. Proiektuaren kontratua eta lotutako proiektua alda ditzakezu, baina ezin duzu proiektu mota aldatu. 

Proiektuaren kontratua erabiliz, proiektu bat edo gehiago faktura ditzakezu aldi berean. Proiektuaren kontratuak proiektuaren egiturako azpiproiektu bakoitzeko fakturazio prozedura koherentea bermatzen ere laguntzen du. 

Fakturatuko den proiektu guztiak proiektuaren kontratu batekin lotu behar du. Proiektu kontratu baten ezarpenak proiektu kontratu horri lotutako proiektu eta azpiproiektu guztiei aplikatzen zaizkie. 

Proiektuaren kontratu batek finantzazio iturri bat edo gehiago zehaztu ditzake. Hori dela eta, fakturazioa hainbat finantzatzaileren artean bana dezakezu, finantziazio mugak ezarri finantziazio iturriek zehaztutako zenbatekoa baino gehiago faktura ez dezaten eta gastuak kobratzeko finantzaketa arauak konfiguratu ditzakezu.

## <a name="funding-for-project-contracts"></a>Proiektuen kontratuetarako finantzaketa
Proiektuen kontratu batzuek zehazten dute hainbat alderdik partekatzen dutela proiektuaren kostuak finantzatzeko ardura. Hona hemen zenbait adibideak:

-   Zatiketa ugari dituen bezero handi batek proiektu baten finantzaketa zatiketa banatzea eskatzen du.
-   Zure enpresak proiektu handi baten kostuak kanpoko erakunde batekin partekatzen ditu.
-   Errepide proiektu bat bi udalek batera finantzatzen dute.
-   Zubi proiektu bat gobernuaren beka batek eta korporazio pribatu batek finantzatzen dute.

Dynamics 365 Finance atalean, transakzio bakar baten edo proiektu oso baten fakturazioa hainbat bezero, diru-laguntza edo erakunderen artean bana dezakezu. 

Hainbat finantzatzaile dituzten proiektuetan, finantzaketa-proiektu aurreratu baten finantzaketan laguntzen duten alderdi guztiei finantzazio-iturri deitzen zaie. Bezeroa, erakundea edo beka finantzaketa iturri gisa definitu ondoren, finantzaketa arau bat edo gehiago esleitu daitezke. Finantzazio arauek proiektuak finantzatzeko iturri desberdinetara nola esleitzen diren zehazten duten irizpideak jasotzen dituzte. 

Hornitutako artikuluak, hala nola, erosketa-eskaeretan eta erosketa-eskaeretan agertzen direnak ezin direnez banatu, kostuaren zenbatekoa ezin da banaketa-unean finantzaketa-iturri anitzen artean banatu. Hori dela eta, finantzazio iturriaren balioa 0 (zero) izaten jarraitzen du inbentarioaren arazoa argitaratu arte. Inbentarioaren arazoa argitaratzen denean, kostuaren zenbatekoa proiektuaren kontuak banatzeko arauen arabera banatzen da.

Hona hemen fakturazioa finantzaketa iturri anitzen artean banatzeko errazago egin ditzakezun urrats batzuk:

-   Zehaztu proiektu baterako sartu diren transakzio guztiek proiektuaren kontratuaren salmenta moneta bera erabiltzen dutela.
-   Ezarri finantzazio mugak, finantzaketa iturri batek proiektu bati zehaztutako zenbatekoa baino gehiago fakturatzen ez dion moduan.
-   Konfiguratu langile, elementu, kategoria, kategoria talde eta transakzio mota bakoitzerako (edo transakzio mota guztietarako) finantzaketa arauak eta finantzaketa mugak.
-   Aukeratu aukerako hasiera eta amaiera datak finantzaketa arau bakoitza baliozkoa den aldia zehazteko.
-   Zehaztu finantzaketa iturri bakoitzak duen portzentajea.
-   Zehaztu zein den iturri finantzarioaren zuzkidura kalkuluak eragindako desberdintasunak biribiltzeko ardura.
-   Konfiguratu arauak, proiektuaren kostuak kanpoko bezeroei fakturatzeko eta barne erakundeei nola kobratuko zaizkien zehazteko.
-   Erregistratu transakzioak atxikitako finantzazio kontu batean, finantzaketa osagarria lortu arte edo kostuak barnean hartzea erabaki arte.

Transakzioarekin zer zerga talde lotu zehazteko, proiektuan zerga talde esleipena bilatu da. Zerga taldeen esleipenik egin ez bada proiektu mailan, proiektuaren kontratua bilatzen da.

### <a name="example-multiple-funding-sources-simple"></a>Adibidez: finantzaketa iturri anitz (sinplea)

Ondorengo taulan finantzaketa-iturri anitzen artean finantzaketa esleipena kudeatzeko agertokiak eskaintzen dira. Eszenatoki hauek hipotesi hauetan oinarritzen dira:

-   Lehentasun ezarpenak funtsak esleitzeko kontuan hartzen dira, beste finantzaketa arau irizpideak aplikatu aurretik.
-   Ez da zehaztu finantziazio araua baliozkoa denean d epea zehazteko.

<table>
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Egoera</strong></td>
<td><strong>Finantzaketa iturria</strong></td>
<td><strong>Esleipenaren ehunekoa</strong></td>
<td><strong>Esleipenaren lehentasuna</strong></td>
</tr>
<tr class="even">
<td>Kostuak finantzaketa-iturri batera bideratu nahi dituzu funtsak agortu arte, kostuak bigarren finantzaketa-iturri batera esleitu bere fondoak agortu arte eta, azkenik, gainerako kostuak hirugarren finantzaketa-iturri batera esleitu.</td>
<td><ul>
<li>Finantzaketa　iturria　1</li>
<li>Finantzaketa　iturria　2</li>
<li>Finantzaketa　iturria　3</li>
</ul></td>
<td><ul>
<li>% 100</li>
<li>% 100</li>
<li>% 100</li>
</ul></td>
<td><ul>
<li>1</li>
<li>2</li>
<li>3</li>
</ul></td>
</tr>
<tr class="odd">
<td>Kostuen ehuneko 75 finantzaketa iturri batera eta ehuneko 25 bigarren finantzaketa iturri batera bideratu nahi duzu. Finantzaketa iturri horietako bat agortzen denean, gainerako kostuak hirugarren finantzaketa iturri batetik ordaindu nahi dituzu.</td>
<td><ul>
<li>Finantzaketa　iturria　1</li>
<li>Finantzaketa　iturria　2</li>
<li>Finantzaketa　iturria　3</li>
</ul></td>
<td><ul>
<li>% 75</li>
<li>% 25</li>
<li>% 100</li>
</ul></td>
<td><ul>
<li>1</li>
<li>1</li>
<li>2</li>
</ul></td>
</tr>
<tr class="even">
<td>Kostuen ehuneko 75 finantzaketa iturri batera eta ehuneko 25 bigarren finantzaketa iturri batera bideratu nahi duzu. Finantzaketa iturri horietako bat agortzen denean, zatitu egin nahi dituzu gainerako kostuak hirugarren finantzaketa-iturri baten eta laugarren finantzaketa-iturri baten artean.</td>
<td><ul>
<li>Finantzaketa　iturria　1</li>
<li>Finantzaketa　iturria　2</li>
<li>Finantzaketa　iturria　3</li>
<li>Finantzaketa　iturria　4</li>
</ul></td>
<td><ul>
<li>% 75</li>
<li>% 25</li>
<li>% 50</li>
<li>% 50</li>
</ul></td>
<td><ul>
<li>1</li>
<li>1</li>
<li>2</li>
<li>2</li>
</ul></td>
</tr>
<tr class="odd">
<td>Kostuen ehuneko lehenengo 25 finantzaketa iturri batera eta ehuneko gainerako bigarren finantzaketa iturri batera bideratu nahi duzu.</td>
<td><ul>
<li>Finantzaketa　iturria　1</li>
<li>Finantzaketa　iturria　2</li>
</ul></td>
<td><ul>
<li>% 25</li>
<li>% 100</li>
</ul></td>
<td><ul>
<li>1</li>
<li>2</li>
</ul></td>
</tr>
</tbody>
</table>

### <a name="example-multiple-funding-sources-complex"></a>Adibidez: finantzaketa iturri anitz (konplexua)

Hiru finantzaketa iturri dituzu, hurrenkera honetan erabili nahi dituzunak:

1.  Erabili berdin 2 finantzaketa iturria eta 3 finantzaketa iturria 2. finantzaketa iturria agortu arte.
2.  Jarraitu 3. finantziazio iturria erabiltzen, agortu arte.
3.  Erabili 1. finantzaketa iturria 3. finantzaketa iturria agortu ondoren.

Helburua lortzeko, honako hau egin beharko duzu lehenbizi:

-   Ezarri 2. iturriaren eta 3. iturriaren finantzazio mugak, dagozkien zenbatekoetarako.
-   Sortu hurrengo finantzaketa-arauak:
    -   1. araua (1. lehentasuna): transakzioen ehuneko 50 2. iturrira bideratu eta ehuneko 50 3. iturrira.
    -   2. araua (2. lehentasuna): transakzioen ehunekoa 100 finantzaketa 3. iturrira bideratu.
    -   3. araua (3. lehentasuna): transakzioen ehunekoa 100 finantzaketa 1. iturrira bideratu.

Konfigurazio honek funtzionatzen du, transakzioak arauen eta mugen arabera egiaztatzen direlako, horietako bat transakzioan aplikatzen den ala ez jakiteko. Transakzioari arau edo muga zehatzik aplikatzen ez bazaio, Transakzio guztiak araua aplikatuko da. Transakzio guztiak araua transakzio guztiekin bat dator. 

Transakzio batekin bat datorren arau bat aurkitzen bada, arau horretan esleitutako portzentajea aplikatuko da lehenik, baina partidak ezarri diren mugen aurka egiaztatu ondoren. Muga bat betetzen bada eta finantzaketa iturri baten funtsak agortzen badira, ez da kontuan hartzen finantzaketa mugarekin lotutako finantzaketa araua, eta programak aplikatzen duen hurrengo araua egiaztatzen du. 

Zenbait kasutan, transakzio baten zati bat soilik esleitu daiteke arau baten arabera. Hori gerta liteke transakzioa esleitzen denean mugara iristen delako. Kasu horretan, kopuru horren araberako kopuru jakin bat bakarrik esleitzen da, hala nola ehuneko 50 finantzaketa iturri bakoitzari. Atal honetan lehen deskribatzen den 1. arauko kasua da. Gainerakoa sekuentziaren hurrengo arauaren arabera esleitzen da. 

Hurrengo taulan eszenatoki hau zehatzago aztertzen da.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Fokua</strong></td>
<td><strong>Xehetasunak</strong></td>
</tr>
<tr class="even">
<td>Finantzaketa arauak</td>
<td><ul>
<li>1. araua (1. lehentasuna): transakzio guztiak. 2. diru iturria % 50-ean esleitu eta 3 % 50-ean.</li>
<li>2. araua (2. lehentasuna): transakzio guztiak. 3. finantziazio iturria % 100ean esleitu.</li>
<li>3. araua (2. lehentasuna): transakzio guztiak. 1. finantziazio iturria % 100ean esleitu.</li>
</ul></td>
</tr>
<tr class="odd">
<td>Finantzaketa mugak</td>
<td><ul>
<li>Finantzaketa iturri 1 muga = 10,000.00</li>
<li>Finantzaketa iturri 2 muga = 500.00</li>
<li>Finantzaketa iturri 3 muga = 750.00</li>
</ul></td>
</tr>
<tr class="even">
<td>1. transakzioa</td>
<td><strong>Transakzioaren zenbatekoa:</strong> 100,00<strong>Finantzaketa:</strong> Transakzioa 1. arauaren arabera soilik ordaintzen da, transakzioa 1. araua aplikatu ondoren guztiz ordaindu delako. Transakzioa berdin finantzatzen da 2. finantzaketa iturriaren eta 3. iturriaren artean.
<ul>
<li>Finantzaketa iturria 2: 50.00</li>
<li>Finantzaketa iturria 3: 50.00</li>
</ul></td>
</tr>
<tr class="odd">
<td>2. transakzioa</td>
<td><strong>Transakzioaren zenbatekoa:</strong> 5.000,00<strong>Finantzaketa:</strong> Transakzioa hiru arauen arabera ordaintzen da. <strong>1. araua</strong>
<ul>
<li>Finantzaketa iturria 2: 450.00</li>
<li>Finantzaketa iturria 3: 450.00</li>
</ul>
<strong>2. araua</strong>
<ul>
<li>Finantzaketa iturria 3: 250.00 (= 750.00 – 50.00 – 450.00)</li>
</ul>
<strong>3. araua</strong>
<ul>
<li>Finantzaketa iturria 1: 3,850.00 (= 5,000.00 – 450.00 – 450.00 – 250.00)</li>
</ul></td>
</tr>
<tr class="even">
<td>Finantzaketa iturri bakoitzerako banatzen diren funtsak guztira</td>
<td><ul>
<li>Finantzaketa iturria 1: 3,850.00</li>
<li>Finantzaketa iturria 2: 500.00</li>
<li>Finantzaketa iturria 3: 750.00</li>
</ul></td>
</tr>
</tbody>
</table>

## <a name="billing-rules"></a>Fakturazio arauak
Bezero batekin proiektuaren kontratua negoziatzen duzunean, bezeroari proiektu bateko lana nola eta noiz fakturatu ahal diozun zehazten duzu. Proiektuaren kontratua eta proiektua konfiguratu ondoren, proiektuaren fakturazio arauak ezar ditzakezu. Fakturazio arauak proiektuaren kontratuan zehaztutako proiektuaren baldintzetan oinarritzen dira. Sortu ditzakezun fakturazio arauak fakturazio arauarekin lotzen dituzun proiektuaren kontratuaren eta proiektu motaren araberakoak dira, esate baterako, Denbora eta materiala edo Prezio finkoa. Fakturazio arau bat baino gehiago sor ditzakezu proiektuaren kontratu baterako. Fakturazio arau bat ere esleitu diezaiekezu proiektu kontratu berarekin lotura duten eta fakturazio baldintza antzekoak dituzten hainbat proiekturi. 

Fakturazio arau mota hauek ezar ditzakezu:

-   **Entrega unitatea** - Bidali faktura bezero bati bidalketa unitate bat osatzean. Bidalketa unitateak zehazten dituzu kontratuan.
-   **Aurrerapena** - Fakturatu bezero bati proiektuaren ehuneko jakin bat osatzen duzunean. Fakturazio-arau bat konfigura dezakezu egindako lanaren ehunekoa automatikoki kalkulatzeko, edo eskuz kalkula dezakezu egindako lanaren ehunekoa eta bezeroari fakturatzeko zenbatekoa.
-   **Mugarria** - Fakturatu bezero bati proiektuaren mugarriaren zenbateko osoa, mugarria lortzen denean.
-   **Kuota** - Fakturatu bezero bati zure zerbitzuengatik gehi kudeaketa-kuota bat, hau da, normalean zerbitzuen kostuaren ehuneko bat.
-   **Denbora eta materiala** - Proiektu batean erabiltzen diren denboraren eta materialen balioa fakturatzea bezeroari.

Fakturazio arau mota guztietarako, bezeroen fakturetatik proiektu bat adostutako fasera iritsi arte atxikitako ehuneko bat zehaztu dezakezu. Ordainketa atxikitzeko ehunekoa proiektuaren kontratuan zehazten da. Zenbatekoa bezeroaren fakturan agertzen diren lerroen guztizko balioaren arabera kalkulatzen da. 

Hurrengorako **Denbora eta materiala** eta **Aurrerapena** fakturazio arauak, kargatzeko kategoriak esleitu ditzakezu. Kobratu beharreko kategoriek bezeroen fakturetan sartu beharko liratekeen eragiketak adierazten dituzte. 

Bezeroari fakturatzeko prest zaudenean, proiektuaren fakturazio zenbatekoa fakturazio arauen arabera kalkulatzen da eta proiektuaren faktura proposamena sortzen da. 

Ondorengo ataletan proiektu baten fakturazio arauak nola konfiguratu eta kudeatu erakusten duten adibideak ematen dira.

### <a name="example-create-a-billing-rule-that-is-based-on-the-number-of-units-delivered"></a>Adibidez: Sortu fakturazio araua entregatutako unitate kopuruaren arabera

Zure erakundeak akordioa sinatzen du bezeroen langileei bost trebakuntza-saio emateko guztira 10.000 kostu dituela prestakuntza-saio bakoitzeko. Prestakuntza saio bakoitzaren ondoren bezeroari fakturatzen diozu. 

Kontratuaren fakturazio arauak konfiguratzen dituzunean, balio hauek erabiltzen dituzu:

-   Emateko unitatea entrenamendu saio bakarra da.
-   Unitatearen prezioa 10.000 da entrenamendu saio bakoitzeko.
-   Unitate kopurua bost entrenamendu saio da.

Prestakuntza saio bat amaitutakoan, 10.000 euroko faktura sor dezakezu, entregatu den lehenengo unitateari eta faktura bezeroari bidali.

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-manual-calculation"></a>Adibidez: Sortu fakturazio araua proiektuaren amaierako ehuneko jakin batean oinarrituta (eskuzko kalkulua)

Zure erakundeak, software aholkularitza enpresak, bezeroarekin akordioa egiten du bezeroak garatzen ari den produktu baten zati bat garatzeko. Zure erakundeak onartzen du software kodea sei hilabetetan entregatzea. Bezeroak onartzen du zure erakundeari 100.000 guztira ordaintzea lanagatik. Fakturazio arau bat sortzen duzu bezeroari fakturatzeko proiektuan amaitutako lan portzentajearen arabera, kontratuan zehazten den moduan.

-   Lehenengo hilabetearen amaieran, bezeroarekin elkartuko zara egindako lanen ehunekoa zehazteko. Zuk eta bezeroak proiektua aztertu ondoren, erabakitzen duzu proiektua ehuneko 15 amaituta dagoela.
-   Faktura bat sortu 15,000 (100,000 ehuneko 15) eta bidali bezeroari.

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-automatic-calculation"></a>Adibidez: Sortu fakturazio araua proiektuaren amaierako ehuneko jakin batean oinarrituta (automatikoa kalkulua)

Zure erakundeak, software garapenerako enpresak, ados dago 30.000 euroko nomina kontabilitate pakete bat garatzea bezeroarentzat. Bezeroak onartzen du onartzea zure erakundea oinarriztu osatutako lanaren ehunekoan. Proiektuaren kostuak 20.000 direla kalkulatzen duzu. Proiektuaren kontratuan fakturazio prozesuan erabiltzen dituzun lan kategoriak zehazten dira. Fakturazio-arauak konfiguratzen dituzu kategoria bakoitzerako egindako lan portzentajearen fakturen zenbatekoak automatikoki kalkulatzen dituztenak. Kategoria bakoitzerako aurrekontua konfiguratzen duzu:

-   **Garapena** - 15.000 kostua eta 20.000 sarrerak
-   **Instalazioa** - 5.000 kostua eta 10.000 sarrerak

Bezeroaren faktura lehenengo aldiz sortzen duzunean, fakturaren zenbatekoa automatikoki kalkulatzen da informazio hau oinarritzat hartuta:

-   Hilabete igarota, proiektuko langileak proiektuaren fitxa aurkezten du. Langilearen orduen kostua 5.000 da garapenerako eta 1.000 instalazioetarako. Garapen lana ehuneko 33 amaituta dago (5.000 benetako kostua / 15.000 aurrekontu kostua), eta instalazio lanak ehuneko 20 amaitu dira (1.000 benetako kostua / 5.000 aurrekontu kostua).
-   Fakturaren zenbatekoa 8.667 automatikoki kalkulatzen da (20.000 ehuneko 33 + 10.000 ehuneko 20).
-   8,667 faktura sortu eta bezeroari bidaliko diozu.

### <a name="example-create-a-billing-rule-that-is-based-on-agreed-upon-milestones"></a>Adibidez: sortu fakturazio arau bat adostutako mugarrietan oinarrituta

Zure erakundeak, kudeaketa aholkularitza enpresak, ados dago bezeroak saltzeko asmoa duen kontsumo produktu baten merkatu ikerketak egitea. Bezeroak onartzen du zure zerbitzuak hiru hilabetez erabiltzea, martxoan hasita, eta zure erakundeari 50.000 ordaintzea onartzen du. Proiektuak hiru mugarri ditu:

-   1. mugarria: bildu kontsumitzaileen datuak - martxoaren 31
-   2. mugarria: kontsumitzaileen datuak aztertu - apirilaren 30a
-   3. mugarria: aurkeztu produktuaren bideragarritasun proposamena - Maiatzak 31

Bezeroa ados dago zure erakundeari 10.000 ordaintzea lehen mugarriagatik, 20.000 bigarren mugarriagatik eta 20.000 hirugarren mugarriagatik. 

Proiektuaren kontratua konfiguratzen duzunean, bezeroari fakturatzea onartzen duzu amaitutako mugarrian oinarrituta. Fakturazio arauaren konfigurazioak urrats hauek ditu:

-   Definitu proiektuaren mugarriak.
-   Mugarri bakoitza amaitutakoan bezeroari fakturatzeko zenbatekoa definitu.

Martxoaren 31n lehenengo mugarria amaitzen denean, mugarria amaituta dagoela markatuko duzu eta, ondoren, 10.000 euroko faktura sortu eta bezeroari bidaliko diozu. Ezin duzu mugarri baten faktura sortu mugarria osatuta dagoela markatu arte.

### <a name="example-create-a-billing-rule-that-is-based-on-services-plus-a-management-fee"></a>Adibidez: sortu fakturazio arau bat zerbitzuetan eta kudeaketa kuotan oinarrituta dagoena

Zure erakundeak, kudeaketa aholkularitza enpresak, ados dago merkatua ikertzea, bezeroak, txikizkako enpresa batek garatzen duen produktu baten bideragarritasuna ebaluatzeko. Hitzarmenaren baldintzetan zehazten da zure kudeaketa aholkulari nagusien zerbitzuak emango dituzula, hauek ikerketa denbora eta materialen arabera egingo baitute. Bezeroak 100 orduko ordaintzea onartzen du, gehi ehuneko 10eko kudeaketa kuota bat proiektuari kobratzen zaizkion aholkularitza orduengatik. 

Proiektuaren kontratua konfiguratzen duzunean, sortu fakturazio araua, ehuneko 10eko kudeaketa kuota gehitzeko proiektuari kobratzen zaizkion aholkularitza orduetan. 

Bezeroarentzako faktura sortzen duzunean, bezeroari ehuneko 10eko kudeaketa kuota gehitzen zaio kontsultarako orduen kostua. Adibidez, hiru aholkulariek proiektuan guztira 200 ordu landu badituzte, 22.000 euroko faktura sortzen da kalkulu hau oinarritzat hartuta:

-   200 ordu 100 orduko = 20.000
-   Kudeaketa ehuneko 10 = 2.000
-   Guztira faktura kopurua = 22,000

Tasak bezero bati zergapetzen badizkio eta proiektuaren kontratuan salmenten gaineko zerga talde bat hautatzen baduzu, salmenten gaineko zerga taldea automatikoki sartuko da tasen fakturazio arauan.

### <a name="example-create-a-billing-rule-for-the-value-of-time-and-materials"></a>Adibidez: Sortu fakturazio araua denboraren eta materialen balioarekin

Zure erakundeak, software aholkularitza enpresak, bost aholkulari tekniko eskaintzea onartzen du datozen sei hilabeteetan bezeroarentzako softwarearen garapen proiektuan lan egiteko. Bezeroak 150 aholku ematen ditu kontsulta ordu bakoitzeko, bulegoko materialaren kostua gehituta. Zure erakundeak faktura bat bidaltzen dio bezeroari hil bakoitzaren amaieran. 

Proiektuaren kontratua konfiguratzen duzunean, bezeroari hilero fakturatzea onartzen duzu proiektuan denbora eta materiala lortzeko. Informazio hau biltzen duen fakturazio araua sortzen duzu:

-   Kontratuaren epea sei hilabetekoa da.
-   Aholkularitza denbora 150 orduko kalkulatzen da.
-   Bulegoko materiala kostuaren arabera fakturatzen da, eta proiektuaren kostu osoa ez da 10.000 baino handiagoa izan behar.
-   Bezeroaren faktura sortzen duzu proiektuan zehar hilabete natural bakoitzaren amaieran.

Lehenengo hilabetean, guztira 800 ordu grabatzen dituzte aholkulariek proiektuan. Proiektuari kargatzen zaizkion bulegoko materialen kostua 2.000 da. Hori dela eta, hilaren amaieran 122.000 faktura sortzen dituzu, hau da, 800 orduko 150 orduko kalkulua, gehi 2.000 bulegoko materialetarako.





[!INCLUDE[footer-include](../includes/footer-banner.md)]