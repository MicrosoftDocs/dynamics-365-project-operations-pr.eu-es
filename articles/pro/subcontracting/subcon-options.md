---
title: Proiektuko taldekideak azpikontratatzeko aukerak
description: Artikulu honek Microsoft-en proiektuko taldekideen azpikontratazio aukerak azaltzen ditu Dynamics 365 Project Operations.
author: rumant
ms.date: 12/03/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 5e0955d58365a4ecbe1c053882736f196758816e
ms.sourcegitcommit: b2224d1f3c0bd4925d647e6ca3960db81a209521
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/11/2022
ms.locfileid: "9261590"
---
# <a name="subcontracting-options-for-project-team-members"></a>Proiektuko taldekideak azpikontratatzeko aukerak

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Microsoft-en Dynamics 365 Project Operations, proiektuko taldekide bat edo gehiagorentzat dauden azpikontratazio aukerak ebalua ditzakezu. Eskuragarri dauden azpikontratazio aukerek aukera ematen dute:

- Sortu azpikontratu berri bat eta/edo sortu lehendik dagoen azpikontratu batean lerro berriak hautatutako proiektu-taldekideentzat. 
- Erreserbatu lehendik dagoen azpikontratu eta azpikontratazio lerro baten aurrean. 

Eskuragarri dauden azpikontratazio-aukeretatik aukera dezakezu proiektu-talde generikoko kideentzat edo kontratu-langilea den baliabide izendun batekin hornitutako proiektu-taldekideen artean aukeratu. 

Ez dago azpikontratazio aukerarik honako hauetarako:

- Langile batekin lan egin duten proiektuko taldeko kideak. 
- Dagoeneko azpikontratu eta azpikontratu lerro bati lotuta dauden proiektu-taldekideak. 

## <a name="subcontracting-an-unstaffed-project-team-member"></a>Langilerik gabeko proiektuko taldekide bat azpikontratatzea

Proiektuko taldekide generiko edo langilerik gabeko baten azpikontratazio-aukerak berrikusi eta aukeratzeko, jarraitu urrats hauek:

1. Hautatu proiektuko taldeko kideen erregistro bat edo gehiago non baliabidea baliabide generikoa den.
2. Ziurtatu hautatutako proiektuko taldekideen erregistroetako bat ere ez dagoela jada azpikontratatuta. 
3. Hautatu **Azpikontratazio aukerak** proiektuko taldekideen azpi-saretan. The **Azpikontratazio aukerak** elkarrizketa-koadroa irekitzen da. 
4. 1. urratsean proiektuko taldeko kideen erregistro bakarra hautatu baduzu, aukera hauek egongo dira eskuragarri:
    - Sortu azpikontratazio lerro berriak. 
    - Erreserbatu lehendik dagoen azpikontratu baten aurka 1. urratsean proiektuko taldekideen erregistro bat baino gehiago hautatu badituzu, erabilgarri dagoen aukera bakarra azpikontratu lerro berri bat sortzea da.
5. Lehendik dagoen azpikontratazio-lerro baten aurka erreserbatzeko aukerak erreserbatu nahi duzun azpikontratazio eta azpikontratazio-lerro bat hautatzeko aukera ematen du. Ahalmena erreserbatzeko azpikontratazio-lerroa hautatzen duzunean, hautatutako azpikontratazio-lerroa denborarako dela eta proiektuko taldekideari eskatutako rola azpikontratazio-lerroan erositako rolarekin bat datorrela ziurtatu behar duzu.
6. Proiektuko taldekideentzako azpikontratazio lerro berriak sortzea hautatzen duzunean, sistemak lerro hauek sortu nahi dituzun azpikontratazioa hautatzeko aukera emango dizu. Lerro berriak sortzeko hautatzen duzun azpikontrata egon beharko litzateke **Zirriborroa** egoera. Hautatutako proiektu-taldekideentzat azpikontratazio-lerro berriak sortzeko aukera honekin, sistemak denborarako azpikontratazio-lerro bat sortuko du proiektuko taldekide bakoitzarentzat. Eginkizuna, orduak eta datak proiektuko taldekidearengandik kopiatuko dira sortzen den azpikontratazio lerro bakoitzean. 
7. Taldekide generiko bat azpikontratu eta azpikontratu lerro batekin lotuta dagoenean, **Langile mota** taldekideen errenkadako eremu orokorrean eguneratuko da **Lan-kontratuko langilea** eta **Azpikontratuaren indarraldia** balioa ezarriko da **Baliozkoa**.

## <a name="subcontracting-a-staffed-project-team-member"></a>Proiektuko taldekide bat azpikontratatzea

Langilerik gabeko taldekide generikoak edo langilerik gabekoak bezala, proiektuko taldekide baten azpikontratazio-aukerak ere ikus ditzakezu, betiere langile-taldekidea kontratuko langilea bada. Langiledun edo izendatutako proiektuko taldekide baten azpikontratazio aukeren artean berrikusi eta aukeratzeko, jarraitu urrats hauek:

1. Hautatu proiektuko taldekideen erregistro bat edo gehiago non baliabidea izendatzen den lan-kontratuko langile bat den.
2. Ziurtatu hautatutako proiektuko taldekideen erregistroetako bat ere ez dagoela jada azpikontratatuta. 
3. Hautatu **Azpikontratazio aukerak** proiektuko taldekideen azpi-saretan. The **Azpikontratazio aukerak** elkarrizketa-koadroa irekitzen da. 
4. 1. urratsean proiektuko taldeko kideen erregistro bakarra hautatu baduzu, aukera hauek egongo dira eskuragarri:
      - Sortu azpikontratazio lerro berriak.
      - Erreserbatu lehendik dagoen azpikontratu baten aurrean.
  1. urratsean proiektuko taldekideen hainbat erregistro hautatu badituzu, eskuragarri dagoen aukera bakarra azpikontratazio-lerro berriak sortzea da.
5. Lehendik dagoen azpikontratazio-lerro baten aurka erreserbatzeko aukerak erreserbatu nahi duzun azpikontratazio eta azpikontratazio-lerro bat hautatzeko aukera ematen du. Ahalmena erreserbatzeko azpikontratazio linea bat hautatzerakoan, honako hau ziurtatu beharko zenuke:
      - Hautatutako azpikontratazio lerroa denborarako da. 
      - Proiektuko taldekideari eskatzen zaion rola bat dator azpikontratazio lerroan erositako rolarekin. 
      - Lan-kontratuko langilea lotzen den saltzailea azpikontratuko saltzailea bera da.
6. Proiektuko taldekideentzako azpikontratazio lerro berriak sortzea hautatzen duzunean, sistemak lerro hauek sortu nahi dituzun azpikontratazioa hautatzeko aukera emango dizu. Aukera honekin, lan-kontratuko langilearen saltzailea azpikontratuko saltzailea bera dela ziurtatu beharko zenuke. 
7. Lerro berriak sortzeko hautatzen duzun azpikontrata egon beharko litzateke **Zirriborroa** egoera. Hautatutako proiektu-taldekideentzat azpikontratazio-lerro berriak sortzeko aukera honekin, sistemak denborarako azpikontratazio-lerro bat sortuko du proiektuko taldekide bakoitzarentzat. Eginkizuna, orduak eta datak proiektuko taldekidearengandik kopiatuko dira sortzen den azpikontratazio lerro bakoitzean.  
8. Izendatutako taldekide bat azpikontratu eta azpikontratu lerro batekin lotuta dagoenean, **Langile mota** izendatutako taldekideen errenkadan eremua eguneratuko da **Lan-kontratuko langilea** eta **Azpikontratuaren indarraldia** balioa ezarriko da **Baliozkoa**.

## <a name="re-costing-subcontractor-assignments"></a>Azpikontratistaren esleipenak berriro kostua

Proiektuko taldekide bat (generikoa edo izenduna) azpikontratazio-lerroekin lotuta dagoenean **Azpikontratazio aukerak** elkarrizketa-koadroa, taldekideak dituen zereginen esleipenak berriro kostua izango dira azpikontratuari atxikitako erosketa prezioen zerrendan oinarrituta. Gainean **Estimazioak** fitxan **Proiektuaren xehetasunak** orrialdea, hautatu **Eguneratu prezioak** botoia azpikontratatzeko erabakiaren ondoriozko prezio eguneratuak edo/eta kostuak ikusteko.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
