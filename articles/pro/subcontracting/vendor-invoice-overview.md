---
title: Saltzaileen fakturazioa - Kontzeptua eta sorkuntza
description: Artikulu honek hornitzaileen fakturen kontzeptua, erabiltzeko eszenatokiak eta Microsoft-en hornitzaileen fakturak nola sortu deskribatzen ditu Dynamics 365 Project Operations.
author: rumant
ms.date: 03/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 38f0760697522b7a5e561cec7d38dfd5c3eaf9fc
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8911443"
---
# <a name="vendor-invoicing---concept-and-creation"></a>Saltzaileen fakturazioa - Kontzeptua eta sorkuntza

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Saltzaileen fakturazioa Microsoft-en Dynamics 365 Project Operations saltzaileek proiektu bateko zerbitzu eta/edo material bidalketen kostuak erregistratzeko erabil daiteke.

Zerbitzuak eta/edo materialak saltzaile bati azpikontratatzen zaizkionean, azpikontratu batek saltzaile horrekin duen kontratu-hitzarmena adierazten du. Saltzaileak zerbitzuak ematen dituen heinean, edo materialak jaso eta proiektuko zereginetan erabiltzen diren heinean, kostuak proiektuan erregistratzen dira. Aldian-aldian, saltzaileak fakturak bidaltzen ditu proiektuan erregistratuta dauden eta egiaztatutako kostuekin bat egiten dutenak. Egiaztapen-prozesua amaitu ondoren, saltzailearen faktura berretsi eta ordaintzeko kaleratzen da.

## <a name="scenarios-for-use"></a>Erabiltzeko eszenatokiak

Proiektu Eragiketetan hornitzaileen fakturak bi agertoki bereizteko erabil daitezke.

### <a name="customers-use-the-full-subcontracting-experiences"></a>Bezeroek azpikontratazio esperientzia osoa erabiltzen dute

Saltzaileen fakturen esperientziek saltzaileen faktura-lerroekin azpikontratatutako osagaiak aipatzen dituzten denbora-sarrerak, materialaren erabilera eta gastu-sarrerak egiaztatzeko eta lotzeko modua eskaintzen dute. Prozesu hau saltzaileen fakturen lerroen zehaztasuna egiaztatzeko erabil daiteke. Egiaztapen-prozesua amaitu eta hornitzailearen faktura berretsi ondoren, aplikazioak onartutako denbora, gastu eta materialaren erabilera-erregistroek erregistratutako benetakoak alderantzikatuko ditu, eta kostu erreal berriak sortuko ditu saltzaileen faktura-lerroak erabiliz.

### <a name="customers-dont-use-the-full-subcontracting-experiences-but-want-to-have-a-unified-view-of-costs-on-projects-in-project-operations"></a>Bezeroek ez dituzte azpikontratazio esperientzia osoak erabiltzen, baina proiektuen kostuen ikuspegi bateratua izan nahi dute Proiektuen Eragiketetan.

Hirugarrenen sistema batean azpikontratazio prozesuaren jarraipena egiten ari bazara, hirugarrenen sistema horretatik kostuak erregistra ditzakezu Project Operations-en, azpikontrataziorik aipatzen ez duten hornitzaileen fakturak sortuz. Modu honetan, zure proiektu-kudeatzaileek proiektu jakin bateko kostu guztien ikuspegi bakarra eta bateratua izan dezakete.

## <a name="creation-of-vendor-invoices-in-project-operations"></a>Saltzaileen fakturak sortzea Proiektu Eragiketetan

Saltzaileen fakturak bi modutara sor daitezke:

- Saltzaileen fakturen zerrenda orritik edo hornitzaile bakarreko fakturaren xehetasunen orrialdetik
- Azpikontratuen zerrendako orrialdetik edo azpikontratu bakar baten xehetasunen orrialdetik

### <a name="creation-from-the-vendor-invoice-list-page-or-details-page"></a>Hornitzaileen fakturen zerrendako orrialdetik edo xehetasunen orritik sortzea

1. Joan **Erosketak** \> **Saltzaileen fakturak**.
2. Saltzaileen fakturen zerrenda orrian edo hornitzaileen faktura bakar baten xehetasunen orrian, hautatu **Berria** hornitzaile-faktura berri bat sortzeko.

Horrela sortzen diren saltzaileen fakturek azpikontratu bati ere erreferentzia egin dezakete.

### <a name="creation-from-the-subcontract-list-page-or-details-page"></a>Azpikontratuen zerrendako orrialdetik edo xehetasunen orritik sortzea

1. Joan **Erosketak** \> **Azpikontratak**.
2. Aukeratu azpikontratu bat edo gehiago.
3. Azpikontratu zerrendako orrian edo azpikontratu bakar baten xehetasunen orrian, hautatu **Sortu saltzaileen faktura** hornitzaile-faktura berri bat sortzeko.

Saltzaileen faktura berri bat sartu da **Zirriborroa** hautatutako azpikontratu bakoitzeko egoera sortzen da.

Modu honetan sortzen dituzun saltzaile-fakturek beti aipatzen dute saltzaile-fakturen goiburuan azpikontratua. Denbora eta materiala fakturatzeko metodoa duen azpikontratuko lerro bakoitzak saltzaileen fakturan lerro bat sortuko du. Prezio finkoko fakturazio-metodoa duen azpikontratuko lerro bakoitzak saltzaileen fakturan lerro bat sortuko du egoera duen azpikontratuaren lerro-mugarri bakoitzeko.**Fakturatzeko prest**.

Eremu hauek eta erlazionatutako erregistroak azpikontratutik saltzaileen fakturaren goiburuan kopiatuko dira:

- Saltzailea.
- Lotutako prezio-zerrendak saltzaileen fakturan kopiatuko dira prezio-zerrenda gisa.
- Moneta.
- Kontratazio-unitatea.
- Ordainketa baldintzak.

Denbora eta materialaren azpikontratazio lerroetarako, eremu hauek eta erlazionatutako erregistroak azpikontratu lerrotik saltzaileen faktura lerrora kopiatuko dira:

- Azpikontratazio eta azpikontratazio lerroen erreferentziak
- Transakzio-klasea
- Funtzioa
- Transakzio-kategoria
- Produktu-eremuak
- Project
- Zeregina
- Baliabide erreserbagarria

Prezio finkoko azpikontratazio-lerroetarako, eremu hauek azpikontratazio lerrotik eta azpikontratu lerroko mugarritik saltzaileen faktura lerrora kopiatuko dira:

- Azpikontratazio eta azpikontratazio lerroen erreferentziak.
- Transakzio klasea. Lehenespenez, balioa izango da **Mugarria**.
- Mugarriaren izena eta zenbatekoa erlazionatutako azpikontratuaren lerroko mugarritik kopiatuko dira.
- Erabiltzaileak proiektu eta zeregin bat hautatu ahal izango ditu saltzaileen faktura lerroan.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
