---
title: Bidaiatzeko eskakizunak
description: Gai honek bidaia-eskakizunei buruzko informazioa ematen du.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 0261405abb9305d7f6abcde9cb90d9b184868580
ms.sourcegitcommit: a0f80d024a5d3112a39781815bd31d0c05ddaf6f
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/30/2020
ms.locfileid: "3906056"
---
# <a name="travel-requisitions"></a>Bidaiatzeko eskakizunak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Bidaia eskaera batean bidaia egiteko sortuko diren gastuak agertzen dira. Bidaia eskaera bat aurkezten da berrikusteko eta gastuak baimentzeko erabil daiteke.

Agian erakundeari kobratzen zaizkion gastuak egin aurretik bidaia eskaera aurkeztu beharko duzu. Betekizun hau aplikatzen da, kreditu-txartel korporatiboari gastuak kobratu, dirua aurreratzeagatik jasotako dirua gastatu edo erakundeak itzuliko dizun poltsikoko gastuak izan.

Bidaia eskaerak eta gidalerroak erabil daitezke erakundearen gastuak kudeatzen laguntzeko. Adibidez, zure erakundeak bidaia behar duen prezio finkoaren proiektuan lan egiten badu, proiektuko taldekideen bidaia gastuak proiektuaren aurrekontuaren barruan sartu behar dira. Bidaia gastuak onartu baino lehen onartuz gero, erakundeak proiektua aurrekontuaren barruan mantenduko dela ziurtatu dezake.

## <a name="configuration"></a>Konfigurazioa 

Bidaia-eskakizunak "derrigorrezko" gisa konfigura daitezke Gastuak kudeatzeko parametroetan "Bidaiaren aurretiazko baimena derrigorrezkoa" parametroa gaituz. 

## <a name="create-and-submit-a-travel-requisition"></a>Sortu eta bidali bidaia eskaera

1. Joan **Nire gastuak: Bidaia eskatzea**, eta hautatu **Bidaia eskakizun berria**.
2. Sartu eskaeraren xedea eta helmuga.
3. **Bidaiaren deskribapena** eremuan, sartu informazio osagarria. 
4. Aurreikusitako gastu bakoitzerako, hala nola Hegaldia, otorduak edo autoen alokairua, sortu gastuko lineako elementu bat. Sartu gastu bakoitzerako zenbatetsitako data, zenbatetsitako zenbatekoa eta moneta. 
5. Aurreikusitako gastuak gehitzen amaitutakoan, hautatu **Gorde**.
6. Bidaiaren eskaera aurkezteko prest zaudenean, hautatu **Lan-fluxua** > **Bidali**.

Onartutako bidaia eskaerak hemen ikus ditzakezu **Nire gastuak: bidaia-eskakizuna**. 

## <a name="view-available-travel-requisitions"></a>Ikusi eskuragarri dauden bidaia eskaerak

Bidaia-eskakizun guztiak ikus ditzakezu **Nire gastuak: bidaia-eskakizunak** aukeran.

## <a name="approve-travel-requisitions"></a>Onartu bidaiatzeko eskakizunak

Aukeratu onartu nahi duzun bidaia-eskaera, eta hautatu **Lan-fluxua** > **Onartu**.  

## <a name="submit-an-expense-report-using-your-approved-travel-requisition"></a>Bidali gastuen txostena onartutako bidaia eskaera erabiliz

1. Sortu gastu-txosten berria eta gastuen txostenaren goiburuan eta, onartutako bidaia-eskaeren zerrendan, hautatu **Esleitu bidaiatzeko eskatzeko**.
2. **Bidaia eskatzeko zenbatekoa** eremua automatikoki eguneratzen da gastuen txostenaren goiburuan.
3. Gehitu bidaiarako sortutako gastu bakoitza. **Aurrez baimenduta** eremua gaituta badago, bateratutako zenbatekoa eta baimendutako kopurua berariazko gastu-kategoriarako eguneratuko dira.

> [!NOTE]
> Gastu-txostena onartutako bidaia-eskaera batera lotzen duzunean, transakzioaren zenbatekoa ezin da baimendutakoa baino handiagoa izan. 
