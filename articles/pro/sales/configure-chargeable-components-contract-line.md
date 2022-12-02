---
title: Konfiguratu proiektuetan oinarritutako kontratuaren lerro bateko kobra daitezkeen osagaiak
description: Gai honetan Project Operations-eko kontratuaren lerroetan osagai kargagarriak gehitzeko moduari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 10/08/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 0e4118e8e56d45ef75f53d828e267a8a9c1c903a
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8922943"
---
# <a name="configure-chargeable-components-of-a-project-based-contract-line"></a>Konfiguratu proiektuetan oinarritutako kontratuaren lerro bateko kobra daitezkeen osagaiak

_**Honetarako aplikatzen da:** inplementazio arina - mahukatik proformako fakturaziora, Baliabideen / stockean oinarritutako eszenatokien Project Operations_

Proiektuetan oinarritutako kontratuaren lerroak osagaiak eta osagai *kargagarriak* *ditu barne*.

Osagai hauek honako hauen menpeko osagaiak dira:

  - Fakturazio metodoa eta bezeroen banaketak
  - Ez gainditzeko mugak 
  - Proiektuan oinarritutako kontratu lerroan zehaztutako fakturen maiztasun ezarpenak

Sartutako osagaien azpimultzoa kargagarria gisa markatu daiteke **Fakturazio mota** eremua. **Fakturazio mota** eremua kontratu lerro baten testuinguruan balio hauek onartzen dituen aukera multzoa da:

  - Kobra daiteke
  - Ezin da kargatu

Osagai kargagarriak zereginetan, roletan eta transakzio kategorietan defini daitezke.

Kargagarritasuna proiektuko kontratu lerro bateko zereginetan definitzen da eta lerroan sartutako transakzio klase guztiei aplikatzen zaie. Kontratuaren lerroko **Gehitu zereginak** eremua hutsik badago edo **Proiektu osoa** gisa ezarrita badago, **Kobratzeko zereginak** fitxa ez da erabilgarri egongo.

Proiektuaren kontratu lerro bateko roletan definitutako kargagarritasuna **Denbora** transakzio klasea. Kontratuaren lerroko **Gehitu denbora** eremua **Ez** gisa ezarrita badago, **Kobratzeko funtzioak** fitxa ez da erabilgarri egongo.

Proiektuaren kontratuaren lerro bateko transakzio-kategorietan definitutako kobragarritasuna **Gastuak** transakzio klasea. Kontratuaren lerroko **Gehitu gastuak** eremua **Ez** gisa ezarrita badago, **Kobratzeko kategoriak** fitxa ez da erabilgarri egongo.

### <a name="update-a-project-task-as-chargeable-or-non-chargeable"></a>Eguneratu proiektuaren zeregina kargagarria edo kargagarria ez den moduan

Proiektuaren zeregina kontratu-lerro zehatz batean kargagarria edo ez kargagarria izan daiteke eta horrek konfigurazio hau posible egiten du:

Proiektuetan oinarritutako kontratu lerroak barne hartzen badu **Denbora** eta zeregin jakin bat, **T1** kargagarri gisa lotzen zaio. Horrek barne hartzen duen bigarren kontratu linea bat badago **Gastua**, T1 zeregina kontratu-lerroan lotu dezakezu kobratzeko moduan. Emaitza da zereginean grabatutako denbora guztia kargagarria dela eta gastu guztiak ez direla kobratzen.

Ataza baten fakturazio mota konfiguratu daiteke **Zeregin kargagarriak** kontratuaren lerroaren fitxa eguneratuz **Fakturazio mota** eremua kontratu lerroaren atazen azpisarea. Bestela, eguneratu dezakezu **Fakturazio mota** ataza azpisarea eremuan, zeregin bati lotutako kontratu lerroak erakusten dituen proiektu baten fakturazio konfigurazioa.

### <a name="update-a-role-as-chargeable-or-non-chargeable"></a>Eguneratu funtzioa kargagarria edo kargagarria ez den moduan

Eginkizun bat kargagarria edo ez kargagarria izan daiteke kontratu-lerro jakin batean.

Rol baten fakturazio mota konfiguratu daiteke **Kargatzeko rolak** kontratu lerro baten fitxa. Horretarako, eguneratu **Fakturazio mota** eremuan **Kargatzeko rolak** azpisarea.

### <a name="update-a-transaction-category-as-chargeable-or-non-chargeable"></a>Eguneratu transakzio-kategoria kargagarria edo kargagarria ez den moduan

Transakzio-kategoria bat kargagarria edo ez kargagarria izan daiteke kontratu-lerro jakin batean.

Transakzio baten fakturazio mota konfiguratu daiteke **Kargatzeko kategoriak** kontratuaren lerro batean oinarritutako proiektatearen fitxa. Horretarako, eguneratu **Fakturazio mota** eremuan **Kargatzeko kategoriak** azpisarea.

### <a name="resolve-chargeability"></a>Kargagarritasuna ebatzi

Denborarako sortutako aurrekontua edo benetakoa soilik kobratuko da:

   - **Denbora** kontratu-lerroan sartzen da.
   - **Rola** kontratu-linean kargatzeko moduan konfiguratuta dago.
   - **Zereginak barne** ezarrita dago **Aukeratutako zereginak** kontratu lerroan.
 
 Hiru gauza hauek egia badira, zeregina kargatzeko moduan konfiguratzen da. 

Gasturako sortutako aurrekontua edo benetakoa soilik kobratuko da:

   - **Gastua** kontratu-lerroan sartzen da
   - **Transakzioaren kategoria** kontratu-linean kargatzeko moduan konfiguratuta dago
   - **Zereginak barne** ezarrita dago **Aukeratutako zeregina** kontratu lerroan
  
 Hiru gauza hauek egia badira, **Zeregina** kargatzeko moduan konfiguratzen da. 

Materialerako sortutako aurrekontua edo benetakoa soilik kobratuko da:

   - **Materialak** kontratu-lerroan sartzen da
   - **Zereginak barne** ezarrita dago **Aukeratutako zereginak** kontratu lerroan

Bi gauza hauek egia badira, **Zeregina** kargatzeko moduan konfiguratzen da. 

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
Fakturazioa denbora errealean: <strong>Kargagarria</strong>
                </p>
                <p>
Fakturazio mota benetako gastuan: <strong>Kargagarria</strong>
                </p>
                <p>
Fakturazio mota benetako materialean: <strong>Kargagarria</strong>
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
Fakturazioa denbora errealean: <strong>Kargagarria</strong>
                </p>
                <p>
Fakturazio mota benetako gastuan: <strong>Kargagarria</strong>
                </p>
                <p>
Fakturazio mota benetako materialean: <strong>Kargagarria</strong>
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
