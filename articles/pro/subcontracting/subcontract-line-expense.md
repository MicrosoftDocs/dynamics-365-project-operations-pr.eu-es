---
title: Azpikontratuaren lerroak gastuen kategorien arabera
description: Gai honetan produktuen azpikontratazio lerroak nola grabatu eta saltzaileek denbora erosketak erregistratzeko eremu desberdinak nola erabili azaltzen da.
author: rumant
ms.date: 08/06/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 9e8e7bb66063dab6db1ac8da1753913aee0ef3fc
ms.sourcegitcommit: 80aa1e8070f0cb4992ac408fc05bdffe47cee931
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "7323806"
---
#  <a name="subcontract-lines-for-expense-categories"></a>Azpikontratuaren lerroak gastuen kategorien arabera

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Urtean azpikontrata Dynamics 365 Project Operations gastuen kategorietarako lerro bat izan dezake. Gastu kategorietarako azpikontratazio lerroei esker, proiektuaren kudeatzaile batek zerbitzu edo produktu kategoriak eros ditzake proiektu batean karga ditzaketen saltzaileei.

Project Operations gastu kategorietarako azpikontratazio lerro bat sortzeko, osatu hurrengo urratsak.

1. Nabigazio panelean, hautatu **Azpikontratak**, eta ireki lan egin nahi duzun azpikontratua.
2. Gainean **Azpikontratatzeko Lineak** fitxa, hautatu **Berria** lerro berri bat sortzeko.
3. Gainean **Sortu bizkor** orrialdean, **Transakzio Klase** eremua, hautatu **Gastua** eta sartu edo hautatu beharrezko edozein eremuko informazioa.

Hurrengo taula hornitu informazioa eremuari buruz **Azpikontrataren lerroa** xehetasunak orria eta **Sortu bizkor** orria.

| **Eremua** |  **Azalpena** |
| ----------| ---------------- |
| Izena | Azpikontratuaren lerroaren izena. |
| Deskribapenak | Zerbitzu edo produktu kategorien deskribapen laburra erosten ari direnak azpikontratuaren lerroan. |
| Lerro mota | Eremu honek balioa lehenetsia dauka **Kopuruan oinarrituta**.  |
| Fakturazio-metodoa | Azpikontratazio lerroaren fakturazio metodoa. Aipatutako lerroaren fakturazio metodoan oinarrituta, Mugarrian oinarritutako fakturen egutegia eskuragarri dago Prezio finkoaren fakturazio metodoarentzat.  |
| Transakzio-klasea | Eremu honek balioa lehenetsia dauka **Denbora**. Produktuak erosteko azpikontrata lerroak sortzeko ezarri **Transakzio Klase** eremua hautatu **Gastua**. Eremu balio honek adierazten du azpikontratazio lerroa proiektuetan erabilitako produktuen edo zerbitzuen kategoria erosketa erregistratzeko erabiltzen dela. |
| Transakzio-kategoria | Hautatu transakzio-kategoria. |
| Eskatutako hasiera | Erosketa kategoriak saltzailearen eskura egon behar duen eguna. Eskatutako hasiera azpikontratari atxikitako proiektuen prezioen zerrendetatik proiektuaren prezioen zerrenda hautatzeko ere erabiltzen da. Azpikontratazio linean kategoria kostua prezio zerrenda horretatik lehenetsita dago. |
| Eskatutako amaiera | Erosketa kategoriak behar ez diren eguna. Data honek abisua deitzen du proiektuaren kudeatzaile batek azpikontratazio lerro hau data horretatik aurrera datatutako proiektuen gastu-kalkulu zehatzekin lotzen duenean. |
| Eskatutako kopurua | Kategoriaren kantitatea erosten da saltzailean. Proiektu kudeatzailean gainjartzen dira erositako kantitatea, abisua agertuko da.  |
| Salmenta-unitatea | Eremu honen balio lehenetsiak hautatutako kategorian ezarritako unitate talde lehenetsian oinarrituta daude. |
| Unitatea | Eremu honen balio lehenetsiak hautatutako kategorian ezarritako unitate lehenetsian oinarrituta daude. Kategoria eta unitatea konbinazioa erabiltzen da lehenetsita prezio-unitatea azpikontratuaren lerroan. |
| Unitate-prezioa | Prezio-unitatearen eremuaren balioak lehenetsia konbinazioa kategoria eta unitatea kategoriaren prezioetatik erlazionatuta proiektura prezio-zerrenda aplikagarria dena eskatutako hasiera azpikontratuaren lerrorako.  |
| Guztizko partziala | Irakurtzeko soilik den eremua da automatikoki honela kalkulatzen dena prezio-unitatearen prezioa kantitatea eta prezio unitarioaren balioak sartzen badira. Eremuetako bat edo biak hutsik badaude, eskuz idatz dezakezu balioa eremu honetan.  |
| Salmenten zerga | Idatzi salmenta-zergaren zenbatekoa.  |
| Zenbatekoa guztira | Azpikontratuaren lerroaren guztizko kantitatea barne hartutako zergak. Eremu honetan kalkulatuta dago azpitotala + salmenten zerga.  |


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
