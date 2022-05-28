---
title: Transakzioen jatorria - Lotu benetakoak haien iturriarekin
description: Gai honek transakzioen jatorriaren kontzeptua benetakoak jatorrizko iturburu-erregistroekin lotzeko nola erabiltzen den azaltzen du, hala nola denbora-sarrera, gastu-sarrera edo materialaren erabilera-erregistroak.
author: rumant
ms.date: 03/25/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 908f78f7d58ec4b18f37d03b6fa7c4e2295491fa
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8584811"
---
# <a name="transaction-origins---link-actuals-to-their-source"></a>Transakzioen jatorria - Lotu benetakoak haien iturriarekin

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Transakzioen jatorri-erregistroak benetakoak beren iturburuarekin lotzeko sortzen dira, hala nola, denbora-sarrerak, gastu-sarrerak, materialaren erabilera-erregistroak eta proiektuaren fakturak.

Hurrengo adibidean Project Operations proiektuaren bizi-zikloko denbora sarreren prozesaketa tipikoa erakusten da.

> ![Prozesatzeko denbora osoak Proiektu Eragiketetan.](media/basic-guide-17.png)
 
1. Denbora-sarrera bidaltzeak bi aldizkari-lerro sortzea eragiten du: kosturako bat eta fakturatu gabeko salmenterako.
2. Denbora-sarreren behin-behinean onartzeak bi erreal sortzen ditu: kosturako bat eta fakturatu gabeko salmentetarako.
3. Erabiltzaileak proiektuaren faktura sortzen duenean, fakturen lerroko transakzioa fakturatu gabeko salmenten egiazko datuak erabiliz sortzen da.
4. Faktura baieztatzen duzunean, fakturatutako bi benetako datu sortzen dira: fakturatu gabeko itzulerak eta fakturatutako salmenta erreal berria sortzen da.

Prozesatzeko lan-fluxu honetako gertaera bakoitzak Transakzio-jatorrizko entitatean erregistroak sortzea abiarazten du, denbora-sarreran, egunkari-lerroan, benetako eta faktura-lerroaren xehetasunetan sortzen diren erregistro horien arteko erlazioen arrastoa eraikitzen laguntzeko.

Hurrengo taulan, aurreko lan-fluxuaren transakzioaren jatorriko entitateko erregistroak agertzen dira.

| Gertaera                        | Jatorria                   | Jatorri mota                       | Transakzioa                       | Transakzio mota         |
|------------------------------|--------------------------|-----------------------------------|-----------------------------------|--------------------------|
| Denbora-sarreraren bidalketa        | Denbora-sarreren erregistroa GIDA   | Denbora-sarrera                        | Kutxako liburuaren lerroaren erregistroa GIDA (kostua)   | Kutxako liburuaren lerroa             |
| Denbora-sarreren erregistroa GIDA       | Denbora-sarrera               | Kutxako liburuaren lerroaren erregistroa GUIDA (salmentak)  | Kutxako liburuaren lerroa                      |                          |
| Orduaren onarpena                | Kutxako liburuaren lerroaren erregistroa GIDA | Kutxako liburuaren lerroa                      | Fakturatu gabeko salmenten erregistroa GIDA        | Benetakoa                   |
| Denbora-sarreren erregistroa GIDA       | Denbora-sarrera               | Fakturatu gabeko salmenten erregistroa GIDA        | Benetakoa                            |                          |
| Kutxako liburuaren lerroaren erregistroa GIDA     | Kutxako liburuaren lerroa             | Benetako kostuen erregistroa GIDA           | Benetakoa                            |                          |
| Denbora-sarreren erregistroa GIDA       | Denbora-sarrera               | Benetako kostuen erregistroa GIDA           | Benetakoa                            |                          |
| Faktura sortzea             | Denbora-sarreren erregistroa GIDA   | Denbora-sarrera                        | Fakturaren lerroaren transakzioak GIDA     | Fakturaren lerroaren transakzioak |
| Kutxako liburuaren lerroaren erregistroa GIDA     | Kutxako liburuaren lerroa             | Fakturaren lerroaren transakzioak GIDA     | Fakturaren lerroaren transakzioak          |                          |
| Faktura berrespena         | Fakturaren lerroa GIDA        | Fakturaren lerroa                      | Fakturatutako salmenten erregistroa GIDA          | Benetakoa                   |
| Faktura GIDA                 | Faktura                  | Fakturatutako salmenten erregistroa GIDA          | Benetakoa                            |                          |
| Fakturaren lerroaren xehetasunak GIDA     | Fakturaren lerroaren xehetasunak      | Fakturatutako salmenten erregistroa GIDA          | Benetakoa                            |                          |
| Denbora-sarreren erregistroa GIDA       | Denbora-sarrera               | Fakturatutako salmenten erregistroa GIDA          | Benetakoa                            |                          |
| Kutxako liburuaren lerroaren erregistroa GIDA     | Kutxako liburuaren lerroa             | Fakturatutako salmenten erregistroa GIDA          | Benetakoa                            |                          |
| Denbora-sarreren erregistroa GIDA       | Denbora-sarrera               | Fakturatu gabeko salmenten itzulera GIDA      | Benetakoa                            |                          |
| Kutxako liburuaren lerroaren erregistroa GIDA     | Kutxako liburuaren lerroa             | Fakturatu gabeko salmenten itzulera GIDA      | Benetakoa                            |                          |
| Faktura-zirriborroen zuzenketa     | GIDA ILD zaharra             | Fakturaren lerroaren transakzioak          | IDL GIDAren zuzenketa               | Fakturaren lerroaren transakzioak |
| IL GIDA zaharra                  | Fakturaren lerroa             | IDL GIDAren zuzenketa               | Fakturaren lerroaren transakzioak          |                          |
| GIDA faktura zaharra             | Faktura                  | IDL GIDAren zuzenketa               | Fakturaren lerroaren transakzioak          |                          |
| Denbora-sarreren erregistroa GIDA       | Denbora-sarrera               | IDL GIDAren zuzenketa               | Fakturaren lerroaren transakzioak          |                          |
| Kutxako liburuaren lerroaren erregistroa GIDA     | Kutxako liburuaren lerroa             | IDL GIDAren zuzenketa               | Fakturaren lerroaren transakzioak          |                          |
| Berretsitako faktura zuzenketa | GIDA ILD zaharra             | Fakturaren lerroaren transakzioak          | Itzulitako fakturatutako salmenten benetako GIDA | Benetakoa                   |
| IL GIDA zaharra                  | Fakturaren lerroa             | Itzulitako fakturatutako salmenten benetako GIDA | Benetakoa                            |                          |
| GIDA faktura zaharra             | Faktura                  | Itzulitako fakturatutako salmenten benetako GIDA | Benetakoa                            |                          |
| Denbora-sarreren erregistroa GIDA       | Denbora-sarrera               | Itzulitako fakturatutako salmenten benetako GIDA | Benetakoa                            |                          |
| Kutxako liburuaren lerroaren erregistroa GIDA     | Kutxako liburuaren lerroa             | Itzulitako fakturatutako salmenten benetako GIDA | Benetakoa                            |                          |
| GIDA ILD zaharra                 | Fakturaren lerroaren transakzioak | Fakturatu gabeko bentako salmenta berrien GIDA    | Benetakoa                            |                          |
| IL GIDA zaharra                  | Fakturaren lerroa             | Fakturatu gabeko bentako salmenta berrien GIDA    | Benetakoa                            |                          |
| GIDA faktura zaharra             | Faktura                  | Fakturatu gabeko bentako salmenta berrien GIDA    | Benetakoa                            |                          |
| Denbora-sarreren erregistroa GIDA       | Denbora-sarrera               | Fakturatu gabeko bentako salmenta berrien GIDA    | Benetakoa                            |                          |
| Kutxako liburuaren lerroaren erregistroa GIDA     | Kutxako liburuaren lerroa             | Fakturatu gabeko bentako salmenta berrien GIDA    | Benetakoa                            |                          |
| IDL GIDAren zuzenketa          | Fakturaren lerroaren transakzioak | Fakturatu gabeko bentako salmenta berrien GIDA    | Benetakoa                            |                          |
| Zuzenketa IL GIDA           | Fakturaren lerroa             | Fakturatu gabeko bentako salmenta berrien GIDA    | Benetakoa                            |                          |
| GIDA fakturaren zuzenketa      | Faktura                  | Fakturatu gabeko bentako salmenta berrien GIDA    | Unekoa"                            |                          |


Ondorengo ilustrazioak hainbat ekitalditan errealen eta haien iturrien artean sortzen diren estekak erakusten ditu Project Operations-en denbora-sarreren adibidea erabiliz.

> ![Errealak nola lotzen diren iturburu-erregistroekin Project Operations-en.](media/TransactionOrigins.png)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
