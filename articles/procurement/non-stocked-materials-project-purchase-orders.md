---
title: Eskatu proiektu baten izakinik gabeko materialak proiektuko erosketa-eskaerak erabiliz
description: Gai honetan proiektu baten izakinik gabeko materialak proiektuko erosketa-eskaerak erabiliz nola eska dezakezun azaltzen da.
author: sigitac
ms.date: 09/27/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 6e0307ad6474feef96fc8080877eccbbbc7259db
ms.sourcegitcommit: 2d96345fb3afc3b174530285f95271b5ccbdea03
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/29/2021
ms.locfileid: "7563007"
---
# <a name="order-non-stocked-materials-for-a-project-using-project-purchase-orders"></a>Eskatu proiektu baten izakinik gabeko materialak proiektuko erosketa-eskaerak erabiliz

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Zure erakundeko Kontratazio Sailak erabil dezake [erosketa aginduak](/dynamics365/supply-chain/procurement/purchase-order-overview) ondasun eta zerbitzuen eskaeren jarraipena egiteko. Izakinik gabeko materialen erosketa-eskaerak proiektu bati eslei dakizkioke. Erosketa eskaera horiek fakturatzeak proiektuaren kostua erregistratzen du.

## <a name="prerequisites"></a>Aurrebaldintzak
Bete urrats hauek proiektuaren erosketa aginduen funtzionaltasuna gaitzeko.

1. Dynamics 365 Finance-n, joan **Eginbideen kudeaketa** lan-eremura.
2. Ezaugarrien zerrendan, bilatu eta hautatu funtzioa, **Gaitu proiektuaren erosketa-erosketak Project Operations-en baliabideetan oinarritutako/izakinik gabeko egoeretarako**.
3. Hautatu **Gaitu**.
4. Konfiguratu ez dauden materialak eta zain dauden saltzailearen fakturak atalean deskribatutako moduan [Konfiguratu ez dauden materialak eta zain dauden saltzailearen fakturak](configure-materials-nonstocked.md).

## <a name="create-a-project-purchase-order-from-the-project-purchase-order-list"></a>Sortu proiektuaren erosketa eskaera proiektuaren erosketa eskaeren zerrendatik

1. Finance-n, joan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuak** > **Proiektu guztiak** aukerara, eta hautatu proiektu bat.
2. Ekintza-panelean, **Kudeatu** fitxan, **Berria** taldean, hautatu **Elementuaren zeregina** > **Erosketa-eskaera**.
3. **Sortu eskaera** orrian, hautatu erosketa eskaera egin nahi duzun saltzailea, idatzi beste informazio egoki bat eta hautatu **Ados**.
4. **Erosketa-eskaera** orrialdean, **Erosketa-eskaeren lerroak** saretan, hautatu **Gehitu lerroa**.
5. Idatzi artikuluaren zenbakia, kantitatea, unitatea, unitateko prezioa eta dagokion informazioa.

    > [!NOTE]
    > Proiektuaren erosketa eskaerekin hornitu gabeko elementuak eta zerbitzuak soilik erabil daitezke. Hornitutako artikuluak eta kontratazio kategoriak ez dira onartzen.

6. Jarraitu elementuak behar bezala gehitzen eta erosketa eskaera berretsi.

    Ondasunen eta zerbitzuen ordainagiriak produktuaren ordainagiria sortuz eta argitaratuz erregistratu daitezke.

    > [!NOTE]
    > Produktuen ordainagiriak ez dira proiektuaren errealitatean erregistratzen Microsoft Dataverse-n eta ez eragin proiektuaren azpiegituran.

    Saltzaile batek erosketa eskaeran elementuen eta zerbitzuen faktura bidali ondoren, kontratazio sailak erosketa eskaeraren faktura sor dezake **Faktura** > **Sortu** > **Faktura** aukeran Ekintza-panelean. Saltzaileen fakturen zain dauden informazio gehiago lortzeko, ikusi [Erosi izakinik gabeko materialak saltzailearen zain dagoen faktura baten bidez](pending-vendor-invoices.md).
