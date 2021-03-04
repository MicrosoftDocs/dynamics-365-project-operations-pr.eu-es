---
title: Project Service Automation-en datu-ereduarekin lan egitea
description: Gai honek datu-ereduarekin lana egiteko moduari buruzko informazioa ematen du.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: d8c212ef2c9fd9dcd6be0b8f0a31aa5a948176bc
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5147638"
---
# <a name="working-with-the-project-service-automation-data-model"></a>Project Service Automation-en datu-ereduarekin lan egitea

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]
[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Dynamics 365 Project Service Automation aplikazioak beste aplikazio entitate batzuk hedatzen ditu eta erakunde propioak sartzen ditu Common Data Service-ren datu-ereduan. Gai honek PSA-ren txostenen egoera tipikoetan topatuko dituzun zenbait entitate deskribatzen ditu.

## <a name="reporting-on-opportunities"></a>Abaguneen txostenak

Project Service Automation-ek Dynamics 365 Sales-eko **Abagunea** entitatea hedatzen du proiektuan oinarritutako egoerak ahalbidetzen dituzten eremuak gehituz. Eremu hauek **msdyn \_** aurrizkida duten eskema-izenarekin identifikatzen dira. PSA-ko abaguneen berri emateko garrantzitsua den eremu berri bat da **Eskaera mota**. Eremu horretarako **Lanean oinarrituta** balioak abagunea PSA abagunea dela adierazten du. Hauek dira erakundeari gehitu zaizkion beste eremu batzuk: **Kontratatu erakundea**, abaguneari eusten dion erakundea harrapatzen duena, eta **Kontu-kudeatzailea**, abagunearen erantzulea den kontu-kudeatzailearen izena biltzen duena.

**Abagunearen lerroa** entitateak Project Service-ri lotutako eremuak ere biltzen ditu. **Fakturazio metodoa** aukerak adierazten du abagunearen lerroa denbora eta materialaren edo prezio finkoaren arabera fakturatu behar ote den, eta **Proiektua** aukerak abagunea babesten ari den proiektuaren izena jasotzen du. Txostena egiteko erabil ditzakezun beste eremu batzuk lerroko elementuen kostuak eta bezeroaren aurrekontuaren zenbatekoa harrapatzen dituzte.

## <a name="reporting-on-quotes"></a>Eskaintzaren txostena

PSA-k Sales-en **Eskaintza** entitatea hedatzen du proiektuarekin lotutako eremuak gehituz. **Eskaera mota** aukerak PSA-ren eskaintzak PSA-koak ez diren eskaintzetatik bereizten ditu. Eremu horretarako **Lanean oinarrituta** balioak eskaintza PSA-ko eskaintza dela adierazten du. PSA-ren eskaintzan berri emateko garrantzitsuak izan daitezkeen beste eremu batzuen artean zenbatekoak daude, besteak beste, **Kobratu daitezkeen kostuak**, **Kobratu ezin daitezkeen kostuak**, **Marjina gordina**, **Aurreikuspenak** eta **Aurrekontua**. Beste eremu erabilgarri batzuek adierazten dute eskaintza errentagarria den ala ez, antolaketan osatuko den ala ez eta bezeroaren aurrekontuen itxaropenak betetzen dituen ala ez.

PSA-k Sales-en **Eskaintzaren lerroa** erakundea ere hedatzen du. PSA-k gehitzen duen eremua bat **Fakturazio metodoa** da, eskaintzaren lerroa nola fakturatuko den adierazten duena (denbora eta materialak edo prezio finkoa). Entitatera gehitu diren beste eremu batzuek eskaintzaren lerroa, fakturazioa, kostua eta aurrekontua babesten dituen proiektu bat harrapatzen dute.

PSA-k eskaintzari lotutako entitate berriak ere gehitu ditu Dynamics 365-eko datu-ereduan. Hona hemen zenbait adibideak:

- **Eskaintzaren lerroaren xehetasunak** - Entitate honek eskaintzaren lerroko proiektuaren aurreikuspenen xehetasunak ditu. Eskaintzaren lerro bakoitzeko bi erregistro ditu. Erregistro batek eskaintzaren lerroaren kostua eta kostuaren xehetasunak gordetzen ditu, eta beste erregistroak eskaintzaren lerroko salmenten zenbatekoa eta salmenta xehetasunak gordetzen ditu.
- **Eskaintzaren lerro fakturazio-antolaketa** - Entitate honek eskaintzaren lerroaren fakturazio egutegia dauka. Antolaketa hori eskaintzaren lerroari esleitzen zaion fakturazio-maiztasunaren arabera sortzen da.
- **Eskaintzaren lerroko mugarria** - Entitate honek prezio finkoko eskaintzaren lerroen fakturazio-mugarriak ditu.
- **Eskaintzaren lerroko analisiaren xehapena** - Entitate honek eskaintzaren lerroko finantzaren xehetasunak ditu. Xehetasun horiek erabilgarriak izan daitezke eskainitako salmenten eta aurreikusitako kostuen zenbatekoen berri emateko hainbat neurriren arabera.

PSA-k eskaintzei gehitzen dien beste erakundeak **Eskaintzaren lerroko proiektuen prezio-zerrenda**, **Eskaintzaren lerroko baliabideen kategoria** eta **Eskaintzaren lerroko transakzio kategoria** dira.

![Aurrekontua, aurrekontuaren lerroa eta proiektuaren erlazioak erakusten dituen diagrama](media/PS-Reporting-image2.png "Aurrekontua, aurrekontuaren lerroa eta proiektuaren erlazioak erakusten dituen diagrama")

## <a name="reporting-on-project-contracts"></a>Proiektu-kontratuen txostena

PSA-k Sales-en **Eskaera** entitatea hedatzen du, proiektu-kontratuak erregistratzen direnean erabiltzen den entitatea. Beste eremu garrantzitsu bat gehitzen du, **Eskaera mota**, kontratua PSA proiektu-kontratu gisa identifikatzen duena salmenta eskaeraren ordez. Eremu horretarako **Lanean oinarrituta** balioak eskaera PSA-ko proiektu-kontratua dela adierazten du. **Eskaera** entitatera gehitzen diren beste eremu batzuk kostuei, PSA-ko kontratuaren egoerari eta kontratuaren jabe den erakundearen xehetasunak ateratzen dituzte.

PSA-k Sales-en **Salmenta-eskaeraren lerroak** erakundea ere hedatzen du. Gehitzen dituen eremuen artean, fakturazio metodoa (denbora eta materialak edo prezio finkoa), bezeroaren aurrekontuaren zenbatekoak eta azpian dagoen proiektua biltzen dituzten eremuak daude.

PSA-k proiektu-kontratuetarako diseinatuta dauden beste entitate batzuk ere gehitu ditu. Hona hemen zenbait adibideak:

- **Proiektu-kontratuaren lerroko xehetasunak** - Entitate honek kontratuaren lerroaren zenbatekora biribiltzen diren lerro-mailako xehetasunak ditu. Zereginen mailan proiektuaren antolaketa batetik sortzen diren lerroko elementuak bezain zehatzak izan daitezke.
- **Kontratuaren lerroaren fakturazio-antolaketa** - Entitate honek kontratuaren lerroari esleitzen zaion faktura maiztasunaren arabera sortzen den fakturazio antolaketa dauka.
- **Kontratuaren mugarriak** - Entitate honek prezio finkoko fakturaziorako epea duten kontratuaren lerroen mugarriak ditu.

PSA-k kontratuei gehitzen dien beste erakundeak **Eskaintzaren lerroko proiektuen prezio-zerrenda**, **Proiektu-kontratuaren lerroko baliabide-kategoria** eta **Proiektu-kontratuaren lerroko transakzio-kategoria** dira.

![Eskaera, eskaera lerroa eta proiektuaren erlazioak erakusten dituen diagrama](media/PS-Reporting-image3.png "Eskaera, eskaera lerroa eta proiektuaren erlazioak erakusten dituen diagrama")

## <a name="reporting-on-projects"></a>Proiektuen txostena

**Proiektuak** entitatea eta lotutako erakundeak PSA-rako esklusiboak dira. **Proiektua** eragiketen lana eta kostua bereganatzeko erabiltzen den goi-mailako entitatea da. Hona hemen lotutako erakundeen zerrenda:

- **Proiektu-taldeko kidea** - Entitate honek proiektuari esleitzen zaizkion baliabide erreserbagarriei buruzko xehetasunak ditu. Baliabide hauek erreserbagarriak diren baliabide generikoak izan daitezke edo proiektu-kudeatzaileak sartutako edo proiektuaren antolaketatik sortutako erreserbagarriak diren baliabide izendatuak izan daitezke.
- **Proiektuaren zeregina** - Entitate honek proiektuaren plana edo antolaketa osatzen duten zereginak ditu.
- **Baliabideen esleipena** - Entitate honek erreserbagarria den baliabidearen zeregina dauka.
- **Baliabideen eskakizuna** - Entitate honek baliabide generikoen taldekideen eskakizunak ditu.
- **Aurreikuspena** eta **Aurreikuspenaren lerroa** - Entitate horiek goiburu/lerro harremana dute eta proiektuaren gastuen aurreikuspenak dituzte. Zereginen aurreikuspenak **Baliabideen estimazioa** erakundean gordetzen dira.

![Baliabide eskakizuna eta proiektuaren erlazioak erakusten dituen diagrama](media/PS-Reporting-image4.png "Baliabide eskakizuna eta proiektuaren erlazioak erakusten dituen diagrama")

## <a name="reporting-on-resources"></a>Baliabideen txostena

Proiektuko baliabideek beste aplikazio batzuekin partekatutako **Baliabide erreserbagarriak** erakundeak erabiltzen dituzte Universal Resource Scheduling (URS) aplikazioan, adibidez, Microsoft Dynamics 365 Field Service. Hona hemen proiektuaren baliabideen berri ematerakoan erabili beharko zenukeen entitateen zerrenda:

- **Baliabide erreserbagarria** - Entitate honek proiektu-taldean erabiltzen diren erabiltzailea, kontaktua, baliabide generikoa, kontua, taldea edo ekipamendua adierazten ditu.
- **Baliabide erreserbagarrien ezaugarriak** - Entitate honek baliabidearen trebetasunak, ziurtagiriak edo hezkuntza biltzen ditu. Ezaugarriek balorazio-ereduak zehaztutako puntuazio-balioak izan ditzakete.
- **Baliabide erreserbagarrien kategoria** - Entitate honek erreserbagarria den baliabidearen funtzioa adierazten du.
- **Baliabide erreserbagarrien erreserbak** - Entitate honek baliabideetarako proiektuetan erreserbatzen den denbora adierazten du. Erreserba bakoitzak goiburu entitateak eta lerroko entitateak ditu, eta lerro bakoitzak erreserbaren egoera adierazten duen egoera du.

![Erreserbatzeko baliabideen ezaugarri erlazioak erakusten dituen diagrama](media/PS-Reporting-image5.png "Erreserbatzeko baliabideen ezaugarri erlazioak erakusten dituen diagrama")

## <a name="reporting-on-actual-transactions"></a>Benetako trantsakzioen txostena

Ordutegi edo gastu bat onartzen duzunean edo kontratu bat PSA-n fakturatzen duzunean, negozio-transakzioa **Benetako datua** erakundean gordeko da. Entitate hori oinarria izan daiteke PSA-ko finantziazioarekin lotutako txosten guztietarako. **Benetako datua** entitateak negozioaren gertaeraren kostu eta salmenta transakzioak hartzen ditu. Hainbat atributu garrantzitsu ere biltzen ditu.

**Benetako datua** entitatearekin lan egiten duzunean, garrantzitsua da entitatean zer transakzio erregistratzen diren eta transakzioak noiz erregistratzen diren ulertzea. Hona hemen denborarekin lan egiten duzuneko ohiko sarrera bat (gastuen sarreren fluxua antzekoa da):

1. Denbora-sarrera gordetzen denean, ez da erregistrorik sortzen **Benetako datua** erakundean.
2. Denbora-sarrera bidaltzen denean, ez da erregistrorik sortzen **Benetako datua** erakundean.
3. Denbora-sarrera onartzen denean, erregistro bat sortzen da **Benetako datua** entitatean, eta bigarren erregistro bat ere sor daiteke. Lehen erregistroak denbora-sarreraren kostua gordetzen du. Bigarren erregistroak denbora-sarreraren fakturatu gabeko salmenta kopurua gordetzen du. Bigarren erregistroa proiektuarengangik independentea da, berdin da bezero bat, eskaintza bat edo kontratuaren lerro bat izan.

    | Dokumentuaren data | Transakzio mota | Transakzio-klasea | Bezeroa         | Kontratua   | Baliabidea     | Baliabide-funtzioa | Fakturazio mota | Kopurua | Unitate-prezioa | Zenbatekoa |
    |---------------|------------------|-------------------|------------------|------------|--------------|---------------|--------------|----------|------------|--------|
    | 2/3/18        | Kostua             | Time              | Alpine Ski House | Alpine CRM | Nerea Ibarrondo | Proiektu-kudeatzailea   | Kobra daiteke   | 8.0      | 50.00      | 400.00 |
    | 2/3/18        | Fakturatu gabeko salmentak   | Time              | Alpine Ski House | Alpine CRM | Nerea Ibarrondo | Proiektu-kudeatzailea   | Kobra daiteke   | 8.0      | 100.00     | 800.00 |

    Bi erregistro hauek bereizitako baina erlazionatutako erregistroak dira. Ez dira ez zorrak ezta kredituak ere.

4. Kontratua proiektuarekin erlazionatuta badago, denbora-sarrera fakturatzen denean, bi erregistro gehiago sortzen dira **Benetako datua** erakundean. Lehenik eta behin, fakturatu gabeko salmenten erregistrorako zenbateko negatiboa sortzen da. Erregistro horrek funtsean fakturatu gabeko salmenta alderantzikatzen du. Bigarren, fakturatutako salmentarako transakzio bat sortzen da. Berriro ere, erregistro hauek bereizitako baina erlazionatutako erregistroak dira, ez zorrak eta kredituak.

    | Dokumentuaren data | Transakzio mota | Transakzio-klasea | Bezeroa         | Kontratua   | Baliabidea     | Baliabide-funtzioa | Fakturazio mota | Kopurua | Unitate-prezioa | Zenbatekoa   |
    |---------------|------------------|-------------------|------------------|------------|--------------|---------------|--------------|----------|------------|----------|
    | 2/4/18        | Fakturatu gabeko salmentak   | Time              | Alpine Ski House | Alpine CRM | Nerea Ibarrondo | Proiektu-kudeatzailea   | Kobra daiteke   | - 8,0    | 100.00     | - 800,00 |
    | 2/4/18        | Fakturatutako salmentak     | Time              | Alpine Ski House | Alpine CRM | Nerea Ibarrondo | Proiektu-kudeatzailea   | Kobra daiteke   | 8.0      | 100.00     | 800.00   |

**Transakzioaren jatorria** entitateak **Benetako datua** erregistroaren jatorria erregistratzen du, eta **Transakzioaren konexioa** entitateak **Benetako datua** entitateak erlazionatutako erregistroak erregistratzen ditu. Gainera, **Benetako datua** erregistroak proiektuaren, proiektuaren kontratua (eskaera), baliabide erreserbagarria eta bezeroaren erreferentziak ditu.

![Transakzioen konexioa, jatorria eta benetako harremanak erakusten dituen diagrama](media/PS-Reporting-image6.png "Transakzioen konexioa, jatorria eta benetako harremanak erakusten dituen diagrama")


[!INCLUDE[footer-include](../includes/footer-banner.md)]