---
title: Lotu benetako datuak jatorrizko erregistroekin
description: Gai honetan azaltzen da nola lotu errealak jatorrizko erregistroekin, hala nola denbora sartzearekin, gastuen sarrerarekin edo materialaren erabilera erregistroekin.
author: rumant
ms.date: 03/25/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b5a70d2c2b3f98028b4e4998ed25ab73a275c66e4b8137eb573b943658a1a41e
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6991741"
---
# <a name="link-actuals-to-original-records"></a>Lotu benetako datuak jatorrizko erregistroekin

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_


Dynamics 365 Project Operations-en , *negozio-transakzioa* entitate batek ordezkatzen ez duen kontzeptu abstraktua da. Hala ere, zenbait entitateren eremu eta prozesu komun batzuk negozio-transakzioen kontzeptua erabiltzeko diseinatuta daude. Entitate hauek kontzepturako erabiltzen dira:

- Eskaintzaren lerroaren xehetasunak
- Kontratuaren lerroaren xehetasunak
- Aurreikuspenaren lerroak
- Kutxako liburuaren lerroak
- Benetakoak

Entitate horien artean, **Eskaintzaren lerroaren xehetasunak**, **Kontratuaren lerroaren xehetasunak** eta **Aurreikuspen lerroak** proiektuaren bizitza zikloan zenbatetsitako fasera sailkatzen dira. **Kutxako liburuaren lerroak** eta **Benetako datuak** proiektuaren exekuzio-fasean kokatzen dira.

Project Operations-ek bost entitate horietako erregistroak negozio-transakzio gisa ezagutzen ditu. Bereizketa bakarra zera da: zenbatespen fasera esleitutako entitateetako erregistroak finantza-aurreikuspen gisa hartzen direla, eta, exekuzio fasean esleitzen diren entitateetako erregistroak dagoeneko gertatu diren gertaera ekonomikoak direla.

## <a name="concepts-that-are-unique-to-business-transactions"></a>Negozio-transakzioetarako soilik diren kontzeptuak
Kontzeptu hauek negozio-transakzioen kontzeptuarentzat bakarrak dira:

- Transakzio mota
- Transakzio-klasea
- Transakzioaren jatorria
- Transakzio-konexioa

### <a name="transaction-type"></a>Transakzio mota

Transakzio motak proiektu baten finantza-eraginaren denbora eta testuingurua adierazten ditu. Aukera multzo batek adierazten du, Project Operations-en onartutako balio hauek dituena:

  - Kostua
  - Proiektu-kontratua
  - Fakturatu gabeko salmentak
  - Fakturatutako salmentak
  - Erakunde arteko salmentak
  - Baliabidearen unitate-kostua

### <a name="transaction-class"></a>Transakzio-klasea

Transakzio klaseak proiektuetan sortzen diren kostu mota ezberdinak adierazten ditu. Aukera multzo batek adierazten du, Project Operations-en onartutako balio hauek dituena:

  - Denbora
  - Gastua
  - Materiala
  - Tasa
  - Mugarria
  - Zergak

**Mugarria** negozioaren logikak Project Operations-en prezio finkoa fakturatzeko erabiltzen du.

### <a name="transaction-origin"></a>Transakzioaren jatorria

**Transakzioaren jatorria** negozio-transakzio bakoitzaren jatorria gordetzen duen entitatea da. Proiektu bat abian jarri ahala, negozio-transakzio bakoitzak beste negozio-transakzio bat sortuko du eta horrek beste bat sortuko du. Transakzioaren jatorria entitatea transakzio bakoitzaren jatorriari buruzko datuak gordetzeko diseinatuta dago, txostenak eta trazabilitatea laguntzeko. 

### <a name="transaction-connection"></a>Transakzio-konexioa

**Transakzioaren konexioa** antzeko negozioen arteko bi negozioren arteko erlazioa gordetzen duen entitatea da, hala nola, kostuen eta erlazionatutako salmenten egiazkoak edo fakturazio-jarduerek eragindako transakzioen itzulketak.

Elkarrekin, **Transakzioaren jatorria** eta **Transakzioen konexioa** erakundeek negozio-transakzio jakin bat eragiten duten ekintzen eta negozioen arteko harremanak kontrolatzen lagunduko dizute.

### <a name="example-how-transaction-origin-works-with-transaction-connection"></a>Adibidea: transakzioaren jatorria nola funtzionatzen duen transakzioarekin

Hurrengo adibidean Project Operations proiektuaren bizi-zikloko denbora sarreren prozesaketa tipikoa erakusten da.

> ![Prozesatzeko denbora Project Service-en bizi-zikloaren itxiera da.](media/basic-guide-17.png)
 
1. Garai bateko sarrera bidaltzeak kutxako liburuaren bi lerro sortzea eragiten du: bata kostuen lerroa eta besterik gabeko salmenten lerroa.
2. Garai bateko sarrera onartzeak benetako bi datu sortzen ditu: bata benetako kostuetarako eta besterik gabeko benetako salmentarako.
3. Erabiltzaileak proiektuaren faktura berria sortzen duenean, fakturen lerroko transakzioa fakturatu gabeko salmenten egiazko datuak erabiliz sortzen da. 
4. Faktura baieztatzen duzunean, fakturatutako bi benetako datu sortzen dira: fakturatu gabeko benetako itzulerak eta fakturatutako salmenta erreal berria sortzen da.

Gertaera horietako bakoitzak erregistro bat sortzen du **Transakzioaren jatorria** eta **Transakzio konexioa** entitateak. Erregistro berri hauek denbora sarrera, aldizkari lerroa, benetakoak eta faktura lerroaren xehetasunetan sortzen diren erregistroen arteko harremanen historia eraikitzen laguntzen dute.

Hurrengo taulan, aurreko lan-fluxuaren **Transakzioaren jatorria** entitateko erregistroak agertzen dira.

| Gertaera                        | Jatorria                   | Jatorri mota                       | Transakzioa                       | Transakzio mota         |
|------------------------------|--------------------------|-----------------------------------|-----------------------------------|--------------------------|
| Denbora-sarreraren bidalketa        | Denbora-sarreren erregistroa GIDA   | Denbora-sarrera                        | Kutxako liburuaren lerroaren erregistroa GIDA (kostua)   | Kutxako liburuaren lerroa             |
| Denbora-sarreren erregistroa GIDA       | Denbora-sarrera               | Kutxako liburuaren lerroaren erregistroa GUIDA (salmentak)  | Kutxako liburuaren lerroa                      |                          |
| Orduaren onarpena                | Kutxako liburuaren lerroaren erregistroa GIDA | Kutxako liburuaren lerroa                      | Fakturatu gabeko salmenten erregistroa GIDA        | Benetakoa                   |
| Denbora-sarreren erregistroa GIDA       | Denbora-sarrera               | Fakturatu gabeko salmenten erregistroa GIDA        | Benetakoa                            |                          |
| Kutxako liburuaren lerroaren erregistroa GIDA     | Kutxako liburuaren lerroa             | Benetako kostuen erregistroa GIDA           | Benetakoa                            |                          |
| Denbora-sarreren erregistroa GIDA       | Denbora-sarrera               | Benetako kostuen erregistroa GIDA           | Unekoa"                            |                          |
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
| GIDA fakturaren zuzenketa      | Faktura                  | Fakturatu gabeko bentako salmenta berrien GIDA    | Benetakoa                            |                          |

Hurrengo taulan, aurreko lan-fluxuaren **Transakzioaren konexioa** entitateko erregistroak agertzen dira.

| Gertaera                          | 1. transakzioa                 | 1. transakzioaren funtzioa | 1. transakzioaren mota           | 2. transakzioa                | 2. transakzioaren funtzioa | 2. transakzioaren mota |
|--------------------------------|-------------------------------|--------------------|------------------------------|------------------------------|--------------------|--------------------|
| Denbora-sarreraren bidalketa          | Kutxako liburuaren lerroa GUIDA (salmentak)     | Fakturatu gabeko salmentak     | msdyn_journalline            | Kutxako liburuaren lerroa GIDA (kostua)     | Kostua               | msdyn_journalline  |
| Orduaren onarpena                  | Fakturatu gabeko benetakoak (salmentak) GIDA  | Fakturatu gabeko salmentak     | msdyn_actual                 | Benetako kostua (kostua) GIDA       | Kostua               | msdyn_actual       |
| Faktura sortzea               | Fakturaren lerroaren xehetasunak GIDA      | Fakturatutako salmentak       | msdyn_invoicelinetransaction | Fakturatu gabeko benetakoak GIDA   | Fakturatu gabeko salmentak     | msdyn_actual       |
| Faktura berrespena           | Benetako GIDA itzultzea         | Itzultzea          | msdyn_actual                 | Jatorrizko fakturatu gabeko salmentak GIDA | Jatorrizkoa           | msdyn_actual       |
| Fakturatutako salmentak GIDA              | Fakturatutako salmentak                  | msdyn_actual       | Fakturatu gabeko benetakoak GIDA   | Fakturatu gabeko salmentak               | msdyn_actual       |                    |
| Faktura-zirriborroen zuzenketa       | Fakturaren lerroaren transakzioak GIDA | Ordezkapena          | msdyn_invoicelinetransaction | Fakturatutako salmentak GIDA            | Jatorrizkoa           | msdyn_actual       |
| Berretsi faktura zuzenketa     | Fakturatutako salmenten itzulera GIDA    | Itzultzea          | msdyn_actual                 | Fakturatutako salmentak GIDA            | Jatorrizkoa           | msdyn_actual       |
| Fakturatu gabeko bentako salmenta berrien GIDA | Ordezkapena                     | msdyn_actual       | Fakturatutako salmentak GIDA            | Jatorrizkoa                     | msdyn_actual       |                    |


[!INCLUDE[footer-include](../includes/footer-banner.md)]
