---
title: Saltzaileen fakturazioa - Kontzeptua eta sorkuntza
description: Artikulu honek saltzaileen fakturen kontzeptua deskribatzen du, erabilera-agertokiak eta Microsoft Dynamics 365 Project Operations-en nola sortu saltzaileen fakturak azaltzen du.
author: rumant
ms.date: 03/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: b57ec8cdb6097e6f2207056667aadfb43ee8acfc
ms.sourcegitcommit: b2224d1f3c0bd4925d647e6ca3960db81a209521
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/11/2022
ms.locfileid: "9261919"
---
# <a name="vendor-invoicing---concept-and-creation"></a>Saltzaileen fakturazioa - Kontzeptua eta sorkuntza

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Saltzaileen fakturazioa Microsoft Dynamics 365 Project Operations-en saltzaileek proiektu batean zerbitzu eta/edo material bidalketen kostuak erregistratzeko erabil daiteke.

Zerbitzuak eta/edo materialak saltzaile bati azpikontratatzen zaizkionean, azpikontratu batek saltzaile horrekin duen kontratu-hitzarmena adierazten du. Saltzaileak zerbitzuak ematen dituen heinean, edo materialak proiektuko zereginetan jaso eta erabiltzen diren heinean, kostuak proiektuan erregistratzen dira. Aldian-aldian, saltzaileak egiaztatzen diren eta proiektuan erregistratzen diren kostuekin bat datozen fakturak bidaltzen ditu. Egiaztapen-prozesua amaitu ondoren, saltzailearen faktura berretsi eta ordaintzeko kaleratuko da.

## <a name="scenarios-for-use"></a>Erabilera-agertokiak

Project Operations-en hornitzaileen fakturak bi agertoki bereizteko erabil daitezke.

### <a name="customers-use-the-full-subcontracting-experiences"></a>Bezeroek azpikontratazio esperientzia osoa erabiltzen dute

Saltzaileen fakturen esperientziek azpikontratatutako osagaiak aipatzen dituzten denbora-sarrerak, material-erabilera eta gastu-sarrerak egiaztatzeko eta hornitzaileen faktura-lerroekin lotzeko modua eskaintzen dute. Prozesu hau saltzaileen fakturen lerroen zehaztasuna egiaztatzeko erabil daiteke. Egiaztapen-prozesua amaitu eta hornitzailearen faktura berretsi ondoren, aplikazioak onartutako denbora, gastu eta materialen erabilera-erregistroek erregistratutako benetakoak alderantzikatzen ditu, eta, ondoren, kostu erreal berriak sortzen ditu saltzaileen faktura-lerroak erabiliz.

### <a name="customers-dont-use-the-full-subcontracting-experiences-but-want-to-have-a-unified-view-of-costs-on-projects-in-project-operations"></a>Bezeroek ez dituzte azpikontratazio esperientzia osoak erabiltzen, baina proiektuen kostuen ikuspegi bateratua izan nahi dute Project Operations-en

Azpikontratazio-prozesuaren jarraipena egiten ari bazara hirugarrenen sistema batean, hirugarrenen sistema horretatik kostuak erregistra ditzakezu Project Operations-en, azpikontrataziorik aipatzen ez duten hornitzaileen fakturak sortuz. Modu honetan, zure proiektu-kudeatzaileek proiektu jakin bateko kostu guztien ikuspegi bakarra eta bateratua izan dezakete.

## <a name="creation-of-vendor-invoices-in-project-operations"></a>Proiektuaren fakturak sortzea Project Operations-en

Saltzaileen fakturak sortzeko bi modu daude:

- Saltzaileen fakturen zerrenda orritik edo hornitzaile bakarreko fakturaren xehetasunen orrialdetik
- Azpikontratu zerrendako orrialdetik edo azpikontratu bakar baten xehetasunen orrialdetik

### <a name="creation-from-the-vendor-invoice-list-page-or-details-page"></a>Saltzaileen fakturen zerrenda orritik edo xehetasunen orritik sortu

1. Joan **Erosketak** \> **Saltzaileen fakturak**.
2. Saltzaileen fakturen zerrenda orrian edo saltzailearen faktura bakar baten xehetasunen orrian, hautatu **Berria** saltzailearen faktura berri bat sortzeko.

Modu honetan sortzen diren saltzaileen fakturek azpikontratu bati ere erreferentzia egin dezakete.

### <a name="creation-from-the-subcontract-list-page-or-details-page"></a>Azpikontratuaren zerrenda orritik edo xehetasunen orritik sortu

1. Joan **Erosketak** \> **Azpikontratuak**.
2. Hautatu azpikontratu bat edo gehiago.
3. Azpikontratuen zerrenda orrian edo azpikontratu bakar baten xehetasunen orrian, hautatu **Sortu saltzailearen faktura** saltzailearen faktura berri bat sortzeko.

Saltzaileen faktura berri bat sortzen da **Zirriborroa** egoeran hautatu duzun azpikontratu bakoitzeko.

Modu honetan sortzen dituzun saltzaile-fakturek beti aipatzen dute saltzaile-fakturen goiburuan azpikontratua. Denbora eta materiala fakturatzeko metodoa duen azpikontratuko lerro bakoitzak saltzaileen fakturan lerro bat sortuko du. Prezio finkoko fakturazio-metodoa duen azpikontratuko lerro bakoitzak saltzaileen fakturan lerro bat sortuko du **Fakturatzeko prest** egoera duen azpikontratuaren lerro-mugarri bakoitzeko.

Eremu hauek eta erlazionatutako erregistroak azpikontratutik saltzaileen fakturaren goiburuan kopiatuko dira:

- Saltzailea.
- Lotutako prezio-zerrendak saltzaileen fakturan kopiatuko dira prezio-zerrenda gisa.
- Moneta.
- Kontratatzailearen unitatea.
- Ordaintzeko baldintzak.

Denbora eta materialaren azpikontratuaren lerroetarako, eremu hauek eta erlazionatutako erregistroak azpikontratuaren lerrotik saltzaileen faktura lerrora kopiatuko dira:

- Azpikontratu eta azpikontratuaren lerroen erreferentziak
- Transakzio-klasea
- Funtzioa
- Transakzio-kategoria
- Produktuaren eremuak
- Project
- Zeregina
- Baliabide erreserbagarria

Prezio finkoaren azpikontratuaren lerroetarako, eremu hauek eta azpikontratuaren lerrotik eta azpikontratuaren lerroaren mugarritik saltzaileen faktura lerrora kopiatuko dira:

- Azpikontratu eta azpikontratuaren lerroen erreferentziak.
- Transakzio-klasea. Lehenespenez, balioa izango da **Mugarria**.
- Mugarriaren izena eta zenbatekoa erlazionatutako azpikontratuaren lerroaren mugarritik kopiatuko dira.
- Erabiltzaileak proiektu eta zeregin bat hautatu ahal izango ditu saltzaileen faktura lerroan.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
