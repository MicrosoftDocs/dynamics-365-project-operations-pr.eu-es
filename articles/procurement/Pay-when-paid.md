---
title: Ordaindu saltzaileen ordainketak ordaintzean
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
# <a name="pay-when-paid-vendor-payments"></a>Ordaindu saltzaileen ordainketak ordaintzean

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai honek ordaintzean ordaindutako egoera (PWP) nola erabili azaltzen du.

## <a name="create-a-purchase-order-that-has-pwp-terms"></a>Sortu PWP baldintzak dituen erosketa-eskaera

Saltzaile baten faktura bat argitaratzen duzunean, saltzailea PWP baldintzen menpe badago, baldintza horiek erosketa-eskaeraren (PO) lerroetan agertzen dira. PWP baldintzak dituen PO bat sortzeko, jarraitu urrats hauei.

1. In Microsoft Dynamics 365 Finantza, jarraitu urrats hauetako bat:

    - Joan **Kontratazioa eta hornidura** \> **Erosketa aginduak** \> **Erosketa eskaera guztiak**. Ekintza panelean, hautatu **Berria**. urtean **Sortu erosketa-eskaera** elkarrizketa-koadroa, hautatu proiektuan PWP baldintzak ezarrita dauden hornitzailea, idatzi behar den beste informazio bat eta hautatu **ADOS**.
    - Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Proiektuak** \> **Proiektu guztiak**. Ekintza-panelean, gunean **Kudeatu** fitxa, hautatu **Elementuaren zeregina**. Hautatu erosketa-eskaera. Hautatu proiektuan PWP baldintzak konfiguratu dituen hornitzailea eta, ondoren, hautatu **Ados**.

2. Gainean **Erosketa-eskaera** orrialdean, **Erosketa-eskaeraren lerroak** Fitxa azkarra, hautatu **Gehitu lerroa** erosketa-eskaeraren lerroa sortzeko.
3. Hautatu elementu-zenbakia edo kontratazio-kategoria eta sartu beharrezko gainerako xehetasunak. Berrikusi saltzailearentzat PO-lerroaren xehetasunak.

    **Ordaindu ordaintzen denean** aukera automatikoki hautatzen da eta balioa **PWP atalasearen ehunekoa** eremua automatikoki kopiatzen da **PWP atalasearen ehunekoa** eremuan **Proiektuak** orrialdea.

4. Ez baduzu nahi PWP baldintzak saltzaileari PO linea baterako aplikatu, garbitu **Ordaindu ordaintzen denean** aukera. Kasu honetan, **PWP atalasearen ehunekoa** PO linearen eremua berrezarriko da **0** (zero).
5. Gainean **Erosketa-eskaera** orrialdean, Ekintza-panelean, atalean **Erosketa** fitxa, hautatu **Berretsi** erosketa-eskaera berresteko.
6. Ekintza-panelean, gunean **Faktura** fitxa, hautatu **Faktura** erosketa-eskaeraren faktura sortzeko.

## <a name="create-a-project-invoice-proposal"></a>Sortu proiektuaren faktura-proposamena

Proiektu-faktura-proposamenak bezeroarentzako proiektu-fakturak sortzeko erabiltzen dira. PWP eszenatokian, saltzaileen ordainketak bezeroen ordainketen menpe daude PWP ezarpenen arabera. Hala ere, ordainketak bezeroak behar duzun moduan ordaindu gabe askatzeko aukerak daude. Bezeroarentzat proiektuaren faktura bat sortzeko, jarraitu urrats hauek.

1. Bezeroen parte hartzeko aplikazioetan, joan hona **Proiektua** \> **Proiektuak**, eta hautatu proiektua.
2. Gainean **Benetakoak** fitxan, hautatu hau duen POk sortzen duen benetako lerroa **Fakturatu gabeko salmentak** transakzio mota. Ondoren, hautatu **Fakturarako prest**.
3. Joan **Salmentak** \> **Salmentak** \> **Proiektuaren kontratua**, eta hautatu proiektuaren kontratua.
4. Ekintza panelean, hautatu **Faktura** bezeroaren faktura sortzeko.
5. Finantzan, joan hona **Proiektuen kudeaketa eta kontabilitatea** \> **Periodikoa** \> **Inportatu eszenatze-taulatik**, eta hautatu **Ados** Proiektuaren eragiketen integrazio aldizkaria sortzeko.
6. Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Proiektuaren fakturak** \> **Proiektuaren faktura-proposamena**, eta hautatu **Argitalpena** proiekturako sortu zen faktura-proposamena argitaratzeko.

## <a name="update-a-customer-payment-and-pay-the-vendor"></a>Eguneratu bezeroaren ordainketa eta ordaindu saltzaileari

Hornitzaile batek proiektu batean bere lana amaitzen duenean eta faktura bat bidaltzen dizunean, proiektuaren egoera eta bezeroen fakturak berrikusi behar dituzu proiekturako PWP baldintzak betetzen ziren ala ez zehazteko. Saltzailearen PWP baldintzak betetzen badira, saltzailearen fakturan zein lerro ordaindu behar dituzun zehaztu dezakezu, proiektuaren bezeroen ordainketen arabera. Saltzaileari ordaintzea erabakitzen baduzu PWP baldintzak betetzen ez diren arren, PWP baldintzak gainidatzi ditzakezu **Saltzailearen faktura ordainduta ordaindutakoan** orrialdea.

1. Finantzan, joan hona **Proiektuen kudeaketa eta kontabilitatea** \> **Proiektuak** \> **Proiektu guztiak**, eta hautatu proiektua.
2. Ekintza panelean, hautatu **Kontrola**, eta gero hautatu **Saltzaileen fakturak** proiekturako sortu diren saltzaileen faktura guztiak erakusteko.
3. **Saltzailearen fakturak ordaindutako ordainduta** orrialdean, bilaketa eremuan, sartu balioak berrikusi nahi duzun saltzailearen faktura aurkitzeko, eta hautatu **Bilatu**.
4. Hautatu **Ordaindu ordaintzean** PWP fakturak soilik ikusteko aukera.
5. Gainean **Saltzaileen faktura lerroak** Fitxa azkarra, hautatu ordainketarako askatu nahi dituzun lerroak.
6. Hautatu **Saltzaileen ordainketa askatu**. **Ordaindu ordaintzen denean** aukera garbitu egiten da, eta **Ordaintzeko prest** eremua aldatu egiten da **Bai**.
