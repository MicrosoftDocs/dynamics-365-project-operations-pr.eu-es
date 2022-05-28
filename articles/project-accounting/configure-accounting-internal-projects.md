---
title: Konfiguratu barne-proiektuen kontabilitatea
description: Gai honek Project Operations-en barne-proiektuetarako kontabilitate-praktikak ezartzeko moduari buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 10/09/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 9da72d8dbf720e380a49a1010caca472ee024783
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8597829"
---
# <a name="configure-accounting-for-internal-projects"></a>Konfiguratu barne-proiektuen kontabilitatea

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Barne-proiektuek enpresei bezero bati fakturatzen ez zaizkion jarduerei lotutako kostuak jarraitzea ahalbidetzen dute. Barne-proiektuen adibideak hauek dira:

- Produktu bat garatzea, hala nola mugikorretarako aplikazio bat, eta garapenarekin lotutako kostuen jarraipena egitea.
- Salmentaren aurreko denbora eta gastuak kudeatzea. Salmentaren aurreko barne proiektu hau fakturatzeko proiektu bihur daiteke gero, aurrekontua irabaziz gero.

Urtean kontratuarekin loturarik ez duen edozein proiektu Dynamics 365 Project Operations barne gisa tratatzen da. Proiektuaren kostua eta diru-sarreren profilak ez dira erabiltzen proiektuaren kontabilitate-arauak zehazteko. Barne-proiektuaren kostua irabazien eta galeren printzipioak erabiliz argitaratzen da beti. Argitaratzeko liburu nagusiko kontuak **Liburu nagusian argitaratzeko konfigurazioa** orrialdean definitzen dira.

- Denborazko transakzioak **Kostua** kontua zordunduta eta **Nominen esleipena** kontuan zordunduta argitaratzen dira.
- Gastuen transakzioak **Kostua** kontua zordunduta eta **Gastuetarako lehenetsitako kontua** zordunduta argitaratzen dira.
- Artikuluen transakzioak zordunketa bidez argitaratzen dira **Kostua** kontua eta kreditua **Kostua - Elementua** kontua.

Transakzioak proiektuan argitaratu ondoren, proiektua proiektuko kontratu batekin lotzen bada, sistemak metatutako transakzio guztiak alderantzikatzen ditu eta fakturagarriak diren transakzio berriak sortzen ditu. Fakturagarriak diren eragiketek Proiektuaren kostu eta diru-sarreren profilean zehaztutako kontabilitate arauak jarraitzen dituzte.




[!INCLUDE[footer-include](../includes/footer-banner.md)]
