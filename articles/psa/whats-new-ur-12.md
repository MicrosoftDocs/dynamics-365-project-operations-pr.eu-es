---
title: Project Service Automation eguneratzearen 12, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation eguneratzea 12, V3 bertsioko berritasunei buruzko informazioa ematen du.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
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
ms.openlocfilehash: 62c3a0c5cfbecb568faef570da309c20afd86de9
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070997"
---
# <a name="project-service-automation-update-release-12-v3"></a>Project Service Automation 12, V3 eguneratze-bertsioa
Atsegin handiz adierazten dugu Dynamics 365 Project Service Automation (PSA) aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroa eta joan soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

Gai honek Project Service Automation V3, 12. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honek V3.10.2.34 konpilazio-zenbakia du eta, oro har, 2019ko urrian jarriko da erabilgarri automatikoki eguneratzeko moduan.

## <a name="update-release-12"></a>12. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

- Denbora eta gastua

    - Konponduta: Denbora-sarreraren errore-mezularitza eguneratu egin da testuinguru adierazgarriagoarekin.
    - Konponduta: Denbora-sarreraren sareta eta antolaketa ongi bistaratzen da korritze-barra bertikalean, eskatzean.
    - Konponduta: Bidalitako gastua eta denbora-sarrerak onar daitezke.
    - Konponduta: Utzi onespenaren berrespenaren elkarrizketa-mezua zuzendu da onespenaren egoera islatzeko **Onartuta** egoeratik **Bidalita** egoerara.
    - Konponduta: **Prezioa** , **Unitatea** eta **Kopurua** eremuak blokeatuta daude Gastuen erregistroan, onartu ondoren.

- Proiektuen kudeaketa

    - Konponduta: **Berria** ekintza **Taldekidea** inprimaki nagusitik kendu da.
    - Konponduta: Baliabideen esleipenak eguneratu egin dira kontura zehatzak ez diren sarrera-erroreengatik, eta horrek zereginen amaiera-data aldatzea eragin du.
    - Konponduta: Zereginen sarean, zerbitzariaren aldeko akatsak agertuko zaizkio erabiltzaileari.
    - Konponduta: Taldekidearen izenak zereginen pertsonen hautatzailean errendatzen da posizioaren izena beharrean.

- Baliabideen kudeaketa

    - Konponduta: Txantiloi batetik sortutako proiektuaren baliabide-eskakizunen xehetasunek proiektuaren egutegia erabiltzen dute orain.
    - Konponduta: Trebetasunak eta gaitasunak lehenetsi egiten dira funtzio nagusitik funtzio horretarako sortutako baliabide-eskakizunera.

- Sales

    - Konponduta: Objektuen ID bikoiztuak aurkitu dira **Kontratu nagusia** inprimakian.
    - Konponduta: Logika eguneratu egin da **Eskaintzaren azterketa** fitxa ikusgai egiteko, fitxaren metadatuen konfigurazioa bistara dadin.
    - Konponduta: Egiazko erregistroan kontabilitate-data denboraren/gastuen sarrera-datatik dator eta ez onespen-datatik.