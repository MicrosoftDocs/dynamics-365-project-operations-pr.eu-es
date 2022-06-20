---
title: Sortu eta berretsi sarrera-egunkariak
description: Artikulu honek Microsoft-en Sarrera aldizkariak sortzeari eta baieztatzeari buruzko informazioa eskaintzen du Dynamics 365 Project Operations.
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

Microsoft-en benetako datuak zuzenean erregistratzeko Entry aldizkariak erabiltzen dituzu Dynamics 365 Project Operations. Sarrera aldizkariak erabiltzen dituzunean, ez duzu denbora, gastu eta materialen erabilera-erregistroak sartu behar Proiektu-eragiketetan.

Sarrera egunkari bakarrak aldizkari-lerro bat baino gehiago sortzeko aukera ematen dizu. Aldizkaria berresten denean, Sarrerako egunkari-lerro batek benetakoa erregistratzen du xehetasun hauetarako:

- Kostua edo diru-sarrera, hautatutako transakzio motaren arabera.
- Hautatutako transakzio-klasea. Eskuragarri dauden klaseak hauek dira **Denbora**, **·**, **·**, **·**, **·**, eta **Zerga**.
- Aldizkariaren lerroan aukeratzen den proiektua edo/eta zeregina.

Jarraitu urrats hauek Proiektu Eragiketetan Sarrera aldizkari bat sortzeko.

1. Joan **Salmentak** \> **Transakzioak** \> **Aldizkariak**.
2. Gainean **Sarrera aldizkariak** zerrenda orrian, Ekintza Panelean, hautatu **Berria** aldizkari bat sortzeko.
3. Gainean **Aldizkari berria** orrialdean, in **Deskribapena** eremuan, idatzi aldizkariaren deskribapena.
4. Ziurtatu hori **Aldizkari mota** eremuan ezarrita dago **Sarrera**, eta gero hautatu **Gorde**. Sarrera egunkari berria gorde ondoren, a **Aldizkariaren lerroak** fitxa aldizkariaren orrian agertu behar da.
5. Gainean **Aldizkariaren lerroak** fitxan, sarearen gaineko tresna-barran, hautatu **Berria** Sarrera egunkari-lerro bat sortzeko.
6. urtean **Sortu azkarra** Sarrera egunkari-lerro bat sortzeko elkarrizketa-koadroa, ezarri eremuak hurrengo taulan azaltzen den moduan.

    | Eremua | Deskribapenak | Inpaktu funtzionala |
    | --- | --- | --- |
    | Transakzio-klasea | Aldizkariaren lerroa sei transakzio klaseetako batean sailka daiteke: **Denbora**, **·**, **·**, **·**, **·**, edo **Zerga**. | The **Zerga** transakzio-klasea zaharkituta geratu da Project Operations-n. <br> Bat sortzen baduzu **Zerga** transakzio klasea, ez da fakturazio bidez edo kostu edo diru-sarreren kalkuluetan prozesatuko. **Mugarria** diru-sarreren soilik transakzio klase bat da. <br>The **Atxilotzailea** transakzio klaseak bezero batengandik jasotako aurrerapena adierazten du. Beti fakturatutako salmenta eta fakturatu gabeko salmenten aldizkari lerroen pare gisa sortu behar da. |
    | Transakzio mota | The **Kostua**, **salmentak**, eta **Baliabideen kostu unitarioa** transakzio motak erabili behar dira kostua erregistratzeko.<br> The **Fakturatu gabeko salmentak** eta **Fakturatutako salmentak** transakzio motak erabili behar dira diru-sarrerak erregistratzeko. | The **Atxilotzailea** transakzio-klasearekin soilik funtzionatzen du **Fakturatu gabeko salmentak** eta **Fakturatutako salmentak** transakzio motak.<br> The **Mugarria** transakzio-klasearekin soilik funtzionatzen du **Fakturatutako salmentak** transakzio mota. <br>The **Interorg salmentak** eta **Baliabideen kostu unitarioa** transakzio motak soilik aplikatzen dira **Denbora** transakzio-klasea eta hauek Sarrera aldizkarietan soilik erabil daitezke Lite inplementazio-eszenatokian eta ez Proiektu-eragiketak Baliabideen / Hornituta ez dauden eszenatokietan zabaltzen direnean. |
    | Hautatu produktua | Noiz **Materiala** transakzio-klasea hautatuta dago, eremu honek aldizkari-lerroa sortzen ari zaren material-transakzioa lehendik dagoen produktua edo idatzizko produktua den zehazten dizu. | Hautatzen baduzu **Idatzizko produktua**, produktuaren izena sar dezakezu. |
    | Produktu | Katalogoko produktuaren erreferentzia. | |
    | Deskribapenak | Aldizkari-lerroaren deskribapena erraz identifikatzen laguntzeko. | Fakturatu gabeko salmenten egunkari-lerroetarako, balioa deskribapen gisa erabiliko da faktura-lerroaren xehetasunak sortzen direnean. |
    | Kanpoko deskribapena | Kanpoko eragileekin partekatzeko erabil daitekeen aldizkari-lerroaren deskribapena. | Fakturatu gabeko salmenten egunkari-lerroetarako, balioa kanpoko deskribapen gisa erabiliko da faktura-lerroaren xehetasunak sortzen direnean. Bezeroari bidaltzen zaion fakturan ere ager daiteke. |
    | Fakturazio mota | Aldizkariaren lerroa proiektuan kobragarri, osagarri edo kargatu gabeko osagai gisa zenbatuko den adierazten duen balio bat. | Fluxu tipiko batean, fakturazio mota kontratuan ezartzen diren adostutako baldintzetatik eratortzen da. Hala ere, aldizkari-lerro bat grabatzen duzunean, eremu honetan balio bat sar dezakezu. |
    | Dokumentuaren data | Erabili data bat transakzioa gertatu zenean. | |
    | Hasiera-data | Erabili transakzioa gertatu zeneko data. | Eremu hau fakturaren eragiketen datarekin alderatzeko erabiltzen da **Fakturatu gabeko salmentak** mota. Konparazio honek transakzioa etorkizuneko edo iraganekoa den erabakitzen lagunduko dizu. Iraganeko transakzioak soilik gehituko zaizkio fakturari. |
    | Amaiera-data | Erabili transakzioa gertatu zeneko data. | |
    | Kontabilitatearen data | Erabili kontabilitate-eragina erregistratuko den data. | |
    | Kontratu lerroko bezeroa | Lehenespenez, kontratu-lerroak bezero bakarra badu, eremu hau kontratu-lerroan bezeroari ezartzen zaio aldizkari-lerroa gordetzen denean. Kontratu-lerroak bezero anitz baditu, hautatu bezero zuzena kontratu-lerroan. | Sistemak ezin badu zehaztu kontratu lerroko bezeroa egunkariko lerroan, eta hutsik badago **Fakturatu gabeko salmentak** aldizkari-lerrotik sortutako mota, benetakoa ez da fakturatuko. |
    | Project | Hautatu proiektua benetakoa grabatzeko. | Hautatutako proiektuan, transakzio-klasean eta zereginean oinarrituta, sistema kontratua, kontratu-lerroa eta kontratu-lerroa bezeroa zehazten saiatuko da. |
    | Zeregina | Hautatu benetako aktibatuta grabatzeko zeregina. | Zereginak kontratu-lerroekin lotu badituzu kontratua konfiguratzean, sistemak hautatutako zeregina erabiliko du, proiektu eta transakzio-klase batekin batera, kontratua, kontratu-lerroa eta kontratu-lerroa bezeroa zehazteko. |
    | Transakzio-kategoria | Hautatu transakzio-kategoria benetakoa grabatzeko. | Gastuetarako, hautatutako transakzio-kategoriak gordetakoan aldizkariko lerroan sartuko den prezio lehenetsia zehazten du. |
    | Funtzioa | Eremu hau garrantzitsua da Time journal-en lerroetarako. Hautatu proiektuan edo/eta zereginean denbora eman duen baliabidearen rola. | Denbora-egunkari-lerroetarako, baliabideen kostu lehenetsiak eta faktura-tasak sartzeko kutxaz kanpoko konfigurazioa erabiltzen baduzu, hautatutako rola baliabide-unitatearekin batera erabiltzen da aldizkari-lerroan sartuko den prezio lehenetsia zehazteko. gordeta dago. Prezio lehenetsiak sartzeko konfigurazio pertsonalizatu bat erabiltzen baduzu, konfigurazio hori berrikusi beharko zenuke ala ez zehazteko **Rola** eremua prezio-balio lehenetsiak sartzeko erabiltzen da. |
    | Azpikontratua | Aldizkari-lerroak azpikontratatutako ahalmena edo azpikontratatutako gastuak edo materialak adierazten baditu, hautatu dagokion azpikontratua. | Kostuen egunkari-lerroak erregistratzen direnean, hautatutako azpikontratuak kostu unitario lehenetsia sartzeko erabiltzen den prezio-zerrenda zehaztuko du. |
    | Azpikontratazio lerroa | Aldizkari-lerroak azpikontratatutako ahalmena edo azpikontratatutako gastuak edo materialak adierazten baditu, hautatu dagokion azpikontratazio-lerroa. | Kostuen egunkari-lerroak erregistratzen direnean, hautatutako azpikontratazio-lerroak azpikontratazio-lerroan erabilgarri dauden edukieraren kalkuluak behar bezala kalkulatzen direla ziurtatuko du. |
    | Zenbatekoa kalkulatzeko metodoa | Lehenespenez, eremu hau ezarrita dago **Biderkatu kantitatea prezioaren arabera**. Metodo hau erabiltzen denean, zenbatekoa honela kalkulatuko da *Kantitatea* ×*Prezioa*. Onartutako beste metodoa da **Prezio finkoa**. Metodo hau erabiltzen denean, prezioa zenbatekoaren arabera ezarriko da, eta kantitatea ez da kalkuluan erabiliko. | |
    | Unitatearen Ordutegia eta Unitatea | Elkarrekin, unitate-programazioak eta unitateak kantitatearen unitatea identifikatzen dute. | Unitatearen eta transakzio-kategoriaren konbinazioa erabiltzen da gastuen prezio lehenetsiak sartzeko. Proiektu Eragiketen konfigurazio lehenetsian, unitatearen, rolaren eta baliabideen unitatearen konbinazioa erabiltzen da denboraren prezio lehenetsiak sartzeko. Prezio lehenetsiak sartzeko konfigurazio pertsonalizatua baduzu, unitatearekin batera erabiliko da. Produktuaren eta unitatearen konbinazioa materialen prezio lehenetsiak sartzeko erabiltzen da. |
    | Kantitatea | Idatzi kantitatea. | |
    | Prezioa | Aldizkariaren lerroa sortzen denean prezioa hutsik geratzen bada, balio egokiak erabiliko dira prezio lehenetsiak sartzeko, transakzio klasearen arabera. Aldizkariaren lerroa sortzen denean prezio bat sartzen bada, prezio hori erabiliko da. | |
    | Zergak | Sartu edozein zerga-kopurua. | Sartzen den zerga-kopuruaren arabera, luzatutako zenbatekoa honela kalkulatuko da *Zenbatekoa* + *Zerga*. |

## <a name="confirm-an-entry-journal"></a>Berretsi Sarrera egunkari bat

Sarrera aldizkari batean aldizkari-lerro guztiak sartu ondoren, aldizkaria berretsi dezakezu. Prozesu honek aldizkari-lerro bakoitza proiektu egokietan erreal gisa erregistratuko du.

Aldizkari bat berretsi ondoren, ezin duzu editatu edo haren lerroetako bat.

## <a name="actuals-created-by-entry-journal-confirmation"></a>Sarrera aldizkariaren berrespenarekin sortutako benetakoak

Sarrerako aldizkariaren berrespenarekin sortutako benetako desberdintasun batzuk eta Proiektuko Eragiketetan Denbora, Gastu eta Materialaren erabilera-erregistroen eta fakturaren berrespenen onarpenean sortzen diren benetakoen artean daude:

- Sarrera aldizkariek ez dute transakzio-konexiorik erabiltzen benetako kostua fakturatu gabeko salmenta errealarekin lotzeko. Denbora, Gastuen eta Materialaren erabilera-erregistroak onartzen direnean sortzen diren errealek transakzio-konexioak erabiltzen dituzte beti kostuak eta fakturatu gabeko salmenten errealak lotzeko.
- Sarrera aldizkariek ez dute transakzioen jatorria erabiltzen kostu errealak eta fakturatu gabeko salmenten errealak jatorrizko edozein erregistrorekin lotzeko. Denbora, Gastuen eta Materialaren erabilera-erregistroak onartzen direnean sortzen diren errealek transakzioen jatorria erabiltzen dute beti kostuak eta fakturatu gabeko salmenten errealak jatorriko denbora-sarrerarekin lotzeko.
- Sarrerako aldizkariaren berrespenarekin sortzen diren fakturatu gabeko salmenten errealak fakturatzen direnean, fakturaren berrespenean sortzen diren fakturatutako salmenten errealak fakturatu gabeko salmenten errealekin lotzen dira, denbora, gastua eta sortzen diren fakturatu gabeko salmenten errealen antzera. Materialaren erabileraren erregistroak onartzen dira.
- Erakundeen arteko baliabideek sartutako denborarako sortzen diren sarrera-egunkari-lerroek ez dute errealak eragiten.**Baliabideen unitateko kostua** eta **Interorg salmentak** automatikoki sortuko diren motak. Erreal hauek eskuz sortu behar dira. Jokabide hori erakundeen arteko baliabideek erregistratzen dituzten denbora-sarreretarako portaeratik desberdina da. Kasu horretan, ordua onartzen denean, aplikazioak automatikoki sortzen ditu benetako datuak **Kostua** idatzi proiektuan eta benetakoak **Baliabideen unitateko kostua** eta **Interorg salmentak** motak langilearen jabetzako dibisioan. Ondoren, transakzio-konexioak erabiltzen ditu benetako horiek elkarrekin lotzeko eta transakzio-jatorriak jatorrizko denbora-sarrerarekin lotzeko.
- Sarrera aldizkariak baieztatzen direnean, benetakoak sortzen dituzte. Hala ere, Zuzenketa aldizkariak ezin dira erabili benetakoak zuzentzeko. Jokaera hau denbora, gastu eta material erabilera-erregistroak onartzen direnean sortzen diren errealen portaeratik desberdina da. Kasu horretan, aplikazioak zuzenketa aldizkariak erabil ditzakezu akatsak konpontzeko benetakoak zuzentzeko, baldin eta egiazkoak oraindik fakturatu ez badira. Dagoeneko fakturatuta badaude, erreal bat zuzendu dezakezu erreal horren kreditu osoa bezeroari prozesatzen bazaio.

> [!NOTE]
> Sarrera aldizkariek ez dute arau zorrotzik ezartzen. Hori dela eta, erabili Sarrera-Aldizkari hauek ahalik eta gutxien, eta kontuz ibili eta kontuz ibili zure sisteman finantza-daturik hondatuta ez duzula sortzen ziurtatzeko. Ahal duzun guztietan, erabili Denbora, Gastuen eta Materialaren erabilera-erregistroak, proiektu-kontratuetako mugarri eta atxikipen-konfigurazioa eta proiektuaren fakturaren berrespen-prozesua, Sarrera egunkarien ordez, benetakoak sortzeko.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
