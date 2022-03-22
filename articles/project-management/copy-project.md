---
title: Kopiatu proiektu bat
description: Gai honek proiektuak Dynamics 365 Project Operations-en kopiatzeari buruzko informazioa ematen du.
author: ruhercul
ms.date: 05/21/2021
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: fe76f59b315fd0f46b25e1d116acde1f6b2864d1753e01d6311ea93ae7d116fc
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "7007176"
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

## <a name="project-properties"></a>Proiektuaren propietateak

Proiektua kopiatzen denean, eremu hauetako balioak kopiatzen dira:

- Izena
- Deskribapena
- Bezeroa
- Egutegiaren txantiloia
- Moneta
- Kontratatzailea
- Proiektu-kudeatzailea
- Egoera
- Proiektuaren egoera orokorra
- Iruzkinak
- Aurreikuspenak
- Aurreikusitako Hasiera Data: proiektua kopiatik sortu den data da.
- Kalkulatutako amaiera-data: data hau kopiatik egindako proiektu berriaren hasierako dataren arabera egokitzen da.
- Ahalegina (orduak)
- Aurreikusitako lan-kostua
- Gastuetan oinarritutako aurreikusitako kostua
- Aurreikusitako materialaren kostua

> [!NOTE]
> Kopiatu proiektua martxan dagoen eragiketa da. Proiektuaren erregistroak, dagozkien atributuak eta erlazionatutako entitate asko ere kopiatzen dira. Eragiketaren iraupen luzea dela eta, kopia hasi ondoren, xede proiektuaren orria blokeatuta dago editatzeko, kopia eragiketa amaitu arte.

## <a name="work-breakdown-structure"></a>Atazen xehapenaren egitura

Proiektua kopiatzen denean, baliabidez kargatutako zereginen xehetasunen egitura osoa kopiatzen da. Izena duten baliabideak baliabide generikoekin ordezten dira. Izendatutako baliabideek baliabide generikoaren lan orduak ez badituzte, ordutegia berriro kalkulatuko da eta zereginen iraupenak alda daitezke.

## <a name="project-team-members"></a>Proiektuaren taldeko kideak

Proiektu talde bat jatorrizko proiektutik kopiatzen denean, baliabide generikoak kopiatzen dira. Baliabide orokorren esleipenak ere mantendu egiten dira, jatorriko proiektuan zeudelako. Izendatutako baliabideak taldeko kide generiko bihurtuko dira.

## <a name="estimates"></a>Aurreikuspenak

Proiektua kopiatzen denean, baliabide, gastu eta materialen estimazio lerroak jatorrizko proiektuetik kopiatzen dira. 

Kopiatu proiektua aukerara programaren bidez nola sartu jakiteko, ikusi [Garatu proiektuaren txantiloiak Kopiatu proiektua aukerarekin](dev-copy-project.md).


[!INCLUDE[footer-include](../includes/footer-banner.md)]
