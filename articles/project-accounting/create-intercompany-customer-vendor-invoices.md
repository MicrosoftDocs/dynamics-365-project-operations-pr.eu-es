---
title: Sortu enpresen arteko bezeroa eta saltzaileen fakturak
description: Gai honek enpresen arteko bezeroen eta saltzaileen fakturak nola sortu jakiteko informazioa eskaintzen du.
author: sigitac
manager: tfehr
ms.date: 11/19/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: f1560469d2bdbb8e81dc26c16b272c44446ab20a
ms.sourcegitcommit: addbe0647619413e85e7cde80f6a21db95ab623e
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/20/2020
ms.locfileid: "4595416"
---
# <a name="create-intercompany-customer-and-vendor-invoices"></a>Sortu enpresen arteko bezeroa eta saltzaileen fakturak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Mailegu-entitate juridiko bateko proiektu-kontulariak enpresa arteko bezeroaren faktura sortzen du mailegu-entitateari transferitzen ari zaizkion proiektuaren kostuengatik. Enpresen arteko bezeroen faktura onartu eta argitaratu ondoren, mailegu-entitate juridikoak enpresen arteko faktura mailegu-entitate juridikoari bidaltzen dio.

Mailegu-entitate juridikoko proiektuaren kontulariak bat-bateko prozesua ezar dezake konpainien arteko fakturak behin eta berriro sortzeko. Proiektuaren kontulariak irizpideak zehazten ditu, hala nola proiektu zehatzak, enpresen arteko fakturak sorta batean sortzeko.

## <a name="manually-create-an-intercompany-customer-invoice-for-project-transactions"></a>Eskuz sortu enpresen arteko bezeroaren faktura proiektuaren transakzioetarako 

Erabili prozedura hori enpresen arteko bezeroaren faktura proiektuaren transakzioetarako eskuz sortzeko. Bilatu langileek mailegu-entitate juridikoetako proiektuetan langileek argitaratutako orduak eta zure entitate juridikoak mailegu-entitate juridikoen izenean egindako gastuak. Pertsona juridikoaren izenaren, proiektuaren kontratuaren zenbakiaren, proiektuaren zenbakiaren, data tartearen edo aukera horien edozein konbinazioen arabera bila dezakezu. Bilaketaren emaitzetan, hautatu enpresen arteko faktura batean gehitzeko eragiketak.

1. Dynamics 365 Finance-n , joan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuaren fakturak** > **Enpresen arteko bezeroen fakturak** aukerara. **Enpresen arteko bezeroen fakturak** zerrenda-orrialdean, Ekintza panelean, hautatu **Berria**.
2. **Enpresen arteko faktura sortu** orrialdean, **Pertsona juridikoa** eremuan, hautatu mailegu-entitate juridikoa.
3. Aukerakoa: Idatzi proiektuaren kontratu zehatza eta proiektuaren zenbakia.
4. Bilaketa mugatu data tartea hautatuta. Idatzi data zehatzak **Hasiera data** eta **Amaiera data** eremuetan. Data tarte horretan argitaratzen diren enpresen arteko transakzioak soilik bistaratzen dira bilaketaren emaitzetan.
5. Ezarri **Proiektua aldizkariaren lerro parametro aurreratua** **Bai** gisa, eta hautatu **Bilatu**.
6. Bilaketaren emaitzetan, hautatu enpresen arteko faktura proposamenean sartu beharreko transakzioak, eta hautatu **Ados**.
7. **Enpresen arteko bezeroaren faktura** orrian, bilaketa-emaitzetan hautatu dituzun enpresen arteko proiektuen transakzioak bistaratzen dira. Eragiketak aldatzeko maileguan dagoen pertsona juridikoari faktura bidali aurretik, egin hau:
  
    1. Ireki **Sortu faktura proposamena** orrialdea. Aukeratu konpainien arteko transakzio osagarriak uneko fakturarako eta, ondoren, hautatu **Gehitu lerroa**.
    2. Lerro bat kentzeko, hautatu **Kendu**.
    3. Ikusi iruzkinak, arrazoiak, dimentsio ekonomikoak eta hautatutako linea bati buruzko beste informazioa **Faktura lerroak** FastTab.
    
8. Enpresen arteko bezeroen faktura argitaratzeko, Ekintza panelean, hautatu **Argitaratu**.

> [!NOTE]
> Zure erakundeak enpresen arteko fakturak berrikusi behar direla argitaratu aurretik, sistemako administratzaile batek enpresen arteko fakturetarako lan-fluxua ezar dezake. Enpresen arteko fakturetarako lan-fluxua konfiguratuta ez badago, enpresen arteko faktura jar dezakezu.

## <a name="create-a-batch-job-for-intercompany-invoices"></a>Sortu enpresen arteko fakturetarako sorta bat

Enpresa arteko faktura anitz sor ditzakezu aldi berean maileguan dauden pertsona juridiko guztientzat. Bilaketa funtzionalitatea erabiliz, adibidez, mailegatutako langileek argitaratutako eta beste pertsona juridiko batzuek kudeatzen dituzten proiektuekin erlazionatutako transakzio guztiak bila ditzakezu. Ondoren, maileguan dagoen pertsona juridiko bakoitzarentzat, enpresen arteko faktura bat sor dezakezu bilaketaren emaitzetan emandako eragiketetarako.

1. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkakoa** > **Proiektuaren fakturak** > **Sortu enpresen arteko bezeroen fakturak** aukerara.
2. **Enpresen arteko bezeroen fakturak** orrialdean, **Enpresa** eremuan, hautatu fakturaren legezko entitatea fakturatzeko. Enpresarik aukeratzen ez baduzu, bilaketa-irizpideak betetzen dituzten transakzio guztiak bistaratuko dira maileguan dauden pertsona juridiko guztientzat.
3. **Sortu faktura bakoitzeko**, aukeratu enpresen arteko transakzioen faktura proiektu batean oinarrituta edo mailegu-erakunde juridiko batean oinarrituta sortuko den.
4. Aukerakoa: enpresen arteko fakturak sortzeko proiektu zehatz bat eta proiektuen kontratua hautatzeko, egin klik **Aukeratu** aukeran. **Kontsulta** orrialdean, **Irizpideak** eremuan, hautatu proiektuaren kontratua, proiektuaren zenbakia edo biak, eta hautatu **Ados**.
5. **Sorta** fitxan, konfiguratu sorta prozesua konpainien arteko fakturak behin eta berriro sortzeko. Informazio gehiagorako, ikusi [Bidali batch prozesatzeko lana inprimaki batetik](https://docs.microsoft.com/dynamicsax-2012/appuser-itpro/submit-a-batch-processing-job-from-a-form).
6. Enpresen arteko fakturak argitaratzeko, Ekintza panelean, hautatu **Argitaratu**.

> [!NOTE]
> Zure erakundeak enpresen arteko fakturak berrikusi behar direla argitaratu aurretik, sistemako administratzaile batek enpresen arteko fakturetarako lan-fluxua ezar dezake. Enpresen arteko fakturetarako lan-fluxua konfiguratuta ez badago, enpresen arteko fakturak jar ditzakezu.

## <a name="post-the-intercompany-vendor-invoice"></a>Bidali enpresen arteko saltzailearen faktura

Mailegu-hartzailea den legezko proiektuko kontulariak enpresa arteko saltzaileen fakturak berrikusi ditzake, enpresa arteko bezeroaren faktura argitaratzen denean. Finantzetan, maileguan dagoen pertsona juridikoan, joan **Ordaintzeko kontuak** > **Fakturak** > **Saltzailearen faktura zain** aukerara. Zain dagoen faktura zenbakia enpresen arteko bezeroaren faktura zenbakiarekin bat etorriko da. Egiaztatu faktura zuzena dela eta bidali faktura. Enpresen arteko saltzailearen faktura argitaratzeak proiektuaren azpiegitura bat eta liburu orokorreko transakzio bat sortzen ditu mailegu-entitate juridikoan transakzio kostuak islatzen dituena.


[!INCLUDE[footer-include](../includes/footer-banner.md)]