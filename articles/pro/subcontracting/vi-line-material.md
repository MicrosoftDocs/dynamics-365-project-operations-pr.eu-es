---
title: Produktuen saltzailearen fakturaren lerroak
description: Gai honetan produktuen saltzailearen faktura lerroak nola grabatu eta saltzaileek produktuen erosketak erregistratzeko eremu desberdinak nola erabili azaltzen da.
author: rumant
ms.date: 03/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: d38a447c576c095a7bbe2f5ed84342a88bf69a9b
ms.sourcegitcommit: b2224d1f3c0bd4925d647e6ca3960db81a209521
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/11/2022
ms.locfileid: "9261543"
---
# <a name="vendor-invoice-lines-for-products"></a>Produktuen saltzailearen fakturaren lerroak

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Saltzaileen faktura bat Microsoft Dynamics 365 Project Operations produktuen saltzaileen faktura-lerroak izan ditzake (materialak ere deitzen zaie). Proiektuen kudeatzaileek produktuen saltzaileen faktura lerroak erabil ditzakete proiektuetan erositako produktuen kostuak erregistratzeko.

Produktuen saltzaileen faktura-lerroek materialen azpikontratazio-lerro bati erreferentzia egin dezakete edo ez. Produktuen saltzaileen faktura-lerro batek azpikontratu bati erreferentzia egiten badio, proiektu-kudeatzaileek saltzaileen faktura-lerroak fakturatzen ari diren produktuak parekatu eta egiaztatu ahal izango dituzte, erositako produktuen erabilera erregistratu eta proiektuko arduradunek proiektuan onartutako gastuekin.

Ondorengo taulan fitxategien eremuei buruzko informazioa ematen da produktuen saltzailearen faktura-lerroan.

| Eremua | Deskribapenak | Inpaktu funtzionala |
| --- | --- | --- |
| Eman izena | Identifikazioan laguntzeko saltzailearen faktura-lerroaren izena. | Izena saltzailearen faktura-lerroetan oinarritutako bilaketa guztietan lehen zutabe gisa erakutsiko da. |
| Deskribapenak | Saltzaileak saltzailearen faktura-lerroan fakturatzen dituen produktuen deskribapen laburra. | Batere ez |
| Azpikontratua | Produktuak hasiera batean agindutako azpikontratua. | Saltzaileen fakturarako azpikontratu bat hautatzen denean, saltzaileen fakturako lerro guztiek hautapen hori heredatuko dute. Saltzaileen faktura batek ezin du izan azpikontratu desberdinak aipatzen dituzten hornitzaileen faktura lerroak. |
| Azpikontratuaren lerroa | Produktuak eskatuta azpikontratuaren lerroa. Hauta daitezkeen azpikontratuaren lerroen zerrenda hautatutako azpikontratuaren lerroetara mugatzen da. | Hornitzaileen faktura lerro batean azpikontratuaren lerro bat hautatzen denean produktuetarako, balio lehenetsiak **Proiektua**, **Zeregin**, eta **Produktua** eremuak azpikontratuaren lerroan dagozkion eremuetatik sartzen dira. Hautatutako azpikontratuaren lerroak balioak baditu **Proiektua**, **Zeregina**, eta **Produktua** eremuetan, hornitzaileen faktura-lerroko dagozkien eremuen balioak ezin dira balio horietatik desberdina izan. |
| Transakzioaren data | Saltzaileen faktura-lerroaren benetako kostua proiektuan erregistratuko den data. | Batere ez|
| Transakzio-klasea | Produktuak fakturatzen direnean, eremu hau ezarri behar da **Materiala**. | **Material** balioak saltzaileen faktura-lerroa erosi ziren produktuen fakturaren zenbatekoa erregistratzeko erabiltzen ari dela adierazten du. |
| Project | Fakturatutako produktuak erabili diren proiektuaren izena. | Eremua beharrezkoa da eta ezin da hutsik utzi. |
| Zeregina | Fakturatutako produktuak erabili diren proiektuaren zereginaren izena. Eremu hau proiektu bat hautatzen bada soilik dago erabilgarri. Proiektuko zeregina hautatzea aukerakoa da. | Eremu hau hutsik geratzen bada, proiektuaren kudeatzaileak hornitzaileen faktura-lerroa proiektuko edozein zereginetan erositako produktuekin lotu dezake. Saltzaileen faktura-lerroak ez badu azpikontratuaren lerrorik aipatzen, eta eremu hau hutsik geratzen bada, saltzaileen faktura-lerroak sortzen duen kostu erreala ez da fakturatu gabeko salmenta errealekin lotuko. Kasu honetan, zereginetan oinarritutako fakturazioa konfiguratzen bada, baliteke kostuak azken bezeroari ezin izango zaizkio fakturatu. |
| Hautatu produktua | Hautatu fakturatutako produktua produktuen katalogoan dagoen gehitutako produktu berezi bat den. | Balio lehenetsia azpikontratazio lerrotik sartzen da azpikontratazio lerro bat hautatzen denean. |
| Produktu | Aukeratu katalogoko produktu bat. Produktua idazteko produktua bada, idatzi produktuaren izena. | Eremu hau lehendik dauden produktuen erosketa prezio lehenetsiak sartzeko erabiltzen da. |
| Kantitatea | Sartu saltzaileak fakturatzen ari den material kopurua faktura lerroan. | Batere ez |
| Salmenta-unitatea | Hautatu fakturatzen den kantitatea adierazten den unitateko unitate-taldea. | Batere ez |
| Unitatea | Balio lehenetsia da hautatuta unitate-taldearen oinarrizko unitatea. Balio hau alda dezakezu hautatutako unitate taldeko edozein unitate ordaintzeko. | **Produktua** eta **Unitatea** balioen konbinazioa lehenetsitako moduan edo balio konputatu gisa erabiliko da saltzailearen faktura-lerroko **Unitatearen prezioa** eremuan. |
| Unitateko prezioa | Unitatearen prezio lehenetsiak erabiltzen ditu saltzailearen faktura-lerroko transakzioaren datan aplikatu daitekeen **Produktua** eta **Unitatea** balioak proiektuaren prezio-zerrendatik. | Batere ez |
| Guztizko partziala | Irakurtzeko soilik den eremua *Kopurua* &times; *Unitatearen prezioa* gisa kalkulatzen da, **Kopurua** eremua eta **Unitatearen prezioa** eremuetan balioak sartzen badira. Eremu bat edo biak hutsik badaude, balio bat sar dezakezu eremu horretan. | Batere ez |
| Salmenten zerga | Idatzi salmenta-zergaren zenbatekoa. | Batere ez |
| Zenbatekoa guztira | Saltzailearen faktura-lerroaren guztizko kantitatea barne hartutako zergak. Eremu honetan kalkulatuta dago *Azpitotala* + *Salmenten zerga*. | Batere ez |

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
