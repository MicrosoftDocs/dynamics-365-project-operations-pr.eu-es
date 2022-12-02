---
title: Proiektu bat kontratudun langileekin eta azpikontratatutako ahalmenarekin hornitzea
description: Artikulu honek lan-kontratuko langileak edo azpikontratatutako gaitasuna erabiliz proiektuaren eskakizunak nola bete daitezkeen azaltzen du Microsoft Dynamics 365 Project Operations.
author: rumant
ms.date: 09/14/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 30e16efeed93ab4568eac57fb3ed46067a08524d
ms.sourcegitcommit: 08eb3be9eda44e9446c43ed9b6aefd58d77927c5
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/15/2022
ms.locfileid: "9522420"
---
# <a name="staffing-a-project-with-contract-workers-and-subcontracted-capacity"></a>Proiektu bat kontratudun langileekin eta azpikontratatutako ahalmenarekin hornitzea

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Proiektu-talde orokorreko kideak langileekin edo lan-kontratuko langileekin egon daitezke. Proiektu bat lan-kontratuko langileekin hornitzean, zure langile-aukerak muga ditzakezu azpikontratu-lerro batera esleitutako lan-kontratuko langile espezifikoetara. 

## <a name="search-for-staff-resource-requirements-with-contract-workers-that-belong-to-a-specific-subcontract-line"></a>Azpikontratazio-lerro jakin bateko langile-kontratudunekin langile-baliabideen eskakizunak bilatzea

Azpikontratazio-lerro jakin bateko langile-kontratudunekin langile-baliabideen eskakizunak bilatzeko, egin hau:

1. Azpikontratu eta azpikontratuaren lerroa aipatzen duten proiektuaren taldeko kide orokorra.
2. Sortu baliabide-eskakizuna proiektuko taldekide generiko honentzat **Sortu eskakizuna** proiektuko taldekideen azpi-sareko botoia.
3. Hautatu taldekideen errenkada eta, ondoren, hautatu **Liburua** azpi-sareko botoia. 
4. Honek Ordutegi-taula irekitzen du eskakizunen testuinguruarekin. Beste atributu batzuekin batera, hala nola datak, rola eta antolakuntza-unitate-eremuak, Programazio-taularen iragazkiak automatikoki betetzen dira baliabide-eskakizuneko hornitzaile, azpikontratu eta azpikontratu lerro-eremuekin.
5. Sistemak iragazki-irizpideak betetzen dituzten baliabideak bilatzen ditu eta zerrendatzen ditu. 
6. Aukeratu iragazitako baliabideetako bat eta erreserbatu baliabidea eskakizunerako. 
7. Azpikontratu eta azpikontratuaren lerroa aipatzen duten proiektuaren taldeko kide orokorra. Joan **Proiektuaren kalkuluak** eta hautatu **Eguneratu prezioak** baliabideen esleipenaren kostu eguneratua ikusteko. 

> [!NOTE]
> Proiektuko taldeko kidea azpikontratu eta azpikontratu lerroaren erreferentzia batekin eguneratzea baliteke beti ez izatea posible erreserba egiterakoan baliabidea azpikontratu lerro anitzetan esleituta badago. Egoera hori duen proiektu-taldekideren bat baldin badago, ireki proiektu-taldearen erregistroa eta eguneratu eskuz azpikontratazio eta azpikontratazio-lerroaren eremuak, finantza-kostuen estimazioak azpikontratistaren kostua zehatz-mehatz isla dezan Estimazioak fitxa.

## <a name="search-for-and-staff-resource-requirements-with-any-contract-worker"></a>Bilatu eta langile-baliabide-eskakizunak edozein lan-kontratuko langileekin

Bilatzeko eta langile-baliabide-eskakizunak edozein lan-kontratuko langileekin, egin hau:

1. Proiektuaren taldekide generikoko kidea bat sortu.
2. Sortu baliabide-eskakizuna proiektuko taldekide generiko honentzat **Sortu eskakizuna** proiektuko taldekideen azpi-sareko botoia.
3. Hautatu taldekideen errenkada eta, ondoren, hautatu **Liburua** azpi-sareko botoia. 
4. Honek Ordutegi-taula irekitzen du eskakizunen testuinguruarekin. Beste atributu batzuekin batera, hala nola datak, rola eta antolakuntza-unitate-eremuak, Programazio-taularen iragazkiak automatikoki betetzen dira baliabide-eskakizuneko hornitzaile, azpikontratu eta azpikontratu lerro-eremuekin. Eskakizunak ez zuelako azpikontratazio edo azpikontratazio lerroko baliorik bete, atributu hauek hutsik egongo dira iragazkien panelean.
5. Sistemak iragazki-irizpideak betetzen dituzten baliabideak bilatzen ditu eta zerrendatzen ditu.
6. Eguneratu **Langile mota** iragazki-paneleko eremua **Lan-kontratuko langilea** bilaketa lan-kontratuko langileei mugatzeko. Eguneratu **Saltzailea** iragazkien panelean, hornitzaile bat hautatzeko bilaketa mugatzeko, hornitzaile-enpresa zehatz bateko lan-kontratuko langileak soilik erakusteko.
7. Hautatu lan-kontratuko langile bat zerrendatik eta erreserbatu eskakizunerako baliabidea.
8. Proiektuaren taldekide bat sortzen da. Hala ere, proiektuko taldeko kidea ez dago azpikontratazio edo azpikontratazio lerro batekin eguneratzen eta, beraz, baliabideen esleipena ez da kosturik izango azpikontratuaren prezioa erabiliz. Eskuz eguneratu proiektuko taldeko kidea azpikontratu lerro batekin eta joan hona **Proiektuaren kalkuluak** eta hautatu **Eguneratu prezioak** baliabideen esleipenaren kostu eguneratua ikusteko.

> [!NOTE]
> Proiektuko taldekideek duten **Langile mota** bezala **Lan-kontratuko langilea** baina ez dute azpikontratu erreferentziarik bezala markatzen dira **Baliogabea** gainean **Proiektuko taldekideak** sareta. Egoera hori duen proiektu-taldekideren bat baldin badago, ireki proiektu-taldearen erregistroa eta eguneratu eskuz azpikontratazio eta azpikontratazio-lerroaren eremuak, finantza-kostuen estimazioak azpikontratistaren kostua zehatz-mehatz isla dezan **Estimazioak** fitxa. 


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
