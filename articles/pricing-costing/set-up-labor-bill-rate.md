---
title: Konfiguratu lanaren fakturazio-tasak
description: Gai honek Project Operations-eko lanaren fakturazio-tasak konfiguratzeari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 04/07/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 0fee2c98713f4d1f8da85a0b60fb3fc2a873e5f82a64cf350ebeb68fe65fab35
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "7003531"
---
# <a name="set-up-labor-bill-rates"></a>Konfiguratu lanaren fakturazio-tasak

**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations

Prezio zerrenda bakoitzak prezio zerrendaren edo lan-tasak edukiarekin eta datarekin eraginkortasunarekin bat datozen lan tasen multzoa du. Dynamics 365 Project Operations-eko denboraren fakturazio-tasak moneta bakarrean konfigura daitezke, hau da, Prezio zerrendaren goiburuko monetan.

1. Salmenta prezioen zerrenda baterako lan fakturaren tasak ezartzeko, joan **Salmentak** > **Bezeroak** > **Prezio-zerrendak** eta hautatu **Berria** prezio zerrenda berria sortzeko. 
2. **Funtzio-prezioak** fitxan, azpisaretan, hautatu **Rol berriaren prezioa**. 
3. **Sorrera bizkorra** panelean, sartu faktura-tasa konfiguratu behar duzun rol eta antolakuntza-unitateen konbinazioa.

   Ondorengo taulan eremuko eremuak biltzen dira **Orokorra** fitxa eta **Sorrera bizkorra** kontuan izan behar duzun rol-prezioen lerroaren panela, salmenta-prezioen zerrendan rol-prezioak sortzen dituzunean:

    | Eremua | Kokapena | Deskribapena | Downstream eragina |
    | --- | --- | --- | --- |
    | Funtzioa | **Orokorra** fitxa eta **Sortu bizkor** panela | Hautatu fakturazio-tasa ezartzen ari zaren funtzioa. | Sarrerako estimazioaren edo benetako eginkizuna lerro honekin parekatuko da fakturazio-tasaren kostua lehenetsi ahal izateko. |
    | Baliabideen enpresa | **Orokorra** fitxa eta **Sortu bizkor** panela | Aukeratu enpresa edo rola esleitutako pertsona juridikoa. Adibidez, Fabrikam Indiako garatzaile bat edo Fabrikam USAko garatzaile bat. | Sarrerako estimazioaren edo benetako enpresako baliabideak lerro honekin parekatuko da rolaren fakturazio-tasa lehenetsi ahal izateko. |
    | Baliabide-unitatea | **Orokorra** fitxa eta **Sortu bizkor** panela | Aukeratu enpresaren antolakuntza unitatea edo banaketa zeregin funtzioa non erabiliko den. Adibidez, Fabrikam Indiako Robotika dibisioko garatzailea edo Fabrikam AEBetako Software dibisioaren garatzailea. | Sarrerako estimazioaren edo benetako unitateko baliabideak lerro honekin parekatuko da rolaren fakturazio-tasa lehenetsi ahal izateko. |
    | Prezioa | **Orokorra** fitxa eta **Sortu bizkor** panela | Konfiguratu eginkizunaren fakturazio-tasa, konpainia hornitzailea eta hornikuntza unitateen konbinazioa. Adibidez, Fabrikam Indiako garatzaile batek 100 USD faktura-tasa du edo Fabrikam AEBetako garatzaile batek 150 USD faktura-tasa. | Fakturazio-sarrerako aurrekontuaren kostu unitateko edo lineako benetako lerroaren kostu lehenetsia da Denbora transakzio klasea. |
    | Moneta | **Orokorra** fitxa eta **Sortu bizkor** panela| Berez, moneta balioa kostuen prezioen zerrendako goiburutik dator. Salmenta prezioen zerrendan, moneta ezin da gainidatzi. | Fakturazio-sarrerako aurrekontuaren kostu unitateko edo lineako benetako salmenten lerroaren kostu lehenetsia da Denbora transakzio klasea. |
    | Unitate-antolaketa | **Orokorra** fitxa eta **Sortu bizkor** panela | Unitatearen ordutegia Denbora lehenetsia da eta ezin da aldatu Role prezioaren entitatean, denbora unitateen bidez tarifa espresak erabiltzen direlako. | Ez dago alor honen beherako eraginik. |
    | Unitatea | **Orokorra** fitxa eta **Sortu bizkor** panela | Unitate-balioa kostuen prezioen zerrendako **Denbora-unitatea** eremuaren salmenten prezio-zerrendaren goiburuan. Baina, balioa gainidatz daiteke. Adibidez, Fabrikam Indiako garatzaile batek 1000 USD kostatzen ditu **India eguna** bakoitzeko. Fabrikam USA-ko garatzaile batek faktura-tasa 1500 USD da **AEBetako eguna**. | Unitate-prezio lehenetsiak sarrerako gutxi gorabeherako eta benetako lerroan, sistemak unitateen eta bihurtze sistema erabiltzen du oinarrizko unitateetan kostu bakoitzeko bat kalkulatzeko sarrerako estimazioan edo benetako lerroan unitateko prezio lehenetsia kalkulatzeko. Adibidez, kalkulua 10 da **India egunak** lana merezi du Indiako garatzaile batek eta unitateak, India eguna 10 ordu gisa definitzen da. Estimazio lerro hori tasatzerakoan, aplikazioak zenbatekoaren unitateko prezioa kalkulatzen du 1000 USD / 10 ordu = 100 USD orduko. |

## <a name="transfer-pricing-or-set-up-bill-rates-for-resources-from-other-organizational-units-or-divisions"></a>Transferitu prezioak edo ezarri beste erakunde unitate edo sail batzuetako baliabideen fakturen tasak 

Proiektuetan oinarritutako konpainiek askotan entitate juridiko desberdinetako eta atal juridiko ezberdinetako langileak erabiltzen dituzte proiektuetan lan egiteko. Proiektuek pertsona juridiko batek exekutatu dezake, baina proiektuan lan egiten duten langile edo aholkulariak pertsona juridiko beretik edo beste batetik etor daitezke, edo bien konbinazioa egon daiteke. Proiektua lege-entitate eta dibisio desberdinetako jendearen konbinazio batek ere osa dezake. Project Operations-en, proiektuaren entregaren jabe den pertsona juridikoa da **Enpresa titularra** eta banaketaren jabea da **Kontratazio Unitatea**. Baliabideak eskaintzen dituzten beste pertsona juridikoak dira **Enpresa hornitzaileak** eta baliabideak eskaintzen dituzten zatiketak dira **Baliabideak hornitzeko unitateak**. Mundu osoko hainbat geografi eta lan merkatuetan eskulanaren kostuen aldeak direla eta, eskulanaren fakturen tasak era desberdinean ezartzen dira geografi desberdinetarako.

Adibidez, Fabrikam Indiako Robotics saila garatzaile batek AEBetako proiektu batean lan egiten duena orduko 100 USD tasarekin fakturatzen da. US Project-en lanean ari den Fabrikam USeko Robotics sailaren garatzaile batek orduko 150 USD fakturatzen du. 

### <a name="example-set-up-a-bill-rate"></a>Adibidez: konfiguratu faktura-tasa 

1. Sortu izeneko salmenta prezioen zerrenda *Fabrikam AEBetako fakturen tasak*, eta data efektibitatea ezarri.
2. Salmenten prezio-zerrenda inprimakian, ondorengo tasa-informazioa sartu:

    | Funtzioa | Baliabideen enpresa | Baliabide-unitatea | Fakturazio-tasa |
    | --- | --- | --- | --- |
    | Garatzailea | Fabrikam India | Fabrikam India- Robotics | 100 USD |
    | Garatzailea | Fabrikam Philippines | Fabrikam Philippines - Robotics | 90 $ |
    | Garatzailea | Fabrikam US | Fabrikam US - Robotics | 150 $ |

3. Erantsi salmenta prezioen zerrenda, **Fabrikam AEBetako fakturen tasak** proiektuaren kontratuaren proiektuaren prezioen zerrendara edo kontu jakin batera.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
