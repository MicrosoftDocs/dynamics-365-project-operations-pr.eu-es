---
title: Saltzaileen eta erosketa prezioen zerrenden kudeaketa Project Operations-en
description: Artikulu honek saltzaileen datuak sortzen eta mantentzen lagunduko dizun informazioa eskaintzen du eta azpikontrataziorako erosteko prezioen zerrendak.
author: rumant
ms.date: 08/02/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 6840ffcbc510fe6385dd3fdaf881e9700c4fdd18
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8914111"
---
# <a name="vendor-and-purchase-price-list-management-in-project-operations"></a>Saltzaileen eta erosketa prezioen zerrenden kudeaketa Project Operations-en

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

## <a name="vendors-in-project-operations"></a>Project Operations-eko saltzaileak

Microsoft Dynamics 365 Project Operations-en, saltzaileen kontuek harreman mota dute **Saltzailea** edo **Hornitzailea**. Azpikontratako saltzaile gisa harreman mota horietako bat duen kontu erregistroa soilik hauta dezakezu.

Erosketa prezioen zerrenda bat edo gehiago saltzaileen erregistroarekin lotu ditzakezu. Hala ere, saltzailearen erregistroarekin lotutako erosketa prezioen zerrenda bakoitzak data eraginkortasuna izan beharko luke. Project Operations-ek ez du onartzen erosketen prezio-zerrenden dataren erabilgarritasuna gainidaztea.

Lehenespenez, saltzailearen erregistro bateko eremu eta kontzeptu hauek erabiltzen dira saltzailearentzat sortzen den azpikontrata egiteko:

- Ordainketa-baldintzak
- Kontaktuaren faktura
- Kontaktu nagusia

    > [!NOTE]
    > Berez, saltzailearen lehen kontaktua azpikontrataren saltzailearen kontu kudeatzaile gisa erabiltzen da.

- Moneta
- Uneko erosketaren prezio-zerrendak

## <a name="purchase-price-lists-in-project-operations"></a>Erosketa prezioen zerrendak Project Operations-en

Prezio zerrenda non **Testuingurua** eremua ezarrita dago **Erosketa** erosketa prezioen zerrendatzat hartzen da. Erosketa prezioen zerrendak defini daitezke denbora, gastu eta materialen erosketa tasen katalogoa irudikatzeko. Erosketa prezioen zerrendak Project Operations-eko kostuen eta salmenta prezioen zerrenden antza dute. Honako kontzeptuak erosketa prezio zerrendetan aplikatzen dira kostu eta salmenta prezio zerrendetan aplikatzen diren modu berean:

- **Data eraginkortasuna**: erosketa prezioen zerrendek data eraginkortasuna dute. Data eraginkortasuna prezio zerrenda bakoitzeko hasiera data eta amaiera data eremuek adierazten dute. Hasiera-data eta amaiera-dataren arteko denbora efektiboaren data da.
- **Moneta**: prezio zerrendaren goiburuko moneta erosketa prezioak katalogoko eskulanaren, gastuen kategorien eta produktuen adierazitako moneta gisa erabiltzen da.
- **Denbora-unitate lehenetsia**: denbora-unitate lehenetsiak erosketen lan-prezioak adierazten ditu. Prezio zerrendako denbora unitatearen eremua balio lehenetsia emateko soilik erabiltzen da. Balio hori rol bakoitzaren prezioen errenkadetan alda daiteke.

Erosketa prezioen zerrendak saltzaileen erregistroetara erants daitezke proiektuen prezioen zerrendak izenarekin ezagutzen diren elkarte gisa. Prezio zerrenda hauek azpikontratazio lerroetan lehenetsitako prezioak sartzeko erabiltzen dira. Berez, saltzaileen erregistroari erosketa prezioen zerrenda anitz eransten zaizkionean, uneko prezio zerrenda saltzaileari sortzen zaizkion azpikontratuetarako erabiltzen da. Prezioen zerrendak soilik **Testuingurua** eremua ezarrita dago **Erosketa** saltzailearen erregistroetara erants daiteke.

### <a name="subcontract-specific-purchase-price-lists"></a>Azpikontratatzeko berariazko erosketa prezioen zerrendak

Erosketa-prezioen zerrendak azpikontratuetan erants daitezke proiektuen prezioen zerrendak izenarekin ezagutzen diren elkarte gisa. Prezio zerrenda hauek azpikontratazio lerroetan lehenetsitako prezioak sartzeko erabiltzen dira. Berez, azpikontrata bati erosketa prezioen zerrenda bat gehitzen zaionean, bakoitzak data eraginkortasuna izan behar du. Project Operations-ek ez du onartzen daten erabilgarritasuna gainidatzita duten erosketen prezio-zerrendak. Prezioen zerrendak soilik **Testuingurua** eremua ezarrita dago **Erosketa** azpikontratuetara erants daiteke.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
