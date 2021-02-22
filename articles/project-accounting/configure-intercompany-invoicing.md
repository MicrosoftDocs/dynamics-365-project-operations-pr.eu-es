---
title: Konfiguratu enpresen arteko fakturazioa
description: Gai honek enpresen arteko fakturazioa proiektuen inguruko informazioa eta adibideak eskaintzen ditu.
author: sigitac
manager: tfehr
ms.date: 11/20/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: bdb6122d8aba84d2b449f9f17a4093388b585614
ms.sourcegitcommit: addbe0647619413e85e7cde80f6a21db95ab623e
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/20/2020
ms.locfileid: "4595418"
---
# <a name="configure-intercompany-invoicing"></a>Konfiguratu enpresen arteko fakturazioa

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Bete urrats hauek enpresen arteko fakturazioa proiektuan konfiguratzeko Dynamics 365 Project Operations. Enpresen arteko transakzioak proiektu bateko kontratu bateko denbora eta gastu transakzioak dira, enpresa edo antolakuntza unitate batekoak diren bitartean, proiektuaren kontratuko baliabideak enpresa edo antolakuntza unitate desberdinetakoak diren bitartean.

## <a name="example-configure-intercompany-invoicing"></a>Adibidez: Konfiguratu enpresen arteko fakturazioa

Hurrengo adibidean, Contoso Robotics USA (USPM) da mailegu-entitatea eta Contoso Robotics UK (GBPM) mailegu-entitatea da. 

1. **Konfiguratu enpresen arteko kontabilitatea pertsona juridikoen artean**. Mailegu- eta mailegu-entitate juridiko bikote bakoitza liburu nagusian konfiguratu behar da [Enpresen arteko kontabilitatea](https://docs.microsoft.com/dynamics365/finance/general-ledger/intercompany-accounting-setup) orrialdea.
    
    1. Dynamics 365 Finance-n, joan **Liburu nagusia** > **Mezuaren konfigurazioa** > **Enpresen arteko kontabilitatea** aukerara. Sortu erregistroa informazio honekin:

        - **Jatorrizko enpresa** = **GBPM**
        - **Helmuga-enpresa** = **USPM**

2. **Pertsona juridikoen arteko merkataritza-harremana konfiguratzea**. Mailegu-entitate juridikoa ordezkatzen duen bezeroaren erregistroa mailegu-entitate juridikoan sortu behar da. Mailegu-entitate juridikoa ordezkatzen duen saltzailearen erregistroa mailegu-entitate juridikoan sortu behar da.

     1. Finantzetan, hautatu pertsona juridikoa **GBPM**.
     2. Joan **Kobratu beharreko kontuak** > **Bezeroa** > **Bezero guztiak**. Sortu erregistro berria pertsona juridikoarentzat, **USPM**.
     3. Zabaldu **Izena**, iragazi erregistroak **Mota** aukeraren arabera, eta hautatu **Pertsona juridikoak**. 
     4. Bilatu eta hautatu bezeroarentzako erregistroa **Contoso Robotics AEB (USPM)**.
     5. Aukeratu **Erabili partida**. 
     6. Aukeratu bezero taldea eta gorde erregistroa.
     7. Hautatu **USPM** legezko entitatea.
     8. Joan **Ordaintzeko kontuak** > **Saltzaileak** > **Saltzaile guztiak**. Sortu erregistro berria pertsona juridikoarentzat, **GBPM**.
     9. Zabaldu **Izena**, iragazi erregistroak **Mota** aukeraren arabera, eta hautatu **Pertsona juridikoak**. 
     10. Bilatu eta hautatu bezeroarentzako erregistroa **Contoso Robotics UK (GBPM)**.
     11. Aukeratu **Erabili partida**, hautatu saltzaile taldea, eta gorde erregistroa.
     12. Saltzailearen erregistroan, hautatu **Orokorra** > **Konfiguratu** > **Enpresa artekoa**.
     13. **Negoziazio-harremana** fitxan, ezarri **Aktiboa** **Bai** gisa.
     14. Aukeratu enpresa saltzailea **GBPM** eta urtean **Nire kontuaren erregistroa**, hautatu prozeduran lehenago sortu zenuen bezeroaren erregistroa.

3. **Konfiguratu enpresen arteko ezarpenak Proiektuen kudeaketa eta kontabilitate parametroetan**. 

    1. Aukeratu pertsona juridikoa **USPM** eta joan **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Proiektuen kudeaketa eta kontabilitate parametroak**.
    2. **Enpresa artekoa** fitxan, hautatu kontratazio kategoria automatikoki sortzen diren saltzailearen fakturekin bat etortzeko.
    3. **Kategoria lehenetsia** aukeran, hautatu **Enpresen arteko baliabideak**.
    4. Aukeratu pertsona juridikoa **GBPM** eta joan **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Proiektuen kudeaketa eta kontabilitate parametroak**.
    5. **Enpresa artekoa** fitxan, hautatu lehenetsitako proiektuen kategoria transakzio mota bakoitzerako. Proiektuen kategoriak zerga konfiguraziorako erabiltzen dira, enpresa arteko eragiketetan fakturatutako kategoria mailegu-entitate juridikoan bakarrik dagoenean. Enpresen arteko transakzioengatik diru-sarrerak eskuratzea aukera dezakezu. Biderketa eragiketak mailegu-entitate juridikoan Project Operations Integration aldizkariaren bidez argitaratzen direnean gertatzen da. Aldizkaria alderantzikatu egiten da enpresen arteko faktura argitaratzen denean.
    6. **Baliabideak mailegu ematean** taldean, hautatu **...** > **Berria**. 
    7. Saretan, idatzi edo hautatu informazio hau:

          - **Pertsona juridikoa maileguan hartzea** = **GBPM**
          - **Diru sarrerak lortu** = **Bai**
          - **Denbora-orriaren kategoria lehenetsia** = **Lehenetsia - Ordua**
          - **Gastu kategoria lehenetsia** = **Lehenetsia - gastua**

4. **Ezarri enpresen arteko kostuen eta diru-sarreren kontuak Ledger argitaratzeko konfigurazioan**. Enpresen arteko diru-sarreren kontua enpresen arteko bezeroen faktura mailegu-entitate juridikoan argitaratzen denean kreditatzen da. Enpresen arteko kostuen kontua enpresen arteko bezeroen faktura mailegu-entitate juridikoan argitaratzen denean zorduntzen da. Kontu horiek dagozkien pertsona juridikoetan daude konfiguratuta. 
      
     1. Finantzetan, hautatu dirua mailegatu zaion pertsona juridikoa **USPM**. 
     2. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Bidalketa** > **Liburu nagusia argitaratzeko konfigurazioa**. 
     3. **Kostuen kontuak** fitxan, **Liburu kontuen mota** aukeran, hautatu **Enpresen arteko kostua**. Sortu erregistro berria informazio honekin:
      
        - **Pertsona juridikoa maileguan ematea** = **GBPM**
        - **Kontu nagusia** = Aukeratu enpresa nagusia kostuaren truke
        
     4. Hautatu dirua emandako **GBPM** legezko entitatea. 
     5. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Bidalketa** > **Liburu nagusia argitaratzeko konfigurazioa**. 
     6. **Diru-sarreren kontuak** fitxan, **Liburu kontuen mota** aukeran, hautatu **Enpresen arteko diru-sarrera**. Sortu erregistro berria informazio honekin:

        - **Pertsona juridikoa maileguan hartzea** = **USPM**
        - **Kontu nagusia** = Aukeratu enpresa nagusia diru-sarreraren truke 

5. **Ezarri eskulanaren transferentzia prezioak**. Enpresen arteko transferentziaren prezioak Project Operations-en konfiguratuta daude Dataverse. Konfiguratu [eskulanaren kostuen tasak](../pricing-costing/set-up-labor-cost-rate.md#transfer-pricing-and-costs-for-resources-outside-of-your-division-or-legal-entity) eta [lan fakturaren tasak](../pricing-costing/set-up-labor-bill-rate.md#transfer-pricing-or-set-up-bill-rates-for-resources-from-other-organizational-units-or-divisions) enpresen arteko fakturaziorako. Transferentzia prezioak ez dira onartzen enpresen arteko gastuen transakzioetarako. Erakundeen arteko unitatearen salmenta-prezioa beti izango da baliabideen unitateko kostuaren prezioaren balio bera.

      Contoso Robotics UK garatzailearen baliabideen kostua 88 GBP da orduko. Contoso Robotics UK-k Contoso Robotics USA fakturatuko du 120 USD baliabide honek AEBetako proiektuetan lan egin duen ordu bakoitzeko. Contoso Robotics USA-k bezeroari Adventure Works 200 USD fakturatuko dio Contoso Robotics UK garatzaile baliabideak egindako lana.

      1. Project Operations-eko Dataverse atalean, joan **Salmenta** > **Prezio zerrendak**. Sortu kostuen prezioen zerrenda berria **Contoso Robotics UK kostu tasak**. 
      2. Kostuen prezioen zerrendan, sortu erregistro bat informazio honekin:
         - **Rola** = **Garatzailea**
         - **Kostua** = **88 GBP**
      3. Joan **Ezarpenak** > **Antolakuntza unitateak** eta erantsi kostuen prezio zerrenda hau **Contoso Robotics UK** antolakuntza unitatea.
      4. Joan **Salmentak** > **Prezio zerrendak** aukerara. Sortu kostuen prezioen zerrenda **Contoso Robotics USA kostu tasak**. 
      5. Kostuen prezioen zerrendan, sortu erregistro bat informazio honekin:
          - **Rola** = **Garatzailea**
          - **Baliabideen enpresa** = **Contoso Robotics UK**
          - **Kostua** = **120 USD**
      6. Joan **Ezarpenak** > **Antolakuntza unitateak** eta erantsi **Contoso Robotics USA kostu-tarifak** kostuen prezio zerrenda **Contoso Robotics USA** antolakuntza unitatea.
      7. Joan **Salmentak** > **Prezio zerrendak** aukerara. Sortu izeneko salmenta prezioen zerrenda **Adventure Works fakturen tasak**. 
      8. Salmenten prezioen zerrendan, sortu erregistro bat informazio honekin:
          - **Rola** = **Garatzailea**
          - **Baliabideen enpresa** = **Contoso Robotics UK**
          - **Fakturazio-tasa** = **200 USD**
      9. Joan **Salmentak** > **Proiektuen kontratuak** eta erantsi **Adventure Works fakturen tasak** proiektuaren kontratuaren Adventure Works proiektuaren prezioen zerrenda.