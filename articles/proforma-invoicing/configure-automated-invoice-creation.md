---
title: Konfiguratu fakturak automatikoak sortzeko aukera
description: Gai honetan sistemak fakturak automatikoki sortzeko konfiguratzeko moduari buruzko informazioa ematen du.
author: rumant
ms.date: 10/13/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 43b75ea823a62acaab708a1ef2fa2467904fdd00
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8583386"
---
# <a name="configure-automatic-invoice-creation"></a>Konfiguratu fakturak automatikoak sortzeko aukera

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_


Bete urrats hauek Dynamics 365 Project Operations-en faktura automatikoa exekutatzeko.

1. Joan **Ezarpenak** > **Lan sortak** atalera.
2. Sortu lan-sortat eta eman izen hau: **Project eragiketek fakturak sortzea**. Lan-sortaren izenak "sortu fakturak" hitzak izan behar ditu.
3. **Lan mota** eremuan, hautatu **Bat ere ez** aukera. Berez, **Maiztasuna egunero** eta **Aktibatuta dago** aukerak ezarrita daude **Bai** aukerarekin.
4. Hautatu **Lan-fluxua exekutatu**. **Begiratu erregistroa** elkarrizketa-koadroan, hiru lan-fluxu ikusiko dituzu:

    - ProcessRunCaller
    - ProcessRunner
    - UpdateRoleUtilization

5. Hautatu **ProcessRunCaller** eta gero hautatu **Gehitu**.
6. Berrespenaren hurrengo elkarrizketa-koadroan, hautatu **Ados**. **Lo** lan-fluxuaren ondoren dator **Prozesua** lan-fluxua.

  > [!NOTE]
  > Aukeratu ere egin dezakezu **ProcessRunner** 5. urratsean. Ondoren, hautatzen duzunean **Ados** aukera, **Prozesua** lan-fluxuaren ondoren dator **Lo** lan-fluxua.

**ProcessRunCaller** eta **ProcessRunner** lan-fluxuek fakturak sortzen dituzte. **ProcessRunCaller** lan-fluxuak **ProcessRunner** lan-fluxuari deitzen dio. **ProcessRunner** fakturak benetan sortzen dituen lan-fluxua da. Fakturak sortu behar diren kontraturen lerro guztietatik igarotzen da eta fakturak sortzen ditu lerro horietarako. Fakturak eratu behar diren kontratuaren lerroak zehazteko, lanpostuak kontratuaren lerroen fakturazio datak aztertzen ditu. Kontratu bakarreko kontratuaren lerroek fakturaren iraupen-data bera badute, transakzioak bi faktura-lerro dituen faktura batean elkartzen dira. Fakturak sortzeko transakziorik ez badago, lanak fakturaren sorrera saltatzen du.

**ProcessRunner** exekutatzen amaitu denean, **ProcessRunCaller** lan-fluxuari deitzen dio, amaiera-ordua ematen du eta itxita dago. **ProcessRunCaller** lan-fluxuak, ondoren, zehaztutako amaiera-ordutik 24 orduz iraungo duen tenporizadorea hasten du. Tenporizadorearen amaieran, **ProcessRunCaller** lan-fluxua itxita dago.

Lan-sortaren prozesua lan errepikaria da. Prozesu-sorta hau askotan exekutatzen bada, lanaren zenbait kasu sortzen dira eta akatsak sor daitezke. Hori dela eta, prozesu-sorta behin bakarrik hasi beharko zenuke eta exekutatzen gelditzen bada bakarrik berrabiarazi beharko zenuke.

> [!NOTE]
> Sortako fakturazioa fakturen egutegien arabera konfiguratutako proiektuen kontratu lerroetarako bakarrik exekutatzen da. Prezio finkoko fakturazio metodoa duen kontratu-lerroak mugarriak konfiguratu behar ditu. Ordua eta materiala fakturatzeko metodoa duen proiektu-kontratuen lerroak fakturen egitaraua finkatuko du. Gauza bera gertatzen da proiektuan oinarritutako kontratu lerroan.     


[!INCLUDE[footer-include](../includes/footer-banner.md)]