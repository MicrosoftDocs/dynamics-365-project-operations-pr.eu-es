---
title: Konfiguratu proiektu fakturagarrien kontabilitatea
description: Gai honek fakturagarriak diren proiektuen kontabilitate aukerei buruzko informazioa eskaintzen du.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 47bb5671c7b80c0e96f3f65e9c4d25f6da8184a5
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4131958"
---
# <a name="configure-accounting-for-billable-projects"></a>Konfiguratu proiektu fakturagarrien kontabilitatea

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations-ek kontabilitate aukera ugari onartzen ditu fakturagarriak diren proiektuetarako, denbora eta materiala eta prezio finkoko transakzioak barne.

- **Denbora eta material transakzioak**: Transakzio hauek fakturatzen dira lanak aurrera egin ahala proiektuaren orduen, gastuen, elementuen edo kuoten kontsumoaren arabera. Transakzio kostu horiek transakzio bakoitzeko diru sarrerekin pareka daitezke eta proiektua fakturatzen da lanak aurrera egin ahala. Proiektuaren diru-sarrerak transakzioa gertatzen den unean ere lor daitezke. Fakturazioan zehar, diru-sarrerak aitortzen dira eta, hala badagokio, metatutako diru-sarrerak alderantzikatzen dira.
- **Prezio finkoko transakzioak**: Transakzio horiek fakturazio-egutegi baten arabera fakturatzen dira, proiektuaren kontratuan oinarrituta. Prezio finko transakzio diru-sarrerak izango dira fakturazio erregistratzen daiteke edo kalkulatu eta aldian behin argitaratua, **Bukatutako kontratua** edo **Osatutako ehunekoa** metodoen arabera.

Proiektu bat fakturagarritzat jotzen da kontratu lerro batekin edo gehiagorekin lotzen denean. Proiektuaren kontratu lerro batek berak zehazten du fakturazio metodoa eta transakzio mota onartzen diren.

Adibide gisa, Fabrikam Robotics-ek proiektu bat lortu du Adatum korporazioarekin ekipamenduak optimizatzeko. Adatum-ek 10.000 $ USD zenbateko finkoa ordainduko du sortutako proiektuaren gastuei aurre egiteko. Prezio finkoko fakturazio-metodoa da hori. Proiektuaren denbora eta tasak erabilera bakoitzeko fakturatuko dira. Denboraren eta materialen fakturazio-metodoa da hori. Lan guztiak Adatum ekipamenduen optimizazioa izeneko proiektu bakar baten jarraipena egingo dute.

Proiektu taldeko kide batek zortzi orduko lana aurkezten du Adatum ekipamenduak optimizatzeko proiektuan. Proiektuaren kudeatzaileak denbora hori onartzen duenean, sistemak denbora eta materiala fakturatzeko metodoa erabiltzen du benetako transakzioak, faktura eta kontua sortzeko. Transakzio hau ez da sartuko prezio finkoko diru-sarreren kalkuluaren kalkuluan.

Proiektuaren taldeko beste kide batek 2000,00 $ USD bidaiarako gastua aurkezten du Adatum ekipamendua optimizatzeko proiektuaren aurka. Proiektuaren kudeatzaileak bidalketa hori onartzen duenean, sistemak prezio finkoko fakturatzeko metodoa erabiltzen du benetako transakzioak eta proiektuaren gastuen kontua sortzeko. Bezeroari ez zaio fakturatuko transakzio horretan oinarrituta. Horren ordez, bereizita konfiguratutako fakturazio mugarriak erabiliz fakturatuko dira. Gastuen transakzio hau, gastuen aurreikuspenekin batera, ez da sartuko prezio finkoko diru-sarreren kalkuluaren kalkuluan.

Proiektuen transakzioen kontabilitate-printzipioak proiektuaren kostuen eta diru-sarreren profiletan definitzen dira. Proiektuaren transakzio bakoitzerako, sistemak proiektuaren kostu eta diru-sarrera profilak zehazten ditu konfiguratu diren proiektuaren kostu eta diru-sarrera profileko arauak erabiliz.

## <a name="define-project-cost-and-revenue-profiles"></a>Definitu proiektu baten kostuaren eta diru-sarreren profilak 

Proiektuaren kostuak eta diru-sarreren profilek proiektu-transakzioen kontabilitate-arauak zehazten dira. Profil hauek Proiektuen kudeaketan eta kontabilitatean konfiguratuta daude. 

Bete urrats hauek proiektuaren kostuen eta diru-sarreren profil berria sortzeko. 

1. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Bidalketa** > **Proiektuaren kostuen eta diru-sarreren profilak**. 
2. Aukeratu **Berria** proiektuaren kostuen eta diru-sarreren profil berria sortzeko.
3. **Izena** eremuan, idatzi izena eta profilaren deskribapen laburra.
4. **Fakturazio-metodoa** eremuan, hautatu **Denbora eta materiala** edo **Prezio finkoa**.
5. Zabaldu **Liburu nagusia** FastTab-a. Fitxa honetako eremuek proiektuaren transakzioak Proiektuaren eragiketen integrazio aldizkaria erabiliz gero proiektuaren faktura proposamenaren bidez fakturatzen direnean erabiltzen diren kontabilitate printzipioak definitzen dituzte.
6. Hautatu dagokion informazioa **Liburu nagusia** FastTab-eko eremu hauetan:

    - **Bidalketa-kostuak - ordua**:

       - *Liburu nagusirik ez*: Denbora-transakzioen kostua ez da liburu nagusian argitaratuko Project Operations integrazio-aldizkaria argitaratzen denean. Hala ere, kontulariak geroago bidali ahal izango ditu kostuak Argitaratu kostuak funtzioa erabiliz.
       - **Balantzea**: Denborazko transakzioen kostua liburu nagusiko kontu motan kargatuko da, *WIP - Kostuaren balioa* eta *Nominak esleitzeko kontua* Liburu nagusiaren argitaratzeko konfigurazioan. Kontulariak Argitaratu kostuak funtzioa erabiliko du kostu hori Saldo kontutik irabazien eta galeren kontura aldiro aldatzeko.
       - **Irabaziak eta galerak**: Project Operations integrazio aldizkaria argitaratzean, denbora transakzioaren kostua Liburu nagusiaren kontu motan kargatuko da *Kostua*, eta kreditatuta *Nominak esleitzeko kontua* fitxategian definitzen da **Kostua** fitxan **Liburu nagusia argitaratzeko konfigurazioa** orrialdea (**Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Bidalketa** \> **Liburu nagusia argitaratzeko konfigurazioa**). Hau denbora eta material transakzioetarako konfigurazio ohikoena da.
        - *Inoiz ez liburu nagusia*: Denborazko transakzioen kostua ez da inoiz liburu nagusian argitaratuko.

    - **Argitaratu kostuak - gastuak**:

         - **Saldoa**: Project Operations integrazio aldizkaria argitaratzean, gastuen transakzio kostua Liburu nagusia kontu motan kargatuko da *WIP - Kostuaren balioa* fitxategian definitzen den moduan **Kostua** fitxan **Liburu nagusia argitaratzeko konfigurazioa** orrialdean eta aldizkariaren lerroan konpentsatutako kontuan kreditatuta. Gastuaren lehenetsitako konpentsazio kontuak atalean definitzen dira **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** \> **Bidalketa** \> **Gastuetarako lehenetsitako kontua**. Kontulariak **Argitaratu kostuak** funtzioa erabiliko du kostu hori saldo-kontutik irabazien eta galeren kontura aldiro aldatzeko.
        - **Irabaziak eta galera**: Project Operations integrazio aldizkaria argitaratzean, gastuen transakzio kostua Liburu nagusia kontu motan kargatuko da *WIP - Kostuaren balioa* fitxategian definitzen den moduan **Kostua** fitxan **Liburu nagusia argitaratzeko konfigurazioa** orrialdean eta aldizkariaren lerroan konpentsatutako kontuan kreditatuta. Gastuaren lehenetsitako konpentsazio kontuak atalean definitzen dira **Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Bidalketa** \> **Gastuetarako lehenetsitako kontua**.
       
    - **Kontuko fakturazioa**:

        - **Balantzea**: Proiektuaren faktura proposamena argitaratzerakoan, kontuko transakzio bat (fakturazio mugarria) kobratuko da Liburu nagusiaren kontu motan *WIP fakturatua - kontura* fitxategian definitzen den moduan **Diru-sarrerak** fitxan **Liburu nagusia argitaratzeko konfigurazioa** orrialdean, eta Bezeroaren oreka kontuan zordunduta.
         - **Irabaziak eta galera**: Proiektuaren faktura proposamena argitaratzerakoan, kontuko transakzio bat (fakturazio mugarria) kobratuko da Liburu nagusiaren kontu motan *Fakturatutako diru-sarrera - kontura* fitxategian definitzen den moduan **Diru-sarrerak** fitxan **Liburu nagusia argitaratzeko konfigurazioa** orrialdean, eta Bezeroaren oreka kontuan zordunduta. Bezeroen balantze-kontuak **Kobratzeko kontuak** \> **Konfigurazioa** \> **Bezeroak bidaltzeko profilak**.

   Denboraren eta materialaren fakturazio metodoen bidalketa-profilak zehazten dituzunean, transakzio mota bakoitzeko (ordua, gastua eta kuota) dirua irabazteko aukera duzu. **Eskuratu diru-sarrerak** aukera **Bai** bada, Project Operations Integration aldizkarian fakturatu gabeko salmenten transakzioak liburu nagusian erregistratuko dira. Salmenten balioa kobratuko da **WIP - salmenten balioaren kontua** eta **Sortutako diru-sarrerak - salmenten balioa** webgunean sortu zen kontua **Liburu nagusia argitaratzeko konfigurazioa** orrialdean, **Diru-sarrerak** fitxa. 
  
  > [!NOTE]
  > Aukera, **Eskuratu diru-sarrerak** eskuragarri dago dagokion transakzio mota denean **Kostua** irabazien eta galeren kontuan sartzen da.
    
7. Zabaldu **Aurreikuspena** FastTab-a. Fitxa honetako eremuek prezio finkoko diru-sarreren kalkuluen ezarpenak zehazten dituzte. Fitxa honetako eremuak Proiektuaren kostuen eta diru-sarreren profilei soilik aplikatzen zaizkie fakturazio-metodoarekin **Prezio finkoa**.
8. Hautatu dagokion informazioa **Aurreikuspena** FastTab-eko eremu hauetan:

    - **Proiektua amaitzeko kalkuluetarako erabilitako printzipioa**:

        - **Bukatutako kontratua**: Kostuen parekapena eta diru-sarreren aitorpena ez da proiektua amaitu arte gertatzen. Kostuak WIP gisa islatzen dira balantzea proiektua amaitu arte.
        - **Osatutako ehunekoa**: Sortutako diru-sarrerak kalkulatu eta liburutegian kontabilizatzen dira aldi bakoitzean, proiektuaren amaierako ehunekoaren arabera. Ehunekoen osaketa kalkulatzeko metodo ugari daude eskuragarri. Metodo hauek automatikoak izan daitezke konfigurazioan oinarrituta edo eskuzkoak.
        - **WIP ez**: Konfigurazio hau denbora tarte laburreko eta faktura eta kostuak aldi berean gertatzen diren prezio finkoetarako erabiltzen da. Kasu honetan, **Kontuko fakturazioa** eremuko balioa **Liburu nagusia** FastTab automatikoki ezartzen da **Irabaziak eta galerak** fakturazioan diru sarrerak aitortzen direla ziurtatzeko. Diru-sarrerak kalkulatzeko prozesua ez da proiektuaren kostu eta diru-sarreren profilerako erabiliko.

    - **Bat etortzeko printzipioa**: Eremu honek zehazten du kalkulatutako salmenten balioa (metatutako diru-sarrerak) liburu nagusian nola argitaratuko den.

        - **Salmenten balioa** printzipioa erabiliz, sistemak salmenten balioa kalkulatuko du kostuak eta diru-sarrerak parekatuz eta gero zenbateko bakar gisa argitaratuz.
        - **Ekoizpena eta etekina** printzipioa erabiliz, sistemak salmenten balioa kostu errealetan eta mozkin kalkulatuetan banatuko du. Hauek bereiz argitaratzen dira.

    - **Kostuen txantiloiak**: Baimendu proiektuen transakzioak transakzio motaren eta proiektuaren kategorien arabera multzokatzea eta talde horien ehunekoaren osaketa kalkulatzeko arauak definitzea.
    - **Aldi-kodeak**: Definitu sarreren kalkuluen maiztasuna proiektuaren kostu eta diru-sarrera profil jakin baterako kalkulatzeko.
    - **Aurrekonturako kategoriak**: Proiektuaren transakzioetan salmenten balioa (metatutako diru-sarrerak) argitaratzeko erabiltzen da. Lehenik eta behin, konfiguratu proiektu baten kategoria dedikatua **Kuota** transakzio mota eta ondoren ezarri bandera, **Aurreikuspena** proiektu kategoria honetarako. Ondoren, hautatutako bat datorren printzipioaren arabera, aukeratu proiektuaren kategoria hau **Salmentak** balioa edo **Irabaziak** eremua Proiektuaren kostuen eta diru-sarreren profilean.

### <a name="sample-configurations-for-project-cost-and-revenue-profiles"></a>Proiektuaren kostuen eta diru-sarreren profilen konfigurazio laginak

Denbora eta materialak - WIP gabe

![Kostuen eta diru-sarreren profila: denbora eta materialak - WIP ez](media/time-material-no-wip.png)

Denbora eta materialak - WIP (diru-sarrerak)

![Kostuen eta diru-sarreren profila: denbora eta materialak - WIP](media/time-material-with-wip.png)

Prezio finkoa - WIP gabe

![Kostuen eta diru-sarreren profila: prezio finkoa - WIPrik ez](media/fixed-price-no-wip.png)

Prezio finkoa - amaitutako kontratua

![Kostuen eta diru-sarreren profila: prezio finkoa - amaitutako kontratua](media/fixed-price-completed-contract.png)

Prezio finkoa - ehunekoaren osaketa

![Kostuen eta diru-sarreren profila: prezio finkoa - ehunekoaren osaketa](media/fixed-price-completed-percentage.png)


## <a name="accounting-event-examples-for-sample-project-cost-and-revenue-profiles"></a>Kontabilitate-gertaeraren adibideak proiektu-kostuen eta diru-sarreren profilen laginetarako.

| Kontabilitate-gertaera                  | Denbora eta materiala - WIP gabe                       | Denbora eta materiala - WIP                                                                                           | Prezio finkoa - WIP gabe                                            | Prezio finkoa - amaitutako kontratua                                                                            | Prezio finkoa - ehunekoaren osaketa                             |
|-----------------------------------|--------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------|
| Denbora transakzioak periodizatzea    | Zordunketa - Kostua <br>Kreditua –Nominen esleipena          | Zordunketa - Kostua <br>Kreditua –Nominen esleipena <br>Zorduna –WIP Salmenten balioa <br>Kreditua –Sarreren irabazien salmenten balioa                | Zordunketa - Kostua <br>Kreditua –Nominen esleipena                         | Zordunketa - Kostua <br>Kreditua –Nominen esleipena                                                                    | Zordunketa - Kostua <br>Kreditua –Nominen esleipena                       |
| Gastuen transakzioak periodizatzea | Zordunketa - Kostua <br>Kreditua - gastuagatik konpentsatutako kontua | Zordunketa - Kostua <br>Kreditua - gastuagatik konpentsatutako kontua <br>Zorduna –WIP Salmenten balioa <br>Kreditua –Sarreren irabazien salmenten balioa      | Zordunketa - Kostua <br>Kreditua - gastuagatik konpentsatutako kontua                 | Zordunketa - Kostua<br> Kreditua - gastuagatik konpentsatutako kontua                                                            | Zordunketa - Kostua <br>Kreditua - gastuagatik konpentsatutako kontua               |
| Bezeroari fakturatzea                | Zorduna –Bezeroen saldoa <br>Kreditua –Fakturatutako diru-sarrerak | Zorduna –Bezeroen saldoa <br>Kreditua –Fakturatutako diru-sarrerak <br>Kreditua - WIP Salmenten balioa Zorduna - Metatutako diru-sarreren salmenten balioa | Zorduna –Bezeroen saldoa <br>Kreditua - Fakturatutako diru-sarrerak - kontura | Zorduna –Bezeroen saldoa <br>Kreditua - WIP - Fakturatutako diru-sarrerak - kontura                                                  | Zorduna –Bezeroen saldoa <br>Kreditua - WIP - Fakturatutako diru-sarrerak - kontura    |
| Diru-sarreren ondorengo aurreikuspenak             | Ez da aplikagarria                                   | Ez da aplikagarria                                                                                                    | Ez da aplikagarria                                                  | Zordunketa - WIP kostuaren balioa <br>Kreditua - kostua                                                                         | Zordunketa – WIP - Salmenten balioa <br>Kreditua – lortutako diru-sarrerak - Salmenten balioa |
| Ezabatu                         | Ez da aplikagarria                                   | Ez da aplikagarria                                                                                                    | Ez da aplikagarria                                                  | Kreditua - WIP kostuaren balioa <br>Zordunketa - Kostua <br>Kreditua – Lortutako diru-sarrerak - Salmenten balioa <br>Zordunketa - WIP - Fakturatutako diru-sarrerak - kontura | Zordunketa - WIP - Fakturatutako diru-sarrerak - kontura <br>Kreditua – WIP - Salmenten balioa     |

## <a name="configure-project-cost-and-revenue-profile-rules"></a>Konfiguratu Proiektu baten kostuaren eta diru-sarreren profilak

Proiektuaren kostuaren eta diru-sarreren profilaren arauek zehazten dute proiektuaren fakturen edozein transakzio prozesatzerakoan erabili behar den Proiektuaren kostu eta diru-sarreren profila. Definitu arauak **Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Bidalketa** \> **Proiektuaren kostua eta diru-sarreren profileko arauak** aukeran.

Arauak proiektuaren kontratuaren, proiektuaren taldearen edo proiektu zehatz baten arabera defini daitezke. Sistemak beti zehaztasun handieneko araua hautatuko du lehenik.
