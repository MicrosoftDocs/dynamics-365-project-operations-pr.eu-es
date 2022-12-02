---
title: Utzi aurrez onartutako denbora- eta gastu-sarrerak
description: Gai honek aldez aurretik onartutako proiektu baten denbora- edo gastu-transakzioa uzteari buruzko informazioa eskaintzen du.
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 03/07/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: 840f163ee9bf1fc98f140efdcc0d37a5424ddb8f
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8933293"
---
# <a name="cancel-previously-approved-time-or-expense-entries"></a>Utzi aurrez onartutako denbora- edo gastu-sarrerak

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Dynamics 365 Project Service Automation-en azken bertsioan, onuradunek aurretik onartu dituzten denbora- edo gastu-sarrerak utzi ditzakete.

## <a name="cancel-a-previously-approved-time-or-expense-entry"></a>Utzi aurrez onartutako denbora- edo gastu-sarrera

Jarraitu urrats hauei aurretik onartutako denbora- edo gastu-sarrera uzteko.

1. Joan **Proiektuak** \> **Nire lana** \> **Onartutakoak** atalera.
2. **Onartutakoak** zerrenda-orrian, aldatu ikuspegia **Nire iraganeko onespenak** egoerara. Aurretik onartu zenituen denbora- eta gastu-sarreren zerrenda agertzen da.
3. Hautatu sarrera bat edo gehiago eta, ondoren, hautatu **Utzi onespena**. Abisu mezu bat jasoko duzu.
4. Hautatu **Utzi** onarpena uzteko.

## <a name="understand-the-impact-of-canceling-a-time-or-expense-entry-approval"></a>Denbora edo gastuak sartzeko baimena baliogabetzeak izan dezakeen eragina ulertu

Onarpena bertan behera uzten denean, bai eragiketa-eragina eta bai finantza-eragina daude.

### <a name="operational-impact"></a>Eragile operazionala

Eragiketen aldean, onespena uzten denean, erregistroaren egoera berrezarri da **Zirriborroa** egoeran, eta onarpena ez da agertzen **Nire iraganeko onespenak** ikuspegian Horren ordez, utzitako onarpena agertzen da **Onarpena emateko denbora-sarrerak** ikuspegian edo **Onarpena emateko gastu-sarrerak** ikuspegian, denbora- edo gastu-sarrera izan den ala ez kontuan hartuta. Gainera, erlazionatutako denbora- edo gastu-sarreren egoera aldatu egiten da **Bidalita** egoerara, eta, beraz, lotura dagokion egoera **Zirriborroa** egoera duten onarpenekin bat etorriko da.

Onartzaile gisa, **Zirriborroa** egoera duten onarpen eremu batzuk editatu ditzakezu. Eremu horien artean daude **Fakturazio mota** eta **Denbora-sarrerarako fakturatu daitezkeen orduak**. Aldaketak egin ondoren, berriro onartu dezakezu erregistroa. Bestela, sarrera ukatu dezakezu. Denbora-sarrera baten onespena ukatzen baduzu, sarreraren egoera aldatu egingo da **Itzulia** egoerara. Gastu-sarrera baten onespena ukatzen baduzu, sarreraren egoera aldatu egingo da **Ukatuta** egoerara. Funtzionalki, itzultutako eta ukatutako sarrerek **Zirriborroa** egoeraren bat duen sarreren antzera funtzionatuko dute. Proiektuko taldekide batek sarrerako beharrezko aldaketak egin ditzake eta, ondoren, berriro bidali, onartzeko edo, bestela, ezabatu egin dezake.

### <a name="financial-impact"></a>Eragin ekonomikoa

Proiektu bat ere ekonomikoki kaltetuta dago onespen bat uzten denean. Lehenik eta behin, kostuari eta salmentei dagozkien datu errealak era honetara eguneratzen dira:

- Doikuntzaren egoera ezarrita dago **Doituta** egoerara.
- Fakturazioaren egoera ezarrita dago **Utzita** egoerara.

Ondoren, itzulera-sarrerak Datu errealak taulan sortzen dira. Itzulera-sarrerak sortzeko, sistemak eremuko balioak baino gehiago kopiatzen ditu jatorrizko datu errealetatik. Kopiatzen ez diren balio bakarrak kantitatearen balioak dira. Horren ordez itzuli egiten dira balio horiek. Itzulitako datu errealak hauetarako sortzen dira: **Kostua** eta **Fakturatu gabeko salmentak**. **Egokitzearen egoera** eremua, itzulitako datu errealetan, **Egokiezina** eremuan ezarrita dago eta fakturazio-egoera ezarrita dago **Utzita** egoeran.

Aldaketa horiek egin ondoren, proiektuan gastatu bezala erregistratzen diren diru-sarrerak eta proiektuan egindako sarreren atzerapenak denbora gehiago izango dute gertaera horiek ordezkatzen dituzten kontuak baino.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
