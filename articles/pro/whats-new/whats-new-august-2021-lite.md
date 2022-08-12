---
title: 2021eko abuztuko berritasunak - Project Operations lite-ren oinarrizko inplementazioa
description: Artikulu honek Project Operations lite inplementazioaren 2021eko abuztuko bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 08/10/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 84318a26d97355fe56794e1d1532576cde4af661
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8922023"
---
# <a name="whats-new-august-2021---project-operations-lite-deployment"></a>2021eko abuztuko berritasunak - Project Operations lite-ren oinarrizko inplementazioa

_Honi aplikatzen zaio: Oinarrizko inplementazioa: kudeatu proformako fakturak_

Artikulu hau honako hauei aplikatzen zaie Dynamics 365 Project Operations osagaiak eta bertsioak:

  - Project Operations Dataverse ingurunearen 4.13.0.152 bertsioa

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

Eginbide hauek sartzen dira bertsio honetan:

- **Onarpen multzoak**: Onarpenak taldearen denbora, gastua edo materialaren erabilera onartzeko eskaerak eragiketa azpimultzo txikiagoetan biltzen ditu. Multzo horri esker, onarpenak proiektuen arabera orden zehatz batean prozesatu daitezke eta berriro saiatzea eta sekuentziatzea ahalbidetzen du. Eskaerak multzokatzeak homologazioen prozesuen fidagarritasuna eta trazabilitatea hobetzen ditu homologazio kopuru handietan. Informazio gehiago lortzeko, ikusi [Onarpen ezarpenak](../../approvals/approval-sets.md).

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| **Ezaugarrien eremua** | **Erreferentzia-zenbakia** | **Kalitatearen eguneratzea** |
| --- | --- | --- |
| Fakturazioa eta prezioak | 2295625 | Mugarriaren izena fakturaren egitarautik fakturaren lerroaren xehetasunera kopiatu behar da. |
| Fakturazioa eta prezioak | 2316323 | Deskontua ez da Project Operations proforma fakturan editatu behar baliabideetan oinarritutako eszenatokietan. |
|   Abaguneen kudeaketa | 2338619 | **Aukera** eta **Aurrekontua** negozio arauak orrialdeetan soilik deitu behar dira. |
| Baliabideen kudeaketa | 2316523 | Erabiltzen **Bidali eskaera** rola erantsita duen baliabide eskakizunetik ez luke akatsik erakutsi behar. |
| Baliabideen kudeaketa | 2326885 | Baliabideen eskakizuna proiektu baten bidez sortzeak ez luke akatsik erakutsi behar. |
| Denbora eta gastua | 2335584 | Zaharkitako zereginak denbora sarreran isurtzen dira. |
| Denbora eta gastua | 2336884 | **Kopiatu Astea** denbora sartzeko botoiak uneko erabiltzailea baino gehiagorako funtzionatu behar du. |