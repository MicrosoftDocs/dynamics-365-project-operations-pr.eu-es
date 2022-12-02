---
title: 2021eko uztaileko berrikuntzak - Balabideetan edo ekoizpenean oinarritutako egoeretarako Project Operations
description: Gai honek 2021eko uztaileko Project Operations bertsioan eskuragarri dauden kalitate-eguneratzeei buruzko informazioa eskaintzen du baliabideetan / ez-ekoizpenean oinarritutako eszenatokietarako.
author: sigitac
ms.date: 07/07/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: c004a6adc265f8f02fc557700d9b88a174c221c4
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8931683"
---
# <a name="whats-new-july-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>2021eko uztaileko berrikuntzak - Balabideetan edo ekoizpenean oinarritutako egoeretarako Project Operations

*Honi aplikatzen zaio: Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations*

Gai hau Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

   - Project Operations Microsoft Dataverse-ko inguruneko bertsioan 4.12.0.148 edo 4.12.0.152.
   - Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunearen 10.0.20 bertsioan.

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

Eginbide hauek sartzen dira bertsio honetan:

- Administratzaileek ezarpenen menutik PSS erregistroak eta Eragiketak Ezartzeko erregistroak ikusteko gaitasuna dute. Erregistroak 90 egunez gordetzen dira.

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Ez dago bertsio honetan Project Operations idazketa bikoitzeko mapen eguneratzerik.

Project Operations idazketa bikoitzeko mapen uneko zerrenda eta bertsioak ikusteko, ikusi [Project Operations idazketa bikoitzeko mapen bertsioak](../environment/resource-dual-write-maps.md).

Exekutatu beti maparen azken bertsioa zure ingurunean eta gaitu erlazionatutako taula-mapa guztiak eguneratzen dituzunean Project Operations Dataverse irtenbidea eta Finantza soluzioaren bertsioa. Zenbait eginbide eta gaitasunek agian ez dute behar bezala funtzionatuko maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Idazketa bikoitza** orrialdean **Bertsioa** zutabean. Aktibatu maparen bertsio berria hautatuta **Taulen mapen bertsioak**, azken bertsioa hautatuz eta ondoren hautatutako bertsioa gordez. Kutxaz kanpoko taulako mapa pertsonalizatu baduzu, aldaketak berriro aplikatu. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa hastean arazoren bat baduzu, jarraitu argibideak [Taulen zutabeak falta dira mapetan arazoa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) idazketa bikoitzeko arazoak konpontzeko gida atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| **Ezaugarrien eremua**              | **Erreferentzia-zenbakia** | **Kalitatearen eguneratzea**                                                                                                                                                                                             |
|-------------------------------|----------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Fakturazioa eta prezioak           | 2224046              | **Transakzio Klase** eremua editagarria da **Aipatu lerroaren xehetasunak** fitxan, baina blokeatuta dago **Aipatu lerroaren xehetasunak** orrialdean.                                                                     |
| Fakturazioa eta prezioak           | 2224400              | **Itxi Aurrekontua Irabazitako moduan** Ekintzak huts egiten du aurrekontuak data mugarririk ez duenean.                                                                                                                                    |
| Fakturazioa eta prezioak           | 2234089              | Produktuaren deskribapena eskuz idazten duzunean, materiala kalkulatzeko zenbateko bat sartu ondoren garbituko da.                                                                                                                         |
| Fakturazioa eta prezioak           | 2234100              | **Zereginen fakturazio konfigurazioa** saretak ez du **Materiala** zutabea eta balioa da **Zereginen fakturazioa** proiektuaren fitxan.                                                                                                       |
| Fakturazioa eta prezioak           | 2277409              | Produktuaren IDa ez dago eskuragarri kontratu-lerroaren xehetasunetan material mota bateko linean.                                                                                                                                        |
| Fakturazioa eta prezioak           | 2281728              | Kontratu lerro bat sortzeak alferrikako datuak ebaluatzen ditu, datuen bolumena nabarmen handituz, eta horrek errendimendua eragiten du.                                                                                |
| Fakturazioa eta prezioak           | 2298668              | Gogoratutako eta ezabatutako gastuarekin lotutako egunkari lerroak ez dira kentzen.                                                                                                                                     |
| Fakturazioa eta prezioak           | 2300192              | Hainbat erabiltzaile faktura bat editatzen ari direnean, baliteke faktura lerroaren xehetasun berri bat sortzea baieztatutako fakturan.                                                                                   |
| Fakturazioa eta prezioak           | 2301569              | Ezin dira fakturak zuzendu \$0 zenbateko atxikipena aplikatu da.                                                                                                                                        |
| Fakturazioa eta prezioak           | 2307965              | Akats bat gertatzen da kategoriako prezioa falta den balioekin sortzen bada.                                                                                                                           |
| Fakturazioa eta prezioak           | 2326870              | Errore bat gertatzen da **Microsoft.Dynamics.ProjectService.Plugins.PostInvoiceLineDelete** elementuan **producttypecode** nulua bada.                                                                            |
| Fakturazioa eta prezioak           | 2332732              | Akats bat gertatzen da kontratu lerroaren mugarri bat eskaera lerro gabe sortzen bada.                                                                                                                |
| Proiektuaren antolaketa eta jarraipena | 2181094              | Project Scheduling APIak orain 90 egunez gordetako PSS erregistroak eta eragiketa multzo erregistroak onartzen ditu.                                                                                                                  |
| Proiektuaren antolaketa eta jarraipena | 2254201              | **Antolaketa modua** etiketa lehenetsitako logika deskribatzen duten xehetasunekin eguneratzen da.                                                                                                                                      |
| Proiektuaren antolaketa eta jarraipena | 2300252              | **openProject** erantzunaren cachea eguneratuta dago eta token jabea cache gakoan sartzen du, **oinarri Url**, eta **Segmentuaren URLa**, **Eskaeraren URLa** beti birsortu ahal izateko **oinarri Url** aldatzen bada. |
| Proiektuaren antolaketa eta jarraipena | 2301312              | **msdyn_membershipstatus** fitxategia kendu da **Proiektuaren taldeko kidea** ikuspegitik.                                                                                                                                        |
| Proiektuaren antolaketa eta jarraipena | 2302759              | Produktuak beharrik gabe eskuratzen dira **Baliabideen esleipena**,**Aurrekontuak**, eta **Gastuen aurrekontuak** fitxetan.                                                                                                        |
| Proiektuaren antolaketa eta jarraipena | 2308050              | **CopyProject** huts egin du errorearekin, "Huts egin du tokenak urruneko zerbitzuarekin hitz egiteko".                                                                                                                           |
| Proiektuaren antolaketa eta jarraipena | 2322650              | **Proiektuaren ataza zerrenda** ikuspegia eguneratu da lehenespenez atazaren data bistaratzeko.                                                                                                            |
| Proiektuaren antolaketa eta jarraipena | 2327266              | **CopyProject** errorea sortzen du "Hiztegian aurkitu ez den gakoa" estimazioak kopiatzean.                                                                                                      |
| Proiektuaren antolaketa eta jarraipena | 2328123              | **CopyProject** errorea sortzen du, "Huts egin du tokenak urruneko zerbitzuarekin hitz egiteko".                                                                                                                          |
| Proiektuaren antolaketa eta jarraipena | 2336258              | **CopyProject** baliabideen posizio izenak gaizki kopiatzen ditu.                                                                                                                                                 |
| Fakturazioa eta prezioak           | 2224476              | **Erreserbatzeko Baliabidea** eremuak ez du behar bezala lehenetsitako saioa hasita duen erabiltzailea **Materialaren erabilera** orrialdean.                                                                                                            |
| Baliabideen kudeaketa           | 2277249              | Akats bat gertatzen da proiektuan oinarritutako baliabideen eskakizuna eguneratzen denean.                                                                                                            |
| Baliabideen kudeaketa           | 2323869              | Baliabideen erabilerak ez ditu iragazitako baliabideak behar bezala ezagutzen.                                                                                                                                             |
| Denbora eta gastua              | 2176538              | Iragazkien operadore okerrak aplikatzen dira **Denbora Sarrera** kontrolean.                                                                                                                                                   |
| Denbora eta gastua              | 2177462              | Sarean denbora-sarrera bat ezabatzeak ez du eguneratzen **Bidali**, **Gogoratu**, **Ezabatu**, eta **editatu sarrera** botoiaren egoera espero bezala.                                                                                        |
| Denbora eta gastua              | 2299985              | **TimeEntriesImportFromResourceAssignment** ez du hasierako / amaierako ordua mantentzen esleipenaren ingeradetatik.                                                                                                  |
| Denbora eta gastua              | 2318426              | Denbora sarrera bidali ondoren, blokeatutako eremuak edita daitezke.                                                                                                                                   |
| Denbora eta gastua              | 2323749              | Akats bat gertatzen da gastua sortzen denetik erreserbatzeko baliabide baten **Erlazionatutakoa** fitxan.                                                                                                      |
| Denbora eta gastua              | 2327678              | Fitxategiaren denbora sarrera bat sortzen duzunean erreserbatzeko baliabide baten **erlazionatutakoa** fitxatik, baliabide nagusia ez da denbora sarrera kontrolera pasatzen.                                                                            |
| Orokorrak                       | 2296857              | Iraupen luzeko lanetarako aurrerapenen jarraipena.                                                                                                                                                                        |
| Orokorrak                       | 2253682              | Project Operations idazketa bikoitzeko soluzioa ezin da instalatu idazketa bikoitzeko nukleoa idazketa bikoitzeko orkestrazio soluziorik gabeko ingurune batean instalatuta dagoenean.                                                |
| Orokorrak                       | 2316420              | Proiektuaren zerbitzuaren oinarrizko hornikuntzak huts egiten du aplikazioaren erabiltzailearen negozio unitatea aldatzen bada.                                                                                                                     |
| Orokorrak                       | 2376405              | Argitaratzaileari zuzendutako eguneratze arazoa konpondu da (kalitatearen eguneratzea 4.12.0.152 bertsioan dago eskuragarri)                                                                                                                     |
### <a name="project-management-and-accounting-on-dynamics-365-finance"></a>Project Management and Accounting Dynamics 365 Finance-n

| Ezaugarrien eremua                      | Erreferentzia-zenbakia | Kalitatearen eguneratzea                                                                                                                                                                                                                                                                                                                |
|-----------------------------------|------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Proiektuaren kudeaketa eta kontabilitatea | 4620267          | Ezin duzu inprimaki pertsonalizaturik gehitu **Helburua** eremua gehitzeko orrialde hauetara: **Proiektuak bidalitako transakzioa**, **Faktura proposamenak sortzea**, edo **Faktura proposamena**.                                                                                                                                                                                         |
| Proiektuaren kudeaketa eta kontabilitatea | 4613449          | Finantzan proiektuaren kontratuaren IDa hautatzen duzunean, Project Operations ingurune integratuak irekitzen du lehendik dagoen proiektuaren kontratua ireki beharrean erregistro berri bat sortzeko.                                                                                                                                           |
| Proiektuaren kudeaketa eta kontabilitatea | 4614445          | Project Operations agertoki integratuaren hedapenean ezin duzu editatu **Artikuluen salmenten gaineko zergaren taldea** fasetik ateratako fakturazio proposamenaren eremua. Artikuluen salmenten gaineko zergaren taldea aldatu egin beharko litzateke transakzio mota guztietako faktura proposamen ireki baterako, kontuan, orduak, gastuak, tasak eta artikuluak barne. |
| Proiektuaren kudeaketa eta kontabilitatea |                  | Ezin da bidali denbora transakzioaren zuzenketa negatiboaren emaitza den faktura proposamenik.                                                                                                                                                                                                                                              |
| Proiektuaren kudeaketa eta kontabilitatea |                  | Faktura proposamenen lerroak bikoiztu egiten dira aldian aldiko prozesuaren hainbat kasutan, **Inportatu eszenaratzetik** aldi berean exekutatzean.                                                                                                                                                                                                                |

