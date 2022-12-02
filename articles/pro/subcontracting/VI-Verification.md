---
title: Saltzailearen fakturen egiaztapena onartutako benetako datuekin
description: Artikulu honek nola egiten duen azaltzen du Microsoft Dynamics 365 Project Operations ditzagun proiektu-zuzendariek egiazta ditzagun hornitzaileen fakturak kontratistak lanak egin eta denbora erregistratu ahala onartu ziren benetakoekin, eta proiektuko taldekideek erabili zituzten gastu eta materialekin.
author: rumant
ms.date: 03/30/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 67e0a0143fa354ca9a87bfac5fbbd6306a97811c
ms.sourcegitcommit: 08eb3be9eda44e9446c43ed9b6aefd58d77927c5
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/15/2022
ms.locfileid: "9522927"
---
# <a name="verification-of-vendor-invoices-with-approved-actuals"></a>Saltzailearen fakturen egiaztapena onartutako benetako datuekin

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Microsoft Dynamics 365 Project Operations ditzagun proiektu-kudeatzaileek saltzaileen faktura-lerroak egiazta ditzagun modu hauetan:

- Erabili **Egiaztapen-egoera** hornitzaileen faktura lerroetako eremua.
- Hornitzaileen faktura-lerroek azpikontratu-lerro bati erreferentzia egiten badiote, lotu azpikontratistaren jardueraren kostu errealak saltzaileen faktura-lerro horiekin. Esteka kostu errealak saltzaileen faktura-lerroekin lotuz sortzen da.

    > [!NOTE]
    > Azpikontratu bat aipatzen ez duten hornitzaileen faktura-lerroen egiaztapen-egoeraren jarraipena egin daitekeen arren, kostu errealak ezin dira lotu saltzaile-faktura-lerro horiei.

## <a name="verification-status"></a>Egiaztapenaren egoera

**Egiaztapen-egoera** Saltzaileen faktura lerroko eremuak egiaztapenaren egoera adierazten du. Egoera hauek onartzen dira:

1. Ez da hasi
2. Abian
3. Osoa

Saltzailearen faktura-lerroa **Hasi gabe** egiaztapen-egoerarekin soilik edita daiteke

Saltzailearen faktura-lerroa **Abian** egiaztapen-egoerarekin ezin dira editatu. Azpikontratu bati erreferentzia egiten dion saltzaileen faktura-lerro baterako, egiaztapen-egoera automatikoki ezarriko da **Abian** lehen kostu erreala saltzaileen faktura-lerroarekin bat datorren bezain laster.

Saltzailearen faktura-lerroa **Osatuta** egiaztapen-egoerarekin ezin dira editatu. Saltzaile-faktura bateko lerro guztiek egiaztapen-egoera hori dutenean, saltzaile-faktura berretsi daiteke.

## <a name="match-cost-actuals-to-vendor-invoice-lines"></a>Saltzailearen fakturaren lerroekin bat etorri kostuen benetako datuak

Kostu errealak parekatzeak saltzaileen faktura-lerro batean egiaztatze-prozesuan laguntzen du. Kostu errealak saltzaileen faktura-lerro batekin lotzeko, jarraitu urrats hauek.

1. Ireki hornitzailearen faktura-lerroa eta hautatu **Kostu errealak paregabeak** fitxa. Sare batek saltzaileen faktura-lerroaren azpikontratazio-lerro bera aipatzen duten kostu errealen zerrenda erakusten du.
2. Hautatu kostu errealetako bat edo gehiago, eta hautatu **Bat etorri** sarearen gaineko tresna-barran. Sistemak balioztatzen du hautatutako kostu errealak parekatu daitezkeela. Balioztatzea gainditu ondoren, kostu errealak saltzaileen faktura-lerroarekin lotzen dira.

### <a name="validation-criteria-that-are-used-to-link-cost-actuals-to-vendor-invoice-lines"></a>Kostu errealak saltzaileen faktura-lerroekin lotzeko erabiltzen diren baliozkotze-irizpideak

Bat-etortze-prozesuan, kostu errealaren eta saltzaileen faktura-lerroaren arteko lotura ezarri ahal izango da baldintza hauek bi betetzen badira soilik:

- **Doikuntza egoera** hautatutako kostu erreal bakoitzeko eremuak hutsik egon behar du. Beste era batera esanda, kostu errealak ez dira beste kostu erreal batzuekin ordezkatu behar berreskurapenean, onarpenean bertan behera uzteko edo zuzenketa aldizkariko prozesu batean.
- Ondorengo eremuen balioak hornitzaileen faktura-lerroaren eta hautatutako kostu errealaren artean bat egiten dute. Saltzaileen faktura-lerroan eremuren bat ezartzen ez bada, ez da bat etortzeko kontuan hartuko.

    - Proiektu-kontratua
    - Proiektu-kontratuaren lerroa
    - Transakzio-klasea
    - Project
    - Zeregina
    - Baliabidearen kategoria
    - Transakzio-kategoria
    - Produktu
    - Azpikontratuaren lerroa
    - Baliabide erreserbagarria

## <a name="unmatch-cost-actuals-from-a-vendor-invoice-line"></a>Saltzailearen fakturaren lerro batekin lotu gabeko benetako kostuak

Kostu errealak ez lotzeak saltzaileen fakturako egiaztapen-prozesuan ere lagun dezake, aurretik ezarritako estekak kentzeko aukera emanez. Saltzailearen faktura-lerroa **Abian** egiaztapen-egoerarekin ezin dira kendu kostuaren datu erreala saltzailetik. Kostu errealak saltzaileen faktura-lerro batetik lotura kentzeko, jarraitu urrats hauek.

1. Ireki hornitzailearen faktura-lerroa eta hautatu **Kostu errealak bat etorrita** fitxa. Sare batek saltzaileen faktura-lerroa aipatzen duten kostu errealen zerrenda erakusten du.
2. Hautatu kostu errealetako bat edo gehiago, eta hautatu **Kendu bat-etortzea** sarearen gaineko tresna-barran.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
