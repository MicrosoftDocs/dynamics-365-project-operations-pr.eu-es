---
title: Sortu prezio-dimentsioen soluzio pertsonalizatuak
description: Gai honek prezio pertsonalizatuko neurriak sortzerakoan irtenbide pertsonalizatua nola sortu azaltzen du.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 3e437fce5b9f1fb330a713788e24100a4fe02948
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071045"
---
# <a name="create-custom-solutions-for-pricing-dimensions"></a>Sortu prezio-dimentsioen soluzio pertsonalizatuak

> [!IMPORTANT]
> Prezio pertsonalizatuen dimentsio aldaketa guztiek beste irtenbide batean egon behar dute. Praktika on garrantzitsu honek etorkizunean malgutasuna eskaintzen du aldaketak eguneratzeko edo kentzeko, zure lana berrerabiltzen lagunduko du eta aldaketak beste instantzia batera eramatea erraztuko du. Beharrezko aldaketa guztiak egin ondoren, esportatu soluzioa **Kudeatutako soluzio** gisa, eta inportatu beste instantzia batzuetan zure prezioen konfigurazioa berrerabiltzeko.

1. Aukeratu **Ezarpenak** > **Soluzioak** eta, ondoren, hautatu **Berria**. 
2. Soluzioari eman **\<your organization name> prezio-dimentsioak** izena, sartu gainerako beharrezko informazioa eta, ondoren, hautatu **Gorde** aukeran.

> ![Sortu prezio-dimentsioetarako soluzio pertsonalizatua](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
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

> ![Gehitu lehendik dauden entitateak prezio-dimentsioen soluzioari](media/Existing-entities-to-PD-solution.png)

> ![Hautatu soluzioaren osagaiak](media/Dimension-Components.png)

> [!NOTE]
> Ziurtatu aukeratutako erakunde bakoitzerako inprimaki eta ikuspegi guztiak sartzea.

4. Hautatutako entitateen menpeko erakunderen bat eskatuko zaizunean, hautatu **Ez** aukeran.

> ![Ez sartu erlazionatutako osagaiak](media/Do-not-include-required.png)

