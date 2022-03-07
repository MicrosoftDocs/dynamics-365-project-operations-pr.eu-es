---
title: Proiektuko taldekideentzako azpikontratazio aukerak
description: Gai honek Microsoft-en proiektuko taldekideen azpikontratazio aukerak azaltzen ditu Dynamics 365 Project Operations.
author: rumant
ms.date: 12/03/2021
ms.topic: article
ms.reviewer: tonyafehr
ms.author: rumant
ms.openlocfilehash: 4db283db728b50ccf76eafabfd643313620bbce2
ms.sourcegitcommit: 45893132bd8bfaf944ee0ac855484684dd1ee945
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/09/2021
ms.locfileid: "7902985"
---
# <a name="subcontracting-options-for-project-team-members"></a>Proiektuko taldekideentzako azpikontratazio aukerak

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Microsoft-en Dynamics 365 Project Operations, proiektuko taldekide bat edo gehiagorentzat dauden azpikontratazio aukerak ebalua ditzakezu. Eskuragarri dauden azpikontratazio-aukerek aukera ematen dute:

- Sortu azpikontratu berri bat eta/edo sortu lehendik dagoen azpikontratu batean lerro berriak hautatutako proiektu-taldekideentzat. 
- Erreserbatu lehendik dagoen azpikontratu eta azpikontratu lerro baten aurrean. 

Eskuragarri dauden azpikontratazio-aukeretatik aukera dezakezu proiektu-talde generikoko kideentzat edo kontratu-langilea den baliabide izendun batekin hornitutako proiektu-taldekideen artean aukeratu. 

Ez dago azpikontratazio aukerarik honako hauetarako:

- Langile batekin lan egin duten proiektuko taldeko kideak. 
- Dagoeneko azpikontratu eta azpikontratu lerro bati lotuta dauden proiektu-taldekideak. 

## <a name="subcontracting-an-unstaffed-project-team-member"></a>Langilerik gabeko proiektuko taldekide bat azpikontratatzea

Proiektuko taldekide generiko edo langilerik gabeko baten azpikontratazio aukeren artean eskuragarri dauden berrikusi eta aukeratzeko, jarraitu urrats hauek:

1. Hautatu proiektuko taldeko kideen erregistro bat edo gehiago non baliabidea baliabide generikoa den.
2. Ziurtatu hautatutako proiektuko taldekideen erregistroetako bat ere ez dagoela jada azpikontratatuta. 
3. Hautatu **Azpikontratazio aukerak** proiektuko taldekideen azpi-saretan. The **Azpikontratazio aukerak** elkarrizketa-koadroa irekitzen da. 
4. 1. urratsean proiektuko taldeko kideen erregistro bakarra hautatu baduzu, aukera hauek egongo dira eskuragarri:
    - Sortu azpikontratazio lerro berriak. 
    - Erreserbatu lehendik dagoen azpikontratu baten aurka 1. urratsean proiektuko taldekideen erregistro bat baino gehiago hautatu badituzu, eskuragarri dagoen aukera bakarra azpikontratu lerro berri bat sortzea da.
5. Lehendik dagoen azpikontratazio-lerro baten aurka erreserbatzeko aukerak erreserbatu nahi duzun azpikontratazio eta azpikontratazio-lerro bat hautatzeko aukera ematen du. Ahalmena erreserbatzeko azpikontratazio-lerroa hautatzen duzunean, hautatutako azpikontratazio-lerroa denborarako dela ziurtatu behar duzu eta proiektuko taldekideari behar den rola bat datorrela azpikontratazio-lerroan erositako rolarekin.
6. Proiektuko taldekideentzako azpikontratazio-lerro berriak sortzea hautatzen duzunean, sistemak lerro hauek sortu nahi dituzun azpikontratazioa hautatzeko aukera emango dizu. Lerro berriak sortzeko hautatzen duzun azpikontrata egon beharko litzateke **Zirriborroa** egoera. Hautatutako proiektu-taldekideentzat azpikontratazio-lerro berriak sortzeko aukera honekin, sistemak denborarako azpikontratazio-lerro bat sortuko du proiektuko taldekide bakoitzarentzat. Eginkizuna, orduak eta datak proiektuko taldekidearengandik kopiatuko dira sortzen den azpikontratazio lerro bakoitzean. 
7. Taldekide generiko bat azpikontratu eta azpikontratu lerro batekin lotuta dagoenean, **Langile mota** taldekideen errenkada generikoko eremua eguneratuko da **Lan-kontratuko langilea** eta **Azpikontratuaren Indarraldia** balioa ezarriko da **Baliozkoa**.

## <a name="subcontracting-a-staffed-project-team-member"></a>Proiektuko taldekide bat azpikontratatzea

Langilerik gabeko taldekide generikoak edo langilerik gabekoak bezala, proiektuko taldekide baten azpikontratazio-aukerak ere ikus ditzakezu, betiere langiledun taldekidea kontratudun langilea bada. Langiledun edo izendatutako proiektuko taldekide baten azpikontratazio aukeren artean berrikusi eta aukeratzeko, jarraitu urrats hauek:

1. Hautatu proiektu-taldeko kideen erregistro bat edo gehiago non baliabidea izendatutako kontratu-langile bat den.
2. Ziurtatu hautatutako proiektuko taldekideen erregistroetako bat ere ez dagoela jada azpikontratatuta. 
3. Hautatu **Azpikontratazio aukerak** proiektuko taldekideen azpi-saretan. The **Azpikontratazio aukerak** elkarrizketa-koadroa irekitzen da. 
4. 1. urratsean proiektuko taldeko kideen erregistro bakarra hautatu baduzu, aukera hauek egongo dira eskuragarri:
      - Sortu azpikontratazio lerro berriak.
      - Erreserbatu lehendik dagoen azpikontratu baten aurrean.
  1. urratsean proiektuko taldekideen erregistro anitz hautatu badituzu, eskuragarri dagoen aukera bakarra azpikontratazio-lerro berri bat sortzea da.
5. Lehendik dagoen azpikontratazio-lerro baten aurka erreserbatzeko aukerak erreserbatu nahi duzun azpikontratazio eta azpikontratazio-lerro bat hautatzeko aukera ematen du. Ahalmena erreserbatzeko azpikontratazio-linea hautatzen duzunean, honako hau ziurtatu beharko zenuke:
      - Aukeratutako azpikontratazio lerroa denborarako da. 
      - Proiektuko taldekideari eskatzen zaion rola bat dator azpikontratazio lerroan erositako rolarekin. 
      - Lan-kontratuko langilea lotzen den saltzailea azpikontratuko saltzailea bera da.
6. Proiektuko taldekideentzako azpikontratazio-lerro berriak sortzea hautatzen duzunean, sistemak lerro hauek sortu nahi dituzun azpikontratazioa hautatzeko aukera emango dizu. Aukera honekin, ziurtatu beharko zenuke lan-kontratuko langilearen saltzailea azpikontratuko saltzailea bera dela. 
7. Lerro berriak sortzeko hautatzen duzun azpikontrata egon beharko litzateke **Zirriborroa** egoera. Hautatutako proiektu-taldekideentzat azpikontratazio-lerro berriak sortzeko aukera honekin, sistemak denborarako azpikontratazio-lerro bat sortuko du proiektuko taldekide bakoitzarentzat. Eginkizuna, orduak eta datak proiektuko taldekidearengandik kopiatuko dira sortzen den azpikontratazio lerro bakoitzean.  
8. Izendatutako taldekide bat azpikontratu eta azpikontratu lerro batekin lotuta dagoenean, **Langile mota** izendatutako taldekideen errenkadako eremua eguneratuko da **Lan-kontratuko langilea** eta **Azpikontratuaren Baliotasuna** balioa ezarriko da **Baliozkoa**.

## <a name="re-costing-subcontractor-assignments"></a>Azpikontratistaren esleipenak birkostua

Proiektuko taldekide bat (generikoa edo izenduna) azpikontratazio-lerroekin lotuta dagoenean **Azpikontratazio aukerak** elkarrizketa-koadroa, taldekideak dituen zereginen esleipenak berriro kostua izango dira azpikontratuari atxikitako erosketa prezioen zerrendan oinarrituta. Gainean **Estimazioak** fitxan **Proiektuaren xehetasunak** orrialdea, hautatu **Eguneratu prezioak** botoia azpikontratatzeko erabakiaren ondoriozko prezio eguneratuak edo/eta kostuak ikusteko.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
