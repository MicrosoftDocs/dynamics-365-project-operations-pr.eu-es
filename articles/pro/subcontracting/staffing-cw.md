---
title: Proiektu bat kontratudun langileekin eta azpikontratatutako ahalmenarekin hornitzea
description: Artikulu honek Microsoft-en lan-kontratuko langileak edo azpikontratatutako gaitasuna erabiliz proiektuaren eskakizunak nola bete daitezkeen azaltzen du Dynamics 365 Project Operations.
author: rumant
ms.date: 12/03/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 8edb053467ef200ca3e051e2fd78106734318389
ms.sourcegitcommit: b2224d1f3c0bd4925d647e6ca3960db81a209521
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/11/2022
ms.locfileid: "9261239"
---
# <a name="staffing-a-project-with-contract-workers-and-subcontracted-capacity"></a>Proiektu bat kontratudun langileekin eta azpikontratatutako ahalmenarekin hornitzea

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proiektu-talde orokorreko kideak langileekin edo lan-kontratuko langileekin egon daitezke. Proiektu bat lan-kontratuko langileekin hornitzean, zure langile-aukerak muga ditzakezu azpikontratu-lerro batera esleitutako lan-kontratuko langile espezifikoetara. 

## <a name="search-for-staff-resource-requirements-with-contract-workers-that-belong-to-a-specific-subcontract-line"></a>Azpikontratazio-lerro zehatz bateko langile-kontratudunekin langile-baliabideen eskakizunak bilatu

Azpikontratazio-lerro zehatz bateko langile kontratudunekin langile-baliabideen eskakizunak bilatzeko eta bilatzeko, jarraitu urrats hauek:

1. Sortu proiektu-taldekide generiko bat, azpikontratu eta azpikontratu lerro bati erreferentzia egiten diona.
2. Sortu baliabide-eskakizuna proiektuko taldekide generiko honentzat **Sortu eskakizuna** proiektuko taldekideen azpi-sareko botoia.
3. Hautatu taldekideen errenkada eta, ondoren, hautatu **Liburua** azpi-sareko botoia. 
4. Honek Ordutegi-taula irekitzen du eskakizunen testuinguruarekin. Beste atributu batzuekin batera, hala nola, datak, rola eta antolakuntza-unitate-eremuak, Programazio-taularen iragazkiak automatikoki betetzen dira baliabide-eskakizuneko hornitzaile, azpikontratu eta azpikontratazio lerro-eremuekin.
5. Sistemak iragazki-irizpideak betetzen dituzten baliabideak bilatzen ditu eta zerrendatzen ditu. 
6. Aukeratu iragazitako baliabideetako bat eta erreserbatu baliabidea eskakizunerako. 
7. Proiektuko taldekide bat sortu eta eguneratzen da azpikontratazio eta azpikontratu lerroen erreferentziekin. Joan **Proiektuaren kalkuluak** eta hautatu **Eguneratu prezioak** baliabideen esleipenaren kostu eguneratua ikusteko. 

> [!NOTE]
> Proiektuko taldeko kidea azpikontratu eta azpikontratu lerroaren erreferentzia batekin eguneratzea baliteke beti ez izatea posible erreserba egiterakoan baliabidea azpikontratu lerro anitzetan esleituta badago. Sistemak ezin badu eguneratu proiektu-taldekidea azpikontratazio eta azpikontratazio-lerro batekin, ireki proiektuaren taldeko kideen erregistroa eta eguneratu eskuz eremu hauek, finantza-kostuen estimazioak azpikontratistaren kostua zehatz-mehatz isla dezan.

## <a name="search-for-and-staff-resource-requirements-with-any-contract-worker"></a>Bilatu eta langile-baliabide-eskakizunak edozein lan-kontratuko langileekin

Edozein lan-kontratuko langileekin langile-baliabide-eskakizunak bilatzeko eta bilatzeko, jarraitu urrats hauek:

1. Sortu proiektuko taldekide generiko bat.
2. Sortu baliabide-eskakizuna proiektuko taldekide generiko honentzat **Sortu eskakizuna** proiektuko taldekideen azpi-sareko botoia.
3. Hautatu taldekideen errenkada eta, ondoren, hautatu **Liburua** azpi-sareko botoia. 
4. Honek Ordutegi-taula irekitzen du eskakizunen testuinguruarekin. Beste atributu batzuekin batera, hala nola, datak, rola eta antolakuntza-unitate-eremuak, Programazio-taularen iragazkiak automatikoki betetzen dira baliabide-eskakizuneko hornitzaile, azpikontratu eta azpikontratazio lerro-eremuekin. Eskakizunak ez zuelako azpikontratazio edo azpikontratazio lerroko baliorik bete, atributu hauek hutsik egongo dira iragazkien panelean.
5. Sistemak iragazki-irizpideak betetzen dituzten baliabideak bilatzen ditu eta zerrendatzen ditu.
6. Eguneratu **Langile mota** iragazki-paneleko eremua **Lan-kontratuko langilea** bilaketa lan-kontratuko langileei mugatzeko. Eguneratu **Saltzailea** iragazkien panelean, hornitzaile bat hautatzeko bilaketa mugatzeko, hornitzaile-enpresa zehatz bateko lan-kontratuko langileak soilik erakusteko.
7. Hautatu lan-kontratuko langile bat zerrendatik eta erreserbatu eskakizunerako baliabidea.
8. Proiektuko taldekide bat sortzen da. Hala ere, proiektuko taldeko kidea ez dago azpikontratu edo azpikontratazio lerro batekin eguneratzen eta, beraz, baliabideen esleipena ez da kostua izango azpikontratuaren prezioa erabiliz. Eskuz eguneratu proiektuko taldeko kidea azpikontratu lerro batekin eta joan hona **Proiektuaren kalkuluak** eta hautatu **Eguneratu prezioak** baliabideen esleipenaren kostu eguneratua ikusteko.

> [!NOTE]
> Duten proiektuko taldekideak **Langile mota** gisa **Lan-kontratuko langilea** baina ez dute azpikontratu erreferentziarik bezala markatzen dira **Baliogabea** gainean **Proiektuko taldekideak** sareta. Egoera hori duen proiektu-taldekideren bat baldin badago, ireki proiektu-taldearen erregistroa eta eguneratu eskuz azpikontratazio eta azpikontratazio-lerroen eremuak, finantza-kostuen estimazioak azpikontratistaren kostua zehatz-mehatz isla dezan.**Estimazioak** fitxa. 


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
