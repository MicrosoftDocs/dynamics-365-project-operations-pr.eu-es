---
title: Gastuak gailu mugikorrak erabiliz
description: Gai hori emateko informazioa buruz Gastuaren kudeaketaren mugikorreko laneko area.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 51da574143b91df636d99f91d37470905a9b0529
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4120888"
---
# <a name="expense-using-mobile"></a>Gastuak gailu mugikorrak erabiliz

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Gai hori emateko informazioa buruz **Gastuaren kudeaketaren** mugikorreko laneko area. Laneko espazio horri esker, erabiltzaileek ordainagiria harrapatu eta kargatu dezakete, gero gastu-txosten batera erantsi ahal izateko. Erabiltzaileek ere azkar sor dezakete gastu lerro bat erantsitako ordainagiria erabiliz eta beren gastuen txostenak sortu eta kudeatu ditzakete. Gainera, onartzaileek **Gastuen kudeaketa** mugikorreko lan eremua, esleitzen zaizkien gastuen txostenak ikusteko eta gastu-txosten horiek onartzeko edo baztertzeko.

Mugikorretarako lan-espazio hau Dynamics 365 Unified Ops mugikorretarako aplikazioarekin erabiltzeko pentsatuta dago.

Erakunde askok eskatzen dute ordainagiriaren kopia bat langileak itzultzeko aurkezten duen bidaiarekin lotutako edo negozioarekin lotutako gastuen txostenari eranstea. **Gastuen kudeaketa** mugikorreko lan-eremuak erabiltzaileei nahi duten gailu mugikorrean azkar sortzeko linea berriak sor ditzake ordainagiriaren erantsitako argazkia erabiliz. Bestela, erabiltzaileek ordainagiriaren argazkia har dezakete eta gero gastuen txostenean erantsi. Langileek beren gastuen txostenak sortu eta kudea ditzakete, eta, ondoren, onartu eta itzultzeko bidal ditzakete beren gailu mugikorra erabiliz.

Zehazki, **Gastuen kudeaketa** mugikorreko lan eremuak erabiltzaileei zeregin hauek burutzeko aukera ematen die:

- Egin ordainagiri baten argazkia. Kargatu ordainagiriaren argazkia eta erantsi geroago gastuen txostenean.
- Kargatu fitxategi bat harrapatutako ordainagiri gisa. Gero fitxategi hori erants dezakezu gastuen txostenean.
- Sortu gastu lerro berri bat erantsitako ordainagiria erabiliz. Ondoren, lerro-elementua gastu-txostenean gehi dezakezu eta onartu eta itzultzeko bidali.

Eginbide hauek ere erabil ditzakezu:

- Sortu gastuen txosten berri bat.
- Erantsi kreditu txartelarekin egindako eragiketak eta aurretik sortutako gainerako gastuak gastuen txostenean.
- Sortu gastu berrien gastuen txostena.
- Erantsi ordainagiria gastuen txostenaren edozein gasturi, ordainagiriaren argazkia aterata edo harrapatutako ordainagiri gisa fitxategi bat kargatuta.
- Enpresaren gastu politikaren arabera, gehitu gonbidatuen zerrenda gastu bati.
- Enpresaren gastu politikaren arabera, banatu gastuak.
- Bidali gastu txostena onartzeko eta itzultzeko.
- Onartu edo ukatu esleitutako onartzailea zaren gastuen txostenak.

## <a name="prerequisites"></a>Aurrebaldintzak
Aurrebaldintzak desberdinak dira, zure erakundean inplementatu den bertsioaren arabera.

### <a name="prerequisites-if-you-use-dynamics-365-finance"></a>Erabiliz gero aurrebaldintzak Dynamics 365 Finance 
Finantzak zure erakundean hedatu badira, sistemaren administratzaileak argitaratu beharko du **Gastuen kudeaketa** mugikorreko lan eremua. 

### <a name="prerequisites-if-you-use-version-1611-with-platform-update-3-or-later"></a>Aurrebaldintzak 1611 bertsioa plataformako 3. eguneratzearekin edo berriagoarekin erabiltzen baduzu
Plataformaren 3. eguneratzearekin edo berriagoarekin 1611 bertsioa zure erakundean hedatu bada, sistemaren administratzaileak honako baldintza hauek bete beharko ditu. 

<table>
<thead>
<tr class="header">
<th>Aurrebaldintza</th>
<th>Funtzioa</th>
<th>Deskribapena</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Ezarri KB 4019015.</td>
<td>Sistemaren administratzailea</td>
<td>KB 4019015 fitxategia duen X ++ eguneratze edo metadatuen zuzenketa zuzena da <strong>Gastuen kudeaketa</strong> mugikorreko lan eremua. KB 4019015 ezartzeko, zure sistemaren administratzaileak urrats hauek jarraitu behar ditu.
<ol>
<li><a href="https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/migration-upgrade/download-hotfix-lcs">Deskargatu Lifecycle Services zerbitzuko eguneratzeak</a>.</li>
<li><a href="https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/migration-upgrade/install-metadata-hotfix-package">Instalatu metadatuen zuzenketa zuzena</a>.</li>
<li><a href="https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/create-apply-deployable-package">Sortu pakete inplementagarri bat</a> horrek dauka <strong>ApplicationSuite</strong> eta <strong>ExpenseMobile</strong> modeloak eta, ondoren, pakete inplementagarria LCS-ra igo.</li>
<li><a href="https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/apply-deployable-package-system">Aplikatu pakete inplementagarria</a>.</li>
</ol></td>
</tr>
<tr class="even">
<td>Argitaratu <strong>Gastuen kudeaketa</strong> mugikorreko lan eremua.</td>
<td>Sistemaren administratzailea</td>
<td>Ikusi <a href="https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/mobile-apps/publish-mobile-workspace">Argitaratu mugikorreko lan eremua</a>.</td>
</tr>
</tbody>
</table>

## <a name="download-and-install-the-dynamics-365-unified-ops-mobile-app"></a>Deskargatu eta instalatu Dynamics 365 Unified Ops mugikorretarako aplikazioa
Deskargatu eta instalatu Dynamics 365 Unified Ops mugikorretarako aplikazioa:

- [Hurrengorako Android telefonoak](https://go.microsoft.com/fwlink/?linkid=850662)
- [iPhone-tarako](https://go.microsoft.com/fwlink/?linkid=850663)

## <a name="sign-in-to-the-mobile-app"></a>Saio hasi mugikorreko aplikazioa
1. Hasi aplikazioa zure mugikorreko gailuan.
2. Idatzi zure Dynamics 365 URL.
4. Saioa hasten duzun lehen aldian, zure erabiltzaile izena eta pasahitza eskatuko zaizu. Idatzi kredentzialak.
5. Saioa hasi ondoren, zure enpresarako erabilgarri dauden lan-eremuak agertzen dira. Zure sistemaren administratzaileak gero laneko espazio berri bat argitaratzen badu, mugikorretarako laneko espazioak berritu beharko dituzula.

## <a name="capture-a-receipt-by-using-the-expense-management-mobile-workspace"></a>Hartu ordainagiria Gastuak kudeatzeko mugikorreko lan eremua erabiliz

1. Zure gailu mugikorrean, ireki **Gastuen kudeaketa** lan eremua.
2. Aukeratu **Hartu ordainagiria**.
3. Aukeratu **Egin argazkia** edo **Aukeratu irudia**.
4. Jarraitu urrats hauetako bat:

   - **Egin argazkia** hautatu baduzu, jarraitu urrats hauei:

      1. Zure gailu mugikorreko kamerara eramaten zaituzte, ordainagiriaren argazkia atera ahal izateko. 
      2. Argazkia ateratzen amaitutakoan, hautatu **Ados** argazkia onartzeko.
      3. Aukerakoa: idatzi argazkiaren izena eta idatzi oharrak.

    - **Aukeratu irudia** hautatu baduzu, jarraitu urrats hauei:

        1. Hautatu irudi bat zerrendan.
        2. Aukerakoa: idatzi irudiaren izena eta idatzi oharrak.

5. Hautatu **Eginda**.

## <a name="quickly-enter-expenses-by-using-the-expense-management-mobile-workspace"></a>Sartu bizkor gastuetan Gastuak kudeatzeko mugikorreko lan eremua erabiliz

1. Zure gailu mugikorrean, ireki **Gastuen kudeaketa** lan eremua.
2. Aukeratu **Gastuen sarrera azkarra**.
3. Aukeratu gastuen kategoria. Lineaz kanpo erabiltzeko aplikazioan kargatutako gastuen kategoriaren zerrenda bat ikusiko duzu. Berez, 50 elementu kargatzen dira, baina garatzaile batek zenbaki hori alda dezake. Informazio gehiagorako, garaitzaileek [Mugikorreko plataforma](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/mobile-apps/platform/mobile-platform-getting-started) ikusi behar dute. Zure kategoria zerrendan ez badago, hautatu **Bilatu** sareko bilaketa bat egiteko. Bilatu gastuen kategorien arabera edo aldatu bilaketa gastu motaren arabera.
4. Idatzi gastuaren transakzio data.
5. Aukerakoa: sartu merkataria gastuaren truke.
6. Idatzi gastuaren zenbatekoa.
7. Hautatu gastuaren moneta. Lineaz kanpo erabiltzeko aplikazioan kargatutako moneta-kodeen zerrenda bat ikusiko duzu. Berez, 400 moneta kargatzen dira, baina garatzaile batek zenbaki hori alda dezake. Informazio gehiagorako, garaitzaileek [Mugikorreko plataforma](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/mobile-apps/platform/mobile-platform-getting-started) ikusi behar dute. Zure moneta zerrendan ez badago, hautatu **Bilatu** sareko bilaketa bat egiteko. Bilatu moneten arabera edo aldatu bilaketa izenaren arabera.
8. Aukeratu **Egin argazkia** edo **Aukeratu irudia**.
9. Jarraitu urrats hauetako bat:

    - **Atera argazkia** hautatu baduzu, zure gailu mugikorreko kamerara eramaten zaituzte, ordainagiriaren argazkia atera ahal izateko. Argazkia ateratzen amaitutakoan, hautatu **Ados** argazkia onartzeko.
    - Aukeratu baduzu **Aukeratu irudia**, hautatu zerrendako irudi bat.

10. Hautatu **Eginda**.

## <a name="approve-an-expense-report-by-using-the-expense-management-mobile-workspace-if-you-use-the-july-2017-update"></a>Onartu gastuen txostena Gastuak kudeatzeko mugikorreko lan eremua erabiliz (2017ko uztaileko eguneratzea erabiltzen baduzu)

1. Zure gailu mugikorrean, ireki **Gastuen kudeaketa** lan eremua.
2. **Gastuen onarpenak** onarpenerako esleitzen zaizkizun gastuen txostenak erakusten ditu. Zenbakia 30 minuturo eguneratzen da gutxi gorabehera. Aukeratu **Gastuen onarpenak**.

    Onartzeko esleitu zaizkizun gastuen txostenen zerrenda bistaratzen da.
    
3. Aukeratu gastuen txostena, horren gastuen xehetasunak ikusteko.
4. Aukeratu gastu bat, horren xehetasunak ikusteko. Gastuetarako erakusten den informazioa ordainagiriak, gonbidatuak eta banaketa xehetasunak biltzen ditu.
5. Itzuli **Gastuen txostena** orrian, hautatu gastu-txostena onartzeko edo ukatzeko.
6. Sartu iruzkinak onarpen ekintzarako.
7. Hautatu **Eginda**.

## <a name="create-a-new-expense-report-and-submit-it-for-approval-by-using-the-expense-management-mobile-workspace-if-you-use-the-july-2017-update"></a>Sortu gastuen txosten bat eta bidali onartzeko, Gastuak kudeatzeko mugikorreko lan eremua erabiliz (2017ko uztaileko eguneratzea erabiltzen baduzu)

1. Zure gailu mugikorrean, ireki **Gastuen kudeaketa** lan eremua.
2. Aukeratu **Gastuen sarrera**.
3. Aukeratu **Txosten berria** edo hautatu zerrendan dagoen gastuen txostena.
4. Gastu berrien txostenetarako, sartu helburua eta eskuragarri dagoen informazio osagarria. Informazio hori aldatu egiten da, gastuak kudeatzeko zure enpresarako konfiguratuta dagoen moduaren arabera.
5. Hautatu **Eginda**.
6. Lehendik dauden gastuak, hala nola kreditu txartelarekin egindako transakzioak, gastuen txostenean gehitzeko, hautatu **Erantsi**.
7. Hautatu gastu bat edo gehiago zerrendan.
8. Hautatu **Eginda**.
9. Gastu txostenean gastu berri bat gehitzeko, hautatu **Gastu berria**.
10. Aukeratu gastuaren kategoria. Lineaz kanpo erabiltzeko aplikazioan kargatutako gastuen kategoriaren zerrenda bat ikusiko duzu. Berez, 50 elementu kargatzen dira, baina garatzaile batek zenbaki hori alda dezake. Informazio gehiagorako, garaitzaileek [Mugikorreko plataforma](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/mobile-apps/platform/mobile-platform-getting-started) ikusi behar dute. Zure kategoria zerrendan ez badago, hautatu **Bilatu** sareko bilaketa bat egiteko. Bilatu gastuen kategorien arabera edo aldatu bilaketa gastu motaren arabera.
11. Aukerakoa: sartu merkataria gastuaren truke.
12. Idatzi gastuaren transakzio data.
13. Idatzi gastuaren zenbatekoa.
14. Hautatu gastuaren moneta. Lineaz kanpo erabiltzeko aplikazioan kargatutako moneta-kodeen zerrenda bat ikusiko duzu. Berez, 400 moneta kargatzen dira, baina garatzaile batek zenbaki hori alda dezake. Informazio gehiagorako, garaitzaileek [Mugikorreko plataforma](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/mobile-apps/platform/mobile-platform-getting-started) ikusi behar dute. Zure moneta zerrendan ez badago, hautatu **Bilatu** sareko bilaketa bat egiteko. Bilatu moneten arabera edo aldatu bilaketa izenaren arabera.
15. Hautatu **Eginda**.
16. Gastuari xehetasun gehiago emateko, hautatu **Gehitu xehetasun gehiago**. Eskuragarri dauden eremuak zure enpresako gastuen kudeaketaren konfigurazioaren araberakoak dira.
17. Enpresaren gidalerroak gastuaren ordainagiria eskatzen badu, hautatu **Ordainagiriak**, eta jarraitu urrats hauei:

    1. Aukeratu **Hartu ordainagiria** edo **Erantsi ordainagiria**.
    2. Jarraitu urrats hauetako bat:

        - **Kapturatu ordainagiria** hautatu baduzu, jarraitu urrats hauei:

            1. Aukeratu **Egin argazkia** edo **Aukeratu irudia**.
            2. Jarraitu urrats hauetako bat:

                - **Egin argazkia** hautatu baduzu, jarraitu urrats hauei:

                    1. Zure gailu mugikorreko kamerara eramaten zaituzte, ordainagiriaren argazkia atera ahal izateko. Argazkia ateratzen amaitutakoan, hautatu **Ados** argazkia onartzeko.
                    2. Aukerakoa: idatzi argazkiaren izena eta idatzi oharrak.

                - **Aukeratu irudia** hautatu baduzu, jarraitu urrats hauei:

                    1. Hautatu irudi bat zerrendan.
                    2. Aukerakoa: idatzi irudiaren izena eta idatzi oharrak.

            3.  Hautatu **Eginda**.

        - **Erantsi ordainagiria** hautatu baduzu, jarraitu urrats hauei:

            1.  Hautatu irudi bat edo gehiago zerrendan.
            2.  Hautatu **Eginda**.

    3. Aukeratu **Itzuli** botoia gastuaren xehetasunetara itzultzeko.

18. Enpresaren gidalerroak gastuaren gonbidatuak eskatzen badu, hautatu **Gonbidatuak**, eta jarraitu urrats hauei:

    1. Aukeratu **Gonbidatua**, **Aurreko gonbidatuak**, edo **Lankideak**.
    2. Jarraitu urrats hauetako bat:

        - **Gonbidatua** hautatu baduzu, jarraitu urrats hauei:

            1. Sartu gonbidatuaren izena.
            2. Aukerakoa: sartu gonbidatuaren erakundea eta / edo herrialdea.
            3. Aukerakoa: Sartu gonbidatuaren izenburua.
            4. Hautatu **Eginda**.

        - **Aurreko gonbidatuak** hautatu baduzu, jarraitu urrats hauei:

            1. Hautatu aurreko gonbidatu bat edo gehiago zerrendan. Konexiorik gabe erabiltzeko zure aplikazioan kargatutako aurreko gastuen txostenetan gehitu dituzun aurreko gonbidatuen zerrenda ikusiko duzu. Berez, 50 elementu kargatzen dira, baina garatzaile batek zenbaki hori alda dezake. Informazio gehiagorako, garaitzaileek [Mugikorreko plataforma](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/mobile-apps/platform/mobile-platform-getting-started) ikusi behar dute. Zure aurreko gonbidatua zerrendan ez badago, hautatu **Bilatu** sareko bilaketa bat egiteko. Bilatu izenaren arabera edo aldatu erakundearen, herrialdearen edo izenburuaren arabera.
            2. Hautatu **Eginda**.

        - **Lankideak** hautatu baduzu, jarraitu urrats hauei:

            1. Hautatu lankide bat edo gehiago zerrendan. Lineaz kanpo erabiltzeko aplikazioan kargatutako lankideen zerrenda bat ikusiko duzu. Berez, 50 elementu kargatzen dira, baina garatzaile batek zenbaki hori alda dezake. Informazio gehiagorako, garaitzaileek [Mugikorreko plataforma](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/mobile-apps/platform/mobile-platform-getting-started) ikusi behar dute. Zure lankide-zerrendan ez badago, hautatu **Bilatu** sareko bilaketa bat egiteko. Bilatu izenaren arabera edo aldatu enpresaren edo izenburuaren arabera.
            2. Hautatu **Eginda**.

    3. Aukeratu **Itzuli** botoia gastuaren xehetasunetara itzultzeko.

19. Enpresaren gidalerroak gastua elementu egitea eskatzen badu, hautatu **Bihurtu elementu**, eta jarraitu urrats hauei:

    1. Hautatu zehaztu nahi duzun lehen data.
    2. Aukeratu **Gehitu itemizazioa**.
    3. Hautatu gastuen elementu egitearen azpikategoria. Lineaz kanpo erabiltzeko aplikazioan kargatutako gastuen azpikategoriaren zerrenda bat ikusiko duzu. Berez, 50 elementu kargatzen dira, baina garatzaile batek zenbaki hori alda dezake. Informazio gehiagorako, garaitzaileek [Mugikorreko plataforma](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/mobile-apps/platform/mobile-platform-getting-started) ikusi behar dute. Zure azpikategoria zerrendan ez badago, hautatu **Bilatu** sareko bilaketa bat egiteko. Bilatu gastuen azpikategoria izenaren arabera.
    4. Idatzi transakzioaren zenbatekoa zehazteko.
    5. Editatu transakzioaren data beharrezkoa bada.
    6. Hautatu **Eginda**.
    7. Errepikatu aurreko pausoak hautatutako datarako elementu guztiak gehitzen amaitu arte.
    8. Egun osagarrietarako, hauta dezakezu **Kopiatu hurrengo egunera** artikuluak hurrengo egunera kopiatzeko. Bestela, zehaztu nahi duzun data hauta dezakezu eta ondoren elementuak gehitu ditzakezu lehen egunean bezala.
    9. Gastua zehazten amaitu ondoren, hautatu **Itzuli** botoia gastuaren xehetasunetara itzultzeko.

20. Aukeratu **Itzuli** botoia **Gastuaren txostena** orrira itzultzeko.
21. Errepikatu aurreko urratsak gastu guztiak gehitzen amaitu arte.
22. Hautatu **Bidali**.
23. Sartu onartzailearentzako iruzkinak.
24. Hautatu **Eginda**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]