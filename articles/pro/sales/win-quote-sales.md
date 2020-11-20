---
title: Itxi eskaintza bat - arina
description: Gai honek Project Operations-eko eskaintzak ixteari buruzko informazioa ematen du.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5ad206232d616cdbdc83e2a17b9177cfb98ffda9
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/30/2020
ms.locfileid: "4175696"
---
# <a name="close-a-quote---lite"></a>Itxi eskaintza bat - arina

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proiektuaren eskaintzak Irabazi edo Galdu bezala itxi daitezke. Eskaintzetako Aktibatu eta Berrikusi eragiketak ez dira onartzen Microsoft Dynamics 365 Project Operations-en; beraz, zirriborroko eskaintza itxi daiteke.

## <a name="close-a-quote-as-won"></a>Itxi eskaintza Irabazita gisa

Irabazitako proiektuaren eskaintza ixtean eskaintza itxi egingo da egoera itxita eta egoeraren arrazoi Irabazitako moduan. Eskaintza ixten baduzu, proiektuaren irakurketa soilik irakurtzen da eta eskaintzaren informazioa jasotzen duen proiektuaren zirriborroko eskaintza sortzen da. Eskaintza itxia ezin denez berriro ireki, baieztapen elkarrizketa-koadroa Baieztapen elkarrizketa-koadroa dago aldaketak egin aurretik, eskaintza itxia ezin baita berriro ireki eta aldaketak atzeraezinak dira.

Aurrekontua aukera bati atxikita badago, aukeraren inguruko beste edozein proiektu automatikoki galduko da itxita.

### <a name="financial-impact-of-closing-a-quote-as-won"></a>Aurrekontua Irabazitako moduan ixteak duen eragin ekonomikoa

Aurrekontu zirriborro bati atxikita dagoen bitartean proiektu batean erregistratutako denboraren berri eman bada, denboraren edo gastuaren kostua bakarrik erregistratuko da. Aurrekontua Irabazi ahala itxi ondoren, aplikazioak kostuak berregokituko ditu kostu zaharrenak alderantzikatuz eta kostu erreal berriak berriro sortuz. Aplikazioak kostu erreal hauek prozesatuko ditu lotutako proiektuaren kontratu lerroaren Fakturazio metodoan oinarrituta. Kostuen fakturak denbora eta material kontratu lerro bati erreferentzia egiten badio, sistemak automatikoki sortuko ditu fakturatu gabeko salmenten fakturak, aurrekontua itxi eta proiektuaren kontratua sortzen denean. Kostuen prezioak prezio finkoko kontratu lerro bati erreferentzia egiten badio, aplikazioak kostuaren fakturak berriro prozesatzeari utziko dio proiektuaren kontratuko bezeroen fakturazio arau zatituetan oinarrituta.

## <a name="closing-a-quote-as-lost"></a>Eskaintza galdu bezala itxi:

Galdutako proiektuaren eskaintza ixtean egoera ezarriko da Itxita eta egoeraren arrazoia Galdua izango da. Eskaintza ixteak proiektuaren eskaintza irakurtzeko soilik bihurtzen du. Aurrekontu itxia ezin denez berriro ireki eta, aurrekontua itxi aurretik, berrespen-elkarrizketa-koadro batek zure aldaketak baieztatuko ditu.

Galduta gisa itxita dagoen proiektuaren aurrekontuak bere lerroetako batean proiektu bat badu erreferentzia, proiektu hori Itxita gisa markatzen da eta egun horretatik aurrerako baliabideen erreserbak bertan behera geratzen dira.

> [!NOTE]
> Project Operations-en, aurrekontua Irabazita edo Galduta gisa ixteak ez du Aukeraren egoera horretan eragingo, irekita egongo da eskuz itxi arte.
