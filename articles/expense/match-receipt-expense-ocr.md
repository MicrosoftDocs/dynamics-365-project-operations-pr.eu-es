---
title: Kapturatu ordainagiriak OCR erabiliz
description: Gai honetan ordainagirien karaktereen ezagutza optikoa (OCR) prozesatzeari buruzko informazioa ematen da.
author: suvaidya
ms.date: 11/10/2021
ms.topic: article
ms.prod: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 4dc1628a0dde0551aaf3bc10af628ef57881d85e
ms.sourcegitcommit: a51f40c905874103040708be2188c04ab0716c38
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/11/2021
ms.locfileid: "7798025"
---
# <a name="capture-a-receipt-using-ocr"></a>Kapturatu ordainagiriak OCR erabiliz

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Gastuen sarrera hobetu da ordainagirien karaktereen ezagutza optikoa (OCR) prozesuaren bidez. Funtzionalitate hau gastuen txostenak sortzerakoan erabiltzailearen esperientzia hobetzeko diseinatuta dago.

## <a name="key-features"></a>Eginbide nagusiak

- Sistemak merkatariaren izena, data eta zenbateko osoa ateratzen ditu ordainagirietatik.
- Sistema erantsitako ordainagiriak lotu gabeko gastuen transakzioekin parekatzen saiatuko da.
- Ordainagirietatik eskuz sartutako gastu transakzioak sor ditzakezu.

## <a name="attach-receipts-to-an-expense-report"></a>Erantsi ordainagiriak gastuen txostenean

Gastu txostena sortzen denean kreditu txartelarekin egindako transakzioak jasotzen dituzten ordainagiriak automatikoki eransteko, jarraitu urrats hauek.

  1. Ireki **Gastuen kudeaketa** lan eremua.
  2. Gainean **Ordainagiriak** fitxa, egiaztatu lotu gabeko ordainagiriak badirela. Ordainagiriak ere karga ditzakezu **Ordainagiriak** fitxa.
  3. **Gastuak** fitxan, egiaztatu lotu gabeko gastuak badirela. Normalean, gastuen administratzaileak gastu horiek kreditu txartelaren hornitzailearen eskutik inportatzen ditu.
  4. Aukeratu **Gastu txosten berria**. Kontuan izan gastuak eta ordainagiriak sar ditzakezula, orain ere, gastuen txostena sortzen duzunean. Gastuak eta ordainagiriak gehitzen badituzu, ordainagirien gastuen pareko automatikoki abiaraziko da.

## <a name="create-or-match-receipts-to-an-expense-report"></a>Sortu edo bat etorri ordainagiriak gastuen txostenean
Gastua sortzeko edo ordainagiriaren gastuarekin bat egiteko, jarraitu urrats hauek.

  1. Gastu txosten batean, **Ordainagiriak** fitxa, erantsi ordainagiria hautatuz **Gehitu ordainagiriak**.
  2. Ordainagiriaren kargatutako irudiaren azpian, ohar ezazu **Sortu** eta **Partidua** aukerak.

      - Aukeratu **Sortu** eskuz sartutako gastuen transakzioa sortzeko eta ordainagiritik ateratako balioak betetzeko.
      - Hautatzen baduzu **Partidua**, sistema lehendik zegoen gastua ordainagiriarekin parekatzen saiatzen da.

## <a name="installation"></a>Instalazioa

Gastu-gaitasun aurreratu hauek erabiltzeko, instalatu Microsoft-en Dynamics 365 Finance Expense Management Service gehigarria eta aktibatu eginbideak zure instantzian. Gehigarria zure proiektutik atzi dezakezu Microsoft Dynamics Lifecycle Services (LCS) atalean.

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
- Ordainagiriak Microsoft Azure Zerbitzu kognitiboen bidez prozesatuko dira, eta metadatuak atera eta gehituko dira.
- Erantsitako loturarik gabeko ordainagiriak biltzen dituen gastu-txostena sortzeko aukera ematen duen aukera gehitzen da.
- Gastu txostenetan gehitzen den aukera batek ordainagiri batetik gastu lerro bat sortzeko aukera ematen du edo lehendik dagoen ordainagiria lehendik dagoen gastu lerro batekin parekatzen saiatzen da.

## <a name="frequently-asked-questions"></a>Ohiko galderak

**Microsoft-ek nire datuak erabiltzen ditu bere modeloetarako?**

Ez, Microsoft-ek Ikaskuntza automatiko eredu orokorra eraiki du ordainagiriak prozesatzeko zerbitzurako. Eredu hau ez dago kargatutako ordainagirietan oinarrituta.

**Non dago erabilgarri eta prozesatu eginbide hau?**

Eginbide honen erabilgarritasuna eskualde ezberdinetan hurrengo taulan ageri da. Zure eskualdea ez bada onartzen, bidali eskaera zure eskualdeko OCR zerbitzuaren erabilgarritasunari lehentasuna emateko. 

| Eskualdea | Onartzen da                         |
|--------|-----------------------------------|
| AEB    | Yes                               |
| CAN    | Yes                               |
| Erresuma Batua     | Yes                               |
| AUS    | Yes                               |
| EB     | Partzialki. Ingelesezko ordainagiriak soilik. |
| Asia   | No                                |
| Japonia  | No                                |
| Afrika | No                                |

**Nora doaz nire ordainagiriak?**

Finance-k Cognitive Service harremanetan jarriko da eremuko datuak ateratzeko. Cognitive Service-k zure ordainagiriaren kopia mantenduko dute 24 orduz gehienez prozesamendua gertatu bitartean. Prozesamendua amaitu ondoren, Cognitive Services-ek ordainagiria kenduko du. Ordainagiriak Finantzan gordetzen dira oraindik.

Informazio gehiagorako, ikus [Gaitu ordainagiriak ulertzeko inprimakia hautagaiaren gaitasun berriarekin](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).


[!INCLUDE[footer-include](../includes/footer-banner.md)]
