---
title: Transakzioaren jatorria - Lotu benetako datuak iturburuarekin
description: Gai honetan azaltzen da nola lotzeko errealak jatorrizko iturburuko erregistroekin erabiltzen den transakzioen jatorriaren kontzeptua, hala nola denbora sartzearekin, gastuen sarrerarekin edo materialaren erabilera erregistroekin.
author: rumant
ms.date: 03/25/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: f1beff392ddd449a930d38016ca6083fea97953b
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8921287"
---
# <a name="transaction-origins---link-actuals-to-their-source"></a>Transakzioaren jatorria - Lotu benetako datuak iturburuarekin

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Transakzioen jatorri-erregistroak benetakoak beren iturriarekin lotzeko sortzen dira, hala nola, denbora-sarrerak, gastu-sarrerak, materialaren erabilera-erregistroak eta proiektuaren fakturak.

Hurrengo adibidean Project Operations proiektuaren bizi-zikloko denbora sarreren prozesaketa tipikoa erakusten da.

> ![Project Operations-en denbora-sarrerak prozesatzea.](media/basic-guide-17.png)
 
1. Garai bateko sarrera bidaltzeak kutxako liburuaren bi lerro sortzea eragiten du: bata kostuetarako eta besterik gabeko salmentarako.
2. Garai bateko sarrera onartzeak benetako bi datu sortzea eragiten du: bata kostuetarako eta besterik gabeko salmentarako.
3. Erabiltzaileak proiektuaren faktura sortzen duenean, fakturen lerroko transakzioa fakturatu gabeko salmenten egiazko datuak erabiliz sortzen da.
4. Faktura baieztatzen duzunean, fakturatutako bi benetako datu sortzen dira: fakturatu gabeko itzulerak eta fakturatutako salmenta erreal berria sortzen da.

Lan-fluxua prozesatzeko gertaera hauetako bakoitzak erregistroak sortzea eragiten du Transakzioaren jatorrizko entitatean, denboraren sarreran, kutxako liburuaren lerroan, egunkarietan eta fakturen lerroko xehetasunetan sortzen diren erregistro horien arteko erlazioen arrastoa eraikitzen laguntzeko.

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


Ondorengo ilustrazioak hainbat gertaeratan erreal mota ezberdinen artean sortzen diren estekak erakusten ditu Project Operations-eko denbora-sarreren adibidea erabiliz.

> ![Errealak nola lotzen diren iturburu-erregistroekin Project Operations-en.](media/TransactionOrigins.png)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
