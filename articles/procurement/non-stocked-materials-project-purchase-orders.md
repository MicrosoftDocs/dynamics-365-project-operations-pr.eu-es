---
title: Eskatu proiektu baten izakinik gabeko materialak proiektuko erosketa-eskaerak erabiliz
description: Gai honetan proiektu baten izakinik gabeko materialak proiektuko erosketa-eskaerak erabiliz nola eska dezakezun azaltzen da.
author: sigitac
ms.date: 09/27/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 2aa8fb94e2f9cbf91182f3f169339284d3eb9f44
ms.sourcegitcommit: 9916f536a71b6a0078297402564ac79308ec6890
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/18/2022
ms.locfileid: "8612688"
---
# <a name="order-procurement-categories-or-non-stocked-materials-for-a-project-using-project-purchase-orders"></a>Eskatu erosketa-kategoriak edo hornituta ez dauden materialak proiektu baterako proiektuko erosketa-aginduak erabiliz

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Zure erakundeko Kontratazio Sailak erabil dezake [erosketa aginduak](/dynamics365/supply-chain/procurement/purchase-order-overview) ondasun eta zerbitzuen eskaeren jarraipena egiteko. Erosketa-kategorien edo stockak ez diren materialen erosketa-eskaerak proiektu bati egotzi ahal zaizkio. Erosketa eskaera horiek fakturatzeak proiektuaren kostua erregistratzen du.

## <a name="prerequisites"></a>Aurrebaldintzak
Bete urrats hauek proiektuaren erosketa aginduen funtzionaltasuna gaitzeko.

1. Dynamics 365 Finance atalean, joan **Ezaugarrien kudeaketa** lan-eremua.
2. Ezaugarrien zerrendan, bilatu eta hautatu funtzioa, **Gaitu proiektuaren erosketa-erosketak Project Operations-en baliabideetan oinarritutako/izakinik gabeko egoeretarako**.
3. Hautatu **Gaitu**.
4. Konfiguratu ez dauden materialak eta zain dauden saltzailearen fakturak atalean deskribatutako moduan [Konfiguratu ez dauden materialak eta zain dauden saltzailearen fakturak](configure-materials-nonstocked.md).
5. Konfiguratu kontratazio-kategoriak atalean deskribatzen den moduan [Erabili erosketa-kategoriak proiektuko erosketa-aginduekin eta zain dauden saltzaileen fakturekin](configure-procurement-categories.md).

## <a name="create-a-project-purchase-order-from-the-project-purchase-order-list"></a>Sortu proiektuaren erosketa eskaera proiektuaren erosketa eskaeren zerrendatik

1. Finance-n, joan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuak** > **Proiektu guztiak** aukerara, eta hautatu proiektu bat.
2. Ekintza-panelean, **Kudeatu** fitxan, **Berria** taldean, hautatu **Elementuaren zeregina** > **Erosketa-eskaera**.
3. **Sortu eskaera** orrian, hautatu erosketa eskaera egin nahi duzun saltzailea, idatzi beste informazio egoki bat eta hautatu **Ados**.
4. **Erosketa-eskaera** orrialdean, **Erosketa-eskaeren lerroak** saretan, hautatu **Gehitu lerroa**.
5. Idatzi elementu-zenbaki bat edo kontratazio-kategoria, kantitatea, unitatea, unitate-prezioa eta dagokion beste informazio bat.

    > [!NOTE]
    > Kontratazio-kategoriak, hornituta ez dauden elementuak eta zerbitzuak soilik erabil daitezke proiektuko erosketa-eskaerekin. Ez dira onartzen gordetako elementuak.

6. Jarraitu elementuak edo kontratazio-kategoriak gehitzen behar bezala, eta berretsi erosketa-eskaera.

    Ondasunen eta zerbitzuen ordainagiriak produktuaren ordainagiria sortuz eta argitaratuz erregistratu daitezke.

    > [!NOTE]
    > Produktuen ordainagiriak ez dira proiektuaren errealitatean erregistratzen Microsoft Dataverse-n eta ez eragin proiektuaren azpiegituran.

    Saltzaile batek erosketa eskaeran elementuen eta zerbitzuen faktura bidali ondoren, kontratazio sailak erosketa eskaeraren faktura sor dezake **Faktura** > **Sortu** > **Faktura** aukeran Ekintza-panelean. Saltzaileen fakturen zain dauden informazio gehiago lortzeko, ikusi [Erosi izakinik gabeko materialak saltzailearen zain dagoen faktura baten bidez](pending-vendor-invoices.md).
