---
title: Kopiatu proiektu bat
description: Artikulu honek proiektuak kopiatzeari buruzko informazioa eskaintzen du Dynamics 365 Project Operations.
author: ruhercul
ms.date: 03/07/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: b358f9e45278d886f3e6e8e8cd747fc0ea30212b
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8925749"
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
- Proiektuaren egiaztapen-zerrendak
- Proiektuaren ontziak

## <a name="project-properties"></a>Proiektuaren propietateak

Proiektua kopiatzen denean, eremu hauetako balioak kopiatzen dira.

| Eremua | Project Operations materialik gabeko materiala | Project Operations Lite | Project for the Web |
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
| <p>Aurreikusitako hasiera-data</p><p><strong>Oharra:</strong> eremuak proiektua kopiatik sortu zeneko data zehazten du. | :heavy_check_mark: | :heavy_check_mark: | |
| <p>Aurreikusitako amaiera-data</p><p><strong>Oharra:</strong> Eremuko data kopiatik egindako proiektu berriaren hasierako dataren arabera egokitzen da.</p> | :heavy_check_mark: | :heavy_check_mark: | |
| Ahalegina (orduak) | :heavy_check_mark: | :heavy_check_mark: | |
| Aurreikusitako lan-kostua | :heavy_check_mark: | :heavy_check_mark: | |
| Gastuetan oinarritutako aurreikusitako kostua | :heavy_check_mark: | :heavy_check_mark: | |
| Aurreikusitako materialaren kostua | | :heavy_check_mark: | |

> [!NOTE]
> Kopiatu proiektua martxan dagoen eragiketa da. Proiektuaren erregistroak, dagozkien atributuak eta erlazionatutako entitate asko ere kopiatzen dira. Eragiketaren iraupen luzea dela eta, kopia hasi ondoren, xede proiektuaren orria blokeatuta dago editatzeko, kopia eragiketa amaitu arte.

## <a name="work-breakdown-structure"></a>Atazen xehapenaren egitura

Proiektua kopiatzen denean, baliabidez kargatutako zereginen xehetasunen egitura osoa kopiatzen da. Izena duten baliabideak baliabide generikoekin ordezten dira. Izendatutako baliabideek baliabide generikoaren lan orduak ez badituzte, ordutegia berriro kalkulatuko da eta zereginen iraupenak alda daitezke.

## <a name="project-team-members"></a>Proiektuaren taldeko kideak

Proiektu talde bat jatorrizko proiektutik kopiatzen denean, baliabide generikoak kopiatzen dira. Baliabide orokorren esleipenak ere mantendu egiten dira, jatorriko proiektuan zeudelako. Izendatutako baliabideak taldeko kide generiko bihurtuko dira.

> [!NOTE]
> Taldeko kideak eta lanak ez dira kopiatzen Project for the Web-en.

## <a name="estimates"></a>Aurreikuspenak

Proiektua kopiatzen denean, baliabide, gastu eta materialen estimazio lerroak jatorrizko proiektuetik kopiatzen dira. 

Kopiatu proiektua aukerara programaren bidez nola sartu jakiteko, ikusi [Garatu proiektuaren txantiloiak Kopiatu proiektua aukerarekin](dev-copy-project.md).

## <a name="quotes-and-contracts"></a>Eskaintzak eta kontratuak

Aurrekontuak eta kontratuak ez daude helmugako proiektuarekin lotuta.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
