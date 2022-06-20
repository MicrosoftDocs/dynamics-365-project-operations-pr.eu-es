---
title: '2021eko uztaileko berritasunak: Project Operations lite-ren oinarrizko inplementazioa'
description: Artikulu honek Project Operations lite inplementazioaren 2021eko uztaileko bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 07/07/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 7964f38c1bc7a8e0440e2e922ff153fd9bede131
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8913973"
---
# <a name="whats-new-july-2021---project-operations-lite-deployment"></a>2021eko uztaileko berritasunak: Project Operations lite-ren oinarrizko inplementazioa

_Honi aplikatzen zaio: Oinarrizko inplementazioa: kudeatu proformako fakturak_

Artikulu hau honako hauei aplikatzen zaie Dynamics 365 Project Operations osagaiak eta bertsioak:

  - Project Operations Dataverse-ko inguruneko bertsioan 4.12.0.148 edo 4.12.0.152.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak
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
