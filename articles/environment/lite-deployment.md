---
title: Inplementatu Project Operations - arina
description: Gai honek Project Operations lite hedapena instalatzeko moduari buruzko informazioa eskaintzen du. Aurre egin fakturazio proformari.
author: stsporen
ms.date: 02/28/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 86293b725e86db3d4b8bdaf5810b16b7c670e8a3
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8930303"
---
# <a name="deploy-project-operations---lite"></a>Inplementatu Project Operations - arina

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_



Project Operations-ek inplementazio eredu ugari onartzen ditu. Inplementazio eredu onena zehazteko, ikusi [Inplementazio motak](determine-deployment-type.md).


> [!IMPORTANT]
> Inplementazio honek, Lite inplementazioa - proformaren fakturazioari aurre egiten dio **Dataverse -Project Operations-en inplementazioa soilik**.

- [Instalatu Project Operations Dataverse ingurune berrian](#new)
- [Instalatu lehendik dagoen Dataverse ingurune batean](#existing)



## <a name="install-project-operations-to-a-new-dataverse-environment"></a><a name="new"></a>Instalatu Project Operations Dataverse ingurune berri batean

1. [Globala edo Power Platform Administratzailea](/power-platform/admin/global-service-administrators-can-administer-without-license) Project Operations lizentziarekin, sortu Dataverse ingurune berria [PowerPlatform administrazio-zentroan](https://admin.powerplatform.com). Ziurtatu hori **Sortu datu-base bat ingurune honetarako** eta **Dynamics 365 aplikazioak** gaituta daude. Informazio gehiago lortzeko, ikusi [Sortu eta kudeatu inguruneak Power Platform administrazio-zentroan](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).
2. Aukeratu **Microsoft Dynamics 365 Project Operations** Dynamics 365 aplikazioen hedapen zerrendatik.


## <a name="install-project-operations-to-an-existing-dataverse-environment"></a><a name="existing"></a>Instalatu Project Operations lehendik dagoen Dataverse ingurune batean
1. Ziurtatu ingurunea ez dela konfiguratu [idazkera bikoitza](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-overview) instalazioak orduan instalatuko baitu [Baliabideetan/ez hornitutako agertokietarako Project Operations](project-operations-integrated-deployment-overview.md) gaitasunak.
2. [Orokorra edo Power Platform Administratzaile](/power-platform/admin/global-service-administrators-can-administer-without-license) gisa Project Operations lizentziarekin, kokatu ingurunea [PowerPlatform administrazio-zentroa](https://admin.powerplatform.com) Project Operations instalatu nahi dituzunean.
3. Instalatu **Microsoft Dynamics 365 Project Operations** Dynamics 365 aplikazioen hedapen zerrendatik. Informazio gehiago eskuratzeko, irakurri [Kudeatu Dynamics 365 aplikazioak](/power-platform/admin/manage-apps).




[!INCLUDE[footer-include](../includes/footer-banner.md)]
