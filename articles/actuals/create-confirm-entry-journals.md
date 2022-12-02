---
title: Sortu eta berretsi sarrera-egunkariak
description: Artikulu honek Microsoft Dynamics 365 Project Operations-en sarrera-egunkari bat sortzeari eta hura berresteari buruzko informazioa ematen du.
author: rumant
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: johnmichalak
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 138dccd72607d6515eeeffb066fa485f83eabbec
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912317"
---
# <a name="create-and-confirm-entry-journals"></a>Sortu eta berretsi sarrera-egunkariak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Sarrera egunkariak Microsoft Dynamics 365 Project Operations-en zuzeneko datuak erregistratzeko erabiltzen dituzu. Sarrera-aldizkariak erabiltzen dituzunean, ez duzu denbora, gastu eta materialen erabilera-erregistroak sartu behar Project Operations-en.

Sarrera-egunkari bakarrak egunkari-lerro bat baino gehiago sortzeko aukera ematen dizu. Aldizkaria berresten denean, Sarrera-egunkariko lerro batek benetakoa erregistratzen du honako xehetasun hauetarako:

- Kostua edo diru-sarrerak, hautatutako transakzio motaren arabera.
- Hautatu transakzio-klasea. Eskuragarri dauden klaseak hauek dira: **Denbora**, **Gastua**, **Materiala**, **Atxikitzailea**, **Mugarria**, eta **Zerga**.
- Egunkari-lerroan aukeratzen den proiektua edo/eta zeregina.

Jarraitu urrats hauek Project Operations-en Sarrera-egunkari bat sortzeko.

1. Joan **Salmentak** \> **Transakzioak** \> **Aldizkariak**.
2. **Sarrera-egunkariak** zerrenda orrian, Ekintza panelean, hautatu **Berria** egunkari bat sortzeko.
3. **Egunkari berria** orrialdean, **Azalpena** eremuan, idatzi egunkariaren deskribapena.
4. Ziurtatu **Egunkari mota** eremua ezarrita dagoela **Sarrera**, eta gero hautatu **Gorde**. Sarrera egunkari berria gorde ondoren, **Egunkari lerroak** fitxa egunkariaren orrian agertu behar da.
5. **Egunkari-lerroak** fitxan, sarearen gaineko tresna-barran, hautatu **Berria** Sarrerako egunkari-lerro bat sortzeko.
6. **Sorrera bizkora** elkarrizketa-koadroan sarrerako egunkari-lerro bat sortzeko, ezarri eremuak hurrengo taulan azaltzen den moduan.

    | Eremua | Deskribapenak | Inpaktu funtzionala |
    | --- | --- | --- |
    | Transakzio-klasea | Egunkari-lerroa sei transakzio klaseetako batean sailka daiteke: **Denbora**, **Gastua**, **Materiala**, **Atxikitzailea**, **Mugarria**, edo **Zerga**. | **Zerga** transakzio-klasea zaharkituta geratu da Project Operations-en. <br> **Zerga** transakzio klase bat sortzen baduzu, ez da fakturazio bidez edo kostu edo diru-sarreren kalkuluetan prozesatuko. **Mugarria** diru-sarrerak soilik transakzio klasea da. <br>**Atxikitzaileak** transakzio-klaseak bezero batengandik jasotako aurrerapena adierazten du. Beti fakturatutako salmenta eta fakturatu gabeko salmenten aldizkari lerroen pare gisa sortu behar da. |
    | Transakzio mota | **Kostua**, **Erakunde arteko salmentak**, eta **Baliabideen unitateko kostua** transakzio motak erabili behar dira kostua erregistratzeko.<br> **Fakturatu gabeko salmentak** eta **Fakturatutako salmentak** transakzio motak erabili behar dira diru-sarrerak erregistratzeko. | **Atxikitzailea** transakzio-klaseak soilik funtzionatzen du **Fakturatu gabeko salmentak** eta **Fakturatutako salmentak** transakzio motekin.<br> **Mugarria** transakzio-klaseak soilik funtzionatzen du **Fakturatutako salmentak** transakzio motarekin. <br>**Erakundea arteko salmentak** eta **Baliabideen unitateko kostua** transakzio motak soilik aplikatzen dira **Denbora** transakzio-klasean eta hauek Sarrera egunkarietan soilik erabilgarri daude Lite inplementazio-eszenatokian eta ez Project Operations Baliabide / Ez hornitutako eszenatokietan zabaltzen direnean. |
    | Hautatu produktua | **Materiala** transakzio-klasea hautatuta dagoenean, eremu honek egunkari-lerroa sortzen ari zaren material-transakzioa lehendik dagoen produktua edo idatzizko produktua den zehazten dizu. | **Idazteko produktua** hautatzen baduzu, produktuaren izena idatzi dezakezu. |
    | Produktu | Katalogoko produktuaren erreferentzia. | |
    | Deskribapenak | Egunkari-lerroaren deskribapena erraz identifikatzen laguntzeko. | Fakturatu gabeko salmenten egunkari-lerroetarako, balioa deskribapen gisa erabiliko da faktura-lerroaren xehetasunak sortzen direnean. |
    | Kanpoko azalpena | Kanpoko eragileekin partekatzeko erabil daitekeen egunkari-lerroaren deskribapena. | Fakturatu gabeko salmenten egunkari-lerroetarako, balioa kanpoko deskribapen gisa erabiliko da faktura-lerroaren xehetasunak sortzen direnean. Bezeroari bidaltzen zaion fakturan ere ager daiteke. |
    | Fakturazio mota | Egunkari-lerroa proiektuan kobragarri, osagarri edo kargatu gabeko osagai gisa zenbatuko den adierazten duen balio bat. | Fluxu tipiko batean, fakturazio mota kontratuan ezartzen diren hitzartutako baldintzetatik eratortzen da. Hala ere, egunkari-lerro bat grabatzen duzunean, eremu honetan balio bat sar dezakezu. |
    | Dokumentuaren data | Erabili data bat transakzioa gertatu zenean. | |
    | Hasiera-data | Erabili data bat transakzioa gertatu zenean. | Eremu hau **Fakturatu gabeko salmentak** motako fakturaren eragiketen datarekin alderatzeko erabiltzen da. Konparazio honek transakzioa etorkizuneko edo iraganekoa den erabakitzen lagunduko dizu. Iraganeko transakzioak soilik gehituko dira fakturan. |
    | Amaiera-data | Erabili data bat transakzioa gertatu zenean. | |
    | Kontabilitatearen data | Erabili kontabilitate-eragina erregistratuko den data. | |
    | Kontratuaren lerroaren bezeroa | Lehenespenez, kontratu-lerroak bezero bakarra badu, eremu hau kontratu-lerroan bezeroari ezartzen zaio egunkari-lerroa gordetzen denean. Kontratu-lerroak bezero anitz baditu, hautatu bezero zuzena kontratu-lerroan. | Sistemak ezin badu zehaztu kontratu-lerroko bezeroa egunkari-lerroan, eta hutsik badago **Fakturatu gabeko salmentak** egunkari-lerrotik sortzen den motan, benetakoa ez da fakturatuko. |
    | Project | Hautatu proiektua benetakoa grabatzeko. | Hautatutako proiektuaren, transakzio-klasearen eta zereginaren arabera, sistema kontratua, kontratu-lerroa eta kontratu-lerroa bezeroa zehazten saiatuko da. |
    | Zeregina | Hautatu zeregina benetakoa grabatzeko. | Zereginak kontratu-lerroekin lotu badituzu kontratua konfiguratzean, sistemak hautatutako zeregina erabiliko du, proiektu eta transakzio-klase batekin batera, kontratua, kontratu-lerroa eta kontratu-lerroa bezeroa zehazteko. |
    | Transakzio-kategoria | Hautatu transakzioaren kategoria benetakoa grabatzeko. | Gastuetarako, hautatutako transakzio-kategoriak gordetakoan egunkari-lerroan sartuko den prezio lehenetsia zehazten du. |
    | Funtzioa | Eremu hau denboraren egunkari-lerroetarako garrantzitsua da. Hautatu proiektuan edo/eta zereginean denbora eman duen baliabidearen rola. | Denboraren egunkari-lerroetarako, baliabideen kostu lehenetsiak eta faktura-tasak sartzeko kutxaz kanpoko konfigurazioa erabiltzen baduzu, hautatutako rola baliabide-unitatearekin batera erabiltzen da egunkari-lerroan sartuko den prezio lehenetsia zehazteko gordetzerakoan. Prezio lehenetsiak sartzeko konfigurazio pertsonalizatu bat erabiltzen baduzu, konfigurazio hori berrikusi beharko zenuke zehazteko **Funtzioa** eremua prezio-balio lehenetsiak sartzeko erabiltzen den ala ez. |
    | Azpikontratua | Egunkari-lerroak azpikontratatutako ahalmena edo azpikontratatutako gastuak edo materialak adierazten baditu, hautatu dagokion azpikontratua. | Kostuen egunkari-lerroak erregistratzen direnean, hautatutako azpikontratuak kostu unitario lehenetsia sartzeko erabiltzen den prezio-zerrenda zehaztuko du. |
    | Azpikontratuaren lerroa | Egunkari-lerroak azpikontratatutako ahalmena edo azpikontratatutako gastuak edo materialak adierazten baditu, hautatu dagokion azpikontratuaren lerroa. | Kostuen egunkari-lerroak erregistratzen direnean, hautatutako azpikontratazio-lerroak azpikontratazio-lerroan erabilgarri dauden edukieraren kalkuluak behar bezala kalkulatzen direla ziurtatuko du. |
    | Zenbatekoa kalkulatzeko metodoa | Eremu hori ezarrita dago **Biderkatu kopurua prezioaren arabera** modu lehenetsian. Metodo hau erabiltzen denean, zenbatekoa honela kalkulatuko da: *Kantitatea* × *Prezioa*. Onartutako beste metodoa da **Prezio finkoa**. Metodo hau erabiltzen denean, prezioa zenbatekoaren arabera ezarriko da, eta kantitatea ez da kalkuluan erabiliko. | |
    | Unitatearen antolaketa eta Unitatea | Elkarrekin, unitate-programazioak eta unitateak kantitatearen unitatea identifikatzen dute. | Unitatearen eta transakzio-kategoriaren konbinazioa erabiltzen da gastuen prezio lehenetsiak sartzeko. Project Operations-en konfigurazio lehenetsian, unitatearen, funtzioaren eta baliabideen unitatearen konbinazioa erabiltzen da denborarako prezio lehenetsiak sartzeko. Prezio lehenetsiak sartzeko konfigurazio pertsonalizatua baduzu, unitatearekin batera erabiliko da. Produktua eta unitatearen konbinazioa erabiltzen da materialen prezio lehenetsiak sartzeko. |
    | Kantitatea | Idatzi kantitatea. | |
    | Prezioa | Egunkari-lerroa sortzen denean prezioa hutsik geratzen bada, balio egokiak erabiliko dira prezio lehenetsiak sartzeko, transakzio klasearen arabera. Egunkari-lerroa sortzen denean prezio bat sartzen bada, prezio hori erabiliko da. | |
    | Zergak | Sartu edozein zerga-kopurua. | Sartzen den zerga-kopuruaren arabera, luzatutako zenbatekoa honela kalkulatuko da *Zenbatekoa* + *Zerga*. |

## <a name="confirm-an-entry-journal"></a>Berretsi Sarrera egunkari bat

Sarrerako egunkari batean egunkari-lerro guztiak sartu ondoren, egunkaria berretsi dezakezu. Prozesu honek egunkari-lerro bakoitza proiektu egokietan erreal gisa erregistratuko du.

Egunkari bat baieztatu ondoren, ezin duzu editatu hura edo bere lerroetako bat.

## <a name="actuals-created-by-entry-journal-confirmation"></a>Sarrera egunkariaren berrespenarekin sortutako benetakoak

Sarrerako egunkariaren berrespenarekin sortutako benetako desberdintasun batzuk eta Project Operations-en Denbora, Gastu eta Materialaren erabilera erregistroak eta fakturaren berrespena onartzean sortzen diren benetakoen artean daude:

- Sarrera egunkariek ez dute transakzio-konexiorik erabiltzen benetako kostua fakturatu gabeko salmenta errealarekin lotzeko. Denbora, Gastuen eta Materialaren erabilera-erregistroak onartzen direnean sortzen diren errealek transakzio-konexioak erabiltzen dituzte beti kostuak eta fakturatu gabeko salmenten errealak lotzeko.
- Sarrera egunkariek ez dute transakzio-jatorririk erabiltzen benetako kostua eta fakturatu gabeko salmenta erreala sortutako erregistroarekin estekatzeko. Denbora, Gastuen eta Materialaren erabilera-erregistroak onartzen direnean sortzen diren errealek transakzio-jatorriak erabiltzen dituzte beti kostuak eta fakturatu gabeko salmenten errealak lotzeko sortutako denbora-sarrerarekin.
- Sarrerako aldizkariaren berrespenarekin sortzen diren fakturatu gabeko salmenten errealak fakturatzen direnean, fakturaren berrespenean sortzen diren fakturatutako salmenten errealak fakturatu gabeko salmenten errealekin lotzen dira, denbora, gastua eta sortzen diren fakturatu gabeko salmenten errealen antzera. Materialaren erabileraren erregistroak onartzen dira.
- Erakundeen arteko baliabideek sartutako denborarako sortzen diren sarrerako egunkari-lerroek ez dute eragiten **Baliabideen unitateko kostua** eta **Erakunde arteko salmentak** motak automatikoki sortzea. benetako hauek eskuz sortu behar dira. Jokabide hori erakundeen arteko baliabideek erregistratzen dituzten denbora-sarreretako portaeratik desberdina da. Kasu horretan, ordua onartzen denean, aplikazioak automatikoki sortzen ditu benetako datuak **Kostua** motarenak proiektuan eta **Baliabideen unitateko kostua** eta **Erakunde arteko salmentak** moten benetakoak langilearen jabetzako dibisioan. Ondoren, transakzio-konexioak erabiltzen ditu benetako horiek elkarrekin lotzeko eta transakzio-jatorriak jatorrizko denbora-sarrerarekin lotzeko.
- Sarrera egunkariak baieztatzen direnean, benetakoak sortzen dituzte. Hala ere, Zuzenketa egunkariak ezin dira erabili benetakoak zuzentzeko. Jokabide hori denbora, gastu eta material erabilera-erregistroak onartzen direnean sortzen diren errealen portaeratik desberdina da. Kasu horretan, aplikazioak zuzenketa egunkariak erabil ditzakezu errealak zuzentzeko akatsak konpontzeko, baldin eta erreal horiek oraindik fakturatu ez badira. Dagoeneko fakturatuta badaude, erreal bat zuzendu dezakezu erreal horren kreditu osoa bezeroari prozesatzen bazaio.

> [!NOTE]
> Sarrera egunkariek ez dute arau zorrotzik ezartzen. Hori dela eta, erabili Sarrera-egunkari hauek ahalik eta gutxien, eta kontuz ibili eta kontuz ibili zure sisteman finantza-daturik hondatuta ez duzula sortzen ziurtatzeko. Ahal duzun guztietan, erabili Denbora, Gastuen eta Materialaren erabilera-erregistroak, proiektu-kontratuetako mugarri eta atxikipenen konfigurazioa eta proiektuaren fakturaren berrespen-prozesua, Sarrera egunkarien ordez, benetakoak sortzeko.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
