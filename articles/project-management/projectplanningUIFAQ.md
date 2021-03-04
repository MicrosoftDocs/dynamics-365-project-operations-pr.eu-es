---
title: Zeregina saretan lan egiteko arazoak konpontzea
description: Gai honek Atazen saretan lan egitean behar diren arazoak konpontzeko informazioa eskaintzen du.
author: ruhercul
manager: tfehr
ms.date: 01/19/2021
ms.topic: article
ms.product: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 89bbad62c2a0a5693a57cf5c9a812ab644486469
ms.sourcegitcommit: c9edb4fc3042d97cb1245be627841e0a984dbdea
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 01/19/2021
ms.locfileid: "5031522"
---
# <a name="troubleshoot-working-in-the-task-grid"></a>Zeregina saretan lan egiteko arazoak konpontzea 

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Gai honek kostuen kudeaketarekin lan egiterakoan topa ditzakezun arazoak nola konpondu deskribatzen ditu.

## <a name="enable-cookies"></a>Gaitu cookieak

Project Operations-ek hirugarrenen cookieak gaitzea eskatzen dute zereginen xehetasunen egitura bihurtzeko. Hirugarrenen cookieak gaituta ez daudenean, zereginak ikusi beharrean, orrialde huts bat ikusiko duzu **Zereginak** fitxan **Proiektua** orrialdean.

![Fitxa hutsa hirugarrenen cookieak gaituta ez daudenean](media/blankschedule.png)


### <a name="workaround"></a>Irtenbidea
Microsoft Edge edo Google Chrome arakatzaileetarako, honako prozedura hauek azaltzen dute nola eguneratu zure arakatzailearen ezarpena hirugarrenen cookieak gaitzeko.

#### <a name="microsoft-edge"></a>Microsoft Edge

1. Ireki Edge arakatzailea.
2. Goiko eskuineko ertzean, hautatu **hiru puntuak** (...), eta hautatu **Ezarpenak**.
3. **Cookieak eta gune baimenak** aukeran, hautatu **Cookieak eta webguneko datuak**.
4. Desaktibatu **Blokeatu hirugarrenen cookieak**.

#### <a name="google-chrome"></a>Google Chrome

1. Ireki Chrome arakatzailea.
2. Goiko eskuineko ertzean, hautatu hiru puntu bertikalak, eta hautatu **Ezarpenak**.
3. **Pribatutasuna eta segurtasuna** aukeran, hautatu **Cookieak eta webguneko beste datuak**.
4. Hautatu **Baimendu cookie guztiak**.

> [!IMPORTANT]
> Hirugarrenen cookieak blokeatzen badituzu, beste gune batzuetako cookieak eta webguneko datuak blokeatuko dira, nahiz eta gunea zure salbuespenen zerrendan onartzen den.

## <a name="pex-endpoint"></a>PEX amaiera-puntua

Project Operations-ek proiektuaren parametro batek PEX amaiera puntua erreferentzia izatea eskatzen du. Amaierako puntu hau lanaren matxura egitura emateko erabiltzen den zerbitzuarekin komunikatzeko beharrezkoa da. Parametroa gaituta ez badago, "Proiektuaren parametroak ez du balio" errorea jasoko duzu. 

### <a name="workaround"></a>Irtenbidea
 ![PEX amaiera-puntua eremua proiektuaren parametroan](media/projectparameter.png)

1. Gehitu **PEX amaiera puntua** eremua **Proiektuaren parametroak** orrialdean.
2. Eguneratu eremua balio honekin: `https://project.microsoft.com/<lang>/?org=<cdsServer>#/taskgrid?projectId=\<id>&type=2`
3. Kendu eremua **Proiektuaren parametroak** orrialdetik.

## <a name="privileges-for-project-for-the-web"></a>Webgunearen proiektuaren pribilegioak

Project Operations kanpoko planifikazio-zerbitzu batean oinarritzen da. Zerbitzuak eskatzen du erabiltzaile batek hainbat funtzio esleituta izatea lanaren banakako egiturarekin lotutako entitateei irakurtzeko eta idazteko. Entitate horien artean daude proiektuaren zereginak, baliabideen esleipenak eta atazen mendekotasunak. Erabiltzaile batek ezin badu zereginen xehetasunen egitura errendatu **Zereginak** fitxa, ziurrenik Project Operations-erako proiektua gaituta ez dagoelako izango da. Erabiltzaile batek segurtasun-funtzio errorea edo sarbidea ukatzearekin lotutako errorea jaso dezake.


## <a name="workaround"></a>Irtenbidea

1. Joan **Ezarpena > Segurtasuna > Erabiltzaileak > Aplikazioaren erabiltzaileak** aukerara.  

   ![Aplikazio-irakurgailua](media/applicationuser.jpg)
   
2. Egin klik bikoitza aplikazioaren erabiltzaile erregistroan hau egiaztatzeko:

 - Erabiltzaileak sarbidea du proiektuan. Egiaztapen hau normalean erabiltzaileak ziurtatzen du **Proiektu-kudeatzailea** segurtasun-funtzioa daukala.
 - Microsoft Project aplikazioaren erabiltzailea badago eta behar bezala konfiguratuta dago.
 
3. Erabiltzailea ez bada existitzen, erabiltzaile-erregistro bat sor dezakezu. Hautatu **Erabiltzaile berriak**. Aldatu sarrera-inprimakia **Aplikazioaren erabiltzailea** aukeran, eta gehitu **Aplikazioaren IDa**.

   ![Aplikazioaren erabiltzaile-xehetasunak](media/applicationuserdetails.jpg)

4. Egiaztatu erabiltzaileari lizentzia zuzena esleitu zaiola eta zerbitzua lizentziaren zerbitzu planen xehetasunetan gaituta dagoela.
5. Egiaztatu erabiltzaileak project.microsoft.com ireki dezakeela.
6. Egiaztatu proiektuaren parametroen bidez sistemak proiektuaren amaierako puntu zuzena adierazten duela.
7. Egiaztatu proiektuaren aplikazioaren erabiltzailea sortu dela.
8. Aplikatu segurtasun rol hauek erabiltzaileari:

  - Dataverse erabiltzailea
  - Project Operations sistema
  - Proiektuaren sistema

## <a name="error-when-updating-the-work-breakdown-structure"></a>Errorea lanaren matxura egitura eguneratzean

Lanaren banakako egiturari eguneratze bat edo gehiago egiten zaizkionean, azkenean aldaketak huts egiten dira eta ez dira gordetzen. Akats bat gertatu da programazio-saretan "Egindako azken aldaketa ezin izan dela gorde".

### <a name="workaround"></a>Irtenbidea

1. Egiaztatu erabiltzaileari lizentzia zuzena esleitu zaiola eta zerbitzua lizentziaren zerbitzu planen xehetasunetan gaituta dagoela.
2. Egiaztatu erabiltzaileak project.microsoft.com ireki dezakeela.
3. Egiaztatu sistemak proiektuaren amaierako puntu zuzena adierazten duela.
4. Egiaztatu Proiektuaren aplikazioaren erabiltzailea sortu dela.
5. Aplikatu segurtasun rol hauek erabiltzaileari:
  
  - Dataverse erabiltzailea edo Base erabiltzailea
  - Project Operations sistema
  - Proiektuaren sistema
  - Project Operations-en idazketa bikoitzeko sistema (funtzio hau beharrezkoa da Project Operations-en baliabidea/biltegiratu gabeko oinarritutako egoera hedatzen ari bazara.)


[!INCLUDE[footer-include](../includes/footer-banner.md)]