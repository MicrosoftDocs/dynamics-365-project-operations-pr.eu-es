---
title: Itxi eskaintza
description: Gai honek Project Operations-eko eskaintzak ixteari buruzko informazioa ematen du.
author: rumant
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 2314444dfdbd4d1a2f38c7de55e2070011e51a86f1e074dd6667d54393c641fe
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6993406"
---
# <a name="close-a-quote"></a>Itxi eskaintza

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Proiektuaren eskaintzak Irabazi edo Galdu bezala itxi daitezke. Aktibatu eta Berrikusi funtzioak ez direnez onartzen Microsoft Dynamics 365 Project Operations-eko eskaintzetan, zirriborroko eskaintza bat itxi dezakezu.

## <a name="close-a-quote-as-won"></a>Itxi eskaintza Irabazita gisa

Proiektuaren eskaintza Irabazita gisa ixtean, eskaintza ren egoera **Itxita** gisa ezarritako da eta egoeraren arrazoia **Irabazita** moduan. Eskaintzak ixten badituzu, irakurtzeko soilik bihurtzen dira eskaintzaren informazio guztiarekin batera proiektuaren zirriborroko kontratua sortzen da. Aurrekontu itxia ezin denez berriro ireki, aurrekontua itxi aurretik, berrespen-elkarrizketa-koadro batek zure aldaketak baieztatuko ditu.

Proiektuaren aurrekontu batetik sortutako proiektuaren kontratua ere eskuragarri dago Project Operations-en Proiektuen kudeaketa eta kontabilitate moduluan. Proiektuen kontratua bere lerroetako edozein proiektutan mapatuta ez badago, proiektuaren kontratu hau proiektu inaktiboaren kontratu gisa erabilgarri egongo da eta aktibo egongo da proiektu bat gutxienez bere kontratu lerroetako batera mapatu bezain laster.

Aurrekontua aukera bati atxikita badago, aukeraren inguruko beste edozein proiektu automatikoki galduko da itxita.

### <a name="financial-impact-of-closing-a-quote-as-won"></a>Aurrekontua Irabazitako moduan ixteak duen eragin ekonomikoa

Aurrekontu zirriborro bati atxikita dagoen bitartean proiektu batean erregistratutako denboraren berri eman bada, denboraren edo gastuaren kostua bakarrik erregistratuko da. Aurrekontua Irabazi ahala itxi ondoren, aplikazioak kostuak berregokituko ditu kostu zaharrenak alderantzikatuz eta kostu erreal berriak berriro sortuz. Aplikazioak kostu erreal hauek prozesatuko ditu lotutako proiektuaren kontratu lerroaren Fakturazio metodoan oinarrituta. Kostuen fakturak denbora eta material kontratu lerro bati erreferentzia egiten badio, sistemak automatikoki sortuko ditu fakturatu gabeko salmenten fakturak, aurrekontua itxi eta proiektuaren kontratua sortzen denean. Kostuen prezioak prezio finkoko kontratu lerro bati erreferentzia egiten badio, aplikazioak kostuaren fakturak berriro prozesatzeari utziko dio proiektuaren kontratuko bezeroen fakturazio arau zatituetan oinarrituta.

Prozesatutako datu guztiak eskuragarri daude Proiektuaren kudeaketa eta kontabilitate moduluan, Proiektuaren kontulariak berrikusi, eguneratu eta liburu nagusian argitaratzeko. 

## <a name="close-a-quote-as-lost"></a>Itxi eskaintza Galduta gisa

Galdutako proiektuaren eskaintza ixtean egoera ezarriko da **Itxita** eta egoeraren arrazoia **Galduta** izango da. Aurrekontua ixteak irakurtzeko soilik bihurtzen du. Aurrekontu itxia ezin denez berriro ireki eta, aurrekontua itxi aurretik, berrespen-elkarrizketa-koadro batek zure aldaketak baieztatuko ditu.

Galduta gisa itxita dagoen proiektuaren aurrekontuak bere lerroetako batean proiektu bat badu erreferentzia, proiektu hori Itxita gisa markatzen da eta egun horretatik aurrerako baliabideen erreserbak bertan behera geratzen dira.

> [!NOTE]
> Project Operations-en, aurrekontua Irabazita edo Galduta gisa ixteak ez du Aukeraren egoera horretan eragingo, irekita egongo da eskuz itxi arte.


[!INCLUDE[footer-include](../includes/footer-banner.md)]