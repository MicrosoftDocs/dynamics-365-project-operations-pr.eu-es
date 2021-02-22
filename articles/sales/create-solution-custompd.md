---
title: Sortu prezio-dimentsio pertsonalizatuetarako soluzioa
description: Gai honek prezio-dimentsio pertsonalizatuetarako soluzioak sortzeko informazioa eskaintzen du.
author: Rumant
manager: tfehr
ms.date: 11/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 441501dff23d16960381b3f9fb4b2cceba2b3ba5
ms.sourcegitcommit: 869bde007805ef255f61b03937e4a44aeef61df9
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/12/2020
ms.locfileid: "4513955"
---
# <a name="create-a-solution-for-custom-pricing-dimensions"></a>Sortu prezio-dimentsio pertsonalizatuetarako soluzioa

 _**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_ 

>[!IMPORTANT]
>Prezio pertsonalizatuen dimentsio aldaketa guztiek beste irtenbide batean egon behar dute. Praktika on garrantzitsu honek malgutasuna eskaintzen du aldaketak eguneratzeko edo kentzeko, zure lana berrerabiltzen lagunduko du eta aldaketak beste instantzia batera eramatea erraztuko du. Beharrezko aldaketa guztiak egin ondoren, esportatu soluzioa **Kudeatuta** soluzio gisa, eta inportatu beste instantzia batzuetan zure prezioen konfigurazioa berrerabiltzeko.

## <a name="create-a-solution-for-custom-pricing-dimensions"></a>Sortu prezio-dimentsio pertsonalizatuetarako soluzioa

1.  Aukeratu **Ezarpenak** > **Soluzioak** eta, ondoren, hautatu **Berria**.
2.  Eman izena irtenbideari, *<your organization name> prezioen neurriak*.
3. Sartu geratzen den informazioa eta, ondoren, hautatu **Gorde** aukeran.

  ![Prezio-dimentsio pertsonalizatuen dimentsio-soluzioa sortzea](./media/Creation-of-custom-pricing-dimension-solution.png)
 
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a>Gehitu beharrezko entitate guztiak eta horiekin lotutako osagaiak prezio-dimentsioaren soluzioan

Gehitu Project Service entitate hauek zure prezioen soluziora prezioen soluzioan eskema aldaketa garrantzitsuak egiteko. Prozedura hau amaitu ondoren, entitateek prezioen dimentsio berriak ezagutuko dituzte.

1.  Hautatu **Ezarpenak** > **Soluzioak** atalean eta ondoren egin klik bikoitza **<*zure erakundearen izena*> prezioen dimentsioak** atalean.
2.  Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Gehitu badaudenak** > **Entitateak**.
3.  **Soluzio-osagaiak** elkarrizketa-koadroan, hautatu aukera hauetariko bat:
 
   - **Unekoa"**
   - **Baliabide erreserbagarria**
   - **Aurreikuspenaren lerroa**
   - **Proiektuaren zeregina**
   - **Fakturaren lerroaren xehetasunak**
   - **Kutxako liburuaren lerroa**
   - **Proiektu-kontratuaren lerroko xehetasunak**
   - **Proiektu-taldeko kidea**
   - **Eskaintzaren lerroaren xehetasunak**
   - **Funtzio-prezioaren gainprezioa**
   - **Funtzioaren prezioa**
   - **Denbora-sarrera**
 
   ![Gehitu lehendik dauden entitateak prezio-dimentsioaren soluzioari](./media/Existing-entities-to-PD-solution.png)
 
 4. Entitate bakoitzerako, berrikusi gehitzen diren osagaiak eta entitate bakoitzaren entitateen aktiboen behin betiko zerrenda. 

   >[!NOTE]
   > Sartu aukeratutako erakunde bakoitzerako inprimaki eta ikuspegi guztiak.

  ![Gehitutako entitateak](./media/solution-component-selection.png)


5.  Hautatutako entitateen menpeko entitateak sartzeko eskatzen zaizunean, hautatu **Ez, ez sartu beharrezko osagaiak**.

    ![Menpeko erakundeak barne](./media/Do-not-include-required.png)