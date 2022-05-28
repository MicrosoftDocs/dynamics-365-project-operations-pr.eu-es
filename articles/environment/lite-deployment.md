---
title: Inplementatu Project Operations - arina
description: Gai honek Project Operations lite hedapena instalatzeko moduari buruzko informazioa eskaintzen du. Aurre egin fakturazio proformari.
author: stsporen
ms.date: 02/28/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: e33506504665f2e7ef7ad48469082f9f64a2a44b
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8580717"
---
# <a name="deploy-project-operations---lite"></a>Inplementatu Project Operations - arina

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_



Project Operations-ek inplementazio eredu ugari onartzen ditu. Inplementazio eredu onena zehazteko, ikusi [Inplementazio motak](determine-deployment-type.md).


> [!IMPORTANT]
> Inplementazio honek, Lite inplementazioa - proformaren fakturazioari aurre egiten dio **Dataverse -Project Operations-en inplementazioa soilik**.

- [Instalatu Project Operations berri batean Dataverse ingurunea](#new)
- [Instalatu lehendik dagoen batean Dataverse ingurunea](#existing)



## <a name="install-project-operations-to-a-new-dataverse-environment"></a><a name="new"></a> Instalatu Project Operations berri batean Dataverse ingurunea

1. bezala [Globala edo Power Platform Administratzailea](/power-platform/admin/global-service-administrators-can-administer-without-license) Project Operations lizentzia batekin, sortu berri bat Dataverse ingurunean [PowerPlatform administrazio zentroa](https://admin.powerplatform.com). Ziurtatu hori **Sortu datu-base bat ingurune honetarako** eta **Dynamics 365 aplikazioak** gaituta daude. Informazio gehiago lortzeko, ikusi [Sortu eta kudeatu inguruneak Power Platform administrazio-zentroan](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).
2. Aukeratu **Microsoft Dynamics 365 Project Operations** Dynamics 365 aplikazioen hedapen zerrendatik.


## <a name="install-project-operations-to-an-existing-dataverse-environment"></a><a name="existing"></a> Instalatu Project Operations lehendik dagoen batean Dataverse ingurunea
1. Ziurtatu ingurunea ez dela konfiguratu [idazkera bikoitza](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-overview) instalazioak orduan instalatuko baitu [Baliabideetan/ez hornituta oinarritutako eszenatokietarako Proiektu Eragiketak](project-operations-integrated-deployment-overview.md) gaitasunak.
2. [Orokorra edo Power Platform Administratzaile](/power-platform/admin/global-service-administrators-can-administer-without-license) gisa Project Operations lizentziarekin, kokatu ingurunea [PowerPlatform administrazio-zentroa](https://admin.powerplatform.com) Project Operations instalatu nahi dituzunean.
3. Instalatu **Microsoft Dynamics 365 Project Operations** Dynamics 365 aplikazioen hedapen zerrendatik. Informazio gehiago eskuratzeko, irakurri [Kudeatu Dynamics 365 aplikazioak](/power-platform/admin/manage-apps).




[!INCLUDE[footer-include](../includes/footer-banner.md)]
