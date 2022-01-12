---
title: Proiektu bat lan-kontratudun langileekin eta azpikontratatutako gaitasunarekin hornitzea
description: Gai honek Microsoft-en lan-kontratuko langileak edo azpikontratatutako gaitasuna erabiliz proiektuaren eskakizunak nola bete daitezkeen azaltzen du Dynamics 365 Project Operations.
author: rumant
ms.date: 12/03/2021
ms.topic: article
ms.reviewer: tonyafehr
ms.author: rumant
ms.openlocfilehash: 7e9a0ca08f472999138589f31ca820b733b6303e
ms.sourcegitcommit: 04dc8d952e6da3ab3eb2a20131c6f7cee6040876
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/10/2021
ms.locfileid: "7903607"
---
# <a name="staffing-a-project-with-contract-workers-and-subcontracted-capacity"></a>Proiektu bat lan-kontratudun langileekin eta azpikontratatutako gaitasunarekin hornitzea

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proiektu-talde orokorreko kideak langileekin edo lan-kontratuko langileekin egon daitezke. Proiektu bat lan-kontratuko langileekin hornitzean, zure langile-aukerak muga ditzakezu azpikontratu-lerro batera esleitutako kontratu-langile zehatzetara. 

## <a name="search-for-staff-resource-requirements-with-contract-workers-that-belong-to-a-specific-subcontract-line"></a>Azpikontratazio-lerro zehatz bateko langile-kontratudunekin langile-baliabideen eskakizunak bilatu

Azpikontratazio-lerro zehatz bateko langile kontratudunekin langile-baliabideen eskakizunak bilatzeko eta bilatzeko, jarraitu urrats hauek:

1. Sortu proiektu-taldekide generiko bat, azpikontratu eta azpikontratu lerro bati erreferentzia egiten diona.
2. Sortu baliabide-eskakizuna proiektuko taldekide generiko honentzat **Sortu eskakizuna** botoia proiektuko taldekideen azpi-sareko.
3. Hautatu taldekideen errenkada eta, ondoren, hautatu **Liburua** azpi-sareko botoia. 
4. Honek Ordutegien taula irekitzen du eskakizunen testuinguruarekin. Data, rola eta antolakuntza-unitate-eremuak bezalako beste atributu batzuekin batera, Programazio-taularen iragazkiak ere automatikoki betetzen dira baliabideen eskakizuneko saltzaile, azpikontrata eta azpikontratazio lerro-eremuekin.
5. Sistemak iragazki-irizpideak betetzen dituzten baliabideak bilatzen ditu eta zerrendatzen ditu. 
6. Aukeratu iragazitako baliabideetako bat eta erreserbatu baliabidea eskakizunerako. 
7. Proiektuko taldekide bat sortzen eta eguneratzen da azpikontratazio eta azpikontratu lerroen erreferentziekin. Joan **Proiektuaren kalkuluak** eta hautatu **Eguneratu prezioak** baliabideen esleipenaren kostu eguneratua ikusteko. 

> [!NOTE]
> Proiektuko taldeko kidea azpikontratu eta azpikontratu lerroaren erreferentzia batekin eguneratzea baliteke beti ez izatea posible erreserba egiterakoan baliabidea azpikontratu lerro anitzetan esleituta badago. Sistemak ezin badu eguneratu proiektuko taldeko kidea azpikontratu eta azpikontratazio lerro batekin, ireki proiektuaren taldeko kideen erregistroa eta eskuz eguneratu eremu hauek, finantza-kostuen estimazioak azpikontratistaren kostua zehatz-mehatz isla dezan.

## <a name="search-for-and-staff-resource-requirements-with-any-contract-worker"></a>Bilatu eta langile-baliabideen eskakizunak edozein lan-kontratuko langileekin

Edozein lan-kontratuko langileekin langile-baliabideen eskakizunak bilatzeko, jarraitu urrats hauek:

1. Sortu proiektuko taldekide generiko bat.
2. Sortu baliabide-eskakizuna proiektuko taldekide generiko honentzat **Sortu eskakizuna** botoia proiektuko taldekideen azpi-sareko.
3. Hautatu taldekideen errenkada eta, ondoren, hautatu **Liburua** azpi-sareko botoia. 
4. Honek Ordutegien taula irekitzen du eskakizunen testuinguruarekin. Data, rola eta antolakuntza-unitate-eremuak bezalako beste atributu batzuekin batera, Programazio-taularen iragazkiak ere automatikoki betetzen dira baliabideen eskakizuneko saltzaile, azpikontrata eta azpikontratazio lerro-eremuekin. Eskakizunak ez zuelako azpikontratazio edo azpikontratazio lerroko baliorik bete, atributu hauek hutsik egongo dira iragazkien panelean.
5. Sistemak iragazki-irizpideak betetzen dituzten baliabideak bilatzen ditu eta zerrendatzen ditu.
6. Eguneratu **Langile mota** iragazki-paneleko eremua **Lan-kontratuko langilea** bilaketa lan-kontratuko langileei mugatzeko. Eguneratu **Saltzailea** iragazkien panelean, hornitzaile bat hautatzeko bilaketa mugatzeko, hornitzaile-enpresa zehatz bateko lan-kontratuko langileak soilik erakusteko.
7. Hautatu lan-kontratuko langile bat zerrendatik eta erreserbatu eskakizunerako baliabidea.
8. Proiektuko taldekide bat sortzen da. Hala ere, proiektuko taldeko kidea ez dago azpikontratu edo azpikontratazio lerro batekin eguneratzen eta, beraz, baliabideen esleipena ez da kosturik izango azpikontratuaren prezioa erabiliz. Eskuz eguneratu proiektuko taldeko kidea azpikontratu lerro batekin eta joan hona **Proiektuaren kalkuluak** eta hautatu **Eguneratu prezioak** baliabideen esleipenaren kostu eguneratua ikusteko.

> [!NOTE]
> Duten proiektuko taldekideak **Langile mota** gisa **Lan-kontratuko langilea** baina ez dute azpikontratu erreferentziarik bezala markatzen dira **Baliogabea** gainean **Proiektuko taldekideak** sareta. Egoera hori duen proiektu-taldekideren bat baldin badago, ireki proiektu-taldearen erregistroa eta eguneratu eskuz azpikontratazio eta azpikontratazio-lerroen eremuak, finantza-kostuen estimazioak azpikontratistaren kostua zehatz-mehatz isla dezan.**Estimazioak** fitxa. 


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
