---
title: Baieztatu proformako faktura
description: Gai honetan Project Operations-eko proformako fakturak berresteari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 4b67ee6848efdcb85cf732c1eaa3e40cdc51a2e2
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070944"
---
# <a name="confirming-a-proforma-invoice"></a>Baieztatu proformako faktura

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_


Proforma faktura baieztatu ondoren, proiektuaren fakturaren egoera eguneratu egingo da **Baieztatuta**. Faktura bat baieztatzen denean, irakurtzeko soilik bihurtzen da. Aurrerantzean, faktura bezeroak hasitako zuzenketak edo kredituak badaude bakarrik zuzendu ahal izango da, faktura ordainduta dagoela markatuta badago.

Hurrengo taulan sistemak sortutako errealitateak zerrendatzen dira. Egitate horiek proiektuaren fakturaren zirriborroan eragiketa batzuk egiten direnean sortzen dira, hori baieztatu aurretik.

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
Atxikipen edo aurrerakin bat fakturatzea </p>
            </td>
            <td width="408" valign="top">
                <p>
Mota bateko fakturatutako salmentak, <strong>Atxikitzailea</strong> aurrerakinaren edo atxikipenaren zenbatekoarengatik sortzen da.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Adiskidetzerako erabili beharreko atxikipenaren edo aurrerakinaren zenbateko negatiboaren fakturaziorik gabeko salmentak.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
Atxikimendu bat edo faktura baten aurrerapena guztiz bateratu ondoren.
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
Faktura honetako zenbatekoaren fakturatutako salmentak.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
Atxikimendu bat edo faktura baten aurrerapena zati batean bateratu ondoren.
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
Faktura honetako zenbatekoaren fakturatutako salmentak.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Etorkizuneko fakturetan adiskidetzerako erabili beharreko geratzen den atxikipenaren edo aurrerakinaren fakturatu gabeko salmenta negatiboak.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
Denbora-transakzio bat fakturatzea zirriborroaren fakturan aldaketarik egin gabe.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Jatorrizko denbora-onespen bateko orduen eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Orduen eta zenbatekoaren fakturatutako salmentak jatorrizko denboraren onarpenean.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
Kopurua murrizteko editatu den denbora-transakzio bat fakturatzea.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Jatorrizko denbora-onespen bateko orduen eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Editatutako fakturaren lerroaren xehetasunean orduak eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, fakturatutako salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Editatutako fakturaren lerroaren xehetasunean geratzen diren orduak eta zuzendutako zenbakiak kendu eta gero zenbatekoa kobratzen ez duen fakturaziorik gabeko salmenta berria, fakturatutako salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
Kopurua areagotzeko editatu den denbora-transakzio bat fakturatzea.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Jatorrizko denbora-onespen bateko orduen eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Editatutako fakturaren lerroaren xehetasunean orduak eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, fakturatu gabeko salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
Gastu transakzio bat fakturatzea zirriborroaren fakturan aldaketarik egin gabe.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Zenbatekoaren eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzeak jatorrizko gastuaren onarpenean.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Zenbatekoaren eta zenbatekoaren fakturatutako salmentak jatorrizko gastuaren onarpenean </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
Kopurua murrizteko editatu den gastu-transakzio bat fakturatzea.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Zenbatekoaren eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzeak jatorrizko gastuaren onarpenean.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Editatutako fakturaren lerroaren xehetasunean kopurua eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, fakturatu gabeko salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Editatutako fakturaren lerroaren xehetasunean geratzen diren kopuruak eta zuzendutako zenbakiak kendu eta gero zenbatekoa kobratzen ez duen fakturaziorik gabeko salmenta berria, fakturatutako salmenten itzulketa eta fakturatu gabeko salmenten baliokide baliokidea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
Kopurua areagotzeko editatu den gastu-transakzio bat fakturatzea.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Zenbatekoaren eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzeak jatorrizko gastuaren onarpenean.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Editatutako fakturaren lerroaren xehetasunean kopurua eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, fakturatu gabeko salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea. 
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
Kuota fakturatzea.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Jatorrizko kutxako liburuaren lerroko zerga-zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
Zenbatekoaren eta zenbatekoaren fakturatutako salmentak zergen kutxako liburuaren lerroan.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
Mugarri bat fakturatzea.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Proiektuaren kontratu linearen jatorrizko mugarriaren zenbatekoaren fakturatutako salmentak.
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
Produktuetan oinarritutako kontratuaren lerroaren fakturazioa.
                </p>
            </td>
            <td width="408" valign="top">
                <p>
Produktu-lerroaren fakturatutako salmentak, produktuan oinarritutako kontratu-lerroaren zenbatekoarekin eta zenbatekoarekin.
                </p>
            </td>
        </tr>
    </tbody>
</table>
