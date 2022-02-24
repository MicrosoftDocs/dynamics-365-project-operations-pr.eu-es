---
title: Fakturazio-prozesuaren informazio orokorra
description: Gai honek Project Operations-en eragiketetan fakturazioari buruzko ikuspegi orokorra eskaintzen du baliabideetan/stockean oinarritutako egoeren Project Operations-en.
author: sigitac
manager: Annbe
ms.date: 01/29/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: fbc1519b6cbcf231cfa89df8b7843d11a8904e49
ms.sourcegitcommit: b4298ca4729643c1040ef35dde8c67f829461ce7
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 01/29/2021
ms.locfileid: "5089199"
---
# <a name="invoicing-process-overview"></a>Fakturazio-prozesuaren informazio orokorra

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Baliabideen/Stockean oinarritutako egoeretarako Project Operations-ek gaitasun integrala eskaintzen du, bai Proiektu zuzendariaren bai Kontu kobratuen bulegariaren / proiektuaren kontulariaren beharretara egokituta. Fakturazio prozesurako, Proiektuaren kudeatzaileak proiektuaren fakturazio-zorroa kudeatzen du eta Kontuak kobratu beharreko funtzionarioak / proiektuaren kontulariak bezeroari begira faktura dokumentu zehatza eta zehatza sortzen du.

![Fakturazio-fluxuen diagrama](./media/invoicing-flow.png)

Proiektuaren kontratu lerroak lotutako proiektuen transakzioen fakturazio metodoa definitzen du. Proiektu kudeatzaileak denbora eta gastuen transakzioak onartzen dituenean, sistemak transakzioak erregistratzen ditu **Proiektuaren benetako datuak** entitateari eta informazioa helbidera bidaltzen du **Proiektuen kudeaketa eta kontabilitatea** moduluan Dynamics 365 Finance-en. Proiektuaren kontulariak gero fitxategiak berrikusi eta argitaratzen ditu [Project Operations-en integrazio-aldizkaria](../project-accounting/project-operations-integration-journal.md). Aldizkari honek proiektuaren datuen kontabilitate-datu garrantzitsuak biltzen ditu, hala nola fakturazioa, salmenten gaineko zerga taldea, fakturazio elementuen salmenten gaineko zerga taldea eta finantza dimentsioak.

Proiektuaren kudeatzaileak fakturatu gabeko salmenten transakzioak berrikusi ditzake denbora eta materialaren fakturazio metodoa erabiliz [Denboraren eta materialaren fakturazio-zorroa](../proforma-invoicing/manage-billing-backlog.md#time-and-material-billing-backlog) eta prezio finkoan fakturatzea [Prezio finkoaren mugarriak](../proforma-invoicing/manage-billing-backlog.md#fixed-price-milestones) aukeran. Ikuspegi horiei esker, hurrengo fakturazio-zikloan sartu behar diren transakzioak iragazi eta hautatu ditzakezu eta ondoren markatu **Fakturatzeko prest**.

[Eskuz sor dezakezu proforma faktura](../proforma-invoicing/create-manual-proforma-invoice.md) edo [aldian aldiko prozesua](../proforma-invoicing/configure-automated-invoice-creation.md) erabil dezakezu. Proiektu-kudeatzaileak [proforma faktura zirriborroa egokitu](../proforma-invoicing/manage-proforma-invoice.md) dezake behar den moduan eta gero berretsi.

Baieztatutako proforma faktura helbidera bidaltzen da **Proiektuen kudeaketa eta kontabilitatea** modulua Finance-n. Proiektuaren kontulariak proiektuaren faktura proposamena formateatu eta eguneratu egiten du eta, ondoren, dokumentua argitaratu eta inprimatzen du. Bidalitako proiektuaren fakturak Liburu Nagusian erregistratzen dira, baita Bezeroaren eta Proiektuaren azpiegituretan ere.
