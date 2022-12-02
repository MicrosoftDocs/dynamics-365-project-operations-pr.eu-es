---
title: Proiektuko taldekideak azpikontratatzeko aukerak
description: Artikulu honek Microsoft Dynamics 365 Project Operations-en proiektuko taldekideentzako azpikontratazio aukerak azaltzen ditu.
author: rumant
ms.date: 09/14/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 046b5d38ef7e433d02e3eac2e858a3333e941c45
ms.sourcegitcommit: 08eb3be9eda44e9446c43ed9b6aefd58d77927c5
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/15/2022
ms.locfileid: "9522263"
---
# <a name="subcontracting-options-for-project-team-members"></a>Proiektuko taldekideak azpikontratatzeko aukerak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Microsoft Dynamics 365 Project Operations-en, proiektuko taldekide bat edo gehiagorentzat dauden azpikontratazio aukerak ebalua ditzakezu. Eskuragarri dagoen azpikontratatzeko aukerek hau ahalbidetzen dute:

- Sortu azpikontratu berri bat eta/edo sortu lehendik dagoen azpikontratu batean lerro berriak hautatutako proiektu-taldekideentzat. 
- Egin erreserbak lehendik dauden azpikontratu eta azpikontratuaren lerroan. 

Eskuragarri dauden azpikontratazio-aukeretatik aukera dezakezu proiektu-talde generikoko kideentzat edo kontratu-langilea den baliabide izendun batekin hornitutako proiektu-taldekideen artean aukeratu. 

Ez dago azpikontratazio aukerarik honetarako:

- Langile batekin lan egin duten proiektuko taldeko kideak. 
- Azpikontratu eta azpikontratuaren lerroarekin erlazionatutako proiektuaren taldeko kideak. 

## <a name="subcontracting-an-unstaffed-project-team-member"></a>Kontratatu gabeko proiektuko taldekideak azpikontratatzeko aukerak

Proiektuko taldekide generiko edo langilerik gabeko baten azpikontratazio-aukerak berrikusteko eta aukeratzeko, jarraitu urrats hauek:

1. Hautatu proiektuko taldeko kideen erregistro bat edo gehiago non baliabidea baliabide generikoa den.
2. Ziurtatu hautatutako proiektuko taldekideen erregistroetako bat ere ez dagoela jada azpikontratatuta. 
3. Hautatu **Azpikontratazio aukerak** proiektuko taldekideen azpi-saretan. **Azpikontratazio aukerak** elkarrizketa irekiko da: 
4. 1. urratsean proiektuko taldeko kideen erregistro bakarra hautatu baduzu, aukera hauek egongo dira eskuragarri:
    - Azpikontratuaren lerro berriak sortu. 
    - Erreserbatu lehendik dagoen azpikontratu baten aurka 1. urratsean proiektuko taldekideen erregistro anitz hautatu badituzu, eskuragarri dagoen aukera bakarra azpikontratazio lerro berri bat sortzea da.
5. Lehendik dagoen azpikontratazio-lerro baten aurka erreserbatzeko aukerak erreserbatu nahi duzun azpikontratazio eta azpikontratazio-lerro bat hautatzeko aukera ematen du. Ahalmena erreserbatzeko azpikontratazio-lerroa hautatzen duzunean, hautatutako azpikontratazio-lerroa denborarako dela ziurtatu behar duzu eta proiektuko taldekideari eskatutako rola bat datorrela azpikontratazio-lerroan erositako rolarekin.
6. Proiektuko taldekideentzako azpikontratazio-lerro berriak sortzea hautatzen duzunean, sistemak lerro hauek sortu nahi dituzun azpikontratazioa hautatzeko aukera emango dizu. Lerro berriak sortzeko hautatzen duzun azpikontrata egon beharko litzateke **Zirriborroa** egoera. Hautatutako proiektu-taldekideentzat azpikontratazio-lerro berriak sortzeko aukera honekin, sistemak denborarako azpikontratazio-lerro bat sortuko du proiektuko taldekide bakoitzarentzat. Eginkizuna, orduak eta datak proiektuko taldekidearengandik kopiatuko dira sortzen den azpikontratazio lerro bakoitzean. 
7. Taldekide generiko bat azpikontratu eta azpikontratu lerro batekin lotzen denean, hau **Langile mota** taldekideen errenkadako eremu orokorrean eguneratuko da **Lan-kontratuko langilea** eta **Azpikontratuaren indarraldia** balioa ezarriko da **Baliozkoa**.

## <a name="subcontracting-a-staffed-project-team-member"></a>Kontratatutako proiektuko taldekideak azpikontratatzeko aukerak

Langilerik gabeko taldekide generikoak edo langilerik gabekoak bezala, proiektuko taldekide batentzako azpikontratazio-aukerak ere ikus ditzakezu, betiere langile-taldekidea kontratuko langilea bada. Proiektuko taldekide generiko edo langilerik gabeko baten azpikontratazio-aukerak berrikusteko eta aukeratzeko, jarraitu urrats hauek:

1. Hautatu proiektuko taldeko kideen erregistro bat edo gehiago non izendatutako kontratu langilea generikoa den.
2. Ziurtatu hautatutako proiektuko taldekideen erregistroetako bat ere ez dagoela jada azpikontratatuta. 
3. Hautatu **Azpikontratazio aukerak** proiektuko taldekideen azpi-saretan. **Azpikontratazio aukerak** elkarrizketa irekiko da: 
4. 1. urratsean proiektuko taldeko kideen erregistro bakarra hautatu baduzu, aukera hauek egongo dira eskuragarri:
      - Azpikontratuaren lerro berriak sortu.
      - Erreserbatu lehendik dagoen Azpikontratu batetik.
  1. urratsean proiektuko taldekideen erregistro anitz hautatu badituzu, eskuragarri dagoen aukera bakarra azpikontratazio lerro berri bat sortzea da.
5. Lehendik dagoen azpikontratazio-lerro baten aurka erreserbatzeko aukerak erreserbatu nahi duzun azpikontratazio eta azpikontratazio-lerro bat hautatzeko aukera ematen du. Ahalmena erreserbatzeko azpikontratazio linea bat hautatzerakoan, honako hau ziurtatu beharko zenuke:
      - Hautatutako azpikontratazio lerroa denborarako da. 
      - Proiektuko taldekideari eskatzen zaion rola bat dator azpikontratazio lerroan erositako rolarekin. 
      - Lan-kontratuko langilea lotzen den saltzailea azpikontratuko saltzailea bera da.
6. Proiektuko taldekideentzako azpikontratazio-lerro berriak sortzea hautatzen duzunean, sistemak lerro hauek sortu nahi dituzun azpikontratazioa hautatzeko aukera emango dizu. Aukera honekin, ziurtatzen da lan-kontratuko langilea lotzen den saltzailea azpikontratuko saltzailea bera da. 
7. Lerro berriak sortzeko hautatzen duzun azpikontrata egon beharko litzateke **Zirriborroa** egoera. Hautatutako proiektu-taldekideentzat azpikontratazio-lerro berriak sortzeko aukera honekin, sistemak denborarako azpikontratazio-lerro bat sortuko du proiektuko taldekide bakoitzarentzat. Eginkizuna, orduak eta datak proiektuko taldekidearengandik kopiatuko dira sortzen den azpikontratazio lerro bakoitzean.  
8. Taldekide generiko bat azpikontratu eta azpikontratu lerro batekin lotzen denean, hau **Langile mota** taldekideen errenkadako eremu orokorrean eguneratuko da **Lan-kontratuko langilea** eta **Azpikontratuaren indarraldia** balioa ezarriko da **Baliozkoa**.

## <a name="re-costing-subcontractor-assignments"></a>Azpikontratistaren esleipenak birkostua

Proiektuko taldekide bat (generikoa edo izenduna) azpikontratazio-lerroekin lotuta dagoenean **Azpikontratazio aukerak** elkarrizketa-koadroa, taldekideak dituen zereginen esleipenak berriro kostua izango dira azpikontratuari atxikitako erosketa prezioen zerrendan oinarrituta. **Estimazioak** fitxan **Proiektuaren xehetasunak** orrialdea, hautatu **eguneratu prezioak** botoia azpikontratatzeko erabakiaren ondoriozko prezio eguneratuak edo/eta kostuak ikusteko.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
