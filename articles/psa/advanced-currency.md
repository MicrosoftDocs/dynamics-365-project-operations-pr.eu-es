---
title: Dibisa anitzeko agertokiak (3.x bertsioa)
description: Gai honek dibisa anitzeko agertokiei buruzko informazioa ematen du.
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 12/26/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 89a91cf3dbbcf81dbb089ee88c8c177c73afb694914ca7d95eae96776d38abed
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "7005106"
---
# <a name="multiple-currency-scenarios"></a>Dibisa anitzeko gertaerak

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Microsoft Dynamics 365 dibisa bi kontzeptu ditu:

- **Transakzio-dibisa**: transakzio bat gertatzen den dibisa. 
- **Oinarrizko dibisa**: Dynamics 365 instantziaren dibisa. Dibisa hau Dynamics 365 instantzia hornitzen denean konfiguratzen da. Ezin da aldatu.

Adibidez, Contoso US-ek 100 kamiseta saldu zizkieten Erresuma Batuko bezero bati, 15 euroko esterlina (GBP) bakoitzeko. Hurrengo taulan, transakzio hau nola erregistratu den eskaera produktuaren entitatean agertzen da.

| Produktua | Kopurua | Prezioa unitate bakoitzeko | Moneta | Zenbatekoa | Kanbio-tasa | Prezioa unitate bakoitzeko (oinarrizkoa)| Zenbatekoa (oinarrizkoa)|
|---------|----------|----------------|----------|--------|---------------|----------------------|--------------|
| Kamiseta | 100      | 15             | GBP      | 1500   | 0.94          | $17.25               | $1,725       |

**Dibisa** zutabeak transakzioaren dibisa erakusten du, salmenta gertatu den dibisa. **Kanbio-tasa** zutabea transakzio-dibisa eta oinarrizko dibisaren arteko kanbio-tasa da. Estatu Batutako oinarrizko dibisa dolarra da (USD). Oinarri hau Dynamics 365 instantzia hornitzen denean konfiguratu zen.
Taulak erakusten duen moduan, transakzio bakoitza transakzio-dibisan eta oinarrizko dibisan erregistratzen da. Dynamics 365-ek dibisa kanbio-tasa erabiltzen du oinarrizko dibisaren zenbatekoak kalkulatzeko.

## <a name="project-service-automation-extensions"></a>Project Service Automation-en luzapenak

Dynamics 365 Project Service Automation -ek transakzioaren dibisan eragina du, negozio-transakzioek bi alderdi izan ohi baitituzte: kostua eta salmentak.

Erakunde hauek negozio-eragiketzat hartzen dira:

- Eskaintzaren lerroaren xehetasunak
- Proiektu-kontratuaren lerroaren xehetasunak
- Aurreikuspenaren lerroa
- Kutxako liburuaren lerroa
- Fakturaren lerroaren xehetasunak
- Benetakoa

Entitate horietako bakoitzean, kostua edo salmenten zenbatekoa adierazten duen erregistroa dago. Dynamics 365 erakundea duen edozein entitateren kasuan **Zenbatekoa** eremua, erregistro bakoitzak transakzio-dibisan eta oinarrizko dibisaren zenbatekoak biltzen ditu. 

PSAk transakzio-dibisa kontzeptua kostuen eta salmenten bidez zabaltzen du modu hauetan:

- Denbora eragiketetarako kostu-transakzioaren dibisa proiektua jabea edo kudeatzen duen erakundearen unitatearen monetakoa da. Antolamendu unitate hau kontratazio unitate bezala ezagutzen da.
- Denbora- eta gastu-transakzioen salerosketa-dibisaren proiektuaren kontratuaren monetakoa da beti.
- Gastuen kostu transakzioen dibisaren gastuen sarreran sortu zen monetarengandik dator.

## <a name="multiple-currency-scenario"></a>Dibisa anitzeko gertaera

Atal honetan Contoso UK-k Fabrikam izena duen bezero batentzat entregatzen duen proiektuaren adibidea deskribatzen du. Hona hemen nola ezarri den eszenatokia:

1. GBP eta yen japoniarra (JPY) daude konfiguratuta **Ezarpenak** \> **Negozio-kudeaketa** \> **Dibisak**. 
2. Izena duen bezeroaren kontua **Fabrikam - Japonia** konfiguratuta dago eta JPY hautatuko da kontuko dibisa gisa.
3. Erakunde unitate bat **Contoso UK** konfiguratuta dago eta GBP moneta gisa hautatzen da.
4. Proiektu-kontratua sortzen da, non **Contoso UK** unitate kontratatzaile gisa zehazten den eta **Fabrikam - Japonia** bezero gisa.
5. Proiektu-kontratuaren lerroak sortzen dira, proiektuko transakzio-klaseen fakturazio-antolamenduak oinarritzat hartuta, hala nola denboraren fakturazioa eta gastuen fakturazioa.
6. Proiektu bat sortzen da non **Contoso UK** unitate kontratatzaile gisa zehazten den. Proiektu hau proiektuaren kontratu lerroetara sortu eta mapatzen da.


Eskaintzaren lerroaren xehetasuna, proiektuaren kontratuaren lerroaren xehetasuna edo antolaketaren estimazio lerroan erabiltzen duten kalkuluan, bi erregistro sortzen dira beti entitatean. Erregistro bat kostua da, eta bestea, berriz, salmentarako.

- Berez, kostuaren erregistroko transakzioen dibisa proiektuaren kontratazio unitatearen moneta finkatzen da. Adibide honetan, dibisa GBP da.
- Berez, salmenten erregistroko transakzioen dibisa proiektu-kontratuaren unitatearen moneta finkatzen da. Adibide honetan, dibisa JPY da.

Aktualitateak denboraz edo kutxako liburuaren lerroa erabiliz sortzen direnean, jokabide hau gertatzen da:

- Berez, kostuaren erregistroko transakzioen dibisa proiektuaren kontratazio unitatearen dibisa finkatzen da.
- Berez, salmenten erregistroko transakzioen dibisa proiektu-kontratuaren unitatearen moneta finkatzen da.

Aktualitateak gastuak kutxako liburuaren lerroa erabiliz sortzen direnean, jokabide hau gertatzen da:

- Gastuen zenbatekoa edozein moneta grabatu dezakezu. Aukeratu moneta hautatzailean **Gastu sarrera** orrialdea edo **Kutxako liburuaren lerroa** orria. Berez, kostuen erregistroko transakzioen dibisa gastuen sarrera unitatearen moneta finkatzen da. 
- Berez, salmenten erregistroko transakzioen dibisa proiektu-kontratuaren unitatearen moneta da. Dibisa hau ezartzeko, sistemak transakzioaren zenbatekoa lehenik eta behin erabiltzaileak sartu duen moneta bihurtzen du. Ondoren, zenbatekoa proiektuko kontratuaren moneta bihurtzen du. 

### <a name="computing-roll-ups-when-project-actuals-are-recorded-in-multiple-transaction-currencies"></a>Prozesuen aktualitatea transakzio-moneta askotan erregistratzen denean

Dynamics 365-ek automatikoki kudeatzen ditu diru-kopuruak moneta desberdinetan. Hau da adibide bat.

| Transakzio-klasea | Transakzio mota| Date   | Baliabidea | Transakzio-kategoria | Kopurua | Unitate-prezioa | Zenbatekoa      | Kanbio-tasa | Zenbatekoa oinarrizkoan |
|-------------------|------------------|--------|----------|----------------------|----------|--------------|-------------|---------------|----------------|
| Time              | Fakturatu gabeko salmentak   | 14-eka | Dabid  |                      | 8 h    | 20,000 JPY    | 160,000 JPY | 123           | 1,300.81 USD    |
| Time              | Fakturatu gabeko salmentak   | 15-eka | Dabid  |                      | 8 h    | 20,000 JPY    | 160,000 JPY | 123           | 1,300.81 USD    |
| Gastua           | Fakturatu gabeko salmentak   | 16-eka | Dabid  | Hotela                | 1 ea     | 250 EUR      | 250 EUR     | 0.94          | 265.95 USD     |
| Gastua           | Fakturatu gabeko salmentak   | 17-eka | Dabid  | Auto-alokairua           | 1 ea     | 150 EUR      | 150 EUR     | 0.94          | 159.57 USD     |

Proiektuan fakturatu gabeko salmenten balio osoa kalkulatzeko, bildu eremua sor dezakezu **Zenbatekoa** eremua, fakturatu gabeko salmenten inguruko errealitate guztietan. Bidalitako eremua Dynamics 365-en eraikuntza da, eta horrekin erlazionatutako erregistroetan formulak azkar egiteko aukera ematen du.


[!INCLUDE[footer-include](../includes/footer-banner.md)]