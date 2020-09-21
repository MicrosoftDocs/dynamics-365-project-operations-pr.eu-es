---
title: Proiekturako erosketa eskaerak
description: Artikulu honetan proiektu baterako erosketa aginduak sortzeko erabil ditzakezun metodoak deskribatzen dira. Erabiltzen duzun metodoa erosketa-aginduaren helburuaren arabera, eta erositako elementuak kontsumitu eta kargatu egiten dira proiektua.
author: KimANelson
manager: AnnBe
ms.date: 09/14/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 83972
ms.assetid: 247e4d72-610b-4fa5-9873-601ed0f4b2d6
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: a4975b9f9e20906fb1259e36a07d8ef3db4f4fee
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748852"
---
# <a name="purchase-orders-for-a-project"></a>Proiekturako erosketa eskaerak

[!include [banner](../includes/banner.md)]

Artikulu honetan proiektu baterako erosketa aginduak sortzeko erabil ditzakezun metodoak deskribatzen dira. Erabiltzen duzun metodoa erosketa-aginduaren helburuaren arabera, eta erositako elementuak kontsumitu eta kargatu egiten dira proiektua.

### <a name="methods-for-creating-a-purchase-order"></a>Erosketa eskaera sortzeko metodoak

Proiektuen kudeaketan eta kontabilitatean erosketa eskaera bat sortzeko metodo hauetako bat erabil dezakezu. Erosketa eskaeraren xedeak zehazten du noiz kontsumitzen den eta, beraz, noiz kobratzen diren proiektu batean proiektuak.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Metodoa</th>
<th>Helburua</th>
<th>Elementuen kontsumoa</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Sortu erosketa-eskaerak zuzenean proiektutik.</td>
<td>Erabili metodo hori erosteko elementuak kanpoko saltzaile bati proiektu batean kontsumitzeko. Erosketa aginduaren sor dezakezu bi modutan:
<ul>
<li>Proiektutik bertatik. Kasu honetan, proiektua dagoeneko zehaztuta dago erosketa eskaerarako.</li>
<li>Proiektuaren erosketa eskaerara nabigatuz. Erosketa eskaera sortzeko saltzailea eta proiektua hautatu behar dituzu.</li>
</ul></td>
<td>Elementuak saltzailearen faktura eguneratzen denean kontsumitzen dira.</td>
</tr>
<tr class="even">
<td>Sortu erosketa agindua erosketa agindutik.</td>
<td>Erabili erosketa-elementuen metodo hori salmenta-agindua sortzerakoan proiektutik.</td>
<td>Artikuluak bezeroari salmenta eskaera fakturatzen zaionean kontsumitzen dira.</td>
</tr>
<tr class="odd">
<td>Sortu erosketa eskaera elementu baten eskakizunetik abiatuta.</td>
<td>Erabili erosketa-elementuen metodo hori elementu-eskakizun bat sortzerakoan proiektutik.</td>
<td>Elementuak kontsumitzen dira elementuaren eskakizunaren pakete irristagarria eguneratuta dago.</td>
</tr>
</tbody>
</table>

> [!NOTE] 
> Saltzailearen faktura edo ontziratze agiria eguneratzen duzunean, elementuaren eskakizunean ontziratze agiria eguneratzeko eskatuko zaizu.

Informazio gehiagorako, ikus [Jaso erosketa eskaeran elementuak eskakizunetik](tasks/receive-items-purchase-order-item-requirement.md).

