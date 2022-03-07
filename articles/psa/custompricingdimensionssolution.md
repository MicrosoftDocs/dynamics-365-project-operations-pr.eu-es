---
title: Sortu prezio-dimentsioen soluzio pertsonalizatuak
description: Gai honek prezio pertsonalizatuko neurriak sortzerakoan irtenbide pertsonalizatua nola sortu azaltzen du.
author: Rumant
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 4dea80d8e4645675d3e89e846532ca7c0f292faa328c45938941c50dc15486fc
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6995251"
---
# <a name="create-custom-solutions-for-pricing-dimensions"></a>Sortu prezio-dimentsioen soluzio pertsonalizatuak

[!include [banner](../includes/psa-now-project-operations.md)]

> [!IMPORTANT]
> Prezio pertsonalizatuen dimentsio aldaketa guztiek beste irtenbide batean egon behar dute. Praktika on garrantzitsu honek etorkizunean malgutasuna eskaintzen du aldaketak eguneratzeko edo kentzeko, zure lana berrerabiltzen lagunduko du eta aldaketak beste instantzia batera eramatea erraztuko du. Beharrezko aldaketa guztiak egin ondoren, esportatu soluzioa **Kudeatutako soluzio** gisa, eta inportatu beste instantzia batzuetan zure prezioen konfigurazioa berrerabiltzeko.

1. Aukeratu **Ezarpenak** > **Soluzioak** eta, ondoren, hautatu **Berria**. 
2. Soluzioari eman **\<your organization name> prezio-dimentsioak** izena, sartu gainerako beharrezko informazioa eta, ondoren, hautatu **Gorde** aukeran.

> ![Sortu prezio-dimentsioetarako soluzio pertsonalizatua.](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a>Gehitu beharrezko entitate guztiak eta horiekin lotutako osagaiak prezio-dimentsioaren soluzioan
Project Service-eko entitate hauek gehitu beharko dituzu prezio-soluzioan. Osatu prozedura honen urratsak prezio-soluzioaren eskema garrantzitsu batzuk egiteko, entitateak prezio-dimentsio berriez jabetzeko.

1. Hautatu **Ezarpenak** > **Soluzioak** eta, ondoren, sakatu bi aldiz **\<your organization name>prezio-dimentsioa**. 
2. Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Gehitu badaudenak** > **Entitateak**.
3. **Soluzio-osagaiak** elkarrizketa-koadroan, hautatu aukera hauetariko bat:

- Unekoa"
- Baliabide erreserbagarria
- Aurreikuspenaren lerroa
- Proiektuaren zeregina
- Fakturaren lerroaren xehetasunak
- Kutxako liburuaren lerroa
- Proiektu-kontratuaren lerroko xehetasunak
- Proiektu-taldeko kidea
- Eskaintzaren lerroaren xehetasunak
- Funtzio-prezioaren gainprezioa
- Funtzioaren prezioa 
- Denbora-sarrera 

> ![Gehitu lehendik dauden entitateak prezio-dimentsioen soluzioari.](media/Existing-entities-to-PD-solution.png)

> ![Hautatu soluzioaren osagaiak.](media/Dimension-Components.png)

> [!NOTE]
> Ziurtatu aukeratutako erakunde bakoitzerako inprimaki eta ikuspegi guztiak sartzea.

4. Hautatutako entitateen menpeko erakunderen bat eskatuko zaizunean, hautatu **Ez** aukeran.

> ![Ez sartu erlazionatutako osagaiak.](media/Do-not-include-required.png)




[!INCLUDE[footer-include](../includes/footer-banner.md)]