---
title: Konfiguratu fakturen sortze automatikoa
description: Gai honek proformako fakturak automatikoki sortzeari eta konfiguratzeari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 04/05/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 027cc711d53c7dd8512e6ef416b54e320357dd26
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8584075"
---
# <a name="set-up-automatic-invoice-creation"></a>Konfiguratu fakturen sortze automatikoa 
 
_**Honetarako aplikatzen da:** inplementazio arina - mahukatik proformako fakturaziora, Baliabideen / stockean oinarritutako eszenatokien Project Operations_

Fakturen sortze automatikoa konfigura dezakezu Dynamics 365 Project Operations-en. Sistemak proforma faktura zirriborro bat sortzen du proiektuaren kontratu eta kontratu lerro bakoitzaren faktura egutegian oinarrituta. Fakturen ordutegiak kontratu lerro mailan konfiguratuta daude. Kontratu bateko lerro bakoitzak faktura ordutegi desberdina izan dezake, edo faktura ordutegi bera kontratuaren lerro guztietan sar daiteke.

Faktura bat sortzen duzunean, sistemak gutxienez faktura bat sortzen du proiektuaren kontratu bakoitzeko. Zenbait kasutan, hainbat faktura sor daitezke. Adibidez, kontratuak bezero anitz baditu, faktura kopuru bera sortuko da proiektuaren kontratu horretan fakturatzeko fakturagarriak diren eragiketak dituzten bezeroen kopurua.

## <a name="understand-how-transactions-are-included-on-an-invoice"></a>Ulertu transakzioak nola sartzen diren faktura batean 

Batzuetan, proiektuan oinarritutako kontratu lerro bakoitzak faktura ordutegi bereizi bat zehazten du. Adibidez, Adatum kontratua gauzatzeko zerbitzuek kontratu lerro hauek dituzte:

- Eskuz sortutako bi mugarri dituen prezio finkoa duen prototipo lana.
- Denbora barne hartzen duen eta astelehenero bi astero fakturatuko den ezarpen lana.
- Hilabeteko lehen astelehenean hilero fakturatu behar diren gastuak.

Bi lerro-elementu horietako bakoitzean zehaztutako fakturen ordutegiek honako taula itxura dute:

| Kontratuaren lerroa | Fakturaren sorrera-data | Transakzioa erabilgarri dagoen azken eguna | Mugarriaren data | Mugarriaren zenbatekoa |
| --- | --- | --- | --- | --- |
| Prototipoaren lana | Urriak 5, astelehena | - | Urriak 5, astelehena | 5000 USD |
| - | Azaroak 3, asteartea | - | Azaroak 3, asteartea | 12,000 USD |
| Inplementazio-lana | Urriak 5, astelehena | Urriak 4, igandea | - | - |
| - | Urriak 19, astelehena | Urriak 18, igandea | - | - |
| - | Azaroak 2, astelehena | Azaroak 1, igandea | - | - |
| - | Azaroak 16, astelehena | Azaroak 15, igandea | - | - |
| Egindako gastuak | Urriak 5, astelehena | Urriak 4, igandea | - | - |
| - | Azaroak 2, astelehena | Azaroak 1, igandea | - | - |

Fakturazio automatikoa martxan dagoenean adibide honetan:

- **Urriaren 4a edo aurreko edozein data**: Ez da fakturarik sortu kontratu honengatik **Fakturen ordutegia** Kontratu-linea horietako bakoitzaren taulak ez du urriaren 4a, igandea deitzen, faktura exekutatzeko data gisa.
- **Urriak 5, astelehena**: Faktura bat sortzen da honetarako:

    - Mugarria barne hartzen duen prototipo lana, gisa markatuta badago **Fakturatzeko prest**.
    - Urriak 4, igandea, transakzioaren amaiera eguna baino lehen sortutako Denborazko transakzio guztiak biltzen dituen inplementazio lana, honela markatuta dagoena **Fakturatzeko prest**.
    - Urriak 4, igandea, transakzioaren amaiera eguna baino lehen sortutako Gastuen transakzio guztiak biltzen dituen egindako gastuak, honela markatuta dagoena **Fakturatzeko prest**.
  
- **Urriaren 6an edo urriak 19 baino aurreko edozein data**: Ez da fakturarik sortu kontratu honengatik **Fakturen ordutegia** Kontratu-linea horietako bakoitzaren taulak ez du urriaren 6 edo urriaren 19 baino aurreko edozein data deitzen, faktura exekutatzeko data gisa.
- **Urriak 19, astelehena**: Urriak 18, igandea, transakzioaren amaiera eguna baino lehen sortutako Denborazko transakzio guztiak biltzen dituen inplementazio lanaren faktura bat sortu da, honela markatuta dagoena **Fakturatzeko prest**.
- **Azaroak 2, astelehena**: Faktura bat sortzen da honetarako:

    - Azaroak 1, igandea, transakzioaren amaiera eguna baino lehen sortutako Denborazko transakzio guztiak biltzen dituen inplementazio lana, honela markatuta dagoena **Fakturatzeko prest**.
    - Azaroak 1, igandea, transakzioaren amaiera eguna baino lehen sortutako Gastuen transakzio guztiak biltzen dituen egindako gastuak, honela markatuta dagoena **Fakturatzeko prest**.

- **Azaroak 3, asteartea**: Faktura bat sortzen da 12000 USD-en mugarria barne hartzen duen prototipo lanetarako, gisa markatuta badago **Fakturatzeko prest**.

## <a name="configure-automatic-invoicing"></a>Konfiguratu fakturatze automatikoa

Osatu urrats hauek exekutatutako faktura automatikoa konfiguratzeko.

1. **Project Operations** aukeran, joan **Ezarpenak** > **Aldizkako faktura konfiguratzea** aukerara.
2. Sortu lan-sorta eta eman izen hau: **Project Operations fakturak sortzea**. Lan-sortaren izenak "sortu fakturak" hitzak izan behar ditu.
3. **Lan mota** eremuan, hautatu **Bat ere ez** aukera. Lehenespenez, **Maiztasuna egunero** eta **Aktibatuta dago** eremuak ezarrita daude **Bai** aukerarekin.
4. Hautatu **Lan-fluxua exekutatu**. **Begiratu erregistroa** elkarrizketa-koadroan, hiru lan-fluxu ikusiko dituzu:

- ProcessRunCaller
- ProcessRunner
- UpdateRoleUtilization

5. Hautatu **ProcessRunCaller** eta gero hautatu **Gehitu**.
6. Berrespenaren hurrengo elkarrizketa-koadroan, hautatu **Ados**. **Lo** lan-fluxuaren ondoren dator **Prozesua** lan-fluxua. 

> [!NOTE]
> Aukeratu ere egin dezakezu **ProcessRunner** 5. urratsean. Ondoren, hautatzen duzunean **Ados** aukera, **Prozesua** lan-fluxuaren ondoren dator **Lo** lan-fluxua.

**ProcessRunCaller** eta **ProcessRunner** lan-fluxuek fakturak sortzen dituzte. **ProcessRunCaller** lan-fluxuak **ProcessRunner** lan-fluxuari deitzen dio. **ProcessRunner** fakturak benetan sortzen dituen lan-fluxua da. Fakturak sortu behar diren kontraturen lerro guztietatik igarotzen da lan-fluxua eta fakturak sortzen ditu lerro horietarako. Fakturak eratu behar diren kontratuaren lerroak zehazteko, lanpostuak kontratuaren lerroen fakturazio datak aztertzen ditu. Kontratu bakarreko kontratuaren lerroek fakturaren iraupen-data bera badute, transakzioak bi faktura-lerro dituen faktura batean elkartzen dira. Fakturak sortzeko transakziorik ez badago, lanak faktura sortzea saltatzen du.

**ProcessRunner** exekutatzen amaitu denean, **ProcessRunCaller** lan-fluxuari deitzen dio, amaiera-ordua ematen du eta itxita dago. **ProcessRunCaller** lan-fluxuak, ondoren, zehaztutako amaiera-ordutik 24 orduz iraungo duen tenporizadorea hasten du. Tenporizadorearen amaieran, **ProcessRunCaller** lan-fluxua itxita dago.

Lan-sortaren prozesua lan errepikaria da. Prozesu-sorta hau askotan exekutatzen bada, lanaren zenbait kasu sortzen dira eta akatsak sor daitezke. Hori dela eta, prozesu-sorta behin bakarrik hasi beharko zenuke eta exekutatzen gelditzen bada bakarrik berrabiarazi beharko zenuke.

> [!NOTE]
> Project Operations-eko sortako fakturazioa fakturen egutegien arabera konfiguratutako proiektuen kontratu lerroetarako bakarrik exekutatzen da. Prezio finkoko fakturazio metodoa duen kontratu-lerroak mugarriak konfiguratu behar ditu. Ordua eta materiala fakturatzeko metodoa duen proiektu-kontratuen lerroak fakturen egitaraua finkatuko du.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
