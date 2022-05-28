---
title: Fakturazio-prozesuaren informazio orokorra
description: Gai honek Project Operations-en eragiketetan fakturazioari buruzko ikuspegi orokorra eskaintzen du baliabideetan/stockean oinarritutako egoeren Project Operations-en.
author: sigitac
ms.date: 01/29/2021
ms.topic: overview
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 0328d5321909bcc17754da4e19d7652b77a665d5
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8582695"
---
# <a name="invoicing-process-overview"></a>Fakturazio-prozesuaren informazio orokorra

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Baliabideen/Stockean oinarritutako egoeretarako Project Operations-ek gaitasun integrala eskaintzen du, bai Proiektu zuzendariaren bai Kontu kobratuen bulegariaren / proiektuaren kontulariaren beharretara egokituta. Fakturazio prozesurako, Proiektuaren kudeatzaileak proiektuaren fakturazio-zorroa kudeatzen du eta Kontuak kobratu beharreko funtzionarioak / proiektuaren kontulariak bezeroari begira faktura dokumentu zehatza eta zehatza sortzen du.

![Fakturazio-fluxuen diagrama.](./media/invoicing-flow.png)

Proiektuaren kontratu lerroak lotutako proiektuen transakzioen fakturazio metodoa definitzen du. Proiektuaren kudeatzaileak denbora eta gastu transakzioak onartzen dituenean, sistemak transakzioak erregistratzen ditu **Proiektuaren benetakoak** entitateari eta informazioa bidaltzen dio **Proiektuen kudeaketa eta kontabilitatea** modulua Dynamics 365 Finance-en. Proiektuaren kontulariak gero fitxategiak berrikusi eta argitaratzen ditu [Project Operations-en integrazio-aldizkaria](../project-accounting/project-operations-integration-journal.md). Aldizkari honek proiektuaren datuen kontabilitate-datu garrantzitsuak biltzen ditu, hala nola fakturazioa, salmenten gaineko zerga taldea, fakturazio elementuen salmenten gaineko zerga taldea eta finantza dimentsioak.

Proiektuaren kudeatzaileak fakturatu gabeko salmenten transakzioak berrikusi ditzake denbora eta materialaren fakturazio metodoa erabiliz [Denboraren eta materialaren fakturazio-zorroa](../proforma-invoicing/manage-billing-backlog.md#time-and-material-billing-backlog) eta prezio finkoan fakturatzea [Prezio finkoaren mugarriak](../proforma-invoicing/manage-billing-backlog.md#fixed-price-milestones) aukeran. Ikuspegi horiei esker, hurrengo fakturazio-zikloan sartu behar diren transakzioak iragazi eta hautatu ditzakezu eta ondoren markatu **Fakturatzeko prest**.

[Eskuz sor dezakezu proforma faktura](../proforma-invoicing/create-manual-proforma-invoice.md) edo [aldian aldiko prozesua](../proforma-invoicing/configure-automated-invoice-creation.md) erabil dezakezu. Proiektu-kudeatzaileak [proforma faktura zirriborroa egokitu](../proforma-invoicing/manage-proforma-invoice.md) dezake behar den moduan eta gero berretsi.

Baieztatutako proforma faktura helbidera bidaltzen da **Proiektuen kudeaketa eta kontabilitatea** modulua Finance-n. Proiektuaren kontulariak proiektuaren faktura proposamena formateatu eta eguneratu egiten du eta, ondoren, dokumentua argitaratu eta inprimatzen du. Bidalitako proiektuaren fakturak Liburu Nagusian erregistratzen dira, baita Bezeroaren eta Proiektuaren azpiegituretan ere.


[!INCLUDE[footer-include](../includes/footer-banner.md)]