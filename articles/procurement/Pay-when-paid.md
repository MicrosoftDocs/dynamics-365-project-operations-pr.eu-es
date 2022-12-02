---
title: Ordaindu ordaintzean saltzailearen ordainketak
description: Gai honek ordaintzean ordaindutako egoera (PWP) nola erabili azaltzen du.
author: mukumarm
ms.date: 08/18/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: mukumarm
ms.openlocfilehash: d1fe8d92663b31b22dc405fc1f3e06d976e6c5dc
ms.sourcegitcommit: b2d05f898daa552179d67fdf4c060c93a9c66bd1
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/16/2022
ms.locfileid: "9525377"
---
# <a name="pay-when-paid-vendor-payments"></a>Ordaindu ordaintzean saltzailearen ordainketak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai honek ordaintzean ordaindutako egoera (PWP) nola erabili azaltzen du.

## <a name="create-a-purchase-order-that-has-pwp-terms"></a>Sortu PWP baldintzak dituen erosketa-eskaera

Saltzaile baten faktura bidaltzen duzunean, saltzaileak PWP baldintzak betetzen baditu, baldintza horiek erosketa eskaera (PO) lerroetan agertzen dira. PWP baldintzak dituen PO bat sortzeko, jarraitu urrats hauei.

1. Microsoft Dynamics 365 Finance-n ,egin ondorengo urratsetako bat:

    - Joan **Kontratazioa eta hornidura** \> **Erosketa aginduak** \> **Erosketa eskaera guztiak**. Ekintza panelean, hautatu **Berria**. **Sortu erosketa-eskaera** elkarrizketa-koadroa, hautatu proiektuan PWP baldintzak ezarrita dauden hornitzailea, idatzi behar den beste informazio bat eta hautatu **ADOS**.
    - Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Proiektuak** \> **Proiektu guztiak**. Ekintza panelean, **Kudeatu** fitxan, hautatu **Elementuaren zeregina**. Hautatu erosketa-eskaera. Hautatu proiektuan PWP baldintzak konfiguratu dituen hornitzailea eta, ondoren, hautatu **Ados**.

2. **Erosketa-eskaera** orrialdean, **Erosketa-eskaeraren lerroak** Fitxa azkarra, hautatu **Gehitu lerroa** erosketa-eskaeraren lerroa sortzeko.
3. Hautatu elementu-zenbakia edo kontratazio-kategoria eta sartu beharrezko gainerako xehetasunak. Berrikusi saltzailearentzat PO-lerroaren xehetasunak.

    **Ordaindu ordaintzen denean** aukera automatikoki hautatzen da eta balioa **PWP atalasearen ehunekoa** eremua automatikoki kopiatzen da **PWP atalasearen ehunekoa** eremuan **Proiektuak** orrialdea.

4. Ez baduzu nahi PWP baldintzak saltzaileari PO linea baterako aplikatu, garbitu **Ordaindu ordaintzen denean** aukera. Kasu honetan **PWP atalasearen ehunekoa** PO lerroaren eremua **0** (zero) berrezarriko da.
5. Gainean **Erosketa-eskaera** orrialdean, Ekintza-panelean, atalean **Erosketa** fitxa, hautatu **Berretsi** erosketa-eskaera berresteko.
6. Ekintza-panelean, gunean **Faktura** fitxa, hautatu **Faktura** erosketa-eskaeraren faktura sortzeko.

## <a name="create-a-project-invoice-proposal"></a>Sortu proiektuaren faktura-proposamena

Proiektu-faktura-proposamenak bezeroarentzako proiektu-fakturak sortzeko erabiltzen dira. PWP eszenatokian, saltzaileen ordainketak bezeroen ordainketen menpe daude PWP ezarpenen arabera. Hala ere, ordainketak bezeroak behar duzun moduan ordaindu gabe askatzeko aukerak daude. Jarraitu urrats hauei proiektuaren faktura bezeroarentzako sortzeko.

1. Customer engagement aplikazioetan, joan **Proiektua** \> **Proiektuak** eta hautatu proiektua.
2. Gainean **Benetakoak** fitxan, hautatu hau duen POk sortzen duen benetako lerroa **Fakturatu gabeko salmentak** transakzio mota. Ondoren, hautatu **Fakturarako prest**.
3. Joan **Salmentak** \> **Salmentak** \> **Proiektuaren kontratua**, eta hautatu proiektuaren kontratua.
4. Bezeroaren faktura sortzeko ekintza panelean, hautatu **Faktura**.
5. Finance-n joan **Proiektuaren kudeaketa eta kontabilitatea** \> **Periodikoa** \> **Inportatu fase taulatik**, eta hautatu **Ados** Project operations integratzeko egunkaria sortzeko.
6. Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Proiektuaren fakturak** \> **Proiektuaren faktura-proposamena**, eta hautatu **Argitalpena** proiekturako sortu zen faktura-proposamena argitaratzeko.

## <a name="update-a-customer-payment-and-pay-the-vendor"></a>Eguneratu bezeroaren ordainketa eta ordaindu saltzaileari

Saltzaile batek proiektu batean egindako lana amaitzen duenean eta faktura bat bidaltzen dizunean, proiektuaren egoera eta bezeroaren fakturak berrikusi behar dituzu proiektuan PWP baldintzak betetzen diren ala ez jakiteko. Saltzailearen PWP baldintzak betetzen badira, saltzailearen fakturan zein lerro ordaindu behar dituzun zehaztu dezakezu, proiektuaren bezeroen ordainketen arabera. Saltzaileari ordaintzea erabakitzen baduzu PWP baldintzak betetzen ez diren arren, PWP baldintzak gainidatzi ditzakezu **Saltzailearen faktura ordainduta ordaindutakoan** orrialdea.

1. Finance-n, joan **Proiektuen kudeaketa eta kontabilitatea** \> **Proiektuak** \> **Proiektu guztiak** aukerara, eta hautatu proiektu bat.
2. Ekintza panelean, hautatu **Kontrola**, eta gero hautatu **Saltzaileen fakturak** proiekturako sortu diren saltzaileen faktura guztiak erakusteko.
3. **Saltzailearen fakturak ordaindutako ordainduta** orrialdean, bilaketa eremuan, sartu balioak berrikusi nahi duzun saltzailearen faktura aurkitzeko, eta hautatu **Bilatu**.
4. Hautatu **Ordaindu ordaintzean** PWP fakturak soilik ikusteko aukera.
5. **Saltzailearen faktura lerroak** Fast Tab-en, hautatu ordaintzeko argitaratu nahi dituzun lerroak.
6. Hautatu **Saltzaileen ordainketa askatu**. **Ordaindu ordaintzen denean** aukera garbitu egiten da, eta **Ordaintzeko prest** eremua aldatu egiten da **Bai**.
