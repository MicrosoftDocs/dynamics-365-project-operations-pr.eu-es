---
title: Inplementatu Project Operations Lite
description: Gai honek Project Operations lite hedapena instalatzeko moduari buruzko informazioa eskaintzen du. Aurre egin fakturazio proformari.
author: stsporen
ms.date: 11/29/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 2c508f56b3018b6a86fea78bcf9ee4136e90f385
ms.sourcegitcommit: 38cb012502cbd640abbc21a0912b195112b27ccb
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/30/2022
ms.locfileid: "9810963"
---
# <a name="deploy-project-operations-lite"></a>Inplementatu Project Operations Lite

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_



Project Operations-ek inplementazio eredu ugari onartzen ditu. Inplementazio eredu onena zehazteko, ikusi [Inplementazio motak](determine-deployment-type.md).


> [!IMPORTANT]
> Inplementazio honek, Lite inplementazioa - proformaren fakturazioari aurre egiten dio **Dataverse -Project Operations-en inplementazioa soilik**.

- [Instalatu Project Operations Dataverse ingurune berrian](#new)
- [Instalatu lehendik dagoen Dataverse ingurune batean](#existing)
- [Instalatu lehendik dagoen Dataverse ingurune batean, idazketa bikoitzeko osagaiak dituena](#existingdw)



## <a name="install-project-operations-lite-to-a-new-dataverse-environment"></a><a name="new"></a> Instalatu Project Operations Lite Dataverse ingurune berri batean

1. [Globala edo Power Platform Administratzailea](/power-platform/admin/global-service-administrators-can-administer-without-license) Project Operations lizentziarekin, sortu Dataverse ingurune berria [PowerPlatform administrazio-zentroan](https://admin.powerplatform.com). Ziurtatu hori **Sortu datu-base bat ingurune honetarako** eta **Dynamics 365 aplikazioak** gaituta daude. Informazio gehiago lortzeko, ikusi [Sortu eta kudeatu inguruneak Power Platform administrazio-zentroan](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).
1. Aukeratu **Microsoft Dynamics 365 Project Operations** Dynamics 365 aplikazioen hedapen zerrendatik.


## <a name="install-project-operations-lite-to-an-existing-dataverse-environment"></a><a name="existing"></a> Instalatu Project Operations Lite lehendik dagoen Dataverse ingurune batean 
1. [Orokorra edo Power Platform Administratzaile](/power-platform/admin/global-service-administrators-can-administer-without-license) gisa Project Operations lizentziarekin, kokatu ingurunea [PowerPlatform administrazio-zentroa](https://admin.powerplatform.com) Project Operations instalatu nahi dituzunean.
1. Instalatu **Microsoft Dynamics 365 Project Operations** Dynamics 365 aplikazioen hedapen zerrendatik. Informazio gehiago eskuratzeko, irakurri [Kudeatu Dynamics 365 aplikazioak](/power-platform/admin/manage-apps).

## <a name="install-project-operations-lite-to-an-existing-dataverse-environment-where-dual-write-solutions-are-already-present"></a><a name="existingdw"></a> Instalatu Project Operations Lite lehendik dagoen Dataverse ingurune batean, non idazketa bikoitzeko soluzioak dauden

Lite Deployment moduan Proiektu Eragiketak exekutatzen jarraitu nahi baduzu, urrats hauek jarraitu beharko dituzu:

1. [Orokorra edo Power Platform Administratzaile](/power-platform/admin/global-service-administrators-can-administer-without-license) gisa Project Operations lizentziarekin, kokatu ingurunea [PowerPlatform administrazio-zentroa](https://admin.powerplatform.com) Project Operations instalatu nahi dituzunean.
1. Instalatu **Microsoft Dynamics 365 Project Operations** Dynamics 365 aplikazioen hedapen zerrendatik. Informazio gehiago eskuratzeko, irakurri [Kudeatu Dynamics 365 aplikazioak](/power-platform/admin/manage-apps).
1. Zure inguruneak finantza- eta operazio-aplikazioetan integratzen laguntzen duten idazketa bikoitzeko osagaiak dituenez instalatuta, Project Operations-en instalazioak Proiektuarekin erlazionatutako datuak finantza- eta operazio-aplikazioetan integratzeko beharrezkoak diren gaitasun eta luzapenak ere instalatuko ditu. Proiektu Eragiketak Lite inplementazioan exekutatu nahi dituzunez, integrazio-osagai hauek kendu egin behar dira, Lite inplementatzeko agertokietarako murrizketak eta gainkostuak sortuko baitituzte. Eskuz desinstalatu soluzioak **Dynamics 365 Project Operations Dual Write** eta **Dynamics 365 Project Operations Dual Write Entity Maps** osagai horiek kentzeko.
1. Joan **Proiektuaren Eragiketak -> Ezarpenak -> Parametroak**. Ireki **Proiektuaren parametroa** xehetasun orria eta ezarri **Solution Upgrade Portaera** eremua **Lite gisa. Bakarrik**. Horrek bermatzen du Project Operations-en ondorengo eguneratzeek ez dituztela berreskuratuko integrazio-osagaiak Project Operations-etan.  

[!INCLUDE[footer-include](../includes/footer-banner.md)]
