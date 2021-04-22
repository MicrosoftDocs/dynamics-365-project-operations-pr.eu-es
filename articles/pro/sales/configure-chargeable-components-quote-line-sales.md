---
title: Konfiguratu eskaintzaren lerro bateko kobra daitezkeen osagaiak
description: Gai honek proiektuan oinarritutako aurrekontu lerro batean kargagarriak eta kargagarriak ez diren osagaiak konfiguratzeari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 1a9e1851bd8c5a4070df2774c945d1f3eabaaa8a
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858278"
---
# <a name="configure-the-chargeable-components-of-a-quote-line"></a>Konfiguratu eskaintzaren lerro bateko kobra daitezkeen osagaiak 

_**Honetarako aplikatzen da:** inplementazio arina - mahukatik proformako fakturaziora, Baliabideen / stockean oinarritutako eszenatokien Project Operations_

Proiektuetan oinarritutako eskaintzaren lerroak *barne* osagaiak eta *kargagarriak* osagaiak kontzeptuak ditu.

Sartutako osagaien menpe daude:

  - Fakturazio metodoa eta bezeroen banaketak
  - Ez gainditzeko mugak 
  - Proiektuan oinarritutako eskaintzaren lerroan zehaztutako fakturen maiztasun ezarpenak

Sartutako osagaien azpimultzoa kargagarria gisa markatu daiteke **Fakturazio mota** eremua. **Fakturazio mota** eremua eskaintzaren lerro baten testuinguruan balio hauek onartzen dituen aukera multzoa da:

  - Kobra daiteke
  - Ezin da kargatu

Osagai kargagarriak zereginetan, roletan eta transakzio kategorietan defini daitezke.

Kargagarritasuna eskaintzaren kontratu lerro bateko zereginetan definitzen da eta lerroan sartutako transakzio klase guztiei aplikatzen zaie. **Gehitu zereginak** eremua **Proiektu osoa** bada edo hutsik badago, **Kobratzeko zereginak** fitxa ez da erabilgarri egongo.

Eskaintzaren lerro bateko roletan definitutako kargagarritasuna **Denbora** transakzio klasea. Eremuan, **Gehitu denbora** eremua **Ez** gisa ezarrita badago proiektuaren kuota lerroan, **Kobratzeko funtzioak** fitxa ez da erabilgarri egongo.

Eskaintzaren lerro bateko transakzio-kategorietan definitutako kobragarritasuna **Gastuak** transakzio klasea. Eremuan, **Gehitu gastuak** eremua **Ez** gisa ezarrita badago proiektuaren kuota lerroan, **Kobratzeko kategoriak** fitxa ez da erabilgarri egongo.

### <a name="update-a-project-task-to-be-chargeable-or-non-chargeable"></a>Eguneratu proiektuaren zeregina kargagarria edo kargagarria ez den moduan

Proiektuaren zeregina proiektuetan oinarritutako eskaintzaren lerro zehatz baten testuinguruan kargagarria edo ez kargagarria izan daiteke eta horrek konfigurazio hau posible egiten du.

Proiektuan oinarritutako aurrekontu lerroak biltzen badu **Denbora** eta zeregina **T1**, zeregina aurrekontu lerroarekin lotzen da kobratzeko moduan. Horrek barne hartzen duen bigarren eskaintzaren lerro bat badago **Gastuak**, **T1** zeregina eskaintzaren lerroan lotu dezakezu kobratzeko moduan. Emaitza da zereginean grabatutako denbora guztia kargagarria dela eta kargagarriak ez diren zereginetako gastu guztiak ez direla erregistratzen.

Ataza baten fakturazio mota konfiguratu daiteke **Zeregin kargagarriak** proiektuan oinarritutako eskaintzaren lerroaren fitxa eguneratuz **Fakturazio mota** eremua **Kontratu lerroaren atazak** azpisarea. Bestela, eguneratu dezakezu **Fakturazio mota** eremuko proiektu-zereginaren fakturazio motaren azpisarea eremuan, zeregin bati lotutako kontratu lerroak erakusten dituen proiektu baten fakturazio konfigurazioa.

### <a name="update-a-role-to-be-chargeable-or-non-chargeable"></a>Eguneratu funtzioa kargagarria edo kargagarria ez den moduan

Eginkizun bat kargagarria edo ez kargagarria izan daiteke proiektuan oinarritutako aurrekontu lerro jakin baten testuinguruan.

Funtzioa baten fakturazio mota konfiguratu daiteke **Funtzio kargagarriak** eskaintzaren lerroaren fitxa eguneratuz **Fakturazio mota** eremua **Funtzio kargagarriak** azpisarea.

### <a name="update-a-transaction-category-to-be-chargeable-or-non-chargeable"></a>Eguneratu transakzio-kategoria kargagarria edo kargagarria ez den moduan

Transakzio-kategoria bat kargagarria edo ez kargagarria izan daiteke eskaintzaren lerro jakin batean.

Transakzioaren fakturazio mota konfiguratu daiteke **Kategoria kargagarriak** eskaintzaren lerroaren fitxa eguneratuz **Fakturazio mota** eremua **Kategoria kargagarriak** azpisarea.

### <a name="resolve-chargeability"></a>Kargagarritasuna ebatzi
Denborarako sortutako aurrekontua edo benetakoa soilik kobratuko da:

   - **Denbora** eskaintza-lerroan sartzen da.
   - **Rola** eskaintza-linean kargatzeko moduan konfiguratuta dago.
   - **Zereginak barne** ezarrita dago **Aukeratutako zereginak** eskaintza-lerroan. 

Hiru gauza hauek egia badira, **Zeregina** kargatzeko moduan ere konfiguratzen da. 

Gasturako sortutako aurrekontua edo benetakoa soilik kobratuko da: 

   - **Gastua** eskaintza-lerroan sartzen da.
   - **Transakzioaren kategoria** eskaintza-linean kargatzeko moduan konfiguratuta dago.
   - **Zereginak barne** ezarrita dago **Aukeratutako zereginak** eskaintza-lerroan.

Hiru gauza hauek egia badira, **Zeregina** kargatzeko moduan ere konfiguratzen da. 

Materialerako sortutako aurrekontua edo benetakoa soilik kobratuko da:

   - **Materialak** eskaintza-lerroan sartzen da.
   - **Zereginak barne** ezarrita dago **Aukeratutako zereginak** eskaintza-lerroan.

Bi gauza hauek egia badira, **Zeregina** kargatzeko moduan ere konfiguratzen da. 


<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p>
                    <strong>Denbora barne</strong>
                </p>
            </td>
            <td width="78" valign="top">
                <p>
                    <strong>Gastua barne</strong>
                    <strong></strong>
                </p>
            </td>
            <td width="63" valign="top">
                <p>
                    <strong>Materialak barne</strong>
                    <strong></strong>
                </p>
            </td>
            <td width="75" valign="top">
                <p>
                    <strong>Gehitutako zereginak</strong>
                    <strong></strong>
                </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>Funtzioa</strong>
                    <strong></strong>
                </p>
            </td>
            <td width="70" valign="top">
                <p>
                    <strong>Kategoria</strong>
                    <strong></strong>
                </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>Ataza</strong>
                    <strong></strong>
                </p>
            </td>
            <td width="350" valign="top">
                <p>
                    <strong>Kargagarritasunaren eragina</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
Yes </p>
            </td>
            <td width="78" valign="top">
                <p>
Yes </p>
            </td>
            <td width="63" valign="top">
                <p>
Yes </p>
            </td>
            <td width="75" valign="top">
                <p>
Proiektu osoa </p>
            </td>
            <td width="65" valign="top">
                <p>
Kobra daiteke </p>
            </td>
            <td width="70" valign="top">
                <p>
Kobra daiteke </p>
            </td>
            <td width="65" valign="top">
                <p>
Ezin da ezarri </p>
            </td>
            <td width="350" valign="top">
                <p>
Fakturazioa denbora errealean: Kargagarria </p>
                <p>
Fakturazio mota benetako gastuan: Kargagarria </p>
                <p>
Fakturazio mota benetako materialean: Kargagarria </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
Yes </p>
            </td>
            <td width="78" valign="top">
                <p>
Yes </p>
            </td>
            <td width="63" valign="top">
                <p>
Yes </p>
            </td>
            <td width="75" valign="top">
                <p>
Hautatutako zereginak soilik </p>
            </td>
            <td width="65" valign="top">
                <p>
Kobra daiteke </p>
            </td>
            <td width="70" valign="top">
                <p>
Kobra daiteke </p>
            </td>
            <td width="65" valign="top">
                <p>
Kobra daiteke </p>
            </td>
            <td width="350" valign="top">
                <p>
Fakturazioa denbora errealean: Kargagarria </p>
                <p>
Fakturazio mota benetako gastuan: Kargagarria </p>
                <p>
Fakturazio mota benetako materialean: Kargagarria </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
Yes </p>
            </td>
            <td width="78" valign="top">
                <p>
Yes </p>
            </td>
            <td width="63" valign="top">
                <p>
Yes </p>
            </td>
            <td width="75" valign="top">
                <p>
Hautatutako zereginak soilik </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>Ezin da kargatu</strong>
                </p>
            </td>
            <td width="70" valign="top">
                <p>
Kobra daiteke </p>
            </td>
            <td width="65" valign="top">
                <p>
Kobra daiteke </p>
            </td>
            <td width="350" valign="top">
                <p>
Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </p>
                <p>
Fakturazio mota benetako gastuan: Kargagarria </p>
                <p>
Fakturazio mota benetako materialean: Kargagarria </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
Yes </p>
            </td>
            <td width="78" valign="top">
                <p>
Yes </p>
            </td>
            <td width="63" valign="top">
                <p>
Yes </p>
            </td>
            <td width="75" valign="top">
                <p>
Hautatutako zereginak soilik </p>
            </td>
            <td width="65" valign="top">
                <p>
Kobra daiteke </p>
            </td>
            <td width="70" valign="top">
                <p>
Kobra daiteke </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>Ez-kargagarria</strong>
                </p>
            </td>
            <td width="350" valign="top">
                <p>
Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </p>
                <p>
Fakturazio mota benetako gastuan: <strong>Ez-kargagarria</strong>
                </p>
                <p>
Fakturazio mota benetako materialean: <strong>Ez-kargagarria</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
Yes </p>
            </td>
            <td width="78" valign="top">
                <p>
Yes </p>
            </td>
            <td width="63" valign="top">
                <p>
Yes </p>
            </td>
            <td width="75" valign="top">
                <p>
Hautatutako zereginak soilik </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>Ez-kargagarria</strong>
                </p>
            </td>
            <td width="70" valign="top">
                <p>
Kobra daiteke </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>Ez-kargagarria</strong>
                </p>
            </td>
            <td width="350" valign="top">
                <p>
Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </p>
                <p>
Fakturazio mota benetako gastuan: <strong>Ez-kargagarria</strong>
                </p>
                <p>
Fakturazio mota benetako materialean: <strong>Ez-kargagarria</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
Yes </p>
            </td>
            <td width="78" valign="top">
                <p>
Yes </p>
            </td>
            <td width="63" valign="top">
                <p>
Yes </p>
            </td>
            <td width="75" valign="top">
                <p>
Hautatutako zereginak soilik </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>Ez-kargagarria</strong>
                </p>
            </td>
            <td width="70" valign="top">
                <p>
                    <strong>Ez-kargagarria</strong>
                </p>
            </td>
            <td width="65" valign="top">
                <p>
Kobra daiteke </p>
            </td>
            <td width="350" valign="top">
                <p>
Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </p>
                <p>
Fakturazio mota benetako gastuan: <strong>Ez-kargagarria</strong>
                </p>
                <p>
Fakturazio mota benetako materialean: Kargagarria </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
                    <strong>No</strong>
                </p>
            </td>
            <td width="78" valign="top">
                <p>
Yes </p>
            </td>
            <td width="63" valign="top">
                <p>
Yes </p>
            </td>
            <td width="75" valign="top">
                <p>
Proiektu osoa </p>
            </td>
            <td width="65" valign="top">
                <p>
Ezin da ezarri </p>
            </td>
            <td width="70" valign="top">
                <p>
                    <strong>Kobra daiteke</strong>
                </p>
            </td>
            <td width="65" valign="top">
                <p>
Ezin da ezarri </p>
            </td>
            <td width="350" valign="top">
                <p>
Fakturazioa denbora errealean: <strong>Ez dago erabilgarri</strong>
                </p>
                <p>
Fakturazio mota benetako gastuan: Kargagarria </p>
                <p>
Fakturazio mota benetako materialean: Kargagarria </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
                    <strong>No</strong>
                </p>
            </td>
            <td width="78" valign="top">
                <p>
Yes </p>
            </td>
            <td width="63" valign="top">
                <p>
Yes </p>
            </td>
            <td width="75" valign="top">
                <p>
Proiektu osoa </p>
            </td>
            <td width="65" valign="top">
                <p>
Ezin da ezarri </p>
            </td>
            <td width="70" valign="top">
                <p>
                    <strong>Ez-kargagarria</strong>
                </p>
            </td>
            <td width="65" valign="top">
                <p>
Ezin da ezarri </p>
            </td>
            <td width="350" valign="top">
                <p>
Fakturazioa denbora errealean: <strong>Ez dago erabilgarri</strong>
                </p>
                <p>
Fakturazio mota benetako gastuan: <strong> Ez-kargagarria</strong>
                </p>
                <p>
Fakturazio mota benetako materialean: Kargagarria </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
Yes </p>
            </td>
            <td width="78" valign="top">
                <p>
                    <strong>No</strong>
                </p>
            </td>
            <td width="63" valign="top">
                <p>
Yes </p>
            </td>
            <td width="75" valign="top">
                <p>
Proiektu osoa </p>
            </td>
            <td width="65" valign="top">
                <p>
Kobra daiteke </p>
            </td>
            <td width="70" valign="top">
                <p>
Ezin da ezarri </p>
            </td>
            <td width="65" valign="top">
                <p>
Ezin da ezarri </p>
            </td>
            <td width="350" valign="top">
                <p>
Fakturazioa denbora errealean: Kargagarria </p>
                <p>
Fakturazio mota benetako gastuan: <strong>Ez dago erabilgarri</strong>
                </p>
                <p>
Fakturazio mota benetako materialean: Kargagarria </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
Yes </p>
            </td>
            <td width="78" valign="top">
                <p>
                    <strong>No</strong>
                </p>
            </td>
            <td width="63" valign="top">
                <p>
Yes </p>
            </td>
            <td width="75" valign="top">
                <p>
Proiektu osoa </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>Ez-kargagarria</strong>
                </p>
            </td>
            <td width="70" valign="top">
                <p>
Ezin da ezarri </p>
            </td>
            <td width="65" valign="top">
                <p>
Ezin da ezarri </p>
            </td>
            <td width="350" valign="top">
                <p>
Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </p>
                <p>
Fakturazio mota benetako gastuan: <strong>Ez dago erabilgarri</strong>
                </p>
                <p>
Fakturazio mota benetako materialean: Kargagarria </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
Yes </p>
            </td>
            <td width="78" valign="top">
                <p>
Yes </p>
            </td>
            <td width="63" valign="top">
                <p>
                    <strong>No</strong>
                </p>
            </td>
            <td width="75" valign="top">
                <p>
Proiektu osoa </p>
            </td>
            <td width="65" valign="top">
                <p>
Kobra daiteke </p>
            </td>
            <td width="70" valign="top">
                <p>
Kobra daiteke </p>
            </td>
            <td width="65" valign="top">
                <p>
Ezin da ezarri </p>
            </td>
            <td width="350" valign="top">
                <p>
Fakturazioa denbora errealean: Kargagarria </p>
                <p>
Fakturazio mota benetako gastuan: Kargagarria </p>
                <p>
Fakturazio mota benetako materialean: <strong> Ez dago erabilgarri</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
Yes </p>
            </td>
            <td width="78" valign="top">
                <p>
Yes </p>
            </td>
            <td width="63" valign="top">
                <p>
                    <strong>No</strong>
                </p>
            </td>
            <td width="75" valign="top">
                <p>
Proiektu osoa </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>Ez-kargagarria</strong>
                </p>
            </td>
            <td width="70" valign="top">
                <p>
                    <strong>Ezin da kargatu</strong>
                </p>
            </td>
            <td width="65" valign="top">
                <p>
Ezin da ezarri </p>
            </td>
            <td width="350" valign="top">
                <p>
Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </p>
                <p>
Fakturazio mota benetako gastuan: <strong> Ez-kargagarria</strong>
                </p>
                <p>
Fakturazio mota benetako materialean: <strong> Ez dago erabilgarri</strong>
                </p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]
