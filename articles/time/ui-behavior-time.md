---
title: Denbora sartzeko UI portaera
description: Gai honek Denbora-sarreraren EIren portaerari buruzko informazioa ematen du.
author: stsporen
manager: AnnBe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 86f805cd33f81e70bf9ae3c1fb20a1c310473604
ms.sourcegitcommit: 2cf93d8bf0be5b61a739195a41334c34d910e9ba
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/05/2020
ms.locfileid: "3961679"
---
# <a name="time-entry-ui-behavior"></a>Denbora sartzeko UI portaera

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_


**Asteko denbora-sarrera** sareta berria kontrol pertsonalizatua da, eta bi atal nagusi ditu: **Neurriak** eta **Iraupena**.

## <a name="dimensions"></a>Dimentsioak
**Neurriak** sekzioak denboraren aurka sartu daitezkeen dimentsio guztiak erakusten ditu. Hauek dira onartzen diren neurri integratuak:

  - Project
  - Proiektuaren zeregina
  - Funtzioa
  - Mota
  - Sarreraren egoera

**Neurriak** sekzioak ez du lineako edizioa onartzen. Sekzio honek eremu pertsonalizatuak asteroko denbora-sarreraren saretan gehitzeko aukera ematen duen ikuspegiaren babesa du.

## <a name="duration"></a>Iraupena
Iraupena sekzioak asteko egunak zutabeetako goiburu gisa erakusten ditu. Sekzio honek lineako edizioa ahalbidetzen du. Neurri egokiak dituen denbora-sarreraren errenkada bat sortu ondoren, erabiltzaileek azkar sar dezakete linean neurri horietan igarotzen duten denbora.

## <a name="create-a-new-time-entry"></a>Sortu beste denbora-sarrera bat

1. Asteroko denbora-sarreraren saretan, hautatu **Berria**. 
2. **Denbora-sarrera azkar sortzeko** elkarrizketa-koadroan, hautatu ordua sartzeko data.
3. Idatzi datuak **Proiektua**, **Proiektuaren zeregina**, **Rola** eta **Iraupena** dimentsioak. Informazio hori minututan, ordutan edo egunetan gehitu behar da idatziz **h**, **m** edo **e**, zenbakiarekin batera. 
4. Kanpokoekin partekatu daitezkeen denbora-sarreraren deskribapenak eta iruzkinak ere sar ditzakete. 

Sarrera gordetzean, sartutako balioak agertzen dira **Neurriak** sekzioan. **Iraupena** eremuan idatzitako informazioa denbora-sarrera sortu zen datan agertzen da.

Sistemaren ikuspegiek bilatze-eremuak babesten dituzte. Adibidez, erabiltzaile bat proiektu batean sartu ondoren, **Proiektuaren zeregina** eremuan **Kopia** ikuspegi gisa ezarrita dago lehenespenez. Erabiltzaile bati esleitu ez zaizkion zereginetarako denbora-sarrerak sortzeko, hautatu **Aldatu ikuspegia** bilaketaren elkarrizketa-koadroan eta, ondoren, hautatu **Proiektu aktiboko zeregin guztiak** ikuspegia.

## <a name="edit-a-time-entry"></a>Editatu denbora-sarrera 
Denbora-sarrera orrialdeko eremu batzuetako xehetasunak, adibidez **Deskribapena** eta **Kanpoko iruzkinak**, ez dira asteroko denbora-sarreraren saretan agertzen. Horren ordez, xehetasun osagarri horiek dituen hiruki adierazle txiki bat agertzen da **Iraupena** gelaxketan. 

1. Denbora sarrera bat editatzeko, hautatu eguneratu nahi duzun gelaxka.
2. Aukeratu **Editatu xehetasunak** fitxategian datuak eguneratzeko **Denbora sartzeko inprimaki nagusia** panelean. 

## <a name="copy-a-time-entry-row"></a>Kopiatu denbora-sarreraren errenkada bat
Errenkada sortu ondoren, **Kopiatu errenkada** aukera dezakezu errenkada osoa errenkada berri batean kopiatzeko. Errenkada bat modu horretan kopiatzean, neurriak eta iraupenak ere kopiatzen dira. **Editatu errenkada** ere aukera dezakezu neurrien balioak eta iraupenen eguneratzeko **Iraupena** sekzioan.

## <a name="open-a-time-entry-behavior"></a>Ireki denbora-sarreraren portaera
Eremu garrantzitsuenetan sarrera egokiak eta azkarrak onartzeko, asteko denbora-sarreraren saretak hautatutako neurrien eta denboraren iraupenaren azpimultzoa erakusten du. Denbora-sarrera bakarraren xehetasun guztiak ikusteko, **Editatu sarrera** atalean, hautatu **Ireki**.

## <a name="submit-a-time-entry"></a>Bidali denbora-sarrera bat
Denbora-sarrera bakar bat edo denbora-sarreren talde bat bidal dezakezu gelaxka bloke bat edo denbora-sarrera errenkada oso bat aukeratuz eta, ondoren, **Bidali** hautatuta. Bidalitako denbora-sarrerak onesteko zain dauden sarrera gisa agertzen dira onartzailearen **Onespena** orrian. Denbora-sarrerak bidali ondoren, ezin dira editatu.

## <a name="recall-a-time-entry"></a>Berreskuratu denbora-sarrera bat
Bidali dituzun denbora-sarrerak berreskura ditzakezu. Denbora-sarrera bakarra, denbora-arreren bloke bat edo denbora-sarreren errenkada oso bat berreskuratu dezakezu. Gogoratutako denbora-sarrerak editatu daitezke.

## <a name="time-entry-status"></a>Denbora-sarreraren egoera

- **Zirriborroa**: Denbora-sarrera berriei automatikoki esleitzen zaie **Zirriborroa** egoera. **Zirriborroa** egoera duten denbora-sarrerak soilik ezaba daitezke.
- **Bidalita**:Denbora-sarrera bidaltzen denean, **Bidalita** egoerara eguneratzen da. 
- **Onartuta**: Bidalitako denbora-sarrera onartzen denean, **Onartuta** egoerara eguneratzen da. 
- **Itzulita**: Denbora-sarrera onartzen ez bada, **Itzulita** egoera eguneratuko da, eta sarrera eskuragarri egongo da zuzentzeko eta berriz bidaltzeko. 

## <a name="view-rejection-comments"></a>Ikusi baztertze-iruzkinak
Onartzaile batek denbora-sarrera bat baztertzen duenean, onartzaileak iruzkinak gehitu ditzake baliabideak baztertzearen zergatia uler dezan. Denbora-sarrera baten baztertze-iruzkinak ikusteko, hautatu **Ireki sarrera**. Baztertze-iruzkinak kronologian erakutsiko dira. Erabiltzaileak sarrera berriro bidali aurretik erantzun diezaieke uko egiteko iruzkinei.

## <a name="copy-week"></a>Kopiatu astea
Denbora sarrera batzuk sortu ondoren, erabiltzaileek aldi berean hainbat sarrera sor ditzakete.

1. **Denbora-sarrerak** inprimakian, hautatu **Kopiatu astea** denbora sarrera osagarriak modu masiboan sortzeko. 
2. **Kopiatu** elkarrizketa-koadroan, **Aldi honetatik** sekzioan, erabili **Hasiera-data** eta **Amaiera-data** eremuak denbora-sarrerak kopiatu behar diren data-tartea zehazteko. 
3. **Aldira** atalean, **Hasiera data** eremuan, zehaztu zein datarako sortu nahi dituzun sarrerak. 
4. Aukeratu **Kopiatu**. **Aldira arte** aldian zehaztutako datarako, **Hasierako aldia** dagokion asteko egunerako denbora-sarreren kopia sortzen da. Adibidez, asteleheneko pasa den asteko denbora-sarrera **Amaierako aldia** zehazten den asteko astelehenean kopiatzen da.

## <a name="import"></a>Inportatu
Oinarrizko prozesu bera erreserbetatik, zereginetatik eta trukeetatik inportatzeko erabiltzen da. Inportatuko diren erreserben data zehaztu dezakezu eta, ondoren, modu esplizituan hautatu behar dira zirriborroen denbora-sarrerak gisa sortu behar diren erreserbak. 
