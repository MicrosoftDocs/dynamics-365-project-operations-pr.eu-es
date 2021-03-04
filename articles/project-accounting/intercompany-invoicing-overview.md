---
title: Enpresen arteko fakturazioaren informazio orokorra
description: Gai honek enpresen arteko fakturazioa proiektuen inguruko informazioa eta adibideak eskaintzen ditu.
author: sigitac
manager: tfehr
ms.date: 11/19/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 670b5d15ecf1ef7dcc034064e625814cbe6d54b0
ms.sourcegitcommit: addbe0647619413e85e7cde80f6a21db95ab623e
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/20/2020
ms.locfileid: "4595415"
---
# <a name="intercompany-invoicing-overview"></a>Enpresen arteko fakturazioaren informazio orokorra

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Zure erakundeak dibisio, filial eta beste pertsona juridiko ugari izan ditzake produktuak eta zerbitzuak elkarri proiektuetarako transferitzen dituztenak. Zerbitzua edo produktua eskaintzen duen pertsona juridikoari deitzen zaio *pertsona juridiko mailegu-emailea*. Zerbitzua edo produktua jasotzen duen pertsona juridikoari deitzen zaio *pertsona juridiko mailegu-hartzailea*.

Hurrengo ilustrazioak agertoki tipikoa erakusten du, non bi pertsona juridikok, Contoso Robotics USA-k (mailegu-hartzailea den pertsona juridikoa) eta Contoso Robotics UK-k (mailegu-emaile den pertsona juridikoa) baliabideak partekatzen dituzten bezeroak, Adventure works-ek proiektu bat entregatzeko. Eszenatoki honetarako, Contoso Robotics USA-k kontratua du lana Adventure Works-i entregatzeko.

![Enpresen arteko fakturazioa](./media/IntercompanyScenario.png) 

Dynamics 365 Project Operations fluxua erabiltzen du enpresen arteko transakzioak prozesatzeko:

1. Mailegu-entitate juridikoaren baliabideek konpainien arteko denbora edo gastuen transakzioak erregistratzen dituzte, denbora eta gastuak erreserbatuz mailegu-entitate juridikoan proiektuen aurka.
2. Denbora eta gastuen kostuak mailegu-enpresan erregistratzen dira mailegu-hartzailearen konpainiaren unitateko kostuen prezioen zerrenda erabiliz.
3. Enpresa arteko fakturatu gabeko salmenta-transakzioak mailegu-enpresan erregistratzen dira mailegu-hartzailearen konpainiaren unitateko kostuen prezioen zerrenda erabiliz.
4. Fakturatu gabeko diru-sarrerak mailegu-enpresan erregistratzen dira proiektuaren kontratuaren salmenta prezioen zerrenda erabiliz. Bezeroari faktura daiteke fakturatu gabeko diru sarrerak erregistratzen direnean. Bezeroak ez du itxaron behar enpresen arteko fakturak prozesatu arte.
5. Enpresen arteko bezeroen fakturak aldian behin sortzen dira mailegu-enpresan. Fakturak eskuz edo aldian aldiko prozesu automatizatu bat erabiliz sortzen dira. Mailegu-entitate juridiko bakoitzeko faktura bakarra sor daiteke edo proiektuaren arabera faktura desberdinak sor daitezke.
6. Enpresa arteko saltzaileen faktura emailearen legezko entitatean argitaratzen denean, dagokion zain dagoen saltzaile-faktura legezko entitate-hartzailean sortuko da. Saltzaileen fakturaren zain dauden kostuak faktura argitaratzen denean proiektuaren azpiegituran erregistratuko dira.

Ondorengo diagramak enpresen arteko fakturazioa erakusten du kontabilitateko gertaerekin eta liburu nagusian espero diren bidalketekin erlazionatuta.

![Enpresen arteko fluxua](./media/IntercompanyFlow.png)

## <a name="additional-resources"></a>Baliabide gehigarriak

- [Konfiguratu enpresen arteko fakturazioa](configure-intercompany-invoicing.md)
- [Grabatu enpresen arteko transakzioak](create-intercompany-transactions.md)
- [Sortu enpresen arteko bezeroa eta saltzaileen fakturak](create-intercompany-customer-vendor-invoices.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]