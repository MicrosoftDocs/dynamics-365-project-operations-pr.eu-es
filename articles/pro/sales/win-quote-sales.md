---
title: Itxi proiektuaren eskaintzak
description: Gai honek Project Operations-eko eskaintzak ixteari buruzko informazioa ematen du.
author: rumant
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 4335fa5467640af840c0f68a648c9b8a6864d834
ms.sourcegitcommit: e0cbbe7c6f03d4978134405cf04bd8bc1d019f65
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/05/2022
ms.locfileid: "9826160"
---
# <a name="close-project-quotes"></a>Itxi proiektuaren eskaintzak

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proiektuaren eskaintzak Irabazi edo Galdu bezala itxi daitezke. Aurrekontuaren zirriborroa itxi daiteke Aktibatu eta Berrikusi komatxoen eragiketak Microsoft Dynamics 365 Project Operations ez direlako onartzen.

## <a name="close-a-quote-as-won"></a>Itxi eskaintza Irabazita gisa

Proiektuaren aurrekontua Irabazitako moduan ixten duzunean, egoera Itxia da eta egoeraren arrazoi Irabazita dago. Eskaintza ixten baduzu, proiektuaren irakurketa soilik irakurtzen da eta eskaintzaren informazioa jasotzen duen proiektuaren zirriborroko eskaintza sortzen da. Aurrekontu itxia ezin denez berriro ireki, berrespen-elkarrizketa-koadro batek aldaketak baieztatuko ditu.

Aurrekontua aukera bati atxikita badago, aukeraren inguruko beste edozein proiektu automatikoki galduko da itxita.

### <a name="financial-impact-of-closing-a-quote-as-won"></a>Aurrekontua Irabazitako moduan ixteak duen eragin ekonomikoa

Aurrekontu zirriborro bati atxikita dagoen bitartean proiektu batean denborari buruzko datuak egiazkoak badira, denboraren edo gastuaren kostua bakarrik erregistratuko da. Aurrekontua Irabazi ahala itxi ondoren, aplikazioak kostuak berregokituko ditu kostu zaharrenak alderantzikatuz eta kostu erreal berriak berriro sortuz. Aplikazioak kostu erreal hauek prozesatuko ditu lotutako proiektuaren kontratu lerroaren Fakturazio metodoan oinarrituta. Kostuen fakturak denbora eta material kontratu lerro bati erreferentzia egiten bazaio, fakturatu gabeko salmenta errealak sortzen dira aurrekontua itxi eta proiektuaren kontratua sortzen denean. Kostuen prezioak prezio finkoko kontratu lerro bati erreferentzia egiten badio, aplikazioak proiektuaren kontratuaren bezeroentzako fakturazio arau zatituetan oinarritutako kostuen fakturak berriro prozesatzeari utziko dio.

## <a name="closing-a-quote-as-lost"></a>Aurrekontu bat galdu bezala ixtea

Proiektuaren aurrekontua Galdutako moduan ixten duzunean, egoera Itxia da eta egoeraren arrazoi Galduta dago. Eskaintza ixteak proiektuaren eskaintza irakurtzeko soilik bihurtzen du. Aurrekontu itxia ezin denez berriro ireki eta, aurrekontua itxi aurretik, berrespen-elkarrizketa-koadro batek zure aldaketak baieztatuko ditu.

Galdutako itxita dagoen proiektuaren aurrekontuak bere lerroetako edozein proiektu aipatzen badu, proiektu hori itxita dagoela ere markatuko da. Egun horretatik aurrera edozein baliabide erreserba bertan behera geratzen da.

> [!NOTE]
> Project Operations-en, aurrekontua Irabazita edo Galduta gisa ixteak ez du Aukeraren egoera horretan eragingo, irekita egongo da eskuz itxi arte.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
