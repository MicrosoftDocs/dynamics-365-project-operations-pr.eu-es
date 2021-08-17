---
title: Proiektuetan oinarritutako eskaintzaren lerroen ikuspegi orokorra
description: Gai honek proiektu-lanaren produktuetan oinarritutako eskaintza-lerroak erabiltzeari buruzko lerroei buruzko informazioa ematen du.
author: rumant
ms.date: 03/30/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: 2f2d38c7fb3bc3ec26cf64525ef8275adecafd7fc48e97d6daef595d341c045d
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "7001551"
---
# <a name="project-based-quote-lines-overview"></a>Proiektuetan oinarritutako eskaintzaren lerroen ikuspegi orokorra 

_**Honetarako aplikatzen da:** inplementazio arina - mahukatik proformako fakturaziora, Baliabideen / stockean oinarritutako eszenatokien Project Operations_

Proiektuetan oinarritutako aurrekontu lerroak proiektu baten konpromisoa kalkulatzen laguntzeko diseinatuta daude. Proiektuan oinarritutako aurrekontu lerroaren egitura proiektuaren kalkuluen arabera hedatzen da, honako kontzeptu hauekin:

- Fakturazio-metodoa
- Proiektuen eta zereginen esleipena
- Transakzio klaseak barne
- Ez gainditzeko muga
- Aplikagarritasun konfigurazioa
- Aurrekontua Lerroaren xehetasunak erabiliz
- Eskaintzaren lerroaren bezeroak

Ondorengo taulan fitxategien eremuei buruzko informazioa ematen da **Orokorra** proiektuan oinarritutako aurrekontu lerroaren fitxa. Eremu horiei esker, proiektuaren inguruko lanen estimazio zehatza eta zehatza egiteko oinarriak ezartzen dira.

| **Eremua** | **Azalpena** | **Downstream eragina** |
| --- | --- | --- |
| Izena | Estimatzen ari den aurrekontuaren osagai diskretua identifikatzen laguntzen duen aurrekontuaren lerroaren izena. | Aurrekontua lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean. |
| Fakturazio-metodoa | Aukera batetik sortutako aurrekontuan, balio hori aukera-lerroan dagokion eremutik kopiatzen da. Eremu honek Dynamics 365 Project Operations-ek onartzen dituen bi kontratazio-eredu nagusiak biltzen ditu:</br>- Prezio finkoa</br>- Denbora eta materiala.| Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da. |
| Project | Erabili aukerako eremu hau konpromiso horretan lana emateko erabiliko den proiektua identifikatzeko. Proiektu bat aurrekontu lerro batera mapeatzen denean, kargagarriak diren atazak ezartzen laguntzen du eta proiektuan oinarritutako aurrekontua aurrekontuaren lerroan aurrekontuaren lerroaren xehetasun gisa ekartzen laguntzen du. Proiektu bat proiektuan oinarritutako aurrekontu lerro batera mapatuta ez dagoenean, aurrekontua eskuz sortu beharko litzateke aurrekontu lerroaren xehetasun bakoitza sortuz. | Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da.|
| Gehitutako zereginak | Aipu lerro hau hautatutako proiektuaren proiektuko zeregin guztietarako edo batzuetarako erabiltzen den adierazten du. Eremuak balio hauek izan ditzake:</br>- Proiektuaren zeregin guztiak</br>- Hautatutako proiektu-zereginak soilik</br>Eremu honetako balio hutsa balioaren baliokidea da **Proiektuaren zeregin guztiak** aukera. | **Aukeratutako proiektuaren zereginak soilik** proiektuaren orrian hautatzen da **Zereginen fakturazio konfigurazioa** fitxak zeregin zehatzak hautatzeko aukera ematen du aurrekontu lerro honekin lotzeko. Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da. |
| Idatzi denbora | **Bai**/**Ez** balioa adierazten du hautatutako proiektuaren denborako transakzioak edo lan kostuak aurrekontu lerro honetako aurrekontuan sartuko diren. **Ez** balioak adierazten du denbora-transakzioak edo lan-kostuak ez direla sartuko aurrekontu honen eskaintzaren lerroan. **Bai** balioak adierazten du denbora-transakzioak edo lan-kostuak sartuko direla aurrekontu honen eskaintzaren lerroan. | Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da. |
| Idatzi gastua | **Bai**/**Ez** balioa adierazten du hautatutako proiektuaren gastuen kostuak aurrekontu lerro honetako aurrekontuan sartuko diren. **Ez** balioak adierazten du gastuak ez direla sartuko aurrekontu honen eskaintzaren lerroan. **Bai** balioak adierazten du gastuak sartuko direla aurrekontu honen eskaintzaren lerroan. | Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da. |
| Sartu materiala | **Bai**/**Ez** balioa adierazten du hautatutako proiektuaren materialaren kostuak aurrekontu lerro honetako aurrekontuan sartuko diren. **Ez** balioa adierazten du materialaren kostuak aurrekontu lerro honetako aurrekontuan ez diren sartuko. **Bai** balioa adierazten du materialaren kostuak aurrekontu lerro honetako aurrekontuan sartuko diren. | Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da. |
| Idatzi prezioa | **Bai**/**Ez** balioa adierazten du hautatutako proiektuaren kostuen aurrekontu lerro honetako aurrekontuan sartuko diren. **Ez** balioak adierazten du komisioak ez direla sartuko aurrekontu honen eskaintzaren lerroan. **Bai** balioak adierazten du komisioak sartuko direla aurrekontu honen eskaintzaren lerroan. | Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da. |
| Eskainitako zenbatekoa | Proiektuan oinarritutako aurrekontu lerro honetan aurreikusitako lan guztiari bezeroari aipatuko zaion zenbatekoa da. Aukera batetik sortutako aurrekontuan, balio hori aukera-lerroaren **Bezeroaren aurrekontua** eremutik kopiatzen da. Proiektuan oinarritutako aurrekontu lerroak lerroaren xehetasunak dituenean, eremu hau blokeatuta dago editatzeko eta aurrekontuaren lerroaren xehetasunetan agertzen den zenbatekoaren arabera laburbiltzen da. | Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da. |
| Aurreikusitako zerga | Eremu editagarria da erabiltzaileak aurrekontu lerroan zenbatetsitako zerga kopurua gehitzeko. Proiektuan oinarritutako aurrekontu lerroak lerroaren xehetasunak dituenean, eremu hau blokeatuta dago editatzeko eta aurrekontuaren lerroaren xehetasunetan agertzen den zerga-zenbatekoaren arabera laburbiltzen da. | Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da. |
| Eskainitako zenbatekoa, zergaren ondoren | Eremu hau zerga ondorengo aurrekontuaren zenbatekoa da eta irakurtzeko soilik da. Eremu honetako zenbatekoa honela kalkulatzen da *Aipatutako zenbatekoa + Zerga*. | Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da. |
| Ez gainditzeko muga | Eremu hau editagarria da eta proiektu bat duten aurrekontu lerroetan soilik dago erabilgarri **Denbora eta materiala** fakturazio metodoa. | Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da. |
| Bezeroaren aurrekontua | Eremu hau editagarria da eta balio hori aukera-lerroan dagokion eremutik kopiatzen da, abagunea eskaintza batetik sorten bada. | Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da. |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a>Proiektuetan oinarritutako aurrekontu lerroen Orokorra fitxako eremuen baliozkotze arauak

**1. araua**: **Zereginak barne** eremua hutsik badago, edo ezarrita badago **Proiektuaren zeregin guztiak**, proiektu bat aurrekontuaren lerroan sartzen da.

**2. araua**: **Zereginak barne** eremua hutsik badago, edo ezarrita badago **Proiektuaren zeregin guztiak**, proiektu bat eta transakzio klase jakin bat aurrekontuaren proiektuan oinarritutako aurrekontu lerro batean bakarrik sar daitezke.

**3. araua**: **Zereginak barne** eremua **Hautatutako proiektuaren zereginak soilik** gisa ezarrita badago, proiektu bat eta transakzio klase jakin bat aurrekontuaren proiektuan oinarritutako aurrekontuan sar daitezke.

**4. araua**: Aukera batek aurrekontu ugari baditu, aurrekontu desberdinetako aurrekontu lerroak egon daitezke, proiektu bera aipatzen dutenak eta transakzio klase bera barne hartzen dutenak.

**5. araua**: Aurrekontuak aukera berekoak ez badira, ezin dute proiektu eta transakzio klase bera sartu.

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="59" valign="top">
                <p>
                    <strong>Abagunea</strong>
                </p>
            </td>
            <td width="39" valign="top">
                <p>
                    <strong>Eskaintza</strong>
                </p>
            </td>
            <td width="40" valign="top">
                <p>
                    <strong>Eskaintzaren lerroa</strong>
                </p>
            </td>
            <td width="41" valign="top">
                <p>
                    <strong>Project</strong>
                </p>
            </td>
            <td width="77" valign="top">
                <p>
                    <strong>Gehitutako zereginak</strong>
                </p>
            </td>
            <td width="45" valign="top">
                <p>
                    <strong>Idatzi denbora</strong>
                </p>
            </td>
            <td width="46" valign="top">
                <p>
                    <strong>Idatzi gastua</strong>
                </p>
            </td>
            <td width="43" valign="top">
                <p>
                    <strong>Sartu materiala</strong>
                </p>
            </td>
            <td width="41" valign="top">
                <p>
                    <strong>Gehitu</strong>
                </p>
                <p>
                    <strong>Tasa</strong>
                </p>
            </td>
            <td width="49" valign="top">
                <p>
                    <strong>Baliozkoa/Baliogabea da</strong>
                </p>
            </td>
            <td width="200" valign="top">
                <p>
                    <strong>Arrazoia</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
1H </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
A1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="45" valign="top">
                <p>
Yes </p>
            </td>
            <td width="46" valign="top">
                <p>
Yes </p>
            </td>
            <td width="43" valign="top">
                <p>
Yes </p>
            </td>
            <td width="41" valign="top">
                <p>
Yes </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
Baliogabea da </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
2. araua haustea. P1 proiektuaren denbora, gastuak eta tasak aurrekontu lerroetan, QL1 eta QL2 barne daude </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
1H </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
A1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="45" valign="top">
                <p>
Yes </p>
            </td>
            <td width="46" valign="top">
                <p>
Yes </p>
            </td>
            <td width="43" valign="top">
                <p>
Yes </p>
            </td>
            <td width="41" valign="top">
                <p>
Yes </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
1H </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
A1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="45" valign="top">
                <p>
Yes </p>
            </td>
            <td width="46" valign="top">
                <p>
No </p>
            </td>
            <td width="43" valign="top">
                <p>
Yes </p>
            </td>
            <td width="41" valign="top">
                <p>
Yes </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
Baliogabea da </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
2. araua haustea. P1 proiektuaren denbora, materialak eta tasak aurrekontu lerroetan, QL1 eta QL2 barne daude </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
1H </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
A1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="45" valign="top">
                <p>
Yes </p>
            </td>
            <td width="46" valign="top">
                <p>
Yes </p>
            </td>
            <td width="43" valign="top">
                <p>
Yes </p>
            </td>
            <td width="41" valign="top">
                <p>
Yes </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
1H </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
A1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="45" valign="top">
                <p>
Yes </p>
            </td>
            <td width="46" valign="top">
                <p>
No </p>
            </td>
            <td width="43" valign="top">
                <p>
Yes </p>
            </td>
            <td width="41" valign="top">
                <p>
Yes </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
Baliozkoa </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
P1 proiektuaren denbora, materialak eta tasak QL1 barne daude <br>
P1 proiektuaren gastuak QL2n sartzen dira <br>
Aurrekontu lerro bakoitzean sartzen denaren gainetik ez dago gainjartzerik eta, beraz, baliozkoa da.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
1H </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
A1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="45" valign="top">
                <p>
No </p>
            </td>
            <td width="46" valign="top">
                <p>
Yes </p>
            </td>
            <td width="43" valign="top">
                <p>
No </p>
            </td>
            <td width="41" valign="top">
                <p>
No </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
1H </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
A1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Hautatutako zereginak soilik </p>
            </td>
            <td width="45" valign="top">
                <p>
Yes </p>
            </td>
            <td width="46" valign="top">
                <p>
Yes </p>
            </td>
            <td width="43" valign="top">
                <p>
Yes </p>
            </td>
            <td width="41" valign="top">
                <p>
Yes </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
Baliogabea da </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
2. araua haustea </p>
                <p>
P1 proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, materiala, gastuak eta tasak sartzen dira </p>
                <p>
QL2-k P1 proiektu osorako denbora, gastuak eta tasak biltzen ditu eta, beraz, Q1-en sartutakoarekin gainjartzen da.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
1H </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
A1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="45" valign="top">
                <p>
Yes </p>
            </td>
            <td width="46" valign="top">
                <p>
Yes </p>
            </td>
            <td width="43" valign="top">
                <p>
Yes </p>
            </td>
            <td width="41" valign="top">
                <p>
Yes </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
1H </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
A1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Hautatutako zereginak soilik </p>
            </td>
            <td width="45" valign="top">
                <p>
Yes </p>
            </td>
            <td width="46" valign="top">
                <p>
Yes </p>
            </td>
            <td width="43" valign="top">
                <p>
Yes </p>
            </td>
            <td width="41" valign="top">
                <p>
Yes </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
Baliozkoa </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
3. arauaren arabera, </p>
                <p>
P1 proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, materiala, gastuak eta tasak sartzen dira.
                </p>
                <p>
QL2k proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, materiala, gastuak eta tasak sartzen dira.
                </p>
                <p>
Balidazio osagarri bakarra QL1-eko zereginen azpimultzoaren inguruan kokatzen da, QL2-ren zereginen azpimultzoaren desberdina dela gainjartzerik ez dagoela ziurtatzeko. Sistemak zereginak lotzen dituenean egiten du.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
1H </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
A1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Hautatutako zereginak soilik </p>
            </td>
            <td width="45" valign="top">
                <p>
Yes </p>
            </td>
            <td width="46" valign="top">
                <p>
Yes </p>
            </td>
            <td width="43" valign="top">
                <p>
Yes </p>
            </td>
            <td width="41" valign="top">
                <p>
Yes </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
1H </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
A1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Proiektuaren zeregin guztiak edo hutsik </p>
            </td>
            <td width="45" valign="top">
                <p>
Yes </p>
            </td>
            <td width="46" valign="top">
                <p>
Yes </p>
            </td>
            <td width="43" valign="top">
                <p>
Yes </p>
            </td>
            <td width="41" valign="top">
                <p>
Yes </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
Baliozkoa </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
5. arauaren arabera, Q1 eta Q2 aukera berdineko bi komatxo dira, beraz, biek proiektu baten osagai berberak kalkula ditzakete.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
2H </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
A1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Proiektuaren zeregin guztiak edo hutsik </p>
            </td>
            <td width="45" valign="top">
                <p>
Yes </p>
            </td>
            <td width="46" valign="top">
                <p>
Yes </p>
            </td>
            <td width="43" valign="top">
                <p>
Yes </p>
            </td>
            <td width="41" valign="top">
                <p>
Yes </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
1H </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
A1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Proiektuaren zeregin guztiak edo hutsik </p>
            </td>
            <td width="45" valign="top">
                <p>
Yes </p>
            </td>
            <td width="46" valign="top">
                <p>
Yes </p>
            </td>
            <td width="43" valign="top">
                <p>
Yes </p>
            </td>
            <td width="41" valign="top">
                <p>
Yes </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
Baliogabea da </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
4. arauaren arabera, Q1 eta Q2 aukera desberrdineko bi komatxo dira, beraz, biek proiektu berean osagai berberak kalkula ditzakete.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O2 </p>
            </td>
            <td width="39" valign="top">
                <p>
1H </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
A1 </p>
            </td>
            <td width="77" valign="top">
                <p>
Proiektuaren zeregin guztiak edo hutsik </p>
            </td>
            <td width="45" valign="top">
                <p>
Yes </p>
            </td>
            <td width="46" valign="top">
                <p>
Yes </p>
            </td>
            <td width="43" valign="top">
                <p>
Yes </p>
            </td>
            <td width="41" valign="top">
                <p>
Yes </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
