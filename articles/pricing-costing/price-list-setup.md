---
title: Konfiguratu prezio-zerrendak
description: Gai honek kostuen eta salmenten prezio-zerrendak konfiguratzeari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/20/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 000c22944b187b6250f2e982d73020028093fde6
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/31/2020
ms.locfileid: "4180177"
---
# <a name="set-up-price-lists"></a>Konfiguratu prezio-zerrendak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations-eko prezio zerrendek tasen katalogoa adierazten dute. Tarifek kostua, salmentak eta fakturen tasak adierazten dituzte. Prezioen zerrendak kostuen tasak edo salmenten eta fakturen tasak adierazten dituen arabera, prezioen zerrendaren testuingurua da **Salmentak** edo **Kostua**.

Hurrengo luzapenak Proiektuaren eragiketetarako zehatzak dira eta Dynamics 365 Sales-eko prezio zerrendetan aplikatzen dira.

- **Testuingurua**: Eremu honek onartutako balioak ditu, **Kostua** eta **Salmentak**. Ez da onartzen **Erosi** balioa. Testuingurua ezarri **Kostua** kostuen prezioen zerrenda egiteko edo testuingurua ezartzeko **Salmentak** salmenta prezioen zerrenda lortzeko. Kostuen prezioen zerrendek kostu motaren prezioa ebazten dute eta benetako erregistroetan ebazten dute. Salmenta prezioen zerrendek fakturatu gabeko eta fakturatutako salmenta moten erregistro estimatuen eta errealen prezioa ebazten dute.
- **Denbora Unitatea**: Horrekin erlazionatutako prezioa ezartzen den denbora unitate lehenetsia da **Rolaren prezioa** prezio zerrenda honetarako taula.
- **Prezioen zerrendako entitatea**: Ezkutuko eremu hau Proiektuaren Eragiketen arabera da, aurrekontu edo kontratuaren araberako prezioen zerrendak bereizteko eta orokorrean aplikagarriak direnak.

## <a name="price-list-header"></a>Prezio-zerrendaren goiburua

Ondorengo taulan eremuko eremuak biltzen dira **Orokorra** salmentetako prezioen zerrenden arabera Proiektuen eragiketetarako soilik diren edo portaeran aldaketa nabarmenak dituzten prezioen zerrendaren fitxa.

| Eremua | Kokapena | Deskribapena | Downstream eragina |
| --- | --- | --- | --- |
| Eman izena | **Orokorra** fitxa eta **Sortu bizkor** inprimakiak | Prezio-zerrendaren nortasuna. | Prezioen-zerrendak balio hori zerrendako orrialde eta goitibeherako aukera guztietan erakusten du.|
| Testuingurua | **Orokorra** fitxa eta **Sortu bizkor** inprimakiak | Eremu hau ezar daiteke **Kostua** edo **Salmentak**. | Prezio zerrenda **Kostua** kalkulatzeko eta kostuen benetako prezioa bilatzeko erabiltzen da. Prezio zerrenda **Salmentak** kalkulatzeko eta salmenten benetako prezioa bilatzeko erabiltzen da. Testuingurua ezarrita duten prezioen zerrendak soilik **Salmentak** bezeroaren, proiektuaren aurrekontuen edo proiektuaren kontratuaren proiektuen prezioen zerrendara erants daiteke. |
| Hasiera-data | **Orokorra** fitxa eta **Sortu bizkor** inprimakiak | Prezioen zerrenda dagoen aldiaren hasiera-data eraginkorra da. | **Amaiera-data** eremuarekin, eremu hau estimazio jakin baterako edo benetako lerro baterako zein prezio-zerrenda aplikagarri den jakiteko erabiltzen da. |
| Amaiera-data | **Orokorra** fitxa eta **Sortu bizkor** inprimakiak | Prezioen zerrenda dagoen aldiaren amaiera-data eraginkorra da. | **Hasiera-data** eremuarekin, eremu hau estimazio jakin baterako edo benetako lerro baterako zein prezio-zerrenda aplikagarri den jakiteko erabiltzen da. |
| Moneta | **Orokorra** fitxa eta **Sortu bizkor** inprimakiak | Eremu hau prezio zerrenda honekin erlazionatutako rol, kategoria edo prezio zerrendako elementu bakoitzaren moneta lehenetsi ahal izateko erabiltzen da. | **Salmentak** prezioen zerrendan, rolak, kategoriak edo prezioen zerrendako elementuen lerroak ezin dira moneta ez den beste moneta batean sortu. **Kostua** prezioen zerrendan, edozein preziotan lerro bat sor dezakezu. Hemen definitutako moneta lehenetsi gisa erabiltzen da. Lotutako rolen prezioak dituen erabiltzailearen konfigurazioak balio hori gainidatz dezake laneko kostuen tasa konfiguratzea edozein monetan. Kategoriaren kostuen tasak eta prezioen zerrendako elementuen kostuak hemen definitutako monetan soilik konfigura daitezke. |
| Denbora-unitatea | **Orokorra** fitxa eta **Sortu bizkor** inprimakiak | Eremu hau prezio zerrenda honekin erlazionatutako rol bakoitzaren denbora-unitate lehenetsi ahal izateko erabiltzen da. | Eremu balio hau erlazionatutako rol prezioen konfigurazioan soilik erabiltzen da. **Kostua** eta **Salmentak** prezioen zerrendetan, edozein denbora-unitatetan lerro bat sor dezakezu. Hemen definitutako denbora-unitate lehenetsi gisa erabiltzen da. Lotutako rolen prezioak dituen erabiltzailearen konfigurazioak balio hori gainidatz dezake laneko kostuen eta fakturazio-tasa konfiguratzea edozein denbora-unitatetan. |
| Deskribapena | **Orokorra** fitxa eta **Sortu bizkor** inprimakiak | Testu eremua da prezio zerrendaren lerro anitzeko deskribapena egiteko aukera emateko. | Eremu hau **Elkartua** erlazionatutako prezio zerrendak dituzten hainbat erakundetako prezioen zerrendari buruzko ikuspegiak. |
