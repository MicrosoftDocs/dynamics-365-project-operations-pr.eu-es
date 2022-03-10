---
title: Segurtasunaren modeloa
description: Gai honek Dynamics 365 Project Operations-eko segurtasun-ereduei buruzko informazioa eskaintzen du.
author: stsporen
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 2f283771921504dc29ddcc26ca659d4e151598840339bd8c1a857e8bf5dde9ed
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6991471"
---
# <a name="security-model"></a>Segurtasunaren modeloa

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Microsoft Dynamics 365 Project Operations rolean oinarritutako negozio segurtasun ereduarekin lankidetzan jarduteko aukera ematen duen segurtasun eredu bakarra dauka Microsoft Office Taldeak. 


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

| Funtzioa           | Deskribapena                                                                                                        | Scope  |
|----------------|--------------------------------------------------------------------------------------------------------------------|--------|
| Proiektuaren erabiltzailea   | Proiektuaren erabiltzaile kolaboratzailea, nork bere proiektuak sortzeko eta haiekin partekatutako proiektuak ikusteko gai dena. | Erabiltzailea   |
| Proiektu sistema | Aplikazioaren testuinguruan erabilitako rola. Bezeroek ez lukete sistema rol hau erabili behar.                                    | Orokorra |

## <a name="security-enforcement"></a>Segurtasuna betearaztea
Proiektu mailan burutzen diren ekintzak saioa hasita duen erabiltzailearen testuinguruan egiten dira. Horrek esan nahi du proiektu bat sortu, ireki edo ezabatzeko, erabiltzaileari CDS sarbidea eskura behar zaiola. CDSrako sarbidea plataforman dauden mekanismo posibleen bidez eman daiteke. Adibidez, esparru zabalagoa duen erabiltzailea sar daiteke proiektuan edo erabiltzaileari sarbidea ematen dion proiektu partekatu esplizitua burutu bada.

Garrantzitsua da hori kontuan hartzea proiektuen eragiketetan proiektuak sortzerakoan.

## <a name="modern-group-collaboration-with-project-operations"></a>Talde-lankidetza modernoa Project Operations-ekin
Weberako Proiektuak eta Proiektuen Eragiketak talde modernoak onartzen dituzte lankidetzarako. Proiektuari talde baten bidez gehitutako erabiltzaileek proiektuaren plana edita dezakete.

Weberako proiektuak erabiltzaileak taldera gehitzen ditu automatikoki esleitzean.

Taldeek proiektuaren eta lankidetzako artefaktuen laguntza baimenak lankidetzan lantzea ahalbidetzen dute. Hurrengo diagraman, talde-esleipen prozesuan gertatzen diren gertaerak eta egoera aldaketak azaltzen dira.

Proiektuaren Eragiketek ez dute talderik sortzen ekintza inplizituaren bidez eta talde sakatuen ekintza esplizituaren bidez bakarrik egiten dute.

Taldeko kideen bilaketa **Taldearen kudeaketa** elkarrizketa-koadroa, inguruneko segurtasun-taldearen zati gisa ezartzen direnetara mugatuta dago. Informazio gehiago lortzeko, ikusi [Kontrolatu erabiltzaileen sarbidea inguruneetara: segurtasun-taldeak eta lizentziak](/power-platform/admin/control-user-access).

![Talde modua.](./media/groupsmode.png)

1. Proiektua sortu duen erabiltzailearen jabetzakoa da.
2. Proiektuaren jabea taldeari eguneratu zaio.
3. Jabe taldea zehaztutako edo sortutako Bulego Taldearekin mapatuta dago.
4. Proiektuaren jatorrizko jabea Bulego Taldean gehitzen da.

## <a name="deployment-recommendation"></a>Inplementazio-gomendioak
Office taldearen lankidetza eredua garatu ahala, funtzionaltasuna gehituko da denboran kontrol zehatzagoa emateko. Gaur egun Project Operations inplementatzen dituzten bezeroei ohiko arreta jartzera animatzen zaie Microsoft Dynamics 365 segurtasun eredua.

Informazio gehiagorako, ikusi [Segurtasuna Common Data Service](/power-platform/admin/wp-security).

## <a name="project-operations-and-microsoft-dynamics-365-finance-security"></a>Project Operations eta Microsoft Dynamics 365 Finance segurtasuna
Project Operations-ek honako rol hauek biltzen ditu:

- Proiektu-kudeatzailea
- Proiektuaren kontabilitatea

Finantzetako segurtasunari buruzko informazio gehiago lortzeko, ikusi [Funtzioetan oinarritutako segurtasuna](/dynamics365/fin-ops-core/dev-itpro/sysadmin/role-based-security).




[!INCLUDE[footer-include](../includes/footer-banner.md)]