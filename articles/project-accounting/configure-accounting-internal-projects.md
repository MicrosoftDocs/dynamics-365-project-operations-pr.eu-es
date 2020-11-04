---
title: Konfiguratu barne-proiektuen kontabilitatea
description: Gai honek Project Operations-en barne-proiektuetarako kontabilitate-praktikak ezartzeko moduari buruzko informazioa eskaintzen du.
author: sigitac
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 504e7481cb2aee6310cb4ace2d0791d1c7fe360d
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070970"
---
# <a name="configure-accounting-for-internal-projects"></a>Konfiguratu barne-proiektuen kontabilitatea

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Barne-proiektuek enpresei bezero bati fakturatzen ez zaizkion jarduerei lotutako kostuak jarraitzea ahalbidetzen dute. Barne-proiektuen adibideak hauek dira:

- Produktu bat garatzea, hala nola mugikorretarako aplikazio bat, eta garapenarekin lotutako kostuen jarraipena egitea.
- Salmentaren aurreko denbora eta gastuak kudeatzea. Salmentaren aurreko barne proiektu hau fakturatzeko proiektu bihur daiteke gero, aurrekontua irabaziz gero.

Dynamics 365 Project Operations-en kontratuarekin loturarik ez dagoen edozein proiektu barne gisa hartzen da. Proiektuaren kostua eta diru-sarreren profilak ez dira erabiltzen proiektuaren kontabilitate-arauak zehazteko. Barne-proiektuaren kostua irabazien eta galeren printzipioak erabiliz argitaratzen da beti. Argitaratzeko liburu nagusiko kontuak **Liburu nagusian argitaratzeko konfigurazioa** orrialdean definitzen dira.

- Denborazko transakzioak **Kostua** kontua zordunduta eta **Nominen esleipena** kontuan zordunduta argitaratzen dira.
- Gastuen transakzioak **Kostua** kontua zordunduta eta **Gastuetarako lehenetsitako kontua** zordunduta argitaratzen dira.

Transakzioak proiektuan argitaratu ondoren, proiektua proiektuko kontratu batekin lotzen bada, sistemak metatutako transakzio guztiak alderantzikatzen ditu eta fakturagarriak diren transakzio berriak sortzen ditu. Fakturagarriak diren eragiketek Proiektuaren kostu eta diru-sarreren profilean zehaztutako kontabilitate arauak jarraitzen dituzte.


