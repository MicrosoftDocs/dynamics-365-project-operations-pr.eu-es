---
title: Sortu proiektuetan oinarritutako faktura zuzentzaileak
description: Gai honek faktura zuzentzailearen inguruko informazioa eskaintzen du Project Operations-en.
author: rumant
ms.date: 03/29/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f0423fe9895b91431b2a83a8fff81118205b0736
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001592"
---
# <a name="create-corrective-project-based-invoices"></a>Sortu proiektuetan oinarritutako faktura zuzentzaileak 

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Egiaztatutako proiektuaren faktura zuzendu daiteke bezeroarekin eta proiektuaren arduradunarekin negoziatutako aldaketak edo kredituak prozesatzeko.

Berretsitako faktura batean aldaketak egiteko, ireki berretsitako faktura eta hautatu **Zuzendu faktura hau**. 

> [!NOTE]
> Aukeraketa hau ez dago erabilgarri proiektuaren faktura baieztatu ezean.

Berretsitako fakturatik faktura zirriborro berria sortzen da. Aurretik baieztatutako fakturaren faktura-lerroaren xehetasun guztiak zirriborro berrira kopiatzen dira. Honako hauek dira faktura zuzendu berriaren lerroaren xehetasunak gehiago ulertzen laguntzeko funtsezko puntu batzuk:

- Kopuru guztiak zero bihurtzen dira. Fakturatutako elementu guztiak guztiz kreditatuta daudela suposatzen du. Behar izanez gero, eskuz egunera ditzakezu kantitate horiek fakturatzen ari diren kopurua eta ez kreditatzen den kopurua. Sartzen duzun kantitatearen arabera, aplikazioak kreditatutako kantitatea kalkulatzen du. Zenbateko hori faktura zuzena baieztatzen denean sortzen diren errealetan islatzen da. Zergaren zenbatekoan aldaketak egiten ari bazara, zergaren zenbateko zuzena sartu behar duzu eta ez kreditatzen den zergaren zenbatekoa.
- Mugarrien zuzenketak kreditu oso gisa prozesatzen dira beti.
- Atxikitako edo aurreratutako zenbatekoak zuzendu daitezke bezeroari zenbateko okerra fakturatzen bazaio.
- Atxikitzaileen eta aurrerakinen bateragarritasuna zuzendu daiteke, aurrez baieztatutako faktura bateko kargekin bateratzeko zenbateko okerra erabili bada.

> [!IMPORTANT]
> Dagoeneko fakturatutako beste karga batzuen zuzenketak diren faktura lerroaren xehetasunek **Zuzenketa** eremua ezarrita dute **Bai**. Faktura lerroaren xehetasunak zuzendu dituzten fakturek izeneko eremua dute **Zuzenketak ditu** hori ere ezarrita dago **Bai**.

## <a name="actuals-created-on-confirmation-of-a-corrective-invoice"></a>Faktura zuzentzailea berrestean sortutako datuak

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
            <td width="216" rowspan="4" valign="top">
                <p>
Berretsi fakturatutako aurrerakinaren edo atxikipenaren zuzenketa.<strong></strong>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Adiskidetzerako sortu zen atxikipenaren edo aurrerakinaren fakturaziorik gabeko salmentak. Zenbateko hori positiboa da, atxikipena edo aurrerakina fakturatu zenean sortutako negatiboa bertan behera uzteko pentsatuta dagoelako.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Fakturatutako salmenten berraztertzea jatorrizko fakturatutako salmentak alderantzikatzeko atxikipena edo aurrerakinaren zenbatekoa sortzen da.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Fakturatutako salmenta berria atxikipeneko zuzendutako zenbatekoarekin edo aurrerakinean oinarritutako zuzendutako kontratuaren lerroarekin sortzen da.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Adiskidetzerako erabili beharreko atxikipenaren edo aurrerakinean oinarritutako zuzendutako fakturaren lerroaren zenbateko negatiboaren fakturaziorik gabeko salmentak.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
Aurretik bateratutako atxikipen edo aurrerakinaren zuzenketaren berrespena.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Adiskidetzerako sortu zen atxikipenaren edo aurrerakinaren fakturaziorik gabeko salmentak. Zenbateko hori positiboa da eta atxikipena edo aurrerakina fakturatu zenean kontziliazioa geratu zenerako pentsatuta dagoelako.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Aurreko fakturako zenbatekoaren fakturatutako alderantzikako salmentak.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Fakturatutako salmenta berria atxikipeneko zuzendutako zenbatekoarekin zuzendutako kontratuaren lerroarekin sortzen da.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Adiskidetzerako erabili beharreko atxikipenaren lerroaren zenbateko negatiboaren fakturaziorik gabeko salmentak.
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
Ez dira onartzen </p>
            </td>
        </tr>        
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
