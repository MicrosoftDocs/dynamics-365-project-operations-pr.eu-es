---
title: Egin lan proiektuetan oinarritutako kontratuaren lerroekin
description: Gai honek proiektuan oinarritutako kontratu lerroei buruzko informazioa eskaintzen du.
author: rumant
ms.date: 10/28/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: c1c935a998cba8bd42ba2f11c8310d41e72de94adac7c2cb83f4c7224127b10b
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6990031"
---
# <a name="work-with-projectbased-contract-lines"></a>Egin lan proiektuetan oinarritutako kontratuaren lerroekin

Dynamics 365 Project Operations proiektuan oinarritutako kontratu lerroak proiektu batean egindako lanen osagai zehatzen aurrekontua eta fakturazio akordioak atxikitzeko diseinatuta daude. Proiektuan oinarritutako kontratu lerroaren egitura proiektuaren kalkuluen eta fakturazio eszenatokietarako hedatzen da, honako kontzeptu hauekin:

- Fakturazio-metodoa
- Proiektuen eta zereginen esleipena
- Transakzio klaseak barne
- Ez gainditzeko muga
- Aplikagarritasun konfigurazioa
- Aurrekontuak kontratuaren lineako xehetasunak erabiliz
- Kontratuaren lerroaren bezeroa

Ondorengo eremuak **Orokorra** proiektuan oinarritutako kontratu lerroen fitxa. Eremu horiek oinarrizko zehaztapen zehatza eta proiektuan oinarritutako lanen fakturazio antolamenduak finkatzen laguntzen dute.

| Eremua | Deskribapena | Downstream eragina |
| --- | --- | --- |
| **Izena** | Kontratuaren lerroaren izenak kalkulatzen ari den kontratuaren osagai diskretua identifikatzen du. Aurrekontu batetik sortutako proiektu kontratu baterako, balio hori proiektuan oinarritutako aurrekontu lerroaren dagokion balio batetik kopiatzen da. | Eremuaren balioa sortzen denean kontratu lerro honetatik sortzen den proiektuaren faktura lerroan kopiatutako izena. |
| **Fakturazio-metodoa** | Aurrekontu batetik sortutako proiektu kontratu baterako, aurrekontuaren lerroaren dagokion balio batetik kopiatzen da. Hau da aukera multzo, Project Operations-ek onartzen dituzten bi kontratazio eredu nagusiak adierazten dituena:</br>- **Prezio finkoa**</br>- **Denbora eta materiala** | Aipatutako kontratu lerroaren fakturazio metodoan oinarrituta, benetako transakzioa prozesatuko da. Benetakoak aipatzen duen kontratu lerroak denbora eta materiala fakturatzeko metodoa badu, kostuen eta fakturatu gabeko salmenten benetako erregistroa sortzen da. Benetakoak aipatzen duen kontratu-lerroak prezio finkoko fakturazio-metodoa badu, benetako kostua soilik sortzen da. |
| **Project** | Erabili eremu hau konpromiso horretan lana emateko erabiliko den proiektua identifikatzeko. | Eremu honetako balio hau honekin batera erabiliko da **Zereginak barne** eta **Barne transakzio klaseak** eremuak kontratu-lerroaren erreferentzia benetako edo aurrekontuko lerro erregistro batean ebazteko. |
| **Idatzi denbora** | Bandera batek hautatutako proiektuaren denborako transakzioak edo lan kostuak kontratu linea honetan sartu diren adierazten du. **Ez** balioak kontratuaren lerroan sartzen ez diren denbora-transakzioak edo kostuak adierazten du. **Bai** balioak egingo dutela adierazten du. | Eremu hau honekin batera erabiliko da proiektua kontratu-lerroaren erreferentzia benetako edo aurrekontuko lerro erregistro batean ebazteko. |
| **Idatzi gastua** | Bandera batek hautatutako proiektuaren kostuak kontratu linea honetan sartuko diren adierazten du. **Ez** balioak kontratuaren lerroan sartzen ez diren gastuen kostuak adierazten du. **Bai** balioak egingo dutela adierazten du. | Eremu hau honekin batera erabiliko da proiektua kontratu-lerroaren erreferentzia benetako edo aurrekontuko lerro erregistro batean ebazteko. |
| **Idatzi prezioa** | Bandera batek hautatutako proiektuaren zergak kontratu linea honetan sartuko diren adierazten du. **Ez** balioak kontratuaren lerroan sartzen ez diren zergak adierazten du. **Bai** balioak egingo dutela adierazten du. | Eremu hau honekin batera erabiliko da proiektua kontratu-lerroaren erreferentzia benetako edo aurrekontuko lerro erregistro batean ebazteko. |
| **Kontratatutako zenbatekoa** | Prezio finkoko kontratu lerroan, hori bezeroari fakturatuko zaion hitzarmenaren balioa da, kontratu lerro honi lotutako lan osagai guztiengatik. Denboraren eta materialaren kontratuaren lerroan, zenbateko hori bezeroari fakturatuko zaion aurreikusitako balioa da, kontratu lerro honi lotutako lan osagai guztiengatik. Aurrekontu batetik sortutako proiektu kontratu baterako, aurrekontuaren lerroaren dagokion balio batetik kopiatzen da. Proiektuan oinarritutako kontratu lerro batek lerroaren xehetasunak dituenean, eremu hau blokeatuta dago editatzeko eta kontratuaren lerroaren xehetasunen zenbatekoaren arabera laburbiltzen da. | Kontratu-lerroak lerroaren xehetasunak dituenean, balio hori alda daiteke lerroaren xehetasunen zenbatekoak aldatuta. Prezio finkoko kontratu lerroan, balio hori aldizkako fakturazio mugarrien gaineko zerga aurretik zenbatekoa sortzeko erabiltzen da. |
| **Aurreikusitako zerga** | Erabiltzaileak eremu hau alda dezake, aurreikusitako zergaren zenbatekoa kontratu lerroan sartzeko. Proiektuan oinarritutako kontratu lerro batek lerroaren xehetasunak dituenean, eremu hau blokeatuta dago editatzeko eta kontratuaren lerroaren xehetasunen zerga-zenbatekoaren arabera laburbiltzen da. | Kontratu-lerroak lerroaren xehetasunak dituenean, balio hori alda daiteke lerroaren xehetasunen zerga-zenbatekoak aldatuta. Prezio finkoko kontratu lerroan, balio hori aldizkako fakturazio mugarrien gaineko zerga sortzeko erabiltzen da. |
| **Kontratatutako zenbatekoa, zergaren ondoren** | Kontratatuaren lerroaren zenbatekoa zergaren ondoren. Eremu hau irakurtzeko soilik da eta honela kalkulatzen da **Kontratatutako zenbatekoa + Zerga**. | Prezio finkoko kontratu lerroan, balio hori aldizkako fakturazio mugarriak sortzeko erabiltzen da. |
| **Ez gainditzeko muga** | Erabiltzaileak eremu hau edita dezake eta fakturazio metodoa denbora eta materialaren fakturazio-metodo gisa ezarrita duten proiektuetan oinarritutako kontratu lerroetan bakarrik dago erabilgarri. | Erabiltzaileak eremu hau edita dezake. Denboraren edo benetako datuen gastuez egindako benetako batek kontratu-lerro hau denboraz eta materialez aipatzen duenean, benetako zenbatekoa kontratu-lerroan gainditu ezin den mugaren arabera ebaluatzen da. |
| **Bezeroaren aurrekontua** | Eremu hau editagarria da eta aurrekontuaren lerroaren dagokion balio batetik kopiatzen da kontratua eskaintza batetik sortu bada. | Eremu hau informaziorako bakarrik erabiltzen da eta ez du beheranzko esangurarik. |

## <a name="validation-rule-for-the-options-on-the-general-tab-of-project-based-contract-lines"></a>Proiektuetan oinarritutako kontratu lerroaren Orokorreko fitxako aukeren baliozkotze arauak

Araua: Proiektu bat eta transakzio klase jakin bat proiektuan oinarritutako kontratu lerro batean bakarrik sar daitezke kontratuan.

| Kontratua | Kontratuaren lerroa | Project | Idatzi denbora | Idatzi gastua | Idatzi prezioa | Baliozkoa/Baliogabea da | Arrazoia                                                                                                                                                                                                  |
|----------|---------------|---------|--------------|-----------------|-------------|-----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| C1       | CL1           | A1      | Yes          | Yes             | Yes         | Baliogabea da       | Araua urratzen du. P1 proiektuaren denbora, gastua eta tasak kontratuaren linea bietan, CL1 eta CL2 barne daude.                                                                                       |
| C1       | CL2           | A1      | Yes          | Yes             | Yes         | Baliogabea da       | Araua urratzen du. P1 proiektuaren denbora, gastua eta tasak kontratuaren linea bietan, CL1 eta CL2 barne daude.                                                                                       |
| C1       | CL1           | A1      | Yes          | +Ez              | Yes         | Baliogabea da       | Araua urratzen du. P1 proiektuaren denbora eta tasak kontratuaren linea bietan, CL1 eta CL2 barne daude.                                                                                                   |
| C1       | CL2           | A1      | Yes          | Yes             | Yes         | Baliogabea da       | Araua urratzen du. P1 proiektuaren denbora eta tasak kontratuaren linea bietan, CL1 eta CL2 barne daude.                                                                                                   |
| C1       | CL1           | A1      | Yes          | +Ez              | Yes         | Baliozkoa           | P1 proiektuaren denbora eta tasak CL1ean sartzen dira. P1 proiektuaren gastuak QL2n sartzen dira. </br>   Kontratu lerro bakoitzean sartzen den horretan ez dago gainjartzerik eta, beraz, balio du.  |
| C1       | CL2           | A1      | +Ez           | Yes             | +Ez          | Baliozkoa           | P1 proiektuaren denbora eta tasak CL1ean sartzen dira. P1 proiektuaren gastuak QL2n sartzen dira. </br>   Kontratu lerro bakoitzean sartzen den horretan ez dago gainjartzerik eta, beraz, balio du.  |
| C1       | CL1           | A1      | Yes          | Yes             | Yes         | Baliogabea da       | Araua urratzen du. P1 proiektuaren denbora, gastua eta tasak kontratuaren linea bietan, bi kontratuetan daude.                                                                                               |
| CL2      | CL2           | A1      | Yes          | Yes             | Yes         | Baliogabea da       | Araua urratzen du. P1 proiektuaren denbora, gastua eta tasak kontratuaren linea bietan, bi kontratuetan daude.                                                                                               |


[!INCLUDE[footer-include](../includes/footer-banner.md)]