---
title: Sortu saltzailearen fakturak
description: Artikulu honek saltzaileen fakturen kontzeptua deskribatzen du eta Microsoft Dynamics 365 Project Operations-en nola sortu azaltzen du.
author: suvaidya
ms.date: 9/12/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: suvaidya
ms.openlocfilehash: 7f6c1ec46f23b6823734b28755b80ced4e3f9325
ms.sourcegitcommit: 60a34a00e2237b377c6f777612cebcd6380b05e1
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/13/2022
ms.locfileid: "9475454"
---
# <a name="create-vendor-invoices"></a>Sortu saltzailearen fakturak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Artikulu honetan deskribatzen den funtzionaltasuna erabiltzeko, gaitu behar duzu **Gaitu azpikontratazio errealak prozesatzea Project Operations-ekin baliabideetan oinarritutako agertokietarako** ezaugarria **Ezaugarrien kudeaketa** lan-eremuan.

Saltzaileen fakturazioa Microsoft Dynamics 365 Project Operations-en saltzaileek burututako proiektu batean zerbitzu eta/edo material bidalketen kostuak erregistratzeko erabil daiteke.

Zerbitzuak eta/edo materialak saltzaile bati azpikontratatzen zaizkionean, azpikontratu batek saltzaile horrekin duen kontratu-hitzarmena adierazten du. Saltzaileak zerbitzuak ematen dituen heinean, edo materialak proiektuko zereginetan jaso eta erabiltzen diren heinean, kostuak proiektuan erregistratzen dira. Ondoren, saltzaileak fakturak bidaltzen ditu aldizka. Faktura horiek egiaztatzen dira eta proiektuan erregistratzen diren kostuekin lotzen dira. Egiaztapen-prozesua amaitu ondoren, saltzailearen faktura berretsi eta ordaintzeko kaleratuko da.

## <a name="scenarios-for-use"></a>Erabilera-agertokiak

Project Operations-en hornitzaileen fakturak bi agertoki bereizteko erabil daitezke:

- Bezeroek azpikontratazio esperientzia osoa erabiltzen dute.
- Bezeroek ez dituzte azpikontratazio esperientzia osoak erabiltzen, baina proiektuen kostuen ikuspegi bateratua izan nahi dute Project Operations-en.

### <a name="customers-use-the-full-subcontracting-experiences"></a>Bezeroek azpikontratazio esperientzia osoa erabiltzen dute

Saltzaileen fakturen esperientziek azpikontratatutako osagaiak aipatzen dituzten denbora-sarrerak, material-erabilera eta gastu-sarrerak egiaztatzeko eta hornitzaileen faktura-lerroekin lotzeko modua eskaintzen dute. Prozesu hau saltzaileen fakturen lerroen zehaztasuna egiaztatzeko erabil daiteke. Egiaztapen-prozesua amaitu eta hornitzailearen faktura berretsi ondoren, sistemak onartutako denbora, gastu eta materialen erabilera-erregistroek erregistratutako benetakoak alderantzikatzen ditu, eta, ondoren, kostu erreal berriak sortzen ditu saltzaileen faktura-lerroak erabiliz.

### <a name="customers-dont-use-the-full-subcontracting-experiences-but-want-to-have-a-unified-view-of-costs-on-projects-in-project-operations"></a>Bezeroek ez dituzte azpikontratazio esperientzia osoak erabiltzen, baina proiektuen kostuen ikuspegi bateratua izan nahi dute Project Operations-en

Azpikontratazio-prozesuaren jarraipena egiten ari bazara hirugarrenen sistema batean, hirugarrenen sistema horretatik kostuak erregistra ditzakezu Project Operations-en, azpikontrataziorik aipatzen ez duten hornitzaileen fakturak sortuz. Modu honetan, zure proiektu-kudeatzaileek proiektu jakin bateko kostu guztien ikuspegi bakarra eta bateratua izan dezakete.

## <a name="create-vendor-invoices-in-project-operations"></a>Sortu proiektuaren fakturak Project Operations-en

Hornitzaileen fakturak Dynamics 365 Finance-n sortzen dira, erabiliz **Ordaintzeko kontuak** modulua. Ezin duzu hornitzaileen fakturarik sortu zuzenean Dataverse-n.

### <a name="set-up-vendor-invoice-verification"></a>Konfiguratu saltzaileen fakturen egiaztapena

Saltzaileen faktura azpikontratu baterako zuzenduta badago Dataverse-n, gaitu behar duzu **PMren eskuzko egiaztapena beharrezkoa da** parametroa. Aukeraren ezarpenak saltzaileen faktura automatikoki berretsi behar den zehazten du Dataverse-n, edo eskuzko berrespena behar duen. Proiektuaren saltzaileen faktura bakoitzaren goiburuak izen bereko aukera bat du. Lehenespenez, proiektuko hornitzaileen faktura guztien goiburuko aukera hemen ezartzen duzun balioarekin ezartzen da. Hala ere, balioa egunera dezakezu saltzaileen banakako fakturen goiburuan behar den moduan.

Aukera ezarrita badago **Bai**, Finance-n sortu eta Dataverse-n sinkronizatuta dagoen hornitzailearen fakturak **Zirriborroa** egoera du. Ondoren, faktura proiektuaren kudeatzaileak balioztatu eta egiaztatu behar du, eta berretsi, prozesatu eta Finance-ko proiektu eta liburuko kontu zehatzetan argitaratu aurretik.

Aukera ezarrita badago **Ez**, saltzailearen faktura automatikoki berresten da. Ez da ekintza gehiago behar.

Saltzailearen fakturaren egiaztapena konfiguratzeko, egin hau.

1. Finance-n, joan **Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Proiektuen kudeaketa eta kontabilitate parametroak**.
1. **Finantza** fitxan, ezarri **PMren eskuzko egiaztapena beharrezkoa da** aukera **Bai** gisa enpresaren politika azpikontratistaren saltzaileen fakturak egiaztatzea eskatzen badu. Proiektuaren kudeatzaileak egiaztatzea beharrezkoa ez bada Dataverse-n, utzi aukera multzoa **Ez** gisa. Lehenespenez, ezarpena aplikazioan erabiliko da **Saltzaileen fakturaren zain** orrialdea.

> [!NOTE]
> Dataverse-n azpikontratetarako sortzen diren saltzaileen fakturak behar bezala prozesatu daiteke baldin eta **PMren eskuzko egiaztapena beharrezkoa da** aukera ezarrita dago **Bai**. Azpikontratistek sortzen dituzten denbora, material eta gastuen kostu errealak eskuz parekatu ditzake saltzaileen faktura-lerroekin proiektu-kudeatzaileak aukera hau honela ezartzen badu soilik: **Bai**.

### <a name="set-up-a-procurement-integration-account-for-vendor-invoices"></a>Konfiguratu kontratazioen integrazio kontua saltzaileen fakturetarako

Hornitzaileen faktura bat Finance for Project Operations-en ingurune integratua (ez-izakinak) atalean argitaratzen denean, finantzak Kontratazio integrazio-kontuan argitaratzen dira. Sistemak benetakoak sortzen ditu Dataverse-n argitaratutako fakturarako. Benetako hauek Finance-n argitaratzen dira, proiektuaren integrazio-egunkaria erabiliz. Proiektuaren integrazio-egunkaria argitaratzeak kontratazio-integrazioaren kontuaren egiazko kostua eta atzerakoak argitaratzen ditu.

Konfiguratzeko kontratazioen integrazio kontua saltzaileen fakturetarako, egin hau.

1. Finance-n, joan **Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Proiektuen kudeaketa eta kontabilitate parametroak**.
1. **Project operations on Dynamics 365 customer engagement** fitxan, hautatu **Materialak** \> **Kontratazioaren integrazio kontua**.

### <a name="create-and-post-subcontract-vendor-invoices"></a>Sortu eta argitaratu saltzaileen fakturak

Ordainketa-langile batek azpikontratistaren faktura bat jasotzen duenean, faktura berri bat sortzen da Finantzan.

1. Finantzan, joan hona **Ordaintzeko kontuak** \> **Fakturak** \> **Saltzaileen fakturak zain**.
1. **Ekintza-panelean**, hautatu **Berria** saltzaileen faktura bat sortzeko.
1. Fakturaren goiburuan, **Faktura kontua** eremuan, hautatu **Azpikontratista**.
1. Hautatu fakturaren data.
1. **Goiburua** fitxan, ezarri **PMren eskuzko egiaztapena beharrezkoa da** aukera **Bai**. Aukera honen ezarpen lehenetsia **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdetik dator. Hala ere, saltzaileen faktura mailan alda daiteke.
1. **Faktura lerroa** FastTab, hautatu **Gehitu lerroa** saltzaileen faktura lerro bat sortzeko.
1. Hautatu azpikontratazio-lerroetarako sortu den kontratazio-kategoria eta sartu prezio unitarioa, neurketa-unitatea eta kantitatea.
1. Saltzaileen faktura-lerroen atalean, **Proiektua** fitxan, hautatu azpikontratatzaileak azpikontratuaren faktura partekatzen duen proiektua.
1. Aukeratu proiektuaren kategoria. Edozein motatakoa izan daiteke: **Elementua**, **Gastua**, **Materialak**, edo **Orduak**.
1. Hautatu rola hautatutako proiektuaren kategoriakoa bada soilik **Ordua** mota.
1. Hautatu **Argitaratu** saltzaileen faktura argitaratzeko.

Bestela, saltzaileen faktura bat sor dezakezu helbidera joanez **Ordaintzeko kontuak** \> **Fakturak** \> **Ireki saltzaileen fakturak** eta hautatzea **Berria**.

Saltzaileen faktura argitaratzen denean, eskuragarri egongo da Dataverse-en proiektuaren zuzendaria egiaztatzeko eta prozesatzeko.

## <a name="vendor-invoice-processing-in-dataverse"></a>Saltzailearen faktura-prozesatzea Dataverse-n

Sortzen den saltzaile-fakturan Dataverse-n, eremu-balio batzuk Finantzan erregistratutako saltzaileen fakturatik datoz. Beste balio batzuk azpikontratatik datozen balio lehenetsiak dira.

Eremu hauek eta erlazionatutako erregistroak azpikontratutik saltzaileen fakturaren goiburuan kopiatuko dira:

- Moneta
- Kontratazio-unitatea
- Ordainketa-baldintzak

Hornitzaileen faktura-lerroetan, Project Operations-ek eremu-balio hauek erabiltzen ditu azpikontratu eta azpikontratu lerroaren erreferentzia lehenetsia sartzeko:

- Transakzio-klasea
- Funtzioa
- Transakzio-kategoria
- Produktuaren eremuak
- Project
- Zeregina

> [!NOTE]
> Prezio finkoko azpikontratazio-lerroak ez dira onartzen Project Operations-en.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
