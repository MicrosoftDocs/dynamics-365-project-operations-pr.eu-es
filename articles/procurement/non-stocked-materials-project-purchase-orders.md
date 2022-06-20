---
title: Eskatu proiektu baten izakinik gabeko materialak proiektuko erosketa-eskaerak erabiliz
description: Artikulu honek proiektu baterako erosketa-eskaerak erabiliz hornituta ez dauden materialak nola eska ditzakezun azaltzen du.
author: sigitac
ms.date: 09/27/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: fe24faa143869af2396f3b0f28aae31417cadda7
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8929797"
---
# <a name="order-procurement-categories-or-non-stocked-materials-for-a-project-using-project-purchase-orders"></a>Eskatu erosketa-kategoriak edo hornituta ez dauden materialak proiektu baterako proiektuko erosketa-aginduak erabiliz

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Zure erakundeko Kontratazio Sailak erabil dezake [erosketa aginduak](/dynamics365/supply-chain/procurement/purchase-order-overview) ondasun eta zerbitzuen eskaeren jarraipena egiteko. Erosketa-kategorien edo stockak ez diren materialen erosketa-eskaerak proiektu bati egotzi ahal zaizkio. Erosketa eskaera horiek fakturatzeak proiektuaren kostua erregistratzen du.

## <a name="prerequisites"></a>Aurrebaldintzak
Bete urrats hauek proiektuaren erosketa aginduen funtzionaltasuna gaitzeko.

1. Dynamics 365 Finance atalean, joan hona **Ezaugarrien kudeaketa** lan-eremua.
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
