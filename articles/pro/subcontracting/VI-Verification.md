---
title: Saltzailearen fakturen egiaztapena onartutako benetako datuekin
description: Artikulu honek Microsoft-ek nola egiten duen azaltzen du Dynamics 365 Project Operations ditzagun proiektu-zuzendariek egiazta ditzagun saltzaileen fakturak kontratistak lana egin eta denbora erregistratu ahala onartutako benetakoekin eta proiektuko taldekideek erabili zituzten gastu eta materialekin.
author: rumant
ms.date: 03/30/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 7bf48dd17063daece5df3ce44c0375eec3dc3cae
ms.sourcegitcommit: 49c2a668b8d7bf0acb9e9b0bb44687e6d3dcaa8c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 07/28/2022
ms.locfileid: "9204159"
---
# <a name="verification-of-vendor-invoices-with-approved-actuals"></a>Saltzailearen fakturen egiaztapena onartutako benetako datuekin

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Microsoft Dynamics 365 Project Operations ditzagun proiektu-kudeatzaileek saltzaileen faktura-lerroak egiazta ditzagun modu hauetan:

- Erabili **Egiaztapen-egoera** hornitzaileen faktura lerroetan.
- Hornitzaileen faktura-lerroek azpikontratu-lerro bati erreferentzia egiten badiote, lotu azpikontratistaren jardueraren kostu errealak saltzaileen faktura-lerro horiekin. Esteka kostu errealak saltzaileen faktura-lerroekin lotuz sortzen da.

    > [!NOTE]
    > Azpikontratu bat aipatzen ez duten hornitzaileen faktura-lerroen egiaztapen-egoeraren jarraipena egin daitekeen arren, kostu errealak ezin dira lotu saltzaileen faktura-lerro horiei.

## <a name="verification-status"></a>Egiaztapen-egoera

The **Egiaztapen-egoera** Saltzaileen faktura lerroko eremuak egiaztapenaren egoera adierazten du. Egoera hauek onartzen dira:

1. Ez da hasi
2. Abian
3. Osoa

Egiaztapen-egoera duten saltzaileen faktura-lerroak **Ez da hasi** editatu daiteke.

Egiaztapen-egoera duten saltzaileen faktura-lerroak **Abian** jada ezin da editatu. Azpikontratu bati erreferentzia egiten dion saltzaileen faktura-lerro baterako, egiaztapen-egoera automatikoki ezarriko da **Abian** lehen kostu erreala saltzaileen faktura-lerroarekin bat datorren bezain laster.

Egiaztapen-egoera duten saltzaileen faktura-lerroak **Osatu** jada ezin da editatu. Saltzaile-faktura bateko lerro guztiek egiaztapen-egoera hori dutenean, saltzaile-faktura berretsi daiteke.

## <a name="match-cost-actuals-to-vendor-invoice-lines"></a>Lotu kostu errealak saltzaileen faktura-lerroekin

Kostu errealak parekatzeak saltzaileen faktura-lerro batean egiaztatze-prozesuan laguntzen du. Kostu errealak saltzaileen faktura-lerro batekin lotzeko, jarraitu urrats hauek.

1. Ireki hornitzailearen faktura-lerroa eta hautatu **Kostu errealak paregabeak** fitxa. Sare batek saltzaileen faktura-lerroaren azpikontratazio-lerro bera aipatzen duten kostu errealen zerrenda erakusten du.
2. Hautatu kostu errealetako bat edo gehiago, eta, ondoren, hautatu **Partidua** sarearen gaineko tresna-barran. Sistemak balioztatzen du hautatutako kostu errealak parekatu daitezkeela. Balioztatzea gainditu ondoren, kostu errealak saltzaileen faktura-lerroarekin lotzen dira.

### <a name="validation-criteria-that-are-used-to-link-cost-actuals-to-vendor-invoice-lines"></a>Kostu errealak saltzaileen faktura-lerroekin lotzeko erabiltzen diren baliozkotze-irizpideak

Bat-etortze-prozesuan, kostu errealaren eta saltzaileen faktura-lerroaren arteko lotura bat ezarri ahal izango da baldintza hauek betetzen badira soilik:

- The **Doikuntza egoera** hautatutako kostu erreal bakoitzeko eremuak hutsik egon behar du. Beste era batera esanda, kostu errealak ez dira beste kostu erreal batzuekin ordezkatu behar gogoraraztean, onarpenean bertan behera uztean edo zuzenketa aldizkariaren prozesu batean.
- Ondorengo eremuen balioak hornitzaileen faktura-lerroaren eta hautatutako kostu errealaren artean bat egiten dute. Saltzaileen faktura-lerroan eremuren bat ezartzen ez bada, ez da bat etortzeko kontuan hartuko.

    - Proiektu-kontratua
    - Proiektu-kontratuaren lerroa
    - Transakzio-klasea
    - Project
    - Zeregina
    - Baliabideen kategoria
    - Transakzio-kategoria
    - Produktu
    - Azpikontratazio lerroa
    - Baliabide erreserbagarria

## <a name="unmatch-cost-actuals-from-a-vendor-invoice-line"></a>Bateratu saltzaileen faktura-lerro bateko kostu errealak

Kostu errealak ez-parekatzeak saltzaileen fakturako egiaztapen-prozesuan ere lagun dezake, aurretik ezarritako estekak kentzeko aukera emanez. Kostu errealak egiaztapen-egoera duten hornitzaileen faktura-lerroetatik soilik izan daitezke **Abian**. Hornitzaileen faktura-lerro bateko kostu errealak parekatzeko, jarraitu urrats hauek.

1. Ireki hornitzailearen faktura-lerroa eta hautatu **Batekatutako kostu errealak** fitxa. Sare batek saltzaileen faktura-lerroari erreferentzia egiten dioten kostu errealen zerrenda erakusten du.
2. Hautatu kostu errealetako bat edo gehiago, eta hautatu **Bat-etortzea** sarearen gaineko tresna-barran.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]