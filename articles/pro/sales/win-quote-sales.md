---
title: Itxi eskaintza bat - arina
description: Gai honek Project Operations-eko eskaintzak ixteari buruzko informazioa ematen du.
author: rumant
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 8ae5e14220ffecab5bcfa016d8d18e6ccfbc5b04be9a4e66cee26f8885125d31
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6994306"
---
# <a name="close-a-quote---lite"></a>Itxi eskaintza bat - arina

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proiektuaren eskaintzak Irabazi edo Galdu bezala itxi daitezke. Aurrekontuaren zirriborroa itxi daiteke Aktibatu eta Berrikusi komatxoen eragiketak Microsoft Dynamics 365 Project Operations ez direlako onartzen.

## <a name="close-a-quote-as-won"></a>Itxi eskaintza Irabazita gisa

Proiektuaren aurrekontua Irabazitako moduan ixten duzunean, egoera Itxia da eta egoeraren arrazoi Irabazita dago. Eskaintza ixten baduzu, proiektuaren irakurketa soilik irakurtzen da eta eskaintzaren informazioa jasotzen duen proiektuaren zirriborroko eskaintza sortzen da. Aurrekontu itxia ezin denez berriro ireki, berrespen-elkarrizketa-koadro batek aldaketak baieztatuko ditu.

Aurrekontua aukera bati atxikita badago, aukeraren inguruko beste edozein proiektu automatikoki galduko da itxita.

### <a name="financial-impact-of-closing-a-quote-as-won"></a>Aurrekontua Irabazitako moduan ixteak duen eragin ekonomikoa

Aurrekontu zirriborro bati atxikita dagoen bitartean proiektu batean denborari buruzko datuak egiazkoak badira, denboraren edo gastuaren kostua bakarrik erregistratuko da. Aurrekontua Irabazi ahala itxi ondoren, aplikazioak kostuak berregokituko ditu kostu zaharrenak alderantzikatuz eta kostu erreal berriak berriro sortuz. Aplikazioak kostu erreal hauek prozesatuko ditu lotutako proiektuaren kontratu lerroaren Fakturazio metodoan oinarrituta. Kostuen fakturak denbora eta material kontratu lerro bati erreferentzia egiten bazaio, fakturatu gabeko salmenta errealak sortzen dira aurrekontua itxi eta proiektuaren kontratua sortzen denean. Kostuen prezioak prezio finkoko kontratu lerro bati erreferentzia egiten badio, aplikazioak proiektuaren kontratuaren bezeroentzako fakturazio arau zatituetan oinarritutako kostuen fakturak berriro prozesatzeari utziko dio.

## <a name="closing-a-quote-as-lost"></a>Eskaintza galdu bezala itxi:

Proiektuaren aurrekontua Galdutako moduan ixten duzunean, egoera Itxia da eta egoeraren arrazoi Galduta dago. Eskaintza ixteak proiektuaren eskaintza irakurtzeko soilik bihurtzen du. Aurrekontu itxia ezin denez berriro ireki eta, aurrekontua itxi aurretik, berrespen-elkarrizketa-koadro batek zure aldaketak baieztatuko ditu.

Galdutako itxita dagoen proiektuaren aurrekontuak bere lerroetako edozein proiektu aipatzen badu, proiektu hori itxita dagoela ere markatuko da. Egun horretatik aurrera edozein baliabide erreserba bertan behera geratzen da.

> [!NOTE]
> Project Operations-en, aurrekontua Irabazita edo Galduta gisa ixteak ez du Aukeraren egoera horretan eragingo, irekita egongo da eskuz itxi arte.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]