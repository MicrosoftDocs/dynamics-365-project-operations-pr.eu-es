---
title: Zuzendu kontabilitatea zirriborro-proiektu baten fakturazio-proposamenetan
description: Gai honetan faktura proposamenaren zirriborroan kontabilitatearekin lotutako informazioa nola egokitu azaltzen da.
author: sigitac
ms.date: 01/05/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 32f566a798d07b698693392f3aa1823f91fe5408
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8921195"
---
# <a name="correct-the-accounting-on-draft-project-invoice-proposals"></a>Zuzendu kontabilitatea zirriborro-proiektu baten fakturazio-proposamenetan

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

*Xehetasun operatiboak* Proiektuaren fakturak proiektuaren kudeatzaileak mantentzen ditu proformako fakturan. Xehetasun horien artean fakturatu behar diren ordu, gastu, material edo mugarriei buruzko erabakia, tarifak eta aurrerakinaren eta atxikipenen zenbatekoen aplikazioa daude. Proformaren jatorrizko faktura berretsi ondoren, operazio xehetasunak doitu ditzakezu sortuz eta berretsiz [pro forma faktura zuzentzailea](../proforma-invoicing/corrective-invoices.md).

*Kontabilitate xehetasunak* proiektuaren fakturak bezeroari begira faktura dokumentu batean mantentzen dira. Xehetasun horien artean salmenten gaineko zergaren kalkulua eta fakturan aplikatzen diren dimentsio ekonomikoak daude. Gai honetan kontabilitate xehetasun horiek proiektuaren faktura proposamenaren zirriborroan nola egokitu daitezkeen zehazten da.

## <a name="adjust-sales-tax"></a>Egokitu salmenten zerga

Lehenetsitako fakturazioaren salmenten gaineko zerga taldeak eta elementuen salmenten gaineko zerga taldeak zuzenean egokitu daitezke faktura proposamenaren dokumentuan. Talde hauek doitzeko, hautatu **Editatu**, eta, ondoren, proiektuaren faktura proposamen lerro bakoitzean, sartu balio berria **Salmenten gaineko zerga taldea** edo **Artikuluen salmenten gaineko zergaren taldea** eremuan.

## <a name="adjust-financial-dimensions"></a>Egokitu finantza-dimentsioak

### <a name="header-dimensions"></a>Goiburuaren dimentsioak

Lehenespenez, fakturaren finantza-dimentsioak fakturatzen ari diren proiektuko transakzio-erregistroetatik ateratzen dira. Hala ere, sistemaren ezarpenek proiektuaren faktura-proposamenen goiburuko finantza-dimentsioak erabil ditzakezu bezeroen saldoak argitaratzeko. Funtzio hau gaitzeko, hautatu **Onartu proiektuaren dimentsioen eguneraketak kobratzeko kontuetarako** gainean **Finantza** fitxan **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea.

Fakturen goiburuetako finantza-dimentsioak edita daitezke faktura bat argitaratu aurretik. **Proiektuaren faktura-proposamena** orrialdera, aldatu **Goiburua** ikusi, eta, gero, editatu balioak **Dimentsio finantzarioak** fitxa.

**Goiburua** ikuspegia sistemaren administratzaileak gaitu ondoren bakarrik dago erabilgarri **Erabili proiektuak fakturatzeko proposamen eta fakturazio-egunkariaren txantiloiak goiburu eta lerroen ikuspegiekin** funtzioan **Ezaugarrien kudeaketa** laneko arean. Eginbide honek Finantza eguneraketa 10.0.25 edo berriagoa behar du.

### <a name="line-dimensions"></a>Lerro dimentsioak

Finantza dimentsioak ezin dira zuzenean editatu proiektuaren faktura proposamenaren lerroan. Horren ordez, jarraitu urrats hauek proiektuaren faktura proposamen batean dimentsio ekonomikoak doitzeko.

1. Proiektuaren faktura proposamenean, hautatu **Ezabatu guztiak** proiektuaren faktura proposamenen lerroak kentzeko.

    **Ezabatu guztiak** botoia sistemaren administratzaileak gaitu ondoren bakarrik dago erabilgarri **Ezabatu faktura proposamenen lerroak Baliabideetan oinarritutako / gordeta ez dauden eszenatokietarako Project Operations erabiltzen dituzunean** funtzioan **Ezaugarrien kudeaketa** laneko arean.

2. Egokitu finantza-dimentsioak:

    - **Kontuko transakzioak (fakturazio mugarriak):** Joan **Proiektu guztiak** \> **Kudeatu** \> **Kontuko transakzioak**, eta hautatu doitzea eskatzen duen mugarria. Ondoren, **Finantza dimentsioak** fitxan, eguneratu balioak behar den moduan.
    - **Denbora, gastua eta transakzio materialak:** **Argitaratutako proiektuaren transakzioak** orrialdean, hautatu **Doitu kontabilitatea** finantza dimentsioak eguneratzeko.

3. Finantza dimentsioaren balioak egokitzen amaitu ondoren, joan hona: **Proiektuen kudeaketa eta kontabilitatea** \> **Aldizkakoa** \> **Proiektu Operazioen integrazioa**, eta hautatu **Inportatu taulako taulatik** aldian aldiko prozesua abiarazteko. Prozesu horrek eguneratutako finantza dimentsioaren balioak erabiltzen ditu proiektuaren faktura proposamenen lerroak berriro sortzeko. Eguneratutako balioak proiektuaren azpi-liburuan eta liburu nagusian erabiltzen dira proiektuaren faktura argitaratzen denean.
