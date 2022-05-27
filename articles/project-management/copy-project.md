---
title: Kopiatu proiektu bat
description: Gai honek proiektuak Dynamics 365 Project Operations-en kopiatzeari buruzko informazioa ematen du.
author: ruhercul
ms.date: 03/07/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: e9b637d2d282d123dfacb8a295292ea06549aa1e
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8574415"
---
# <a name="copy-a-project"></a>Kopiatu proiektu bat

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations-ekin, proiektu berriak azkar eraiki ditzakezu **Kopiatu proiektua** hautatuta **Proiektuak** inprimakian. Proiektu bat kopiatzeko, ireki kopiatu nahi duzun proiektua eta hautatu **Kopiatu proiektua**. Ekintzak honako hau kopiatuko du:

- Proiektuaren propietateak 
- Atazen xehapenaren egitura
- Proiektuaren taldeko kideak
- Proiektuaren aurreikuspenak
- Proiektuaren gastuen aurreikuspenak
- Proiektu-materialaren aurreikuspenak
- Proiektuen kontrol-zerrendak
- Proiektuen kuboak

## <a name="project-properties"></a>Proiektuaren propietateak

Proiektua kopiatzen denean, ondoko eremuetako balioak kopiatzen dira.

| Eremua | Proiektuaren Eragiketak Izakigabeko Materialak | Project Operations Lite | Weberako proiektua |
|-------|------------------------------------------|-------------------------|---------------------|
| Eman izena | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| Deskribapenak | :heavy_check_mark: | :heavy_check_mark: | |
| bezero hori | :heavy_check_mark: | :heavy_check_mark: | |
| Egutegiaren txantiloia | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| Moneta | :heavy_check_mark: | :heavy_check_mark: | |
| Kontratatzailea | :heavy_check_mark: | :heavy_check_mark: | |
| Jabetzadun enpresa | :heavy_check_mark: | | |
| Proiektu-kudeatzailea | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| Fasea | :heavy_check_mark: | :heavy_check_mark: | |
| Proiektuaren egoera orokorra | :heavy_check_mark: | :heavy_check_mark: | |
| Iruzkinak | :heavy_check_mark: | :heavy_check_mark: | |
| Aurreikuspenak | :heavy_check_mark: | :heavy_check_mark: | |
| <p>Aurreikusitako hasiera-data</p><p><strong>Ohar:</strong> Eremu honek proiektua kopiatik sortu den data zehazten du. | :heavy_check_mark: | :heavy_check_mark: | |
| <p>Aurreikusitako amaiera-data</p><p><strong>Ohar:</strong> Eremu honetako data kopiatik egin den proiektu berriaren hasiera-dataren arabera egokitzen da.</p> | :heavy_check_mark: | :heavy_check_mark: | |
| Ahalegina (orduak) | :heavy_check_mark: | :heavy_check_mark: | |
| Aurreikusitako lan-kostua | :heavy_check_mark: | :heavy_check_mark: | |
| Gastuetan oinarritutako aurreikusitako kostua | :heavy_check_mark: | :heavy_check_mark: | |
| Aurreikusitako materialaren kostua | | :heavy_check_mark: | |

> [!NOTE]
> Kopiatu proiektua martxan dagoen eragiketa da. Proiektuaren erregistroak, dagozkien atributuak eta erlazionatutako entitate asko ere kopiatzen dira. Eragiketaren iraupen luzea dela eta, kopia hasi ondoren, xede proiektuaren orria blokeatuta dago editatzeko, kopia eragiketa amaitu arte.

## <a name="work-breakdown-structure"></a>Atazen xehapenaren egitura

Proiektua kopiatzen denean, baliabidez kargatutako zereginen xehetasunen egitura osoa kopiatzen da. Izena duten baliabideak baliabide generikoekin ordezten dira. Izendatutako baliabideek ez badute baliabide generikoaren lanordu berdinak, ordutegia berriro kalkulatuko da eta baliteke zereginen iraupena aldatzea.

## <a name="project-team-members"></a>Proiektuaren taldeko kideak

Proiektu talde bat jatorrizko proiektutik kopiatzen denean, baliabide generikoak kopiatzen dira. Baliabide orokorren esleipenak ere mantendu egiten dira, jatorriko proiektuan zeudelako. Izendatutako baliabideak taldeko kide generiko bihurtuko dira.

> [!NOTE]
> Taldeko kideak eta lanak ez dira kopiatzen Weberako proiektuan.

## <a name="estimates"></a>Aurreikuspenak

Proiektua kopiatzen denean, baliabide, gastu eta materialen estimazio lerroak jatorrizko proiektuetik kopiatzen dira. 

Kopiatu proiektua aukerara programaren bidez nola sartu jakiteko, ikusi [Garatu proiektuaren txantiloiak Kopiatu proiektua aukerarekin](dev-copy-project.md).

## <a name="quotes-and-contracts"></a>Eskaintzak eta kontratuak

Aurrekontuak eta kontratuak ez daude helmugako proiektuarekin lotuta.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
