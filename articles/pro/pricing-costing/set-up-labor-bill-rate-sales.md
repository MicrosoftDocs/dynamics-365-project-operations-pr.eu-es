---
title: Lanaren fakturazio-tasak konfiguratzea
description: Gai honek Project Operations-eko lanaren fakturazio-tasak konfiguratzeari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/16/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: e6294895857442f3a24a9d73ee07d2b90926a4fb
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071098"
---
# <a name="setting-up-bill-rates-for-labor-rate-billing"></a>Lan-tasaren fakturazioari buruzko fakturak ezartzea 

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Prezio zerrenda bakoitzak prezio zerrendaren edo lan-tasak edukiarekin eta datarekin eraginkortasunarekin bat datozen lan tasen multzoa du. Dynamics 365 Project Operations zerbitzuaren fakturazio tasak moneta bakarrean konfigura daitezke, hau da, Prezio zerrendaren goiburuko moneta.

1. Salmenta prezioen zerrendako lan fakturaren tasak ezartzeko, sortu prezioen zerrenda prezio zerrendaren goiburuan oinarrituta. 
2. **Funtzio-prezioak** fitxan, azpisaretan, hautatu **+Rol berriaren prezioa**. 
3. **Sorrera bizkorra** panelean, sartu faktura-tasa konfiguratu behar duzun rol eta antolakuntza-unitateen konbinazioa.

  Ondorengo taulan eremuko eremuak biltzen dira **Orokorra** fitxa eta **Sorrera bizkorra** kontuan izan behar duzun rol-prezioen lerroaren panela, salmenta-prezioen zerrendan rol-prezioak sortzen dituzunean:

  | Eremua | Kokapena | Garrantzia, xedea eta orientazioa | Downstream eragina |
  | --- | --- | --- | --- |
  | Funtzioa | **Orokorra** fitxa eta **Sortu bizkor** panela | Hautatu fakturazio-tasa ezartzen ari zaren funtzioa. | Sarrerako estimazioaren edo benetako eginkizuna lerro honekin parekatuko da fakturazio-tasaren kostua lehenetsi ahal izateko. |
  | Baliabide-unitatea | **Orokorra** fitxa eta **Sortu bizkor** panela | Aukeratu enpresaren antolakuntza unitatea edo banaketa zeregin funtzioa non erabiliko den. Adibidez, Fabrikam Indiako Robotika dibisioko garatzailea edo Fabrikam AEBetako Software dibisioaren garatzailea. | Sarrerako estimazioaren edo benetako unitateko baliabideak lerro honekin parekatuko da rolaren fakturazio-tasa lehenetsi ahal izateko. |
  | Prezioa | **Orokorra** fitxa eta **Sortu bizkor** panela | Konfiguratu eginkizunaren fakturazio-tasa, konpainia hornitzailea eta hornikuntza unitateen konbinazioa. Adibidez, Fabrikam Indiako garatzaile batek 100 USD faktura-tasa du edo Fabrikam AEBetako garatzaile batek 150 USD faktura-tasa. | Fakturazio-sarrerako aurrekontuaren kostu unitateko edo lineako benetako lerroaren kostu lehenetsia da Denbora transakzio klasea. |
  | Moneta | **Orokorra** fitxa eta **Sortu bizkor** panela| Berez, moneta balioa kostuen prezioen zerrendako goiburutik dator. Salmenta prezioen zerrendan, moneta ezin da gainidatzi. | Fakturazio-sarrerako aurrekontuaren kostu unitateko edo lineako benetako salmenten lerroaren kostu lehenetsia da Denbora transakzio klasea. |
  | Unitate-antolaketa | **Orokorra** fitxa eta **Sortu bizkor** panela | Unitatearen ordutegia Denbora lehenetsia da eta ezin da aldatu Role prezioaren entitatean, denbora unitateen bidez tarifa espresak erabiltzen direlako. | Ez dago alor honen beherako eraginik. |
  | Unitatea | **Orokorra** fitxa eta **Sortu bizkor** panela | Unitate-balioa kostuen prezioen zerrendako **Denbora-unitatea** eremuaren salmenten prezio-zerrendaren goiburuan. Baina, balioa gainidatz daiteke. Adibidez, Fabrikam Indiako garatzaile batek 1000 USD kostatzen ditu **India eguna** bakoitzeko. Fabrikam USA-ko garatzaile batek faktura-tasa 1500 USD da **AEBetako eguna**. | Unitate-prezio lehenetsiak sarrerako gutxi gorabeherako eta benetako lerroan, sistemak unitateen eta bihurtze sistema erabiltzen du oinarrizko unitateetan kostu bakoitzeko bat kalkulatzeko sarrerako estimazioan edo benetako lerroan unitateko prezio lehenetsia kalkulatzeko. Adibidez, kalkulua 10 da **India egunak** lana merezi du Indiako garatzaile batek eta unitateak, India eguna 10 ordu gisa definitzen da. Estimazio lerro hori tasatzerakoan, aplikazioak zenbatekoaren unitateko prezioa kalkulatzen du 1000 USD / 10 ordu = 100 USD orduko. |


## <a name="transfer-pricing-or-set-up-bill-rates-for-resources-from-other-organizational-units-or-divisions"></a>Transferitu prezioak edo ezarri beste erakunde unitate edo sail batzuetako baliabideen fakturen tasak 

Proiektuetan oinarritutako enpresak enpresako sail desberdinetako langileak proiektuetan lan egiteko erabiltzeko. Proiektuak dibisio batetik exekutatu daitezke langileak edo aholkulariak enpresako dibisio beretik datozen bitartean. Proiektua dibisio desberdinetako jendearen konbinazio batek ere osa dezake. Project Operations-en, proiektuaren entregaren jabe den enpresari **Kontratazio unitatea**. Baliabideak eskaintzen dituzten gainerako atal guztiei **Baliabideak hornitzeko unitateak**. Mundu osoko hainbat geografi eta lan merkatuetan eskulanaren kostuen aldeak direla eta, eskulanaren fakturen tasak era desberdinean ezartzen dira geografi desberdinetarako.

Adibidez, Fabrikam Indiako garatzaile batek AEBetako proiektu batean lan egiten duena orduko 100 USD tasarekin fakturatzen da. US Project-en lanean ari den Fabrikam USeko garatzaile batek orduko 150 USD fakturatzen du.

### <a name="example-set-up-a-bill-rate"></a>Adibidez: konfiguratu faktura-tasa

1. Sortu izeneko salmenta prezioen zerrenda *Fabrikam AEBetako fakturen tasak* , eta data efektibitatea ezarri.
2. Salmenten prezio-zerrenda inprimakian, ondorengo tasa-informazioa sartu:

    | Funtzioa | Erakunde-unitatea | Fakturazio-tasa |
    | --- | --- | --- |
    | Garatzailea | Fabrikam India | 100 USD |
    | Garatzailea | Fabrikam Philippines | 90 $ |
    | Garatzailea | Fabrikam US | 150 $ |

3. Erantsi salmenta prezioen zerrenda, **Fabrikam AEBetako fakturen tasak** proiektuaren kontratuaren proiektuaren prezioen zerrendara edo kontu jakin batera.