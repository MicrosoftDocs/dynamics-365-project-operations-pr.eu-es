---
title: Proiektu bat kontratudun langileekin eta azpikontratatutako ahalmenarekin hornitzea
description: Artikulu honetan azaltzen da nola hornitu daitezkeen proiektuko baldintzak, kontratatutako langileen edo Microsoften azpikontratatutako gaitasunaren bidez Dynamics 365 Project Operations.
author: rumant
ms.date: 12/03/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 173e1c20d2d046ee2120ec178e51d4868b70847d
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8922069"
---
# <a name="staffing-a-project-with-contract-workers-and-subcontracted-capacity"></a>Proiektu bat kontratudun langileekin eta azpikontratatutako ahalmenarekin hornitzea

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proiektuko lantaldeko kide generikoak enplegatuak edo kontratatutako langileak izan daitezke. Kontratatutako langileak dituen proiektu bati langileak ematean, azpikontratazio-lerro bati esleituta dauden langile kontratatu espezifikoei mugatu ahal izango dizkie langileak hornitzeko aukerak. 

## <a name="search-for-staff-resource-requirements-with-contract-workers-that-belong-to-a-specific-subcontract-line"></a>Azpikontratu espezifikoko linea bateko langile kontratatuak dituzten langileen baliabideen betekizunak bilatzea

Azpikontratu espezifikoko linea bateko langile kontratatuak dituzten langileen baliabideen baldintzak eta baldintzak bilatzeko, jarraitu pauso hauek:

1. Proiektuko lantaldeko kide generiko bat sortzen du, azpikontratu bat eta azpikontratu-lerro bat aipatuko duena.
2. Proiektuko taldeko kide generiko honentzat baliabide-betekizun bat sortzen du **, proiektuko taldeko kideen azpi-kuadrikulan baldintza** sortzea botoiaren bidez.
3. Aukeratu taldeko kideen ilara eta, ondoren, **aukeratu erreserba-botoia** azpi-kuadrikulan. 
4. Horrek programazio taula irekitzen du, baldintza-testuinguruarekin. Beste atributu batzuekin batera, hala nola data-eremuekin, rolekin eta antolaketa-unitateekin, programazio-batzordearen iragazkiak automatikoki betetzen dira baliabide-betekizunaren hornitzaile-lerro-eremuekin, azpikontratuarekin eta azpikontratuarekin.
5. Sistemak iragazki-irizpideak betetzen dituzten eta zerrendatzen dituzten baliabideak bilatzen ditu. 
6. Hautatu iragaztutako baliabideetako bat eta gorde ezazu baldintzarako baliabidea. 
7. Proiektu-taldeko kide bat sortu eta eguneratzen da, azpikontratu eta azpikontratoen lerroen erreferentziekin. Zoaz proiektuaren estimazioetara **eta** aukeratu **prezioak** eguneratzea, baliabideen esleipenaren kostu eguneratua ikusteko. 

> [!NOTE]
> Proiektuko taldeko kidea azpikontratu-lerroaren eta azpikontratuaren erreferentzia batekin eguneratzea ez da beti posible izango erreserban, baldin eta baliabidea azpikontrato-lerro batzuei esleitzen bazaio. Sistemak ezin badu proiektuko taldeko kidea eguneratu azpikontratu eta azpikontrato lerro batekin, ireki proiektuko taldeko kideen erregistroa, eta eremu horiek eskuz eguneratu, finantza-kostuaren zenbatespenak azpikontratistaren kostua zehaztasunez isla dezan.

## <a name="search-for-and-staff-resource-requirements-with-any-contract-worker"></a>Kontratatutako edozein langilerekin langile-baliabideak bilatzea eta baldintzak

Kontratatutako edozein langilerekin langile-baliabideak bilatzeko eta baldintzak betetzeko, jarraitu pauso hauek:

1. Proiektuaren taldeko kide generiko bat sortzen du.
2. Proiektuko taldeko kide generiko honentzat baliabide-betekizun bat sortzen du **, proiektuko taldeko kideen azpi-kuadrikulan baldintza** sortzea botoiaren bidez.
3. Aukeratu taldeko kideen ilara eta, ondoren, **aukeratu erreserba-botoia** azpi-kuadrikulan. 
4. Horrek programazio taula irekitzen du, baldintza-testuinguruarekin. Beste atributu batzuekin batera, hala nola data-eremuekin, rolekin eta antolaketa-unitateekin, programazio-batzordearen iragazkiak automatikoki betetzen dira baliabide-betekizunaren hornitzaile-lerro-eremuekin, azpikontratuarekin eta azpikontratuarekin. Betekizunak azpikontrato-lerroaren edo azpikontratu betearen inolako baliorik ez zuenez, atributu horiek hutsik egongo dira iragazki-panelean.
5. Sistemak iragazki-irizpideak betetzen dituzten eta zerrendatzen dituzten baliabideak bilatzen ditu.
6. Langile motaren **alorra** eguneratu langile kontratatuen **filtro-panelean,** kontratatutako langileen bilaketa mugatzeko. **Hornitzaileak** iragazki-panelean eguneratu, bilaketa mugatzen duen hornitzaile bat aukeratzeko, enpresa hornitzaile espezifiko bateko langile kontratatuak bakarrik agintzeko.
7. Zerrendako langile kontratatu bat hautatu eta gorde betekizunerako errekurtsoa.
8. Proiektuaren taldeko kide bat sortzen da. Hala ere, proiektuko lantaldeko kidea ez azpikontratoarekin edo azpikontrato-lerro batekin eguneratuta, eta, beraz, baliabideen esleipena ez da kalkulatuko azpikontratuaren prezioak erabiliz. Eguneratu proiektuko taldeko kidea azpikontratu-lerro batekin eta proiektuaren estimazioetara **joan** eta **prezioak** eguneratu, baliabideen esleipenaren kostu eguneratua ikusteko.

> [!NOTE]
> Proiektuko taldeko kideek langile mota kontratatuta **dute**, baina ez dute azpikontrato **erreferentziarik, eta proiektuko** taldeko kideen **laukian ez dute balio**.**·** Proiektu-taldeko kideren bat baldin badago estatu horrekin, ireki proiektu-taldeko kideen erregistroa, eta eskuz eguneratu azpikontratoko eta azpikontratoko lerro-eremuak, finantza-kostuen zenbatespenak zehaztasunez isla dezan azpikontratistak betilean **duen** kostua. 


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
