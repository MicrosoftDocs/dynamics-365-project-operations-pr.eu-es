---
title: Antolaketa moduak
description: Gai honek antolaketa moduei buruzko informazioa ematen du.
author: ruhercul
ms.date: 05/28/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: 3cbe14f8d458c5d9631e0595912afa8cbb87b9de
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8923633"
---
# <a name="scheduling-modes"></a>Antolaketa moduak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_


Dynamics 365 Project Operations gaitasuna ematen die erakundeei lanaren banakako egituraren zereginetan aldagai gakoen aldaketak nola kudeatzen dituzten definitzeko. Erakundearen behar espezifikoetan oinarrituta, proiektuen arduradunek planifikazio moduan aldaketak egin ditzakete proiektu bat sortzen denean.

Project Operations-en hiru programazio modu daude eskuragarri:

  - Iraupen finkoa (modu lehenetsia da)
  - Ahalegin finkoa (*Lana*)
  - Unitate finkoak

Programazio modu zehatz baten definizioak eragindako balioak honako formula honen bidez zehazten dira:

  Esfortzua = Iraupena x Unitateak

Proiektu baten antolaketa modua definitzen duzunean, balio horietako bat ezartzen ari zara, gero aldatu ezin direnak. Balio hori konstante gisa mantentzeak lehentasuna ematen dio balio horri, eta horrek sistemari beste bi balioak aldatzen direnean ez aldatzeko jakinarazten dio. Ondorengo taulan modu zehatz bat hautatzearen eraginari buruzko informazioa ematen da.

| **Zereginean**             | **Unitateak berrikusten badituzu**   | **Iraupena berrikusten baduzu** | **Esfortzua berrikusten baduzu**  |
|----------------------|---------------------------|----------------------------|---------------------------|
| Unitate-zeregin finkoak     | Iraupena berriro kalkulatzen da. | Ahalegina berriro kalkulatzen da.    | Iraupena berriro kalkulatzen da. |
| Ahalegin finkoaren zeregina    | Iraupena berriro kalkulatzen da. | Unitateak berriro kalkulatzen dira.    | Iraupena berriro kalkulatzen da. |
| Iraupen finkoko zeregina  | Ahalegina berriro kalkulatzen da.   | Ahalegina berriro kalkulatzen da.    | Unitateak berriro kalkulatzen dira.   |

Modu jakin baten inplikazioei buruzko informazio gehiago lortzeko, ikusi [Aldatu zeregin mota programazio zehatzagoa lortzeko](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72). Gaian, terminoa **Lana** ordez erabiltzen da **Esfortzua**.

## <a name="change-the-organizations-scheduling-mode"></a>Aldatu erakundearen programazio modua

Osatu urrats hauek erakunde baten antolaketa modua definitzeko.

1. Joan **Ezarpenak**\> **Orokorra** \> **Parametroak** aukerara, eta hautatu proiektuaren parametroa. 
2. **Proiektuaren parametroak** orrialdean, hautatu antolaketarako antolaketa modu lehenetsia eta, ondoren, proiektuaren kudeatzaileak proiektu berria sortzerakoan ezarpena gainidazteko duen gaitasuna definitu.

## <a name="change-the-scheduling-mode-setting-on-a-project"></a>Aldatu proiektu baten antolaketa moduaren ezarpena

Erakunde batek proiektuaren kudeatzaileari antolaketa modu lehenetsia gainbideratzen uzten badio, proiektuaren kudeatzaileak proiektu hori sortzen duenean aldaketa hori egin dezake. Hala ere, proiektua gorde eta gero, ezin da planifikazio modua aldatu.

## <a name="copied-projects"></a>Kopiatutako proiektuak

Kopiatu proiektuaren ekintza egiten denean proiektu bat sortzen denez, Proiektu kudeatzaileak ezin du planifikazio modua ezarri. Helmugako proiektuak beti antolaketa mailan definitutako modua lehenetsiko du.

## <a name="copied-tasks"></a>Kopiatutako zereginak

Zeregin bat proiektu batetik bestera kopiatzen denean, zereginak helmugako proiektuaren antolaketa modua heredatzen du.
