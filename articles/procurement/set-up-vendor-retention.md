---
title: Konfiguratu saltzailearen atxikipena
description: Artikulu honetan, hornitzaileen atxikipena nola konfiguratu azaltzen da.
author: sigitac
ms.date: 09/27/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: f30e8829d8d5d99c81fce730cb93cd7ce31913fe
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8929751"
---
# <a name="set-up-vendor-retention"></a>Konfiguratu saltzailearen atxikipena

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Artikulu honetan hornitzaileen atxikipena nola konfiguratu behar den ematen da.

## <a name="set-up-a-vendor-retention-account-in-general-ledger"></a>Konfiguratu saltzailearen atxikitze kontua liburu nagusian

1. Dynamics 365 Finance-n, joan **zaitez transakzio automatikoetarako liburu nagusiaren** > **kontabilizatzeko konfigurazio-kontabilitatera** > **·**.
2. Gehitu lerroa.
3. **Bidalketa mota** eremuan, hautatu **Saltzailearen atxikipena**.
4. Aukeratu saltzailearen atxikipena argitaratzeko kontu nagusia.

## <a name="create-vendor-retention-terms"></a>Sortu saltzailearen atxikipen baldintzak

Erabili **Saltzailearen atxikipen baldintzak** orria saltzailearen ordainketetarako atxikipen baldintzak konfiguratzeko eta mantentzeko. Idatzi gorde beharreko saltzailearen ordainketaren portzentajea eta aldez aurretik gordetako zenbatekoen portzentajea. Kopuruak automatikoki gordetzen dira saltzailearen fakturetan, kontratua zehaztutako amaierako egoerara iritsi arte. Saltzaile bati atxikitzeko baldintzak ezarri ondoren, saltzaileak lan egiten duen edozein proiektutan aplika ditzakezu.

1. Finance-n, joan **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Atxikipena** > **Saltzailearen ordainketa atxikitzeko baldintzak** aukerara.
2. Aukeratu **Berria** saltzailearen atxikipen epe berria gehitzeko. Aldi berriko **Arauaren IDa** eremuko balioa automatikoki sartzen da. 
3. **Azalpena** eremuan, idatzi aldi berriaren izen deskribatzailea.
4. **Aldiak** fitxan, hautatu **Gehitu lerroa** saltzailearen atxikipen epe bat sartzeko.
5. **Entregatutako unitateen ehunekoa** eremuan, idatzi arauaren osatze ehunekoa. Zenbatekoak automatikoki gordetzen dira saltzailearen fakturetan, proiektuaren amaierako fasea sartzen duzun ehunekoaren berdina izan arte. Adibidez, 50,00 idazten baduzu, zenbatekoak mantenduko dira proiektua ehuneko 50 arte osatu arte.
6. **Atxikitzeko ehunekoa** eremuan, sartu gorde beharreko saltzailearen fakturaren zenbatekoa. Adibidez, eremu honetan 10,00 sartzen badituzu, saltzailearen fakturen zenbatekoaren ehuneko 10 mantenduko da proiektua proiektuan hautatutako osatze ehunekoa lortu arte **Entregatutako unitateen ehunekoa** eremuan.
7. **Askatzeko ehunekoa** eremuan, sartu aurretik gordetako zenbatekoen ehunekoa hautatutako proiektua amaitzean.

> [!NOTE]
> Proiektua osatzeko maila desberdinetarako mugarri bat baino gehiago badituzu, idatzi saltzailearen atxikipen epe lerro bereizi atxikipen arau bakoitzerako. Lerro bakoitzak atxikitzeko ehuneko desberdina eta askatu beharreko ehunekoa zehaztu dezake proiektuaren amaierako maila bakoitzerako.

## <a name="set-up-a-vendor-agreement-for-the-project"></a>Ezarri proiektuarentzako saltzailearen akordioa

Konfiguratu proiektuari aplikatzen zaizkion saltzaileen atxikitze baldintzak. Saltzaileari atxikitzeko baldintzak saltzailearentzat sortzen dituzun erosketa-eskaeretan ere agertzen dira.

1. Finance-n, joan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuak** > **Proiektu guztiak** aukerara. 
2. Aukeratu proiektu bat eta Ekintza panelean, hautatu **Proiektu taldea** > **Saltzaileen akordioak**.
3. **Saltzaileen akordioak** orrialdean, gehitu lerro berria.
4. **Kontuaren kodea** eremuan, hautatu aukera hauetako bat:
   - **Taula**: Saltzailearen atxikitze-baldintzak saltzaile bakar bati aplikatzen zaizkio.
   - **Taldea**: Saltzailearen atxikitze-baldintzak saltzaile talde bateko saltzaile guztiei aplikatzen zaizkie.
   - **Guztia**: Saltzailearen atxikitze-baldintzak saltzaile guztiei aplikatzen zaizkie.
5. **Saltzailea/Saltzaile taldea** eremuan, hautatu saltzailea edo saltzaile taldea zein saltzaileren atxikitze baldintzak aplikatzen diren. Aukeratu baduzu **Guztiak** aurreko urratsean, eremu hau ez dago erabilgarri.
6. **Saltzailearen atxikipen-epeak** eremuan, hautatu arau IDa saltzaile honi aplikatzeko atxikipen baldintzetarako.
