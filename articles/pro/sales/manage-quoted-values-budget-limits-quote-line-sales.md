---
title: Proiektuetan oinarritutako eskaintzaren lerroak (Pro)
description: Gai honek proiektu-lanaren produktuetan oinarritutako eskaintza-lerroak erabiltzeari buruzko lerroei buruzko informazioa ematen du. (Pro)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a409d1e378afe97de7fb6c77cf3ad6703661bdff
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070966"
---
# <a name="project-based-quote-lines-pro"></a>Proiektuetan oinarritutako eskaintzaren lerroak (Pro)

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proiektuetan oinarritutako aurrekontu lerroak proiektu baten konpromisoa kalkulatzen laguntzeko diseinatuta daude. Proiektuan oinarritutako aurrekontu lerroaren egitura proiektuaren kalkuluen arabera hedatzen da, honako kontzeptu hauekin:

- Fakturazio-metodoa
- Proiektuen eta zereginen esleipena
- Transakzio klaseak barne
- Ez gainditzeko muga
- Aplikagarritasun konfigurazioa
- Aurrekontua Lerroaren xehetasunak erabiliz
- Eskaintzaren lerroaren bezeroak

Ondorengo taulan fitxategien eremuei buruzko informazioa ematen da **Orokorra** proiektuan oinarritutako aurrekontu lerroaren fitxa. Eremu horiei esker, proiektuaren inguruko lanen estimazio zehatza eta zehatza egiteko oinarriak ezartzen dira.

| **Eremua** | **Garrantzia, xedea eta orientazioa** | **Downstream eragina** |
| --- | --- | --- |
| Izena | Estimatzen ari den aurrekontuaren osagai diskretua identifikatzen lagunduko dizun aurrekontuaren lerroaren izena. | Aurrekontua lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean. |
| Fakturazio-metodoa | Aukera batetik sortutako aurrekontuan, balio hori aukera-lerroan dagokion eremutik kopiatzen da. Eremu honek Dynamics 365 Project Operations-ek onartzen dituen kontratazio eredu nagusiak biltzen ditu:</br>- Prezio finkoa</br>- Denbora eta materiala.| Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean. |
| Project | Erabili aukerako eremu hau konpromiso horretan lana emateko erabiliko den proiektua identifikatzeko. Proiektu bat aurrekontu lerro batera mapeatzen denean, kargagarriak diren atazak ezartzen laguntzen du eta proiektuan oinarritutako aurrekontua aurrekontuaren lerroan aurrekontuaren lerroaren xehetasun gisa ekartzen laguntzen du. Proiektu bat proiektuan oinarritutako aurrekontu lerro batera mapatuta ez dagoenean, aurrekontua eskuz sortu beharko litzateke aurrekontu lerroaren xehetasun bakoitza sortuz. | Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.|
| Gehitutako zereginak | Aipu lerro hau hautatutako proiektuaren proiektuko zeregin guztietarako edo batzuetarako erabiltzen den adierazten du. Eremuak balio hauek izan ditzake:</br>- Proiektuaren zeregin guztiak</br>- Hautatutako proiektu-zereginak soilik</br>Eremu honetako balio hutsa balioaren baliokidea da **Proiektuaren zeregin guztiak** aukera. | **Aukeratutako proiektuaren zereginak soilik** hautatzen denean proiektuaren orrian, **Zereginen fakturazio konfigurazioa** fitxak zeregin zehatzak hautatzeko aukera ematen du aurrekontu lerro honekin lotzeko. Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean. |
| Idatzi denbora | **Bai**/**Ez** banderak adierazten du hautatutako proiektuaren denborako transakzioak edo lan kostuak aurrekontu lerro honetako aurrekontuan sartuko diren. **Ez** balioak adierazten du denbora-transakzioak edo lan-kostuak ez direla sartuko aurrekontu honen eskaintzaren lerroan. **Bai** balioak adierazten du denbora-transakzioak edo lan-kostuak sartuko direla aurrekontu honen eskaintzaren lerroan. | Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean. |
| Idatzi gastua | **Bai**/**Ez** banderak adierazten du hautatutako proiektuaren denborako gastuak aurrekontu lerro honetako aurrekontuan sartuko diren. **Ez** balioak adierazten du gastuak ez direla sartuko aurrekontu honen eskaintzaren lerroan. **Bai** balioak adierazten du gastuak sartuko direla aurrekontu honen eskaintzaren lerroan. | Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerro baten gainean kopiatu da aurrekontua irabazten denean. |
| Idatzi prezioa | **Bai**/**Ez** banderak adierazten du hautatutako proiektuaren denborako komisioak aurrekontu lerro honetako aurrekontuan sartuko diren. **Ez** balioak adierazten du komisioak ez direla sartuko aurrekontu honen eskaintzaren lerroan. **Bai** balioak adierazten du komisioak sartuko direla aurrekontu honen eskaintzaren lerroan. | Eremuaren balioa eskaintzaren lerro honetatik sortzen den Proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean. |
| Eskainitako zenbatekoa | Proiektuan oinarritutako aurrekontu lerro honetan aurreikusitako lan guztiari bezeroari aipatuko zaion zenbatekoa da. Aukera batetik sortutako aurrekontuan, balio hori aukera-lerroaren **Bezeroaren aurrekontua** eremutik kopiatzen da. Proiektuan oinarritutako aurrekontu lerroak lerroaren xehetasunak dituenean, eremu hau blokeatuta dago editatzeko eta aurrekontuaren lerroaren xehetasunetan agertzen den zenbatekoaren arabera laburbiltzen da. | Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean. |
| Aurreikusitako zerga | Eremu editagarria da erabiltzaileak aurrekontu lerroan zenbatetsitako zerga kopurua gehitzeko. Proiektuan oinarritutako aurrekontu lerroak lerroaren xehetasunak dituenean, eremu hau blokeatuta dago editatzeko eta aurrekontuaren lerroaren xehetasunetan agertzen den zerga-zenbatekoaren arabera laburbiltzen da. | Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean. |
| Eskainitako zenbatekoa, zergaren ondoren | Eremu hau zerga ondorengo aurrekontuaren zenbatekoa da eta irakurtzeko soilik da. Eremu honetako zenbatekoa honela kalkulatzen da *Aipatutako zenbatekoa + Zerga*. | Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean. |
| Ez gainditzeko muga | Eremu hau editagarria da eta proiektu bat duten aurrekontu lerroetan soilik dago erabilgarri **Denbora eta materiala** fakturazio metodoa. | Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean. |
| Bezeroaren aurrekontua | Eremu hau editagarria da eta balio hori aukera-lerroan dagokion eremutik kopiatzen da, abagunea eskaintza batetik sorten bada. | Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean. |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a>Proiektuetan oinarritutako aurrekontu lerroen Orokorra fitxako eremuen baliozkotze arauak

**1. araua** : **Zereginak barne** eremua hutsik badago, edo ezarrita badago **Proiektuaren zeregin guztiak** , proiektu bat aurrekontuaren lerroan sartzen da.

**2. araua** : **Zereginak barne** eremua hutsik badago, edo ezarrita badago **Proiektuaren zeregin guztiak** , proiektu bat eta transakzio klase jakin bat aurrekontuaren proiektuan oinarritutako aurrekontu lerro batean bakarrik sar daitezke.

**3. araua** : **Zereginak barne** eremua **Hautatutako proiektuaren zereginak soilik** gisa ezarrita badago, proiektu bat eta transakzio klase jakin bat aurrekontuaren proiektuan oinarritutako aurrekontuan sar daitezke.

**4. araua** : Aukera batek aurrekontu ugari baditu, aurrekontu desberdinetako aurrekontu lerroak egon daitezke, proiektu bera aipatzen dutenak eta transakzio klase bera barne hartzen dutenak.

**5. araua** : Aurrekontuak aukera berekoak ez badira, ezin dute proiektu eta transakzio klase bera sartu.

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p>
                    <strong>Abagunea</strong>
                </p>
            </td>
            <td width="41" valign="top">
                <p>
                    <strong>Eskaintza</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Eskaintzaren lerroa</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Project</strong>
                </p>
            </td>
            <td width="90" valign="top">
                <p>
                    <strong>Gehitutako zereginak</strong>
                </p>
            </td>
            <td width="48" valign="top">
                <p>
                    <strong>Idatzi denbora</strong>
                </p>
            </td>
            <td width="48" valign="top">
                <p>
                    <strong>Idatzi gastua</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Sartu</strong>
                </p>
                <p>
                    <strong>Prezioa</strong>
                </p>
            </td>
            <td width="54" valign="top">
                <p>
                    <strong>Baliozkoa/Baliogabea da</strong>
                </p>
            </td>
            <td width="308" valign="top">
                <p>
                    <strong>Arrazoia</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
1H </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
Baliogabea da </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
2. araua haustea. P1 proiektuaren denbora, gastuak eta tasak aurrekontu lerroetan, QL1 eta QL2 barne daude.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
1H </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
1H </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
+Ez </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
Baliogabea da </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
2. araua haustea. P1 proiektuaren denbora eta tasak aurrekontu lerroetan, QL1 eta QL2 barne daude.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
1H </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
1H </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
+Ez </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
Baliozkoa </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
P1 proiektuaren denbora eta tasak QL1-en sartzen dira.
P1 proiektuaren gastuak QL2n sartzen dira.
Aurrekontu lerro bakoitzean sartzen den horretan ez dago gainjartzerik, eta balio du.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
1H </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="48" valign="top">
                <p>
+Ez </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
+Ez </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
1H </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Hautatutako zereginak soilik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
Baliogabea da </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
2. araua haustea eta gehiago </p>
                <p>
P1 proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, gastuak eta tasak sartzen dira.
                </p>
                <p>
QL2-k P1 proiektu osorako Denbora, Gastuak eta Tasak barne hartzen ditu eta Q1-n sartutakoarekin gainjartzen da.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
1H </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
1H </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Hautatutako zereginak soilik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
Baliozkoa </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
3. arauaren eta abarren arabera, </p>
                <p>
P1 proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, gastuak eta tasak sartzen dira.
                </p>
                <p>
P1 proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, gastuak eta tasak sartzen dira.
                </p>
                <p>
Balidazio osagarri bakarra QL1-eko zereginen azpimultzoaren inguruan kokatzen da, QL2-ren zereginen azpimultzoarekin alderatuta. Honek gainjartzerik ez dagoela ziurtatzen du. Sistemak zereginak lotzen dituenean egiten du.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
1H </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Hautatutako zereginak soilik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
1H </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Proiektuaren zeregin guztiak edo hutsik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="54" valign="top">
                <p>
Baliozkoa </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
5. arauan oinarrituta, Q1 eta Q2 aukera berdineko bi komatxo dira, beraz, biek proiektu baten osagai berberak kalkula ditzakete.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
2H </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Proiektuaren zeregin guztiak edo hutsik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="54" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
1H </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Proiektuaren zeregin guztiak edo hutsik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="54" valign="top">
                <p>
Baliozkoa </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
4. arauan oinarrituta, Q1 eta Q2 aukera desberdineko bi komatxo dira, beraz, proiektu berean ezin dira osagai berberak kalkulatu.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O2 </p>
            </td>
            <td width="41" valign="top">
                <p>
1H </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="90" valign="top">
                <p>
Proiektuaren zeregin guztiak edo hutsik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="54" valign="top">
                <p>
Baliogabea da </p>
            </td>
        </tr>
    </tbody>
</table>

