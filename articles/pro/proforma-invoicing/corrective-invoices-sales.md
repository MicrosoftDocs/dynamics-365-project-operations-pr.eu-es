---
title: Proiektuaren faktura zuzentzaileak
description: Artikulu honek faktura zuzentzaileak sortu eta baieztatzeari buruzko informazioa eskaintzen du Project Operations-en.
author: rumant
ms.date: 04/05/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 3e8e10d69368f4704ec6121106fbfd35394dc441
ms.sourcegitcommit: 95dacb0e74fa8970f56fdb1cbaa915d3fbec6e0f
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/17/2022
ms.locfileid: "9023644"
---
# <a name="corrective-project-invoices"></a>Proiektuaren faktura zuzentzaileak

_**Honetarako aplikatzen da:** inplementazio arina - mahukatik proformako fakturaziora, Baliabideen / stockean oinarritutako eszenatokien Project Operations_

Egiaztatutako proiektuaren faktura zuzendu daiteke bezeroarekin eta proiektuaren arduradunarekin negoziatutako aldaketak edo kredituak prozesatzeko.

Berretsitako faktura batean aldaketak egiteko, ireki berretsitako faktura eta hautatu **Zuzendu faktura hau**. 

> [!NOTE]
> Aukeraketa hau ez dago erabilgarri proiektuaren faktura baieztatu ezean.

Berretsitako fakturatik faktura zirriborro berria sortzen da. Aurretik baieztatutako fakturaren faktura-lerroaren xehetasun guztiak zirriborro berrira kopiatzen dira. Honako hauek dira faktura zuzendu berriaren lerroaren xehetasunak ulertzeko gakoetako batzuk:

- Kopuru guztiak zero bihurtzen dira. Aplikazioak fakturatutako elementu guztiak guztiz kreditatuta daudela suposatzen du. Behar izanez gero, eskuz egunera ditzakezu kantitate horiek fakturatzen ari diren kopurua eta ez kreditatzen den kopurua. Sartzen duzun kantitatearen arabera, aplikazioak kreditatutako kantitatea kalkulatzen du. Zenbateko hori faktura zuzena baieztatzen denean sortzen diren errealetan islatzen da. Zergaren zenbatekoan aldaketak egiten ari bazara, zergaren zenbateko zuzena sartu behar duzu eta ez kreditatzen den zergaren zenbatekoa.
- Aurretik baieztatutako produktuetan oinarritutako kontratu lerroak ez dira kopiatzen. Ez da onartzen produktuan oinarritutako proiektuaren fakturan zuzenketak prozesatzea.
- Mugarrien zuzenketak kreditu oso gisa prozesatzen dira beti.
- Atxikitako edo aurreratutako zenbatekoak zuzendu daitezke bezeroari zenbateko okerra fakturatzen bazaio.
- Atxikitzaileen eta aurrerakinen bateragarritasuna zuzendu daiteke, aurrez baieztatutako faktura bateko kargekin bateratzeko zenbateko okerra erabili bada.

> [!IMPORTANT]
> Jada fakturatutako beste karga batzuen zuzenketen faktura-lerroaren xehetasunak daude **Zuzenketa** ezarri **Bai**. Faktura lerroaren xehetasunak zuzendu dituzten fakturek izeneko eremua dute **Zuzenketak ditu** hori ere ezarrita dago **Bai**.

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
Ez dira onartzen </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
Aurretik fakturatutako produktuan oinarritutako kontratu lerro baten kredituak eta zuzenketak.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Ez dira onartzen </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
