---
title: Produktuak
description: Artikulu honetan, bezeroei beren erakundeak eskaintzen dituen produktuei eta prezioei buruzko informazioa emateko erabil ditzakeen produktuen katalogoari buruzko informazioa ematen da.
author: rumant
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: johnmichalak
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: d45a705c48df84a8f5b3f60121fbcc25e225e6e5
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8933063"
---
# <a name="products"></a>Produktuak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Produktuak zure erakundearen berariazko backbone dira. Dynamics 365 Sales Professional-eko produktuen katalogoa produktuei eta beren prezio-informazioari leku da. Egin salmenta-agenteak zure produktuen katalogoa sortu beren salmentak areagotzeari bizkorrago.

## <a name="add-a-product"></a>Gehitu produktua

1.  Ziurtatu Salmenta-kudeatzaile profesionala edo Sistemaren administratzailearen funtzioa edo antzeko baimenak dituzula Dynamics 365 Sales Professional-en produktuak gehitu ahal izateko.
2.  Gunearen mapako **Konfigurazioa** atalean, hautatu **Produktuak**.
3.  Aukeratu **Gehitu produktua** eta bete informazio hau:

    -  **Izena**
    -  **Produktuaren IDa**
    -  **Bazkidea**: hautatu produkturako produktu-familia nagusia. Produktu-familiaren bigarren mailako produktu multzo bat sortzen ari bazara, produktu-familia nagusiaren izena hemen beteta dago. Hori ezin da aldatu erregistroa gorde ondoren.
    -  **Baliozkoa data honetatik**/**Baliozkoa data honetara arte**: zehaztu produktua baliozkoa izango den denbora tartea; horretarako, hautatu **Baliozkoa data honetatik** and **Baliozkoa data honetara arte** datak.
    -  **Salmenta-unitatea**: Hautatu salmenta-unitatea. Salmenta-unitateko unitate hainbat saltzeko produktuak eta elementuak banakako modua zehazten leku gehienez zatitu taldekatzen diren da. Adibidez, haziak gehitzen ari bazara produktu gisa, "Haziak" izena duen salmenta-talde bat sortu behar duzu eta bere unitate nagusia "Pakete"gisa zehaztu behar duzu.
    -  **Lehenetsitako unitatea**: hautatu produktua gehien salduko duen unitatea. Unitateak produktuak saltzen dituzun kantitateak edo neurketak dira. Adibidez, haziak gehitu badituzu produktu gisa, paketetan, kaxetan edo paletetan sal ditzakezu. Produktuaren unitate bakoitzaren horien da. Seeds gehienak saltzen packets atalean, hautatu duzun unitate gisa.
    -  **Lehenetsitako prezio-zerrenda**: produktua berria bada, eremu hau irakurtzeko soilik izango da. Prezio-zerrenda lehenetsia hautatu ahal izateko, aurrena dagozkion beharrezko eremu guztiak bete eta, ondoren, erregistroa gorde behar duzu. Lehenetsitako prezio-zerrenda beharrezkoa ez den arren, produktuaren erregistroa gordetzen duzunean, komeni da produktu bakoitzarentzat lehenetsitako prezio-zerrenda bat ezartzea. Ondoren, bezero baten erregistroak prezio-zerrendarik ez badu, Sales aplikazioak lehenetsitako prezio-zerrenda erabil dezake eskaintzak, eskaerak eta fakturak sortzeko.
    -  **Onartutako hamartarrak**: sartu 0 eta 5 arteko zenbaki oso bat. Produktua ezin bada zatikietan zatitu, 0 idatzi. Zehaztasun maila **Kopurua** eremuan eskaintza, eskaera edo faktura-produktu erregistroan balioztatutako balioa da eremu honetan produktuak erlazionatutako prezio-zerrendarik ez badu.
    -  **Gaia**: erlazionatu produktua gai batekin. Gaiak produktuak sailkatzeko eta txostenak iragazteko erabil ditzakezu.

4.  Sakatu **Gorde**.
5.  **Xehetasun gehiago** fitxan, **Prezio-zerrendako elementuak** atalean, hautatu **Komando gehiago**, eta hautatu **Gehitu prezioen zerrenda berria**.
7.  **Xehetasun gehiago** fitxan, **Produktuen erlazioa** atalean, hautatu **Komando gehiago** ikonoa, eta hautatu **Gehitu produktu berrien erlazioa**.
8.  Aplikazioan, **Produktu-erlazio Berria** inprimakian, idatzi honako xehetasunak eta komando-barran, hautatu **Gorde eta itxi**:

    -   **Erlazionatutako produktua**: Hautatu kudeatzen ari zaren eta lehendik dagoen produktu-erregistroan erlazionatutako produktu gisa gehitu nahi duzun produktua.
    -   **Salmenten erlazio mota**: Gehitu produktu bat gidatua, salmenta gurutzatua, accessory gisa edo ordezko produktu nahi duzun hautatu.
    -   **Zuzenketa**: Hautatu produktuak arteko erlazioa izango noranzko bakarrekoa edo noranzko bikoa den ala ez. Hautatzean Noranzko Bakarrekoa, aukeran hautatu duzun produktu **Erlazionatutako produktua** aukera gomendio gisa erakutsiko da lehendik dagoen produkturako baina ez alderantziz.

9.  Produktuen inprimakian, hautatu **Gorde**.

## <a name="import-products"></a>Inportatu produktuak

Inportazio txantiloiak erabil ditzakezu produktu solteak bidaltzeko Dynamics 365 Sales-era.

## <a name="revise-a-product"></a>Berrikusi produktuak

Mantendu bizkor guztietatik beharren produktuak propietateak eta argitaratu berriro informazioa horrela, zure agente salmenta-inbentarioa azken aldaketak ikus ditzakezu eguneratu produktu-inbentarioa.

1.  Ziurtatu ondorengo segurtasun-funtzio edo baimen baliokideetako bat duzula: Sistemaren administratzailea, Sistemaren pertsonalizatzailea, Salmenten arduraduna, Salmenten zuzendariordea, Marketineko zuzendariordea edo Zuzendari nagusia.
2.  Gunearen mapan, hautatu **Produktuak**.
3.  Ireki aldatu nahi duzun produktu, multzo edo familia aktibo bat eta, komando-barran, hautatu **Berrikusi**.
4.  **Berretsi berrikustea** elkarrizketa-koadroan, hautatu **Berretsi**. Honek produktu egoera aldatzen **Atalean Berrikuspenaren**
5.  Aldaketak egin ondoren, komando-barran, hautatu **Argitaratu**.

    > [!TIP]
    > Aldaketak berreskuratzeko eta produktuaren azken bertsio aktiboarekin jarraitzeko, hautatu **Itzuli**. Produktuaren egoera babeskopia aldaketak hau **Aktibo**

## <a name="clone-a-product"></a>Produktuak klonatu 

Produktu berri bat sortzen ari bazara, denbora aurrezteko lehendik dagoen bat kopia dezakezu. Sortzen du jatorrizko kopia xehetasunekin guztiak izan ezik, izena eta ida.

1.  Ziurtatu ondorengo segurtasun-funtzio edo baimen baliokideetako bat duzula: Sistemaren administratzailea, Sistemaren pertsonalizatzailea, Salmenten arduraduna, Salmenten zuzendariordea, Marketineko zuzendariordea edo Zuzendari nagusia.
2.  Gunearen mapan, hautatu **Produktuak**.
3.  Hautatu klonatu nahi duzun produktu bat eta, komando-barran, hautatu **Klonatu**. Berresteko elkarrizketa-koadroa agertzen da.
4.  Hautatu **Berretsi**.

Produktu-erregistro berri bat irekiko bera izan ezik, izena eta ida. jatorrizko duzuna gisa xehetasunekin

## <a name="retire-a-product"></a>Erretiratu produktuak 

Erakundeak ez badu gehiago saltzen produktu bat, ken ezazu saltzaileek erabilgarri eduki ez dezaten.

1.  Ziurtatu Sistemaren administratzailearen edo Sales Professional kudeatzailearen funtzioa edo antzeko baimenak dituzula.
2.  Gunearen mapan, hautatu **Produktuak**.
3.  Ireki kendu nahi duzun produktua, multzo edo familia aktibo bat eta, komando-barran, hautatu **Kendu**.
4.  **Berretsi erretiratzea** elkarrizketa-koadroan, hautatu **Berretsi**.


## <a name="delete-a-product"></a>Ezabatu produktu bat

Horrela, produktu bat saltzen gelditzeko, ezaba ezazu.

> [!IMPORTANT]
> Ezin duzu eskuratu ezabatutako erregistro bat.

1.  Ziurtatu Sistemaren administratzailearen edo Sales Professional kudeatzailearen funtzioa edo antzeko baimenak dituzula.
2.  Gunearen mapan, hautatu **Produktuak**.
3.  Hautatu ezabatu nahi duzun produktu bat eta, komando-barran, hautatu **Ezabatu**.
4.  **Berretsi ezabatzea** elkarrizketa-koadroan, hautatu **Jarraitu**.
 
 ## <a name="quantity-factors-for-products"></a>Produktuen kantitate faktoreak

Kantitate faktoreak erabiltzen ditu harpidedun oinarritutako produktuen salmenta sustatzeko. Harpidetzetan oinarritutako produktuetarako, aurrekontuan edo proiektuaren kontratuaren lerroan erabiltzaile-hilabete kopurua adierazten da.

Normalean, harpidedun softwarearen prezioa katalogoan gordetzen da erabiltzaile bakoitzeko prezio gisa. Hala ere, beste denbora deskribapen batzuk erabil ditzakezu. Salmenta prozesuan, aurrekontuen lerroko prezioa erabiltzaile bakoitzeko, salmentako IT agentearen bidez negoziatu eta deskontatu zen hileko prezioa izan ohi da. Akordio bakoitzak erabiltzaile kopurua eta harpidetza hilabete desberdinak ditu. Aurrekontuen lerroaren zenbatekoa kalkulatzeko erabiltzen den kantitatea erabiltzaile kopurua eta harpidetza hilabeteen produktua da.

Kopuru-faktoreek produktuaren atributuetan oinarritzen dira. Produktu baterako propietate espezifikoak konfiguratzen dituzunean, propietate horien edo propietate guztien azpimultzoa uzten dizu kantitate faktore gisa.

Sistemak balioztatzen du zenbakizko datu mota bat duten zenbakizko propietateak edo produktuaren propietateak kantitate faktore gisa markatzen direla. Kantitate-faktoreak konfiguratutako produktu bat aurrekontu-lerrora gehitzen denean, **Kopurua** aurrekontuen lerroan irakurtzeko soilik eremu bihurtzen da. Kantitate faktoreak diren produktuaren propietateen balioak sartu ondoren, aurrekontuen lerroaren kantitatea kalkulatzen du.

Adibidez, propietate hauek badaude: 

- **Erabiltzaile kop**: erabiltzaile kopurua 
- **Hilabete kop**: harpidetza-hilabete kopurua
- **SKU produktua** 

**Erabiltzaile kop** eta **Hilabete kop** propietateak kantitate faktore gisa markatu daitezke produktuaren lerroko propietateak editatzean. 


[!INCLUDE[footer-include](../includes/footer-banner.md)]