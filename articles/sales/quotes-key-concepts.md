---
title: Eskaintzak - Gako-kontzeptuak
description: Gai honek eskuragarri dauden proiektuen eskaintzei eta salmenta-eskaintzei buruzko informazioa eskaintzen du Project Operations-en.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 8d113111f5fbf6f5d23ef02cae36d85a27beed93
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121293"
---
# <a name="quotes---key-concepts"></a>Eskaintzak - Gako-kontzeptuak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations-en, bi aurrekontu mota daude, proiektuak eta salmentak. Kuoten bi motak modu desberdinetan bereizten dira:

- **Lerro-elementuen saretak**: Salmenta-eskaintzetan, lerroentzako elementuen sareta bakarra dago. Edo proiektu-eskaintza batean, lerroentzako bi sareta ditu. Sareta bat proiektu-lerroetarako da eta bestea produktu-lerroetarako.
- **Aktibazioa eta berrikuspenak**: Salmenten aurrekontuek aktibazioa eta berrikuspenak onartzen dituzte. Prozesu hauek ez dira onartzen proiektuaren aurrekontuan.
- **Atxikitako eskaerak**: Hainbat eskaera erantsi diezaiokezu salmenta-eskaintzari. Proiektu-kontratu bakarra erants dakioke proiektu-eskaintzari.
- **Aurrekontua irabaztea**: Salmenten aurrekontua irabazten duzunean, erlazionatutako aukerak zabalik egon daitezke. Proiektu-eskaintza irabazi ondoren, erlazionatutako abagunea itxita dago.
- **Eremuak eta kontzeptuak**: Salmenta-eskaintzak ez ditu proiektu-eskaintzan biltzen diren zenbait eremu eta kontzeptu biltzen. Eremuek **Kontratazio-unitatea**, **Kontuen kudeatzailea**, eta **Harreman-izenaren faktura** dituzte.  
- **Mota**: Salmenta-eskaintzak eta proiektu-eskaintzak multzoan oinarritutako eremua moduan, **Mota**, ere identifikatzen dira. Salmenta-eskaintzak lortzeko, eremuak balio hau du: **Elementuan oinarritutakoa**. Proiektu-eskaintza lortzeko, balio hau du: **Lanean oinarritutakoa**.

Gai honek proiektu-eskaintzen xehetasunak fokuratzen ditu ardatz.

Project Operations-en proiektu-eskaintzak lerro bat baino gehiago edo eskaintzaren lerro bat izan dezake. Izan ere, proiektu-eskaintzak lerroentzako bi sareta ditu. Sareta bat aurreikuspen zehatzak egiteko aukera ematen duten proiektuetan oinarritutako lerroetarako da. Beste sareta produktu unitateko prezio sinplea eta kantitatean oinarritutako hurbilketa erabiltzen duten produktuetarako oinarritutako lerroetarako da.

- **Proiektuan oinarritutakoa**: eskaintza-balioa zenbat lan egin behar den kalkulatu ondoren zehazten da. Lanak maila altuan kalkula ditzakezu, aurrekontu lerro bakoitzaren azpian lerroaren xehetasun gisa zuzenean edo oinarrian egindako kalkuluetan oinarrituta, proiektu bat eta proiektuaren plana erabiliz. Proiektuetan oinarritutako eskaintzaren lerroak proiektuetan oinarritutako eskaintzetan baino ez dira aurkitzen Project Operations erabiliz. Eskaintzaren lerro mota hau idazketa-lerroen inprimaki pertsonalizatua da, Microsoft Dynamics 365 Sales-en eskuragarri dagoena..

- **Produktuan oinarritutakoa**: eskaintza-balioa saltzen den unitate kantitatearen eta salmenta prezioaren unitatearen arabera zehazten da. Produktuetan oinarritutako lerro bateko produktua Sales-en produktuen katalogotik dator edo zuk definitzen duzun produktua izan daiteke. Eskaintzaren lerro mota hau Project Opertions erabiliz sortutako proiektuan oinarritutako eskaintzetan ere eskuragarri dago.

Eskaintza baten zenbatekoa produktuetan oinarritutako lerroetan eta proiektuan oinarritutako lerroetan dago.

> [!NOTE]
> Eskaintzak eta eskaintzaren lerroak ez dira Project Operations behar. Proiektuaren prozesua proiektuaren kontratuarekin has dezakezu (saldu den proiektua). Hala ere, abagunea beharrezkoa da beti, eskaintza batekin edo proiektu-kontratu batekin hasi ala ez.

## <a name="project-based-quote-lines"></a>Proiektuetan oinarritutako eskaintzaren lerroak

Project Operations-en proiektuan oinarritutako eskaintzaren lerroak fakturazio metodo hauek ditu:

- Denbora eta materiala
- Prezio finkoa

### <a name="time-and-material"></a>Denbora eta materiala

Denboraren eta materialaren fakturazioaren metodoa kontsumoan oinarritzen da. Fakturazio metodo hau hautatzen duzunean, bezeroari fakturatu egingo zaio proiektuak kostuak suposatzen dituelako. Fakturak datan oinarritutako maiztasun periodikoan sortzen dira. Salmenta prozesuan, denboraren eta materialaren osagai baten balio estali bezeroak azken kostuaren aurreikuspena baino ez dio ematen bezeroari. Saltzaileak ez du konpromisoa hartzen proiektua aipatutako balioarekin zehazki osatzeko. Denboraren eta materialen osagaiek bezeroaren arriskua areagotzen dute. Bezeroek gainditu nahi ez duten klausula osagarriak negoziatu nahi dituzte arriskua minimizatzeko. Project Operations-ek ez du gainditzen ez diren klausularik onartzen.

### <a name="fixed-price"></a>Prezio finkoa

Prezio finkoa fakturatzeko metodoaren barruan, saltzaileak proiektua bezeroari kostu finkoan entregatzeko konpromisoa hartzen du. Bezeroari prezio finkoaren eskaintzaren lerroko kotizazio balioa fakturatzen zaio, saltzaileak eskaintzaren lerro hori entregatzeko sortzen dituen gastuak kontuan hartu gabe. Prezio finkoaren eskaintzaren lerroko balioa honako modu hauetako batean fakturatzen da: 

- Proiektuaren hasieran edo amaieran, edo proiektuaren mugarri bat lortzen denean, diru-kopuru gisa. 
- Eskaintzaren lerroko balio finkoaren kuota berdinen maiztasunean oinarritutako datan. Hitzaldi hauek epekako mugarri gisa ezagutzen dira.
- Proiektuan lortzen diren lanaren aurrerapenarekin edo mugarri zehatzekin lerrokatutako diru-balioa duten kuotetan. Kasu honetan, kuota bakoitzaren balioa desberdina izan daiteke, baina eskaintzaren lerroan dagoen balio finkoa gehitu beharko dute guztiek.

Project Operations-ek hiru fakturen antolaketa mota guztiak onartzen ditu prezio finkoko eskaintza lerroetarako.

## <a name="transaction-classification"></a>Transakzio-sailkapena

Zerbitzu profesionalen erakundeek normalean bezeroei eskaini eta fakturatzen diete kostuen sailkapenaren arabera. Kostuak transakzioen sailkapen honekin irudikatzen dira:

- **Ordua**: sailkapen honek proiektu baten lan edo giza baliabideen denboraren kostua adierazten du.
- **Gastua**: sailkapen honek proiektu bateko gainerako gastuak adierazten ditu. Gastuak modu zabalean sailka daitezkeenez, erakunde gehienek azpikategoriak sortzen dituzte, hala nola, bidaia, autoen alokairua, hotela edo bulegoko materiala.
- **Matrikula**: sailkapen honek bezeroaren gaineko kargak, zigorrak eta gainerako elementuak adierazten ditu. 
- **Zerga**: sailkapen honek erabiltzaileek gastuak sartzen dituztenean gehitzen dituzten zerga-zenbatekoak dira.
- **Materialaren transakzioa**: sailkapen honek produktuen lerroetako fakturak adierazten ditu proiektuaren faktura batean.
- **Mugarria**: sailkapen hori prezio finkoaren fakturazio logikaren arabera erabiltzen da.

Transakzio-sailkapen hauetako bat edo gehiago eskaintzaren lerro bakoitzarekin erlazionatuta egon daiteke. Eskaintza irabazi ondoren, transakzio-sailkapenaren eta eskaintzaren lerroaren arteko esleipenak kontratuaren lerrora transferitzen dira.
  
Adibidez, eskaintzak bi eskaintzaren lerro izan ditzake: 

- Ordua eta materiala fakturatzeko metodoa erabiltzen duten aholkularitza lana, denbora eta kuota transakzioen sailkapenak aplikagarriak direnean. Adibidez, ordainketa denbora eta kuota guztiak **Dinamika AX inplementazioa** adibide-proiekturako, bezeroari fakturatzen zaizkio erabiltzen diren denbora eta materialen arabera. 
- Prezio finkoko fakturazio metodoa erabiltzen duten erlazionatutako bidaien gastuak. Adibidez, bidaiarako gastu guztiak **Dinamika AX inplementazioa** adibide-proiekturako, diru-balio finkoan fakturatzen dira.

> [!NOTE]
> Proiektuaren eta transakzioen sailkapenen konbinazioa **Ordua**, **Gastu**, eta **Matrikula** eskaintzekin edo kontratuaren lerroarekin lotzen direnak bakarrak izan behar dute. Proiektuaren eta transakzioen klase konbinazio bera kontratuaren lerro edo eskaintzaren lerro bat baino gehiagorekin lotzen bada, Project Operations-ek ez du ondo funtzionatuko.

## <a name="billing-types"></a>Fakturazio motak

**Fakturazio mota** eremuak kargagarritasun kontzeptua definitzen du. Aukera multzo bat da, balore hauek ditu:

- **Kargagarria**: funtzio/kategoria hori jasotzen duen kostua proiektuaren exekuzioa bultzatzen duen kostu zuzena da, eta bezeroak lan hori ordainduko du. Ordainketa antolaketa-materiala edo prezio-finkoa bezala administratu daiteke. Hala ere, denbora hori igarotzen duen langileak dagokion kreditua jasoko du diruaren erabileragatik.
- **Ez kargagarria**: funtzio/kategoria hori jasotzen duen kostua proiektuaren exekuzioa bultzatzen duen kostu zuzentzat hartzen da, bezeroak lan hori errekonozitu ez eta ordaintzen ez badu ere. Denbora hori igarotzen duen langileak ez du horren faktura erabilgarri ordainduko.
- **Doan**: funtzio/kategoria hori jasotzen duen kostua proiektuaren exekuzioa bultzatzen duen kostu zuzentzat hartzen da, eta bezeroak hori errekonozituko du. Denbora hori igarotzen duen langileak horren faktura erabilgarri hori ordaintzeko baimena izango du. Hala ere, kostu hori ez zaio bezeroari kobratuko.
- **Ez dago eskuragarri**: aukera hau erabiliz diru-sarrerak jarraitzea eskatzen ez duten barne proiektuetan sortzen diren kostuak dira.

## <a name="invoice-schedule"></a>Fakturazio-antolaketa

Fakturazio-antolaketa proiektuen fakturazioa eguneratzen den data bat da. Aukeran fakturazio-antolaketa sor dezakezu eskaintza lerro batean. Eskaintza lerro bakoitzak bere fakturazio-antolaketa izan dezake. Fakturazio-antolaketa sortzeko, atributu-balio hauek eman behar dituzu:

- Fakturazioaren hasiera-data 
- Proiektuan fakturazioaren amaiera adierazten duen entrega-data
- Fakturen maiztasuna

Hiru atributu-balio hauek erabiliko ditu fakturazioan finkatzeko data-sorta sortzeko.

## <a name="invoice-frequency"></a>Fakturen maiztasuna

Faktura maiztasuna fakturak sortzearen maiztasuna adierazten laguntzen duten atributu-balioak gordetzen dituen entitatea da. Honako atributu hauek fakturaren maiztasuna entitatea adierazten edo zehazten dute:

- **Epea**: hilean behin, bi astean behin eta astero onartzen dira. 
- **Aldi bakoitzeko exekutatzen dira**: astean behin eta bi astetan behin, aldi bakoitzeko exekuxio bakarra defini dezakezu. Hileroko aldietan, aldi bakoitzeko 1-4 exekuzio artean defini dezakezu. 
- **Exekuzio egunak**: fakturak noiz exekutatu behar diren. Atributuak bi modutara konfigura ditzakezu:
  - **Lanegunetan**: adibidez, fakturazioa astelehenero edo bi astelehenero exekutatzen dela zehaztu dezakezu. Fakturazioa lanegunean exekutatzeko ezarri behar duten bezeroek konfigurazio mota hau nahiago dute. 
  - **Egutegiko egunak**: adibidez, fakturazioa hileko zazpigarren egunean eta hogeita batean egiten dela zehaztu dezakezu. Erakunde batzuek konfigurazio mota hau nahiago dute, fakturazioa hilero antolaketa finko batean exekutatzen dela bermatzen laguntzen duelako.
  
### <a name="invoice-schedule-for-a-fixed-price-quote-line"></a>Prezio-finkoko eskaintzen lineako fakturen antolaketa

Prezio-finkoko eskaintzen lerrorako, erabil dezakezu **Fakturen egutegia** sareta, eskaintzaren lerroaren balio berdina duten fakturazio-mugarriak sortzeko.

- Berdin banatzen diren fakturazio-mugarriak sortzeko, hautatu fakturen maiztasuna, sartu fakturazioaren hasiera-data aurrekontuen lerroan eta hautatu **Eskatutako amaiera-data** orrialdeko eskaintza lortzeko **Laburpena** sekzioan eskaintzaren goiburuan. Ondoren, hautatu **Sortu aldizkako mugarriak** hautatutako fakturen maiztasunean oinarritutako mugarri berdinak sortzeko. 
- Ordainpeko fakturaziorako mugarri bat sortzeko, mugarri bat sortu eta, ondoren, sartu eskaintzaren lerroko balioa mugarri zenbateko gisa.
- Proiektu-planean zeregin zehatzetan oinarritutako fakturazio-mugarriak sortzeko, mugarri bat sortu eta proiektuaren egitarauaren elementua esleitu ezazu fakturazio-mugarriko erabiltzailearen interfazean.


[!INCLUDE[footer-include](../includes/footer-banner.md)]