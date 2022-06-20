---
title: Konfiguratu azpikontratatzaileak baliabide erreserbagarri gisa
description: Artikulu honetan, sisteman erabiltzaile eta kontaktuetatik sortzen diren azpikontratisten baliabideak nola konfiguratu eta mantendu azaltzen da, Microsoften azpikontratuekin elkartu ahal izateko Dynamics 365 Project Operations.
author: rumant
ms.date: 07/28/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: f005a05fb874f9e32a0041db5fc8fa1228fc91f1
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8927497"
---
# <a name="set-up-subcontractors-as-bookable-resources"></a>Konfiguratu azpikontratatzaileak baliabide erreserbagarri gisa

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Jarraitu urrats hauek azpikontratatuak erreserbatzeko baliabide gisa konfiguratzeko Microsoft Dynamics 365 Project Operations-en.

1. Joan **Proiektua** \> **Baliabideak** aukerara eta hautatu **Berria**.
2. Gainean **Erreserbatzeko baliabide berria** orrialdean, **Baliabide mota** eremuan, hautatu aukera hauetako bat:

    - **Erabiltzailea**: aukeratu baliabide mota hau azpikontratistak Project Operations-era sartu behar badu denbora edo gastuak sartzeko. Hautatzen baduzu **Erabiltzailea**, azpikontratistak baliozko lizentzia behar du sistemara sartzeko.
    - **Kontaktua** edo **Kontua**: aukeratu baliabide mota hauetako bat azpikontratistak Project Operations-erako sarbidea behar ez badu, baina eginkizunak esleitzeko edo proiektuen erreserbetarako eskuragarri egon behar badu. Baliabide mota hauetakoren batek ere ez du sistemarako sarbidea eskaintzen. Aukeratu **Kontua** saltzailearen enpresa ordezkatzeko baliabide erreserbagarri gisa. Aukeratu **Kontaktua** saltzailearen banakako langileak ordezkatzeko.

3. Aukeratu duzun baliabide motaren arabera, dagokion erabiltzailea, kontua edo harremanetarako erregistroa hautatzeko eskatuko zaizu.
4. Urtean **Langile mota** eremuan, hautatu "Kontratupeko langilea" azpikontratista erreserbatzeko baliabide gisa konfiguratzeko.

    > [!NOTE]
    > Uzten baduzu **Langile mota** eremua hutsik dagoenean, erreserbatuko den baliabidea langiletzat hartuko da.

5. Aukeratu baduzu **Kontratuetako langilea** langile mota gisa, hautatu baliabideak lan egiten duen saltzailea.
6. Aukeratu baliabidearen ordu zona, eta hautatu **Gorde**. Laneko ordu txantiloia erreserbatzeko baliabideari esleitzeko, hauta dezakezu **Ezarri egutegia** gainean **Erreserbatzeko Baliabidea** zerrenda orria.

Azpikontratuaren lerroko baliabidearrekin erlazionatuta egoteko, honako baldintza hauek bete behar ditu baliabide-erreserbagarriak:

- Erreserbatu daitekeen baliabideak itunpeko langilea izan behar du.
- Webguneko baliabide erreserbagarria **Kontaktua** baliabide mota saltzailearen kontuarekin lotu behar da kontaktu gisa. Webguneko baliabide erreserbagarria **Erabiltzailea** baliabide mota ez du egon behar saltzailearen kontuarekin erlazionatuta.
- Balioa **Saltzailea** erreserbatzeko baliabidearen eremuak **Saltzailea** azpikontrataren eremua.

## <a name="update-the-type-of-worker-and-vendor-mapping-for-bookable-resources"></a>Eguneratu baliabide erreserbagarrien langile eta saltzaileen mapa mota

**Langile mota** baliabide erreserbagarriaren eremuak zehazten du baliabide erreserbagarria kontratuko langilea edo langilea den. **Saltzailea** eremuak erreserbatzeko baliabidearekin lotzen den saltzailearen kontua definitzen du. Erreserbatzeko baliabide bat saltzaile batekin kontaktu gisa lotzen baduzu, kontaktua saltzailearen enpresako langilea dela adierazten duzu.

Bada **Langile mota** eta **Saltzailea** erreserbatzeko baliabide baten eremuak aldatu egiten dira, aldaketek erreserbatzeko baliabideak sortzen dituen erregistro berrietako balidazioei eragiten diete, hala nola denbora sarrerak. Hala ere, aldaketek ez dituzte lehendik dauden erregistroak baliogabetzen.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
