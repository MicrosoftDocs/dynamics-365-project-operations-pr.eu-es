---
title: Proiektuaren faktura zuzentzaileak
description: Gai honek faktura zuzentzaileak sortu eta berresteko Project Operations-en informazioa ematen du.
author: rumant
manager: Annbe
ms.date: 04/05/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ae6d881e4e68b9f467478afe9735fc3186e6b0a8
ms.sourcegitcommit: ca0fc078d1a12484eca193fe051b8442c0559db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/07/2021
ms.locfileid: "5866576"
---
# <a name="corrective-project-invoices"></a>Proiektuaren faktura zuzentzaileak

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

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
