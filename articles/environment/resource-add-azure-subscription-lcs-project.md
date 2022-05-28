---
title: Gehitu Azure harpidetza LCS proiektu batean
description: Gai honek zure Azure harpidetza LCS proiektu batera konektatzeko moduari buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 04/12/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 839c510838b0bccb718b8ca8a4f71a1c46e7ea3f
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8595897"
---
# <a name="add-an-azure-subscription-to-an-lcs-project"></a>Gehitu Azure harpidetza LCS proiektu batean

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Hodeian ostatatutako inguruneak lehendik dagoen Azure harpidetza erabiliz inplementatu behar dira. Gai honek zure lehendik duzun Azure harpidetza LCS proiektu batera konektatzeko moduari buruzko informazioa azaltzen du. 

## <a name="grant-admin-consent"></a>Eman administratzailearen baimena

1. Zure LCS proiektuan, **Inguruneak** atala, hautatu **Microsoft Azure ezarpenak**.

![Microsoft Azure ezarpenak.](./media/1MicrosoftAzureSettings.png)

2. **Proiektuaren ezarpenak** orrialdean, **Azure konektoreak** fitxa, hautatu **Baimendu**. Horri esker, inguruneak proiektu honetara zabaldu daitezke.

![Azure konektoreak.](./media/2AzureConnectors.png)

3. Aukeratu **Baimendu** berriro administratzailearen baimena emateko.

![Eman administratzailearen baimena.](./media/3GrantAdminConsent.png)

4. Onartu baimen eskaera.

![Onartu baimen-eskaera.](./media/4AcceptPermissionRequest.png)

Baimena amaitu da. 

![Baimena arrakastatsua da.](./media/5AuthorizationComplete.png)

## <a name="provide-dynamics-deployment-services-access-to-your-azure-subscription"></a><a name="provide"></a>Eman Dynamics Deployment Services sarbidea Azure harpidetzarako

1. Joan [Microsoft Azure fakturazioa](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) aukerara eta hautatu harpidetza. Dynamics Deployment Services-ek harpidetza honetara sartu behar du inguruneak zabaldu ahal izateko.

![Azure harpidetzaren xehetasunak.](./media/6AzureSubscription.png)

2. Aukeratu **Sarbide kontrola (IAM)** nabigazio panelean, eta hautatu **Gehitu rol esleipena**.
3. Eskuineko aldean, hautatu **Laguntzaile-funtzioa**, eta emandako zerrendan, bilatu eta hautatu **Dynamics-en inplementazio-zerbitzuak**. 
4. Sakatu **Gorde**.

![Harpidetzaren sarbidea.](./media/7SubscriptionAccess.png)

### <a name="add-a-subscription-connector-to-an-lcs-project"></a>Gehitu harpidetzaren konektorea LCS proiektu batean

1. Zure LCS proiektuan **Microsoft Azure ezarpenak** orrialdean, hautatu **Gehitu** konektore berria gehitzeko.
2. Idatzi zure Azure harpidetzaren IDa. Zure Azure harpidetzaren IDa [Azure atarian](https://ms.portal.azure.com/), **Ezarpenak** pantailaren beheko ezkerrean.
3. **Konfiguratu Azure Resource Manager erabiltzeko** eremuan, hautatu **Bai**.
4. Ziurtatu Azure Harpidetzaren AAD maizter domeinua erabiltzen ari zaren domeinuaren jabe den Azure harpidetzarekin bat datorrela eta hautatu **Hurrengoa**.
5. **Microsoft Azure Konfigurazioa** pantailan, hautatu **Hurrengoa** baieztatzeko. Pantaila honetan errore bat jasotzen baduzu, itzuli [Eman Dynamics Deployment Services sarbidea Azure harpidetzarako](#provide) atalera gai honetan eta ziurtatu urrats guztiak bete dituzula.
6. Deskargatu Azure kudeaketa ziurtagiria zure ordenagailuko karpeta lokal batera. Eskatu Azure harpidetzaren administratzaileari ziurtagiria Azure Management Portal-era kargatzeko harpidetza hautatuta eta **Ezarpenak** > **Kudeaketa ziurtagiriak** aukerara joanda. Ziurtagiri honi esker, LCS-k Azure-rekin zure izenean komunikatzeko aukera ematen du. Urrats hau salta dezakezu zure erabiltzaileak harpidetzarako sarbidea badu.
7. Hautatu **Hurrengoa**.
8. Aukeratu zabaltzeko Azure eskualdea eta hautatu sistema hau erabiltzeko asmoa duzun tokitik gertu dagoen datu zentroa.
9.  Hautatu **Konektatu**.

Azure harpidetza behar bezala konektatu duzu. Orain Dynamics 365 Finance hodeian ostatatutako inguruneak inplementa ditzakezu.




[!INCLUDE[footer-include](../includes/footer-banner.md)]
