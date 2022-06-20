---
title: Konfiguratu gastuen kostu- eta salmenta-tasak
description: Artikulu honek transakzio eta gastu kategorien kostuak eta salmenta-tasak konfiguratzeari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 04/07/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: c503230348750af246f6ee7a4af1176d7bf22ba4
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8911857"
---
# <a name="set-up-cost-and-sales-rates-for-expenses"></a>Konfiguratu gastuen kostu- eta salmenta-tasak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Transakzio kategorien kostua eta salmenta prezioak konfigura ditzakezu Dynamics 365 Project Operations-en. Kostua eta salmenta prezioak Gastuetarako diseinatuta daudenez, hauek biltzen dituen transakzio kategoria bakoitza gastu kategoria gisa ere ezarri behar da. Konfigurazio honek beheranzko funtzionaltasunean zehaztasuna bermatzen du. Transakzio kategorien kostua eta salmenta prezioak moneta bakarrean zerrendatu daitezke, hau da, prezio zerrendaren goiburuko moneta izan behar da.

Transakzio kategorien kostua eta salmenta tasak konfiguratzeko, jarraitu urrats hauek. 

1. Joan **Salmentak** > **Bezeroak** > **Prezio-zerrendak**.
2. Hautatu **Berria** prezio-zerrenda berri bat sortzeko. 
3. **Kategoriaren prezioak** eremuan, azpisarea menuan, hautatu **Kategoria berria**. 
4. **Sorrera bizkorra** orrian, sartu prezio berria sortzen ari zaren transakzio kategoria eta unitatea.

Ondorengo taulan eremuko eremuak biltzen dira **Orokorra** fitxa eta **Sorrera bizkorra** kontuan izan behar duzun prezioen lerroaren panela, salmenten edo kostuaren prezioen zerrendan rol-prezioak sortzen dituzunean:

| Eremua | Kokapena | Deskribapena | Downstream eragina |
| --- | --- | --- | --- |
| Transakzio-kategoria | **Orokorra** fitxa eta **Sortu bizkor** orrialdeak | Aukeratu salmenta edo kostu prezioa sortzen ari zaren transakzio kategoria. | Sarrerako transakzioren kategoria edo gastuen benetako enpresako baliabideak lerro honekin parekatuko da rolaren kostu edo salmenta-tasa lehenetsi ahal izateko. |
| Unitate-antolaketa | **Orokorra** fitxa eta **Sortu bizkor** orrialdeak | Unitate-programak transakzio-kategoriako unitate-programaren lehenetsiak dira. | Ez dago alor honen beherako eraginik. |
| Unitatea | **Orokorra** fitxa eta **Sortu bizkor** orrialdeak | Aukeratu tasak ezartzeko unitatea. | Sarrerako aurrekontuaren edo benetako unitatea linea honetako unitatearen parekoa da gastuaren aurrekontuaren edo benetakoaren tasa lehenesteko. |
| Prezio-metodoa | **Orokorra** fitxa eta **Sortu bizkor** orrialdeak | **Prezioen metodoa** eremua dira, **Unitateko prezioa**, **Kostata** eta **Markaketa kostuaren gainetik**. | Prezioa konfiguratzerakoan, hautatu **Unitateko prezioa** blokeatzen du **Ehunekoa** kategoria prezioen lerroan. **Kostata** hautatuta dago **Prezioa** eta **Ehunekoa** eremuak salmenta prezioen zerrendan blokeatuta daude. **Markaketa kostuaren gainetik** blokeatzen du **Prezioa** salmenta prezioen zerrendako eremua. Gastuetarako sarrerako benetako lerro batean **Kostata** edo **Markaketa kostuaren gainetik** prezioen metodoari esker, dagokion fakturaziorik gabeko salmenta-lerroa egiazko kostuaren prezioaren berdina edo prezioaren gaineko marka gisa kalkulatutako prezioa esleitzen da. |
| Prezioa | **Orokorra** fitxa eta **Sortu bizkor** orrialdeak | Ezarri unitate bakoitzeko tarifa transakzio kategoria eta unitate konbinaziorako. Adibidez, kilometrajearen tasa miliako 10 USD da eta Kilometro bakoitzeko 8 USD. | Kilometroen tasa aurrekontuaren prezio edo kostu unitateko edo lineako benetako lerroaren kostu lehenetsia da gastuen transakzio klasea.|
| Ehunekoa | **Orokorra** fitxa eta **Sortu bizkor** orrialdeak | Konfiguratu unitate bakoitzeko tarifa transakzio kategoria eta unitate konbinaziorako. Adibidez, hegazkinen salmenta-tasa ehuneko 10 markatu behar da sortutako hegaldiaren gastuaren gainetik. | Kostuaren gainprezioaren salmenten prezio-zerrendari aplikatuko zaio soilik prezio-metoda **Kostuaren gainprezioa** denean soilik. |
| Moneta | **Orokorra** fitxa eta **Sortu bizkor** orrialdeak | Berez, balioa kostuen prezioen zerrendako goiburutik dator. Transakzio-kategorien prezioetarako, ezin da moneta gainidatzi. | Fakturazio-sarrerako aurrekontuaren benetako salmenten lerroaren kostu lehenetsia da. |

## <a name="pricing-methods-for-expenses"></a>Gastuen prezio metodoak

Gastuen prezioen testuinguruan soilik garrantzitsuak diren kategoriako prezioak konfiguratzen dituzunean, hiru prezio metodo hauetako bat erabil dezakezu:

- **Prezioa unitate bakoitzeko**
- **Kostuan**
- **Markaketa kostuaren gainetik**

### <a name="price-per-unit"></a>Prezioa unitate bakoitzeko
Prezio-metodo hau salmenta-prezioen zerrenda batekin lotuta dagoen kategoriako prezioen lerroan hautatzen denean, kategoria eta unitate konbinazioaren prezioak lehenetsitakoak dira bai estimazioan bai benetakoan. Gastuaren zenbatespen lerroek proiektu bateko proiektu bateko gastuak, eskaintzaren lerroaren xehetasuna eta kontratuaren lerroaren xehetasuna.

### <a name="at-cost"></a>Kostuan
Prezio-metodo hau salmenta-prezioen zerrenda batekin lotuta dagoen kategoriako prezioen lerroan hautatzen denean, kategoria eta unitate konbinazioaren prezioak lehenetsitakoak soilik dira benetako gastuak. Adibidez, fakturatu gabeko salmenten fakturak gastuen transakzio klaserako. Prezio unitarioa fakturatu gabeko salmenten gainean ezartzen da gastu horren kostu errealaren unitateko prezioan. Kostuaren araberako prezio lehenetsia ez da gastuetarako proiektuaren aurrekontuetan edo aurrekontuaren lerroan eta kontratuaren lerroaren xehetasunetan egiten.

### <a name="markup-over-cost"></a>Markaketa kostuaren gainetik
Prezio-metodo hau salmenta-prezioen zerrenda batekin lotuta dagoen kategoriako prezioen lerroan hautatzen denean, kategoria eta unitate konbinazioaren prezioak lehenetsitakoak soilik dira benetako gastuak. Adibidez, fakturatu gabeko salmenten fakturak gastuen transakzio klaserako. Unitate-prezio hori fakturatu gabeko salmenten gainean ezartzen da gastu horren kostu errealaren gaineko balio kalkulatuaren arabera, zehaztutako ehuneko markatua aplikatu ondoren. Kostuaren araberako prezio lehenetsia ez da gastuetarako proiektuaren aurrekontuetan edo aurrekontuaren lerroan eta kontratuaren lerroaren xehetasunetan egiten.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
