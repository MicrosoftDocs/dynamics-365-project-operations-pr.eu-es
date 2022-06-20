---
title: Proiektuetan oinarritutako faktura zuzentzaileak
description: Artikulu honek proiektuan oinarritutako faktura zuzentzaileak sortu eta berresteko informazioa eskaintzen du Project Operations-en.
author: rumant
ms.date: 03/29/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: eecaf3dedeab5ff72d12808eb3144f9161313009
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8931085"
---
# <a name="corrective-project-based-invoices"></a>Proiektuetan oinarritutako faktura zuzentzaileak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Egiaztatutako proiektuaren faktura zuzendu daiteke bezeroarekin eta proiektuaren arduradunarekin negoziatutako aldaketak edo kredituak prozesatzeko.

Berretsitako faktura batean aldaketak egiteko, ireki berretsitako faktura eta hautatu **Zuzendu faktura hau**. 

> [!NOTE]
> Aukeraketa hau ez dago erabilgarri proiektuaren faktura baieztatzen ez bada edo proiektuan oinarritutako fakturak aurrerakinak edo atxikipenak edo aurrerakinen edo atxikipenak bateratzeko.

Berretsitako fakturatik faktura zirriborro berria sortzen da. Aurretik baieztatutako fakturaren faktura-lerroaren xehetasun guztiak zirriborro berrira kopiatzen dira. Honako hauek dira faktura zuzendu berriaren lerroaren xehetasunak ulertzeko gakoetako batzuk:

- Kopuru guztiak zero bihurtzen dira. Dynamics 365 Project Operations fakturatutako elementu guztiak guztiz kreditatuta daudela suposatzen du. Behar izanez gero, eskuz egunera ditzakezu kantitate horiek fakturatzen ari diren kopurua eta ez kreditatzen den kopurua. Sartzen duzun kantitatearen arabera, aplikazioak kreditatutako kantitatea kalkulatzen du. Zenbateko hori faktura zuzena baieztatzen denean sortzen diren errealetan islatzen da. Zergaren zenbatekoan aldaketak egiten ari bazara, zergaren zenbateko zuzena sartu behar duzu eta ez kreditatzen den zergaren zenbatekoa.
- Mugarrien zuzenketak kreditu oso gisa prozesatzen dira beti.


> [!IMPORTANT]
> Dagoeneko fakturatutako beste karga batzuen zuzenketak diren faktura lerroaren xehetasunetarako **Zuzenketa** eremua ezarrita dago **Bai**. Zuzendutako fakturaren lerroak dituzten fakturen xehetasunak, **Zuzenketak ditu** eremua ezarrita dago **Bai**.

## <a name="actuals-created-when-a-corrective-invoice-is-confirmed"></a>Faktura zuzentzailea baieztatzean sortutako datuak

Hurrengo taulan faktura zuzentzailea baieztatzen denean sortzen diren errealitateak agertzen dira.

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p>
                    <strong>Egoera</strong>
                </p>
            </td>
            <td width="808" valign="top">
                <p>
                    <strong>Berrespenean sortutako datuak</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
Aurretik fakturatutako denbora transakzio baten kreditu osoa fakturatzea.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Denboraren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako salmenten alderantzikatzea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Denboraren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
Kreditu partziala fakturatzea denborako transakzio batean.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Denboraren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako salmenten alderantzikatzea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Editatutako fakturaren lerroaren xehetasunean orduak eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, horien itzulketa eta fakturatutako salmenten baliokide baliokidea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Fakturarik gabeko salmenten faktura berri bat, fakturazio lerroaren xehetasunean zuzendu diren zifrak kendu ondorengo gainerako orduetan eta zenbatekoan kobratuko dena.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
Aurretik fakturatutako gastua transakzio baten kreditu osoa fakturatzea.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Gastuaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako zenbatekoaren alderantzikatzea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Gastuaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatu gabeko zenbatekoaren alderantzikatzea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
Aurretik fakturatutako gastua transakzio baten kredituaren zati bat fakturatzea.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Gastuaren jatorrizko fakturatutako lerroko xehetasunen eta zenbatekoaren fakturatutako zenbatekoaren alderantzikatzea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Editatutako fakturaren lerroaren xehetasunean kopurua eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, horien itzulketa eta fakturatutako salmenten baliokide baliokidea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Fakturarik gabeko salmenten faktura berri bat, fakturazio lerroaren xehetasunean zuzendu diren zifrak kendu ondorengo gainerako kopuruan eta zenbatekoan kobratuko dena
                </p>
            </td>
        </tr>
                <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
Aurretik fakturatutako transakzio material baten kreditu osoa fakturatzea.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Fakturatutako salmenten itzulketa materialaren jatorrizko fakturaren lerroaren xehetasunean dagoen kantitatea eta zenbatekoa.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Fakturatu gabeko salmenten benetako datuak materialaren jatorrizko fakturaren lerroaren xehetasunean dagoen kantitatea eta zenbatekoa.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
Transakzio material baten kreditu partziala fakturatzea.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Fakturatutako salmenten itzulketa materialaren jatorrizko fakturaren lerroaren xehetasunean dagoen fakturatutako kantitatea eta zenbatekoa.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Editatutako fakturaren lerroaren xehetasunean zenbatekoaren eta zenbatekoaren kargura dagoen fakturaziorik gabeko salmenta berri bat, honen itzulketa eta fakturatutako salmenten baliokide baliokidea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Fakturarik gabeko salmenten faktura berri bat, fakturazio lerroaren xehetasunean zuzendu diren zifrak kendu ondorengo gainerako kopuruan eta zenbatekoan kobratuko dena
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
Aurretik fakturatutako zerga transakzio baten kreditu osoa fakturatzea.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Zergaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako zenbatekoaren alderantzikatzea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Zergaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatu gabeko zenbatekoaren alderantzikatzea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
Aurretik fakturatutako zerga transakzio baten kredituaren zati bat fakturatzea.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Zergaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako zenbatekoaren alderantzikatzea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Editatutako fakturaren lerroaren xehetasunean kopurua eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, horien itzulketa eta fakturatutako salmenten baliokidea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
Aurretik fakturatutako mugarri baten kreditu osoa fakturatzea.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Mugarriaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako salmenten alderantzikatzea.
                </p>
                <p>
Mugarriaren fakturaren egoera eguneratzen da <b>Bezeroaren faktura argitaratua</b> <b>Fakturatzeko prest</b>.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
Aurretik fakturatutako mugarri baten kredituaren zati bat fakturatzea.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Egoera hau ez da onartzen.
                </p>
            </td>
        </tr>       
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
