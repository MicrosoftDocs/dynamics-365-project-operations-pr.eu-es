---
title: Zeregina saretan lan egiteko arazoak konpontzea
description: Gai honek Atazen saretan lan egitean behar diren arazoak konpontzeko informazioa eskaintzen du.
author: ruhercul
ms.date: 09/22/2021
ms.topic: article
ms.product: ''
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 67136229d84a09886fffe9677b10f671aea3c393
ms.sourcegitcommit: 74a7e1c9c338fb8a4b0ad57c5560a88b6e02d0b2
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/23/2021
ms.locfileid: "7547184"
---
# <a name="troubleshoot-working-in-the-task-grid"></a>Zeregina saretan lan egiteko arazoak konpontzea 


_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egin, webgunerako proiektua_

Zereginen sareta Dynamics 365 Project Operations ostatatutako iframe barruan dago Microsoft Dataverse. Erabilera horren ondorioz, baldintza zehatzak bete behar dira autentifikazioak eta baimenak ondo funtzionatzen dutela ziurtatzeko. Gai honek sarearen errendatzeko edo zereginak kudeatzeko gaitasunean eragina izan dezaketen arazo arruntak azaltzen ditu lanaren banakako egituran (WBS).

Ohiko arazoak dira:

- **Egitekoa** fitxa sareko fitxa hutsik dago.
- Proiektua irekitzerakoan, proiektua ez da kargatzen eta erabiltzailearen interfazea (UI) biraka itsatsita dago.
- Pribilegioak administratzea **Project for the Web**.
- Aldaketak ez dira gordetzen ataza bat sortu, eguneratu edo ezabatzen duzunean.

## <a name="issue-the-task-tab-is-empty"></a>Arazoa: Ataza fitxa hutsik dago

### <a name="mitigation-1-enable-cookies"></a>1. arintzea: cookieak gaitu

Project Operations-ek eragiketek hirugarrenen cookieak gaitzea eskatzen dute lanaren banakako egitura bihurtzeko. Hirugarrenen cookieak gaituta ez daudenean, zereginak ikusi beharrean, orrialde huts bat ikusiko duzu **Zereginak** fitxan **Proiektua** orrialdean.

Microsoft Edge edo Google Chrome arakatzaileetarako, honako prozedura hauek azaltzen dute nola eguneratu zure arakatzailearen ezarpena hirugarrenen cookieak gaitzeko.

#### <a name="microsoft-edge"></a>Microsoft Edge

1. Ireki Edge arakatzailea.
2. Goiko eskuineko ertzean, hautatu **hiru puntuak** (...), eta hautatu **Ezarpenak**.
3. **Cookieak eta gune baimenak** aukeran, hautatu **Cookieak eta webguneko datuak**.
4. Desaktibatu **Blokeatu hirugarrenen cookieak**.
5. Freskatu arakatzailea. 

#### <a name="google-chrome"></a>Google Chrome

1. Ireki Chrome arakatzailea.
2. Goiko eskuineko ertzean, hautatu hiru puntu bertikalak, eta hautatu **Ezarpenak**.
3. **Pribatutasuna eta segurtasuna** aukeran, hautatu **Cookieak eta webguneko beste datuak**.
4. Hautatu **Baimendu cookie guztiak**.
5. Freskatu arakatzailea. 

> [!NOTE]
> Hirugarrenen cookieak blokeatzen badituzu, beste gune batzuetako cookieak eta webguneko datuak blokeatuko dira, nahiz eta gunea zure salbuespenen zerrendan onartzen den.

### <a name="mitigation-2-validate-the-pex-endpoint-has-been-correctly-configured"></a>2. arintzea: baliozkotu PEX amaiera puntua behar bezala konfiguratu da

Project Operations-ek proiektuaren parametro batek PEX amaiera puntua erreferentzia izatea eskatzen du. Amaierako puntu hau beharrezkoa da lanaren matxura egitura errendatzeko erabiltzen den zerbitzuarekin komunikatzeko. Parametroa gaituta ez badago, "Proiektuaren parametroak ez du balio" errorea jasoko duzu. PEX Endpoint eguneratzeko, jarraitu urrats hauek.

1. Gehitu **PEX amaiera puntua** eremua **Proiektuaren parametroak** orrialdean.
2. Identifikatu erabiltzen ari zaren produktu mota. Balio hau PEX amaiera puntua ezartzen denean erabiltzen da. Berreskuratu ondoren, produktu mota PEX amaiera puntuan definitzen da dagoeneko. Mantendu balio hori.
3. Eguneratu eremua balio honekin: `https://project.microsoft.com/<lang>/?org=<cdsServer>#/taskgrid?projectId=<id>&type=2`. Hurrengo taulan produktu motaren arabera erabili behar den motaren parametroa ematen da.

      | **Produktu mota**                     | **Parametro mota** |
      |--------------------------------------|--------------------|
      | Project for the Web erakunde lehenetsian   | type=0             |
      | Project for the Web CDS izeneko erakundean | type=1             |
      | Project Operations                   | type=2             |

4. Kendu eremua **Proiektuaren parametroak** orrialdetik.

## <a name="issue-the-project-doesnt-load-and-the-ui-is-stuck-on-the-spinner"></a>Arazoa: Proiektua ez da kargatzen eta UI birabarkian itsatsita dago

Autentifikazioaren ondorioetarako, leiho gainerakorrak gaituta egon behar dute Ataza sareak kargatzeko. Pop-upak gaituta ez badaude, pantaila kargatzeko biraka itsatsita egongo da. Ondorengo grafikoak helbide barran pop-up etiketa blokeatuta duen URLa erakusten du, eta horri esker, biratzailea orrialdea kargatu nahian trabatzen da. 

   ![Blindatuta eta pop-up bloke itsatsia.](media/popupsblocked.png)

### <a name="mitigation-1-enable-pop-ups"></a>1. arintzea: popup-ak gaitu

Zure proiektua birakariari itsatsita dagoenean, baliteke pop-upak gaituta ez egotea.

#### <a name="microsoft-edge"></a>Microsoft Edge

Zure Edge arakatzailean pop-upak gaitzeko bi modu daude.

1. Edge arakatzailean, hautatu jakinarazpena arakatzailearen goiko eskuinean.
2. Aukeratu **Baimendu beti leiho gainerakorrak eta birbideratzeak** Dataverse ingurune zehatza.
 
     ![Pop-up leihoa blokeatuta.](media/enablepopups.png)

Bestela, urrats hauek egin ditzakezu.

1. Ireki Edge arakatzailea.
2. Goiko eskuineko izkinan, hautatu **hiru puntuak** (...), eta gero hautatu **Ezarpenak** > **Gunearen baimenak** > **Popup-ak eta birbideratzeak**.
3. Txandakatu **Popup-ak eta birbideratzeak** desaktibatu leiho gainerakorrak blokeatzeko edo aktibatu zure gailuan leihoak irekitzeko.
4. Popup-ak gaitu ondoren, freskatu arakatzailea. 

#### <a name="google-chrome"></a>Google Chrome
1. Ireki Chrome arakatzailea.
2. Joan laster-leihoak blokeatuta dauden orrira.
3. Helbide barran, hautatu **Popup-a blokeatuta**.
4. Aukeratu ikusi nahi duzun pop-uparen esteka.
5. Popup-ak gaitu ondoren, freskatu arakatzailea. 

> [!NOTE]
> Gunearen popup-ak beti ikusteko, hautatu **Onartu beti popup-ak eta birbideratzeak [gunetik]** eta, ondoren, hautatu **Eginda**.

## <a name="issue-3-administration-of-privileges-for-project-for-the-web"></a>3. arazoa: Pribilegioak administratzea Project for the Web-erako.

Project Operations kanpoko planifikazio-zerbitzu batean oinarritzen da. Zerbitzuak erabiltzaileari WBSarekin erlazionatutako entitateei irakurtzeko eta idazteko aukera ematen dien hainbat eginkizun izatea eskatzen du. Entitate horien artean daude proiektuaren zereginak, baliabideen esleipenak eta atazen mendekotasunak. Erabiltzaile batek ezin badu WBS errendatu webgunera nabigatzean **Zereginak** fitxa, seguruenik **Proiektua** **Project Operations** ez da gaitu. Erabiltzaile batek segurtasun-funtzio errorea edo sarbidea ukatzearekin lotutako errorea jaso dezake.

### <a name="mitigation-1-validate-the-application-user-and-end-user-security-roles"></a>1. arintzea: aplikazioaren erabiltzailearen eta azken erabiltzailearen segurtasun rolak balioztatu

1. Joan **Ezarpena** > **Segurtasuna** > **Erabiltzaileak** > **Aplikazioaren erabiltzaileak** aukerara.  

   ![Aplikazio-irakurgailua.](media/applicationuser.jpg)
   
2. Egin klik bikoitza aplikazioaren erabiltzaile erregistroan egiaztatzeko:

     - Erabiltzaileak sarbidea du proiektuan. Erabiltzaileak edukia duela egiaztatuta egin dezakezu **Proiektu-kudeatzailea** segurtasun-funtzioa.
     - Microsoft Project aplikazioaren erabiltzailea badago eta behar bezala konfiguratuta dago.
 
3. Erabiltzaile hau existitzen ez bada, sortu erabiltzaile erregistro berria. 
4. Aukeratu **Erabiltzaile berriak**, aldatu sarrera-inprimakia **Aplikazioaren erabiltzailea** aukerara, eta, ondoren, gehitu **Aplikazioaren IDa**.

   ![Aplikazioaren erabiltzaile-xehetasunak.](media/applicationuserdetails.jpg)


## <a name="issue-4-changes-arent-saved-when-you-create-update-or-delete-a-task"></a>4. arazoa: Aldaketak ez dira gordetzen ataza bat sortu, eguneratu edo ezabatzen duzunean

WBSren eguneratze bat edo gehiago egiten dituzunean, aldaketek huts egiten dute eta ez dira gordetzen. Ordutegiko saretan errore bat gertatu da "Azken aldaketak ezin izan dira gorde" dioen mezuarekin.

### <a name="mitigation-1-validate-the-license-assignment"></a>1. arintzea: lizentzia esleitzea balioztatu

1. Egiaztatu erabiltzaileari lizentzia zuzena esleitu zaiola eta zerbitzua lizentziaren zerbitzu planen xehetasunetan gaituta dagoela.  
2. Egiaztatu erabiltzaileak **project.microsoft.com** ireki dezakeela.
    
### <a name="mitigation-2-validation-configuration-of-the-project-application-user"></a>2. arintzea: Proiektuaren aplikazioaren erabiltzailearen baliozkotzearen konfigurazioa
1. Egiaztatu Proiektuaren aplikazioaren erabiltzailea sortu dela.
2. Aplikatu segurtasun rol hauek erabiltzaileari:
  
  - Dataverse erabiltzailea edo Base erabiltzailea
  - Project Operations sistema
  - Proiektuaren sistema
  - Project Operations idazketa dualeko sistema. Funtzio hori behar da Project Operations-en baliabideetan edo izakinik gabeko produktuetan oinarritutako egoera inplementatzeko.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
