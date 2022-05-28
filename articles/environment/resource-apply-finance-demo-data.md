---
title: Aplikatu demo-datuak Finance-ren hodeian ostatatutako ingurune batean
description: Gai honek Project Operations-en demo datuak Dynamics 365 Finance Hodeian ostatatutako ingurune batean nola aplikatu azaltzen du.
author: sigitac
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: e4ccc7eb02fabdc0476fe454f33bff637ab8b835
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8588951"
---
# <a name="apply-demo-data-to-a-finance-cloud-hosted-environment"></a>Aplikatu demo-datuak Finance-ren hodeian ostatatutako ingurune batean

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

> [!IMPORTANT]
> Gai hau soilik aplikagarria da Microsoft Dynamics 365 Finance 10.0.13 bertsioa eta hodeian ostatatutako ingurune batean bakarrik egin daiteke. Osatu gai honetako urratsak **AURRETIK** ingurumenari kalitatezko eguneratzeak aplikatzen dizkiozu.

1. Zure LCS proiektuan, ireki **Ingurumenaren xehetasunak** orrialdea. Ohar zaitez urruneko mahaigaineko protokoloa (RDP) erabiliz ingurunearekin konektatzeko behar diren xehetasunak biltzen dituela.

![Ingurumen-xehetasunak.](./media/1EnvironmentDetails.png)

Nabarmendutako kredentzialen lehen multzoa tokiko kontuaren egiaztagiriak dira eta urruneko mahaigaineko konexiorako hiperesteka bat dute. Kredentzialen artean, inguruneko administratzaile izena eta pasahitza daude. Ingurune honetan SQL Server zerbitzuan saioa hasteko bigarren kredentzial multzoa erabiltzen da.

2. Konektatu ingurunearekin hiperesteka bidez **Tokiko kontuak**, eta erabili **Tokiko kontuaren egiaztagiriak** autentifikatzeko.
3. Joan **Interneteko Informazio Zerbitzuak** > **Aplikazio multzoak** > **AOSZerbitzua** eta zerbitzua gelditu. Une honetan zerbitzua gelditzen ari zara, SQL datu basea ordezkatzen jarrai dezazun.

![Gelditu AOS.](./media/2StopAOS.png)

4. Joan **Zerbitzuak** eta gelditu bi elementu hauek:

- Microsoft Dynamics 365 Unified Operations: Loteen kudeaketa zerbitzua
- Microsoft Dynamics 365 Unified Operations: Datuak Inportatzeko Esportazio Esparrua

![Gelditu zerbitzuak.](./media/3StopServices.png)

5. Ireki Microsoft SQL Server Management Studio. Hasi saioa SQL zerbitzariaren egiaztagiriekin eta erabili axdbadmin erabiltzailea eta LCSko pasahitza **Inguruneen xehetasunak** orrialdea.

![SQL Server Management Studio.](./media/4SSMS.png)

6. Object Explorer-en, **Datu-baseak** eta kokatu **AXDB**. Datu-basea datu-basean ordeztuko duzu [Deskarga-zentroan](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip). 
7. Kopiatu zip fitxategia urrun zauden VM-ra eta atera zip edukia.
8. SQL Server Management Studio-n, egin klik eskuineko botoiaz **AxDB** eta, ondoren, hautatu **Zereginak** > **Berreskuratu** > **Datu basea**.

![Leheneratu datu-basea.](./media/5RestoreDatabase.png)

9. Aukeratu **Iturburu-gailua** eta joan kopiatu duzun zip-etik ateratako fitxategira.

![Iturri gailuak.](./media/6SourceDevice.png)

10. Aukeratu **Aukerak** eta, ondoren, hautatu **Gainidatzi lehendik dagoen datu basea** eta **Itxi dauden konexioak helmugako datu basera**. 
11. Hautatu **Ados**.

![Leheneratu ezarpenak.](./media/7RestoreSetting.png)

AXDB berreskurapena arrakastatsua izan dela baieztatuko duzu. Baieztapen hau jaso ondoren, SQL Services Management Studio itxi dezakezu.

12. Itzuli **Interneteko Informazio Zerbitzuak** > **Aplikazio multzoak** > **AOSZerbitzua** aukerara eta hasi AOSZerbitzua.
13. Joan **Zerbitzuak** eta hasi lehen gelditu zenituen bi zerbitzuak.

14. Aurkitu AdminUserProvisioning tresna VM honetan. Begiratu azpian, K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.
15. Exekutatu .ext fitxategia zure erabiltzailearen helbidea erabiliz **Helbide elektronikoa** eremua. 
16. Hautatu **Bidali**.

![Administratzaile-erabiltzailearen hornitzea.](./media/8AdminUserProvisioning.png)

Minutu pare bat behar dira. Admin erabiltzailea ondo eguneratu dela baieztatzeko mezua jaso beharko zenuke.

17. Azkenean, exekutatu komando-gonbita administratzaile gisa eta burutu iisreset

![IIS berrezartzea.](./media/9IISReset.png)

18. Itxi urruneko mahaigaineko saioa eta erabili LCS **Ingurumenaren xehetasunak** orria ingurunean saioa hasteko espero bezala funtzionatzen duela baieztatzeko.

![Finantza eta Eragiketak.](./media/10FinanceAndOperations.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]