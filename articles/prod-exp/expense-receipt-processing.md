---
title: Gastuen agiriak prozesatzea
description: Gai honetan ordainagirien karaktereen ezagutza optikoa (OCR) prozesatzeari buruzko informazioa ematen da. Ezaugarri hau erabiltzailearen esperientzia hobetzeko diseinatuta dago gastuen txostenak sortzen direnean Microsoft Dynamics 365 Finantza.
author: stsporen
ms.date: 05/14/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: johnmichalak
ms.search.region: Global
ms.author: stsporen
ms.search.validFrom: 2019-11-20
ms.dyn365.ops.version: 10.0.8
ms.openlocfilehash: 067432106742447d2b8fa215ec05bf05f4b41e70
ms.sourcegitcommit: 2c2a5a11d446adec2f21030ab77a053d7e2da28e
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/04/2022
ms.locfileid: "8684305"
---
# <a name="expense-receipt-processing"></a>Gastuen agiriak prozesatzea

Gastuen sarrera hobetu da ordainagirien karaktereen ezagutza optikoa (OCR) prozesuaren bidez. Eginbide hau sortutako gastuen txostenak sortzerakoan erabiltzailearen esperientzia hobetzeko diseinatuta dago.

## <a name="key-features"></a>Eginbide nagusiak

- Merkatariaren izena, data eta zenbateko osoa ateratzen dira ordainagirietatik.
- Eginbidea erantsitako ordainagiriak lotu gabeko gastuen transakzioekin parekatzen saiatzen da.
- Erabiltzaileek ordainagirietatik eskuz sartutako gastu transakzioak sor ditzakete.

## <a name="usage-examples"></a>Erabilera-adibideak

Gastu txostena sortzen denean kreditu txartelarekin egindako transakzioak jasotzen dituzten ordainagiriak automatikoki eransteko, egin hau:

  1. Ireki **Gastuen kudeaketa** lan eremua.
  2. Gainean **Ordainagiriak** fitxa, egiaztatu lotu gabeko ordainagiriak badirela. Ordainagiriak ere karga ditzakezu **Ordainagiriak** fitxa.
  3. **Gastuak** fitxan, egiaztatu lotu gabeko gastuak badirela. Normalean, gastuen administratzaileak gastu horiek kreditu txartelaren hornitzailearen eskutik inportatzen ditu.
  4. Aukeratu **Gastu txosten berria**. Kontuan izan gastuak eta ordainagiriak sar ditzakezula, orain ere, gastuen txostena sortzen duzunean. Gastuak eta ordainagiriak gehitzen badituzu, ordainagirien gastuen pareko automatikoki abiaraziko da.

Gastua sortzeko edo ordainagiriaren gastuarekin bat egiteko, egin hau:

  1. Gastu txosten batean, **Ordainagiriak** fitxa, erantsi ordainagiria hautatuz **Gehitu ordainagiriak**.
  2. Ordainagiriaren kargatutako irudiaren azpian, ohar ezazu **Sortu** eta **Partidua** aukerak.

      - Aukeratu **Sortu** eskuz sartutako gastuen transakzioa sortzeko eta ordainagiritik ateratako balioak betetzeko.
      - Hautatzen baduzu **Partidua**, sistema lehendik zegoen gastua ordainagiriarekin parekatzen saiatzen da.

## <a name="installation"></a>Instalazioa

Ezaugarri hau **Gastuen txostenak berriro imajinatu ziren** funtzioa gastuen esperientzia errazten laguntzeko. Ezaugarri hau Tier 2+ inguruneetarako bakarrik dago erabilgarri, Sandbox eta Production.

Gastu-gaitasun aurreratu hauek erabiltzeko, instalatu Expense Management Service gehigarria Microsoft Dynamics 365 Finantza, eta aktibatu eginbideak zure instantzian. Gehigarria zure proiektuan sar dezakezu Microsoft Dynamics Lifecycle Services (LCS).

1. Hasi saioa LCS-n eta ireki nahi duzun ingurunea.
2. Joan **Xehetasun guztiak**.
3. Aukeratu **Mantendu** edo joan behera **Ingurumeneko gehigarriak** FastTab.
4. Aukeratu **Instalatu gehigarri berria**.
5. Hautatu **Gastuen kudeaketa-zerbitzua**.
6. Jarraitu instalazio gida eta onartu baldintzak.
7. Hautatu **Instalatu**

Urtean **Ezaugarrien kudeaketa** laneko eremua, aktibatu ezaugarri hauek:

- Gastu-txostenen itxura berria
- Lotu automatikoki eta sortu gastua jasotzetik

Ezaugarri hauek aktibatzean ekintza hauek gertatzen dira:

- Daudenak **Gastuen kudeaketa** lan-eremua lan-eremu berriarekin ordezkatzen da.
- Gastu eremuen ikusgarritasunerako menu elementu berria gehitzen da.
- Lehenengoa ireki dezakezu **Gastuen txostenak** orrialdera joanda **Gastuen kudeaketa> Nire gastuak> Gastuen txostenak**.
- Lan-fluxuek eta edozein onarpenek lehendik dauden gastuen txostenen orrialdera eramaten zaituzte.
- Ordainagiriak bidez prozesatuko dira Microsoft Azure Cognitive Services-k eta metadatuak erauzi eta gehituko dira.
- Erantsitako loturarik gabeko ordainagiriak biltzen dituen gastu-txostena sortzeko aukera ematen duen aukera gehitzen da.
- Gastu txostenetan gehitzen den aukera batek ordainagiri batetik gastu lerro bat sortzeko aukera ematen du edo lehendik dagoen ordainagiria lehendik dagoen gastu lerro batekin parekatzen saiatzen da.

Gastuen txostenak berriro imajinatutako eginbideari buruzko informazio gehiago lortzeko, ikusi [Gastuen txostenak berriro pentsatu ziren](ExpenseWorkspaceNew.md).

## <a name="frequently-asked-questions"></a>Ohiko galderak

**Microsoft-ek nire datuak erabiltzen ditu bere modeloetarako?**

Ez, Microsoft-ek Ikaskuntza automatiko eredu orokorra eraiki du ordainagiriak prozesatzeko zerbitzurako. Eredu hau ez dago kargatutako ordainagirietan oinarrituta.

**Non dago erabilgarri eta prozesatu eginbide hau?**

Gaur egun, Estatu Batuak onartzen dira.

**Nora doaz nire ordainagiriak?**

Finance-k Cognitive Service harremanetan jarriko da eremuko datuak ateratzeko. Cognitive Service-k zure ordainagiriaren kopia mantenduko dute 24 orduz gehienez prozesamendua gertatu bitartean. Prozesamendua amaitu ondoren, Cognitive Services-ek ordainagiria kenduko du. Ordainagiriak Finantzan gordetzen dira oraindik.

Informazio gehiagorako, ikus [Gaitu ordainagiriak ulertzeko inprimakia hautagaiaren gaitasun berriarekin](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).


[!INCLUDE[footer-include](../includes/footer-banner.md)]