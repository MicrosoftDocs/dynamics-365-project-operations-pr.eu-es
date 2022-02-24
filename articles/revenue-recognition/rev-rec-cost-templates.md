---
title: Konfiguratu kostuen txantiloiak
description: Gai honek Project Operations-en kostuen txantiloiak nola sortu eta erabili informazioa eskaintzen du.
author: sigitac
manager: tfehr
ms.date: 11/18/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 786b2b9b140f82d406044c2ed05761d7f46ee9e0
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642708"
---
# <a name="set-up-cost-templates"></a>Konfiguratu kostuen txantiloiak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_


Gai honek Project Operations-en kostuen txantiloiak nola sortu eta erabili informazioa eskaintzen du. Kostuen txantiloiak zehazten ditu:

- Aurreikuspenen eta benetako transakzioen proiektuen kategoriak proiektuaren amaierako kalkuluaren ehuneko batean sartu behar dira. Ehuneko osoko balioa gero zenbat diru sarrera aitortzen den kalkulatzeko erabiltzen da.
- Amaitzearen ehunekoa alda daitekeen automatikoki kalkulatzen bada.
- Osatutako ehunekoa zenbatekoen edo unitateen arabera kalkulatzen den.

## <a name="cost-template-example"></a>Kostuen txantiloiaren adibidea

Webguneak diseinatzeko proiektu batean ari zara lanean bezeroarentzako. USD 10.000 kuota finkoa kobratzen duzu. Proiektua burutzeko 100 ordu (5.000 USD) beharko direla aurreikusi duzu. Gainera, bi hegazkin txartel eta lau gau hotel batean aurreikusten dituzu bezeroaren gunera joateko (1.800 USD). Horrek guztira aurreikusitako USD 6.800 kostua lortzen du.

Hilaren bukaeran aurrekontua sortzeko prezio finkoko diru-sarrerak ezagutzeko prozesua abiarazten duzunean, proiektuan 35 ordu lan egin dituzula ikusiko duzu. Honek oraindik ez ditu hegaldiak edo hotelaren kostuak barne. Laguntzaile bat ere izan zenuen proiektuaren bost orduko ikerketa burutzeko aurreikusita ez zenuen USD 100 kostuarekin.

Proiektu honen ehuneko balio osoa kalkulatzen duzunean, aukera hauek egin behar dituzu:

- Kostu guztiak (orduak eta gastuak) edo orduak bakarrik sartu nahi dituzu?
- Ordu guztiak edo antolatutako orduak soilik sartu nahi dituzu?
- Osatutako ehunekoa kalkulatu nahi al duzu aurreikusitako orduetako dolarraren kostuaren arabera (5.000 USD) edo ordu kopuruaren arabera (100)?

Galdera hauen erantzunek zehazten dituzte kostuaren txantiloian ezartzen dituzun aukerak eta kostu txantiloiaren lerroetan hautatzen dituzun kategoriak.

Hurrengo taulan agertoki honetako ehuneko osoko balioa kalkulatzeko metodo desberdinen emaitzak azaltzen dira.

| Oinarritutako osaketa | Dolarraren kostua edo unitateak | Osatutako ehunekoa | Kalkulua |
| --- | --- | --- | --- |
| Ordu guztiak, gasturik gabe | Dolarraren kostua | % 37 35 x USD 50 + USD 100 = USD 1,850 USD 1.850/USD 5.000 |
| Ordu guztiak, gasturik gabe | Unitateak | % 40 | 40 ordu / 100 ordu (planifikatu gabeko bost ordu barne) |
| Antolatutako orduak, gasturik gabe | Dolarraren kostua edo unitatea | % 35 | 35/100 ordu edo 35 x USD 50 / 5.000 |
| Ordu eta gastu guztiak | Dolarraren kostua | % 27,2 | USD 1.850 / 6.800 USD |

Kostuen txantiloia sortzeko zein planteamendu hartu erabakitzea hainbat konturen araberakoa izan daiteke:

- Aurreikusi gabeko orduak kostu txantiloian sartzen badituzu, proiektua amaitu aurretik ehuneko 100 osora iristeko arriskua duzu. Benetako orduak aurreikusitako orduak baino handiagoak izango direlako gertatzen da. Taulan zerrendatutako lehen bi metodoetako bat erabiltzen baduzu, plana aldatu beharko zenuke (aurreikusitako unitateak) desbiderapenez jabetzen zarenean. Kasu honetan, ordua gehitu edo kenduko zenuke proiektua amaitzeko behar denaren ezagutzan oinarrituta. Proiektuak beste 65 ordu beharko balitu, bost ordu gehituko zenioke planari 105 guztira. Badakizu zure laguntzaileak beste bost orduko ikerketa egingo duela, guztira 110 ordu bihurtuko dira.
- Taulan agertzen den hirugarren metodoa erabiltzen baduzu, aurreikusitako orduak zure egunerako soilik eguneratuko dituzu ehuneko osoko kalkulua zehatza izan dadin. Zure errentagarritasuna aldatu egingo da planifikatu gabeko orduak erregistratzen direnean, baina ehuneko osoko ibilbide ezagunean jarraituko duzu.
- Taulan agertzen den laugarren metodoa erabiltzen baduzu, arriskua une irregularrean gastuak gertatzea da eta baliteke amaitzearen aurrerapenean ez izatea. Hori dela eta, gastuak sartzen badira, zure ehuneko osoak desiratzen duena baino gehiago aldatzea eragin dezake. Adibidez, oraindik ez zenuen hegaldirik hartu, zure ehuneko osoa ehuneko 27 zen, ehuneko 35 edo % 37 izan beharrean, kalkulua denboran bakarrik oinarrituko bazenu. Bi gauetan bidaia bat egin eta zure hegaldiaren eta hotelaren kostuak zehaztasunez aurreikusiko bazenitu, ehuneko osoa ehuneko 40,4 izango zen (1850 dolar eskulanerako eta USD 900 gastuetarako = USD 2750 / USD 6800 = ehuneko 40,4). Hori dela eta, hegazkin bidaia bakarreko gastuak egiteak ehuneko osoa ehuneko 27tik % 40ra aldatuko luke.

## <a name="create-cost-templates"></a>Sortu kostuen txantiloiak
Kostuen txantiloiak sortzeko, jarraitu urrats hauei:

1. Kostuen txantiloiak atzitzeko, Dynamics 365 Finance ingurunea, joan **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Aurrekontuak** > **Kostuen txantiloia** aukerara.
2. Hautatu **Berria** kostuen txantiloi berria sortzeko. Idatzi izena eta deskribapena.
3. Eman kostu lerroaren IDa transakzio mota bakoitzerako.
4. Aukeratu lehenetsitako osatze-metodoa:

  - **Automatikoa**: Bukaeraren ehunekoa automatikoki kalkulatzen da proiektu batean. Ezin da aldatu lortutako balioa.
  - **Eskuzkoa**: Bukaeraren ehunekoa automatikoki kalkulatzen da proiektu batean. Lortutako balioa alda daiteke.

  > [!NOTE]
  > Eskuzko kalkuluak egiteko, osatze portzentajea urtean mantentzen da **Eskuzko kalkulua** **Orokorra** fitxan **Estimazioa** orrialdean.

5. **Oinarritutako osaketa** aukeran, hautatu balio hauetako bat:

  - **Zenbatekoa**: Kontabilitate monetan zenbatekoak osatutako ehunekoa kalkulatzen du.
  - **Unitatea**: Kopuruak osatutako ehunekoa kalkulatzen du.
  - **Lerro zuzena**: Sistemak osatutako ehunekoa proportzionalki kalkulatzen du proiektuaren hasiera eta amaiera datak erabiliz proiektuaren iraupena zehazteko.

6. Aukeratu **Kostuen lerroak** kostuen txantiloiaren kostu lerroak berrikusteko. Gutxienez kostu lerro bat behar da transakzio mota bakoitzeko. Hala ere, kostu lerro ugari sor ditzakezu transakzio mota berdinetarako eta lerro horietarako nahi dituzun atributuak ezar ditzakezu.
7. **Kategoriak** fitxan, hautatu kostuaren txantiloiaren lerroan sartu beharreko proiektuen kategoriak.
8. **Orokorra** fitxan, hautatu lerro hau osatze-kalkuluaren ehunekoan sartuko den.
9. Aukeratu osatzeko portzentaia kalkulatzeko erabili beharreko metodoa osatzeko kostua.
