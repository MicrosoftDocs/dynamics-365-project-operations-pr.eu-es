---
title: Konfiguratu eta erabili ordaindu ordaintzean saltzailearen ordainketak
description: Gai honetan ordaindutakoan (PWP) baldintzak nola sortu azaltzen da, saltzaileen ordainketa partzialak askatu ahal izateko, bezeroen ordainketetan oinarrituta.
author: RadhikaRS
ms.date: 03/30/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: johnmichalak
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 71f7b1db58c0d6aacc4f47920e5ad39dbb35ec51
ms.sourcegitcommit: 2c2a5a11d446adec2f21030ab77a053d7e2da28e
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/04/2022
ms.locfileid: "8683898"
---
# <a name="set-up-and-use-pay-when-paid-vendor-payments"></a>Konfiguratu eta erabili ordaindu ordaintzean saltzailearen ordainketak

[!include [banner](../includes/banner.md)]

Saltzaile bat azpikontratatu gisa lan egitea onartzen duzunean, saltzaileari ordainketa gorde nahi diozu, bezeroak proiektua ordaindu arte. Eszenatoki hau onartzeko, ordaindutakoan (PWP) baldintzak konfigura ditzakezu saltzailearekin erosketa eskaera (PO) konfiguratzen duzunean.

Adibidez, bezeroak proiektuaren fakturan zenbateko bat ordaintzen duenean, saltzailearen fakturaren zenbateko bat edo guztia askatu dezakezu. Just konfiguratu PWP baldintzak zehazten duten saltzaileari ordainduko dela bezeroarekin erlazionatutako ordainketaren ehuneko bat jaso ondoren. Bezero baten ordainketa partziala jasotzen baduzu, erlazionatutako saltzailearen faktura batzuk eskuz askatu ditzakezu ordainketa egiteko.

Hurrengo adibidean PWP terminoak erabiltzen direnean prozesua azaltzen da.

## <a name="example"></a>Adibidez

Zure erakundeak onartzen du bezeroari softwarea instalatuta duten 100 ordenagailu eskaintzea, ordenagailu bakoitzeko 150,00 dolar (USD) prezioan. Saltzaile bat kontratatuko duzu softwarea instalatuta duten ordenagailuak hornitzeko. Hitzarmenaren arabera, bezeroak zure erakundeari ordaindu aurretik ordenagailuen kalitatea onartu behar du. Zure erakundearen gidalerroa saltzaileei ordainketa atxikitzea da, bezeroak ordaindu arte. Hori dela eta, proiektua % 100eko PWP ehunekoa izan dezan konfiguratzen duzu.

Saltzaileak softwarea instalatuta duten 100 ordenagailuak bidaltzen dizkizu, 10.000,00 USD fakturarekin batera. PWP baldintzak zure proiektuan konfiguratuta daudenez, ez duzu saltzaileari ordainduko ordenagailuak jaso ondoren. Horren ordez, ordenagailuak bezeroari bidaltzen dizkiozu, 15.000,00 fakturarekin batera. Bezeroak ordenagailuak ikuskatu eta proiektuaren fakturaren zenbateko osoa onartzen du.

Bezeroaren ordainketa osoa jaso ondoren, saltzaileari 10.000,00 ordainduko diozu, saltzailearen fakturaren zenbateko osoa.

## <a name="set-up-pwp-terms-for-a-project"></a>Konfiguratu PWP baldintzak proiektu baterako

Proiektu baterako PWP baldintzak konfiguratzen dituzunean, portzentaje gisa zehaztu behar duzu bezeroak proiektuari ordaindu behar dizun gutxieneko kopurua saltzaileari ordaindu aurretik. Atalasearen zenbatekoa automatikoki kalkulatzen da proiektuaren bezeroen fakturetan. Jarraitu urrats hauei PWP baldintzetarako atalasearen ehunekoa konfiguratzeko.

1. Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Proiektuak** \> **Proiektu guztiak**.
2. Bilatu eta ireki PWP baldintzak konfiguratu nahi dituzun proiektua.
3. **Saltzaileen akordioak** FastTab-en, hautatu **Gehitu lerroa**.
3. **Kontuaren kodea** eremuan, hautatu aukera hauetako bat:

    - **Taula**: PWP baldintzak saltzaile bakar bati aplikatzen zaizkio.
    - **Taldea**: PWP baldintzak saltzaile talde bateko saltzaile guztiei aplikatzen zaizkie.
    - **Guztiak**: PWP baldintzak saltzaile guztiei aplikatzen zaizkie.

4. Aukeratu baduzu **Taula** edo **Taldea** aurreko urratsean, **Saltzailea/Saltzaile taldea** eremuan, hautatu PWP baldintzak aplikatzen zaizkion saltzailea edo saltzaile taldea. Aukeratu baduzu **Guztiak** aurreko urratsean,**Saltzailea/Saltzaile taldea** eremua ezin da editatu.
5. Saltzailearen atxikipen baldintzak proiektuan saltzailearentzat ezarrita badaude, **Saltzailearen atxikitze baldintzak** eremuan, hautatu erregelaren IDa atxikipen baldintzetarako.
6. **PWP atalasearen ehunekoa** eremuan, sartu proiektuaren atalase portzentajea. Proiektuan sartzen duzun ehunekoak bezeroak saltzaileari ordaindu aurretik ordaindu behar dizun gutxieneko zenbatekoa definitzen du.

## <a name="create-a-po-that-has-pwp-terms"></a>Sortu PWP baldintzak dituen PO bat

Saltzaile baten faktura bidaltzen duzunean, saltzaileak PWP baldintzak betetzen baditu, baldintza horiek PO lerroetan agertzen dira. PWP baldintzak dituen PO bat sortzeko, jarraitu urrats hauei.

1. Joan **Kontratazioa eta hornidura** \> **Erosketa aginduak** \> **Erosketa eskaera guztiak**.
2. Ekintza panelean, hautatu **Berria**. Ondoren, **Sortu eskaera** elkarrizketa-koadroan, sartu beharrezko informazioa eta hautatu **Ados**.

    Bestela, ireki lehendik dagoen PO bat **Erosketa eskaera guztiak** zerrenda orria.

4. **Erosketa-eskaera** orrialdean, **Erosketa eskaeren lerroak** FastTab-en, berrikusi saltzailearen PO linearen xehetasunak. **Ordaindu ordaintzen denean** aukera automatikoki hautatzen da eta balioa **PWP atalasearen ehunekoa** eremua automatikoki kopiatzen da **PWP atalasearen ehunekoa** eremuan **Proiektuak** orrialdea.
6. Ez baduzu nahi PWP baldintzak saltzaileari PO linea baterako aplikatu, garbitu **Ordaindu ordaintzen denean** aukera. Kasu honetan **PWP atalasearen ehunekoa** PO lerroaren eremua 0 (zero) berrezarriko da.

## <a name="update-a-customer-payment-and-pay-the-vendor"></a>Eguneratu bezeroaren ordainketa eta ordaindu saltzaileari

Saltzaile batek proiektu batean egindako lana amaitzen duenean eta faktura bat bidaltzen dizunean, proiektuaren egoera eta bezeroaren fakturak berrikusi behar dituzu proiektuan PWP baldintzak betetzen diren ala ez jakiteko. Saltzailearen PWP baldintzak betetzen badira, saltzailearen fakturan zein lerro ordaindu behar dituzun zehaztu dezakezu, proiektuaren bezeroen ordainketen arabera. Saltzaileari ordaintzea erabakitzen baduzu PWP baldintzak betetzen ez diren arren, PWP baldintzak gainidatzi ditzakezu **Saltzailearen faktura ordainduta ordaindutakoan** orrialdea.

1. Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Kontsultak eta txostenak** \> **Atxikitzeko kontsultak** \> **Saltzailearen faktura ordainduta ordaindutakoan**.
2. **Saltzailearen fakturak ordaindutako ordainduta** orrialdean, bilaketa eremuan, sartu balioak berrikusi nahi duzun saltzailearen faktura aurkitzeko, eta hautatu **Bilatu**.
3. **Saltzailearen faktura lerroak** FastTab-en, hautatu aldatu nahi dituzun lerroak.
4. **Ordaindu ordaintzen denean** fakturazio lerroan baldintzak betetzen dira, hautatu **Saltzailearen ordainketa askatu**. **Ordaindu ordaintzen denean** aukera garbitu egiten da, eta **Ordaintzeko prest** eremua aldatu egiten da **Bai**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]