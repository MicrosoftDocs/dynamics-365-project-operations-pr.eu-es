---
title: Desinstalatu Dynamics 365 Project Operations
description: Gai honek Dynamics 365 Project Operations desinstalatzeko moduari buruzko informazioa eskaintzen du.
author: stsporen
ms.date: 11/09/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: b87c9324b1c95c10ef1e18b0fbf4572bdbe76827
ms.sourcegitcommit: b8b7a59eee7d93638446e93726d270316e45ab3d
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/10/2021
ms.locfileid: "7783628"
---
# <a name="uninstall-dynamics-365-project-operations"></a>Desinstalatu Dynamics 365 Project Operations 

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Dynamics 365 Project Operations desinstalatzeko, Administratzaile rola esleitu behar zaizu.

1. Joan **Ezarpenak** > **Soluzioak** atalera.

    ![Ezarpenen orria.](./media/uninstall-proj-ops-solutions.png)
  
2. Kendu disoluzioak hurrengo taulan ageri diren ordena zehatzean. 

    | Urratsa | Soluzioaren izena                                    | Oharra                                                                                         |
    |------|----------------------------------------------------|----------------------------------------------------------------------------------------------|
    | 1 | msdyn_ProjectServiceUpgrade_managed.cab            | Aurkitu ezean, saltatu irtenbide hau.                                                            |
    | 2 | ProjectOperations_Anchor                           | Aurkitu ezean, saltatu irtenbide hau.                                                            |
    | 3 | Dynamics365ProjectOperationsDualWriteEntityMaps    | Aurkitu ezean, saltatu irtenbide hau.                                                            |
    | 4 | Dynamics365ProjectOperationsDualWrite              | Aurkitu ezean, saltatu irtenbide hau.                                                            |
    | 5 | ProjectService                                     | Ez dago ohar gehigarririk.                                                                         |
    | 6 | ProjectServiceCore_Patch                           | Ez dago ohar gehigarririk.                                                                         |
    | 7 | ProjectServiceCore                                 | Ez dago ohar gehigarririk.                                                                         |
    | 8 | ProjectServiceDeprecatedComponents                 | Aurkitu ezean, saltatu irtenbide hau.                                                            |
    | 9 | FieldServiceCommon                                 | Beharrezkoa da Dynamics 365 Finance edo Dynamics 365 Supply Chain Management-ekin idazketa duala egiteko.   |
    | 10 | msdyn_AssetCommon                                  | Beharrezkoa da Dynamics 365 Finance edo Dynamics 365 Supply Chain Management-ekin idazketa duala egiteko.   |
    | 11 | msdyn_TESA_Anchor                                  | Beharrezkoa da Dynamics 365 Field Service-rako.                                                     |
    | 12 | msdyn_TESA_Patch                                   | Beharrezkoa da Dynamics 365 Field Service-rako.                                                     |
    | 13 | msdyn_TESA                                         | Beharrezkoa da Dynamics 365 Field Service-rako.                                                     |
    | 14 | ResourceSchedulingControls                         | Beharrezkoa da Dynamics 365 Field Service-rako.                                                     |
    | 15 | MicrosoftDynamicsScheduling3_CumulativePatch       | Beharrezkoa da Dynamics 365 Field Service-rako.                                                     |
    | 16 | MicrosoftDynamicsScheduling_Patch_xx               | Beharrezkoa da Dynamics 365 Field Service-rako.                                                     |
    | 17 | MicrosoftDynamicsScheduling                        | Beharrezkoa da Dynamics 365 Field Service-rako.                                                     |
    | 18 | Dynamics365FinanceAndOperationsAnchor              | Aurkitu ezean, saltatu irtenbide hau.                                                            |
    | 19 | Dynamics365Notes                                   | Aurkitu ezean, saltatu irtenbide hau.                                                            |
    | 20 | Dynamics365FinanceAndOperationsDualWriteEntityMaps | Aurkitu ezean, saltatu irtenbide hau.                                                            |
    | 21 | DualWriteCore                                      | Aurkitu ezean, saltatu irtenbide hau.                                                            |
    | 22 | Dynamics365AssetManagementApp                      | Aurkitu ezean, saltatu irtenbide hau.                                                            |
    | 23 | Dynamics365AssetManagement                         | Aurkitu ezean, saltatu irtenbide hau.                                                            |
    | 24 | Dynamics365SupplyChainExtended                     | Aurkitu ezean, saltatu irtenbide hau.                                                            |
    | 25 | Dynamics365FinanceExtended                         | Aurkitu ezean, saltatu irtenbide hau.                                                            |
    | 26 | HCMCommon                                          | Aurkitu ezean, saltatu irtenbide hau.                                                            |
    | 27 | Dynamics365FinanceAndOperationsCommon              | Aurkitu ezean, saltatu irtenbide hau.                                                            |
    | 28 | Jaia                                              | Aurkitu ezean, saltatu irtenbide hau.                                                            |
    | 29 | Dynamics365Company                                 | Aurkitu ezean, saltatu irtenbide hau.                                                            |
    | 30 | CurrencyExchangeRates                              | Aurkitu ezean, saltatu irtenbide hau.                                                            |
    | 31 | AssetCommon                                        | Aurkitu ezean, saltatu irtenbide hau.                                                            |
