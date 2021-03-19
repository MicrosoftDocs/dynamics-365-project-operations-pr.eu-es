---
title: Enpresen arteko fakturazioa
description: Artikulu honek enpresen arteko fakturazioari buruzko informazioa eta adibideak eskaintzen ditu proiektuetarako.
author: Yowelle
manager: AnnBe
ms.date: 09/14/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LedgerInterCompany
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 94153
ms.assetid: 33e98da7-01c1-4369-923d-aa1c8326cb80
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 76eba87e7cc78dcc14510a8fb53677d626bf204f
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5270753"
---
# <a name="intercompany-invoicing"></a>Enpresen arteko fakturazioa

[!include [banner](../includes/banner.md)]

Artikulu honek enpresen arteko fakturazioari buruzko informazioa eta adibideak eskaintzen ditu proiektuetarako.

Zure erakundeak dibisio, filial eta beste pertsona juridiko ugari izan ditzake produktuak eta zerbitzuak elkarri proiektuetarako transferitzen dituztenak. Zerbitzua edo produktua eskaintzen duen pertsona juridikoari deitzen zaio *pertsona juridiko mailegu-emailea*, eta zerbitzua edo produktua jasotzen duen pertsona juridikoari *zor juridikoa*. 

Ondorengo ilustrazioak agertoki tipikoa erakusten du; bi pertsona juridikok, SI FRk (mailegu maileguan dagoen pertsona juridikoa) eta SI USAk (mailegu maileguaren pertsona juridikoa) baliabideak partekatzen dituzte bezeroarentzako A. Eszenatoki honetarako, SI FR kontratatuta dago lana bezeroarentzako A. 

[![Enpresen arteko fakturazioaren adibidea](./media/interco.invoicing-01.jpg)](./media/interco.invoicing-01.jpg) 

Helburua konpainien arteko proiektuen transakzioen kostuen kontrola, diru-sarreren aitorpena, zergak eta transferentziaren prezioa malguagoak eta indartsuagoak izatea da. Gainera, gaitasun hauek eskaintzen dira:

-   Sortu mailegu-erakunde juridiko bateko proiektu baten aurkako bezeroaren fakturak, enpresen arteko orriak, gastuak eta saltzaileen fakturak mailegu-entitate juridiko batean erabiliz.
-   Zergen kalkuluak eta zeharkako kostuak lagundu.
-   Atzeratu diru-sarreren aitorpena mailegu-entitate juridiko batean eta mailegu-hartzaile batek kostua aitortu behar duenean.
-   Mailegu-entitate juridikoan izapidetutako lanak (WIP) irabaztea.
-   Ezarri hainbat prezio ereduetan oinarrituta egon daitezkeen transferentzia prezioak. Hona hemen zenbait adibideak:
    -   **Kopurua** - Sartu duzun zenbatekoa **Prezioak** eremua kantitate edo unitate bakoitzeko benetako kostua da.
    -   **Kargen zenbatekoa** - Transakzio bakoitzeko prezioa / kostua gehi tarifan sartutako gastuen zenbatekoa **Prezioak** zelaia.
    -   **Kargen ehunekoa** - Transferentziaren prezioa transakzio bakoitzeko prezioa / kostua da **Prezioak** zelaia.
    -   **Salmenta prezioaren ehunekoa** - Mailegu-entitate juridikoari transferitzen zaion salmenta-prezioaren ehunekoa.
    -   **Salmenta prezioaren azpitik dagoen zenbatekoa** - Mailegu-entitate juridikoak mailegu-entitate juridikoari transferitu aurretik salmenta-prezioetatik gordetzen duen kopurua.
    -   **Ekarpen ratioa** - Sartu duzun zenbakia **Prezioak** eremua kotizazio ratioa da, salmenta prezioaren ehuneko gisa adierazten dena.

## <a name="example-1-set-up-parameters-for-intercompany-invoicing"></a>1. adibidea: Konfiguratu enpresen arteko fakturaziorako parametroak
Adibide honetan, USSI mailegu-entitate juridikoa da, eta bere baliabideek azken bezeroarekin kontratua duen FRSI mailegu-hartzailea den pertsona juridikoari emandako denboraren berri ematen ari dira. USSIko langileek salatzen dituzten orduak eta gastuak FRSIk sortzen duen proiektuaren fakturan sar daitezke. Horrez gain, mailegu-entitate juridikotik (adibide honetan USSI) sor daitekeen transakzioen hirugarren iturria dago, saltzaile partekatuen zerbitzuak filialei (hala nola, FRSI) eskaintzen dizkionean eta, ondoren, kostu horiek filial horien barruan dauden proiektuetara bideratzen dituenean. Bat datorren faktura dokumentu guztiak eta zergen kalkuluak Finantzak betetzen ditu. 

Adibide honetarako, FRSIk USSI entitate juridikoan bezeroa izan behar du eta USSIk FRSI entitate juridikoan saltzailea. Bi pertsona juridikoen arteko enpresa arteko harremana ezar dezakezu. Ondorengo prozedurak parametroak nola konfiguratu erakusten ditu, pertsona juridiko biek enpresen arteko fakturazioan parte har dezaten.

1. Konfiguratu FRSI bezero gisa USSI entitate juridikoan, eta konfiguratu USSI saltzaile gisa FRSI entitate juridikoan. Zeregin horretarako beharrezkoak diren urratsetarako hiru sarrera puntu daude.

   | Urratsa |                                                       Sarrera-puntua                                                        |                                                                                                                                                                                               Deskribapenak                                                                                                                                                                                               |
   |------|--------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
   |  A   | USSI aplikazioan, egin klik <strong>Kobratu beharreko kontuak</strong> &gt; <strong>Bezeroak</strong> &gt; <strong>Bezero guztiak</strong>. |                                                                                                                                                                  Sortu bezeroen erregistro berria FRSIrentzat, eta hautatu bezero taldea.                                                                                                                                                                  |
   |  Si   |    FRSIn, egin klik <strong>Ordaintzeko kontuak</strong> &gt; <strong>Saltzaileak</strong> &gt; <strong>Saltzaile guztiak</strong>.     |                                                                                                                                                                    Sortu saltzaileen erregistro berria FRSIrentzat, eta hautatu saltzaile taldea.                                                                                                                                                                    |
   |  C   |                                  FRSIn, ireki sortu berri duzun saltzailearen erregistroa.                                  | Ekintza panelean, <strong>Orokorra</strong> fitxan, <strong>Konfiguratu</strong> taldea, klik egin <strong>Enpresen artekoa</strong>. Gainean <strong>Enpresa artekoa</strong> orrialdean, <strong>Negoziazio harremana</strong> fitxa, ezarri <strong>Aktiboa</strong> hurrengora graduatzailea <strong>Bai</strong>. <strong>Bezeroen enpresa</strong> eremuan, hautatu A urratsean sortu duzun bezeroaren erregistroa. |


2. Egin klik **Proiektuen kudeaketa eta kontabilitatea** &gt; **Konfigurazioa** &gt; **Proiektuak kudeatzeko kontabilitate parametroak**, eta egin klik **Enpresa artekoa** fitxa. Parametroak konfiguratzeko modua maileguan dagoen pertsona juridikoa edo mailegu-emailea denaren araberakoa da.
   -   Mailegu-hartzaile juridikoa bazara, hautatu kontratazio-kategoria, automatikoki sortzen diren saltzailearen fakturekin bat egiteko erabili beharko litzatekeena.
   -   Mailegu-entitate juridikoa bazara, mailegu-entitate bakoitzerako, hautatu lehenetsitako proiektuaren kategoria transakzio mota bakoitzerako. Proiektuen kategoriak zerga konfiguraziorako erabiltzen dira, enpresa arteko eragiketetan fakturatutako kategoria mailegu-entitate juridikoan bakarrik dagoenean. Enpresen arteko transakzioengatik diru-sarrerak eskuratzea aukera dezakezu. Metaketa hori transakzioak erregistratzen direnean egiten da, eta gero alderantziz egiten da enpresen arteko faktura argitaratzen denean.

3. Egin klik **Proiektuen kudeaketa eta kontabilitatea** &gt; **Konfigurazioa** &gt; **Prezioak** &gt; **Transferentziaren prezioa**.
4. Aukeratu moneta, transakzio mota eta transferentziaren prezioaren eredua. Fakturan erabiltzen den moneta mailegu-entitate juridikoan mailegu-entitate juridikoarentzako bezeroaren erregistroan konfiguratuta dagoen moneta da. Moneta transferentzia prezioen taulako sarrerekin bat egiteko erabiltzen da.
5. Egin klik **Liburu nagusia** &gt; **Mezuaren konfigurazioa** &gt; **Enpresen arteko kontabilitatea**, eta harreman bat sortu USSI eta FRSI-rentzat.

## <a name="example-2-create-and-post-an-intercompany-timesheet"></a>2. adibidea: Enpresen arteko orri bat sortu eta argitaratu
USSIk, mailegu-emaile den entitateak, FRSI-k (mailegu-entitate juridikoa) proiektu baten denbora-orria sortu eta argitaratu behar du. Zeregin horretarako beharrezkoak diren urratsetarako bi sarrera puntu daude.

| Urratsa | Sarrera-puntua                                                                       | Deskribapenak                                                                                                                                                                                       |
|------|-----------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A    | **Proiektuen kudeaketa eta kontabilitatea** &gt; **Orriak** &gt; **Denbora-orri guztiak** | Sortu denbora-orria berri bat. Ordu-orriaren lerroan **Pertsona juridikoa** eremua, hautatu **FRSI**. **Proiektuaren IDa** eremuan, hautatu proiektua FRSIn. Sartu asteko egun bakoitzeko orduak. |
| Si    | **Denbora-orria** orrialdea                                                                | Lan-fluxua exekutatu ondoren, argitaratu denbora-orria eta idatzi bonuaren zenbakiaren oharra.                                                                                                               |

## <a name="example-3-create-and-post-an-intercompany-vendor-invoice"></a>3. adibidea: Sortu eta argitaratu enpresen arteko saltzaile faktura
USSIk, mailegu-emaile den entitateak, FRSI-k (mailegu-entitate juridikoa) proiektu baten enpresen arteko saltzailearen faktura sortu eta argitaratu behar du. Saltzailearen faktura honek USSIk ordaintzen dituen saltzaileek egindako azpikontratatutako eskulana eta gastua adierazten ditu. Zeregin horretarako beharrezkoak diren urratsetarako bi sarrera puntu daude.

| Urratsa | Sarrera-puntua                                                                                      | Deskribapenak                                                                                                                                                                                                                                                                          |
|------|--------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A    | **Ordaintzeko kontuak** &gt; **Fakturak** &gt; **Ireki saltzailearen fakturak** &gt; **Saltzailearen faktura berria** | Sortu saltzailearen faktura berria, eta sartu FRSIren proiektuaren izenean eskuratutako zerbitzuak.                                                                                                                                                                                  |
| Si    | **Saltzailearen faktura** orrialdea                                                                      | Sartu azpikontratatutako zerbitzuak ordezkatzen dituzten lineak FRSIren izenean. Gainean **Lerroaren xehetasunak** FastTab, **Proiektua** Faktura lerroaren fitxa, **Proiektuaren enpresa** eremua, sartu **FRSI**. Idatzi proiektua eta dagokion informazioa. Ondoren, bidali saltzailearen faktura. |

## <a name="example-4-create-and-post-the-intercompany-invoice"></a>4. adibidea: Sortu eta argitaratu enpresen arteko faktura
USSIk, mailegu-emaileak, enpresen arteko faktura sortu eta argitaratu behar du. Zeregin horretarako beharrezkoak diren urratsetarako bi sarrera puntu daude.

| Urratsa | Sarrera-puntua                                                                                             | Deskribapenak                                                                                                                                      |
|------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
| A    | **Proiektuen kudeaketa eta kontabilitatea** &gt; **Proiektuaren fakturak** &gt; **Enpresen arteko bezeroaren faktura**  | Egin klik **Berria** irekitzeko **Enpresen arteko faktura sortu** orrialdea.                                                                                  |
| Si    | **Proiektuen kudeaketa eta kontabilitatea** &gt; **Proiektuaren fakturak** &gt; **Enpresen arteko bezeroaren fakturak** | Gainean **Enpresen arteko faktura sortu** orrialdean, sartu pertsona juridikoa, zehaztu sartu beharreko transakzioa eta egin klik **Bilatu**. |
| C    | **Proiektuen kudeaketa eta kontabilitatea** &gt; **Proiektuaren fakturak** &gt; **Enpresen arteko bezeroaren fakturak** | Aukeratu fakturatzeko eragiketak edo egin klik **Hautatu guztiak** zerrendako transakzio guztiak fakturatzeko eta egin klik **Ados**.                  |
| D    | **Enpresen arteko faktura** orrialdea                                                                       | Enpresen arteko bezeroen faktura proposamena agertzen da.                                                                                             |
| E    | **Enpresen arteko faktura** orrialdea                                                                       | Egin klik **Bidali**.                                                                                                                                  |

## <a name="example-5-post-the-vendor-invoice-and-invoice-the-customer"></a>5. adibidea: Bidali saltzailearen faktura eta fakturatu bezeroari
USSI mailegu-emaileak enpresa arteko bezeroen faktura argitaratzen duenean, zain dagoen saltzailearen faktura bat sortzen da mailegu-entitate juridikoan, FRSI. Saltzailearen faktura hau argitaratu ondoren, FRSIk USSIk sartu dituen orduak ere fakturatzen dizkio proiektuaren bezeroari. Zeregin horretarako beharrezkoak diren urratsetarako hiru sarrera puntu daude.

| Urratsa | Sarrera-puntua                                                                                        | Deskribapenak                                                                                                             |
|------|----------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------|
| A    | **Ordaintzeko kontuak** &gt; **Fakturak** &gt; **Saltzailearen fakturak zain**                            | Berrikusi faktura, denbora-orriaren balioak sartzen direla egiaztatzeko eta, ondoren, bidali saltzailearen faktura.                  |
| Si    | **Proiektuen kudeaketa eta kontabilitatea** &gt; **Proiektuaren fakturak** &gt; **Proiektuaren faktura-proposamenak** | Sortu proiektuaren faktura berria proiektuan, eta egiaztatu argitaratutako orduen transakzioak agertzen direla.            |
| C    | **Proiektuaren faktura** orrialdea                                                                       | Aukeratu proiektuaren faktura eta egin klik **Xehetasunak ikusi** kostua eta salmenten zenbatekoa berrikusteko. Ondoren, bidali faktura. |


Informazio gehiagorako, ikus [Konfiguratu enpresen arteko proiektuen fakturazioa](tasks/configure-intercompany-project-invoicing.md).




[!INCLUDE[footer-include](../includes/footer-banner.md)]