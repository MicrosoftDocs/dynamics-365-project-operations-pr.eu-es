---
title: Segurtasunaren modeloa
description: Gai honek segurtasun-ereduari buruzko informazioa eskaintzen du Dynamics 365 Project Operations-en.
author: stsporen
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: ffcfa8a9c8e31c5665acd3c3919fa90d36a3f3ca
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896716"
---
# <a name="security-model"></a>Segurtasunaren modeloa

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Microsoft Dynamics 365 Project Operations-ek segurtasun eredu bakarra du, lankidetzan oinarritutako negozio segurtasun eredu bat ahalbidetzen duena Microsoft Office Taldeak. 


## <a name="security-roles"></a>Segurtasun-funtzioak
Project Operations front-end gaitasunek honako rol hauek dituzte:

| Funtzioa                          | Deskribapena                                                                                                                                                                 | Scope |
|-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|
| Praktika-administratzailea              | Proiektuen arteko txostenak onartzen ditu.                                                                                                            | Negozio-unitatea              |
| Proiektuaren onartzailea              | Denbora eta gastuak onartzen ditu proiektu batean.                                                                                                                              | Negozio-unitatea |
| Proiektuaren fakturazio-administratzailea | Faktura proposamena sortzen du.                                                                                                                                                 | Negozio-unitatea |
| Proiektu-kudeatzailea               | Proiektuaren plana sortzen du eta baliabideak eskatzen ditu.                                                                                                                              | Negozio-unitatea |
| Proiektu-baliabidea              | Erreserbatu daitezkeen taldekideak eta jakinarazi denbora.                                                                                                          | Negozio-unitatea|
| Baliabide-kudeatzailea              | Baliabideen kudeaketa funtzio guztiak, hala nola baliabideen eskaerak eta erreserbak, bereizita daude Proiektu kudeatzaile hibridoa + Baliabide kudeatzailearen konfigurazioa eta Baliabide kudeatzaile rol bakarra eta zentralizatua onartzeko. | Negozio-unitatea |


Weberako Microsoft Project-ek eginkizun hauek ditu:
| Funtzioa                          | Deskribapena                                                                                                          | Scope |                                                       
|-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----|
| Proiektuaren erabiltzailea | Proiektuaren erabiltzaile kolaboratzailea, nork bere proiektuak sortzeko eta haiekin partekatutako proiektuak ikusteko gai dena.| Erabiltzailea|
| Proiektu sistema | Aplikazioaren testuinguruan erabilitako rola. Bezeroek ez lukete sistema rol hau erabili behar. | Orokorra|

## <a name="security-enforcement"></a>Segurtasuna betearaztea
Proiektu mailan burutzen diren ekintzak saioa hasita duen erabiltzailearen testuinguruan egiten dira. Horrek esan nahi du proiektu bat sortu, ireki edo ezabatzeko, erabiltzaileari CDS sarbidea eskura behar zaiola. CDSrako sarbidea plataforman dauden mekanismo posibleen bidez eman daiteke. Adibidez, esparru zabalagoa duen erabiltzailea sar daiteke proiektuan edo erabiltzaileari sarbidea ematen dion proiektu partekatu esplizitua burutu bada.

Garrantzitsua da hori kontuan hartzea proiektuen eragiketetan proiektuak sortzerakoan.

## <a name="modern-group-collaboration-with-project-operations"></a>Talde-lankidetza modernoa Project Operations-ekin
Weberako Proiektuak eta Proiektuen Eragiketak talde modernoak onartzen dituzte lankidetzarako. Proiektuari talde baten bidez gehitutako erabiltzaileek proiektuaren plana edita dezakete.

Weberako proiektuak erabiltzaileak taldera gehitzen ditu automatikoki esleitzean.

Taldeek proiektuaren eta lankidetzako artefaktuen laguntza baimenak lankidetzan lantzea ahalbidetzen dute. Hurrengo diagraman, talde-esleipen prozesuan gertatzen diren gertaerak eta egoera aldaketak azaltzen dira.

Proiektuaren Eragiketek ez dute talderik sortzen ekintza inplizituaren bidez eta talde sakatuen ekintza esplizituaren bidez bakarrik egiten dute.

Taldeko kideen bilaketa **Taldearen kudeaketa** elkarrizketa-koadroa, inguruneko segurtasun-taldearen zati gisa ezartzen direnetara mugatuta dago. Informazio gehiago lortzeko, ikusi [Kontrolatu erabiltzaileen sarbidea inguruneetara: segurtasun-taldeak eta lizentziak](https://docs.microsoft.com/power-platform/admin/control-user-access).

1. Proiektua sortu duen erabiltzailearen jabetzakoa da.
2. Proiektuaren jabea taldeari eguneratu zaio.
3. Jabe taldea zehaztutako edo sortutako Bulego Taldearekin mapatuta dago.
4. Proiektuaren jatorrizko jabea Bulego Taldean gehitzen da.

## <a name="deployment-recommendation"></a>Inplementazio-gomendioak
Office taldearen lankidetza eredua garatu ahala, funtzionaltasuna gehituko da denboran kontrol zehatzagoa emateko. Gaur egun Project Operations inplementatzen dituzten bezeroei ohiko arreta jartzera animatzen zaie Microsoft Dynamics 365 segurtasun eredua.

Informazio gehiagorako, ikusi [Segurtasuna Common Data Service](https://docs.microsoft.com/power-platform/admin/wp-security).

## <a name="project-operations-and-microsoft-dynamics-365-finance-security"></a>Project Operations eta Microsoft Dynamics 365 Finance segurtasuna
Project Operations-ek honako rol hauek biltzen ditu:

- Proiektu-kudeatzailea
- Proiektuaren kontabilitatea

Finantzetako segurtasunari buruzko informazio gehiago lortzeko, ikusi [Funtzioetan oinarritutako segurtasuna](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/role-based-security).


