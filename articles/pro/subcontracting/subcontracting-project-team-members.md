---
title: Proiektuko taldekideak azpikontratatzea
description: Artikulu honek Microsoft-en proiektuko taldeko kideak nola azpikontratatu azaltzen du Dynamics 365 Project Operations.
author: rumant
ms.date: 9/14/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: a2f17d6f270029e3a517e99c7bb518cdb19b8d23
ms.sourcegitcommit: 08eb3be9eda44e9446c43ed9b6aefd58d77927c5
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/15/2022
ms.locfileid: "9522780"
---
# <a name="subcontracting-project-team-members"></a>Proiektuko taldekideak azpikontratatzea

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Microsoft-en Dynamics 365 Project Operations, langilerik gabeko edo langilerik gabeko proiektuko taldekideak azpikontratatzea aukera dezakezu.

- Langilerik gabeko proiektuko taldekideek baliabide generiko bat dute esleituta.
- Langileen taldekideek baliabide izendatua dute.

Proiektu-taldeko kide bat azpikontratu-lerro batekin lotzen duzunean, taldekideak dituen zereginen esleipenak azpikontratuari atxikitako erosketa-prezioen zerrendan oinarrituta egingo dira.  Gainean **Estimazioak** fitxan **Proiektuaren xehetasunak** orrialdea, hautatu **Eguneratu prezioak** botoia azpikontratatzeko erabakiaren ondoriozko prezio eguneratuak eta/edo kostuak ikusteko. 

## <a name="subcontracting-an-unstaffed-project-team-member"></a>Langilerik gabeko proiektuko taldekide bat azpikontratatzea
The **Taldekidearen xehetasunak** orrialdeak azpikontratazio eta azpikontratazio lerro-eremuak ditu, proiektuaren kudeatzaile bati azpikontratu batetik eskatutako ahalmena nola atera nahiko lukeen adierazteko aukera ematen diotenak. Proiektuko taldekide bat baliabide generiko gisa azpikontratatzeko, jarraitu urrats hauek:

1.  Aukeratu azpikontratu bat **Taldekidearen xehetasuna** orrialdea.

2.  Honekin soilik hauta ditzakezu azpikontratuak **Zirriborroa** edo **Baieztatuta** egoera. **Itxita** edo **Bertan behera utzita** ezin dira azpikontratuak hautatu. 

3.  The **Azpikontratazio lerroa** eremua ikusgai geratzen da azpikontratu bat hautatu ondoren.

4.  urtean **Azpikontratazio lerroa** eremuan, denborarako diren azpikontratazio lerroak soilik hauta ditzakezu. Ezin duzu azpikontratatutako lerroak hautatu gastuetarako edo materialetarako.

5.  Proiektuko taldekideen erregistroaren rolak bat etorri behar du azpikontratuaren lerroko rolarekin. Horrek ziurtatzen du proiektuan estimatzen den rolaren denbora azpikontratazio lerroan erosten den rol bera dela. 

Taldekide generiko bat azpikontratu eta azpikontratu lerro batekin lotzen denean, hau **Langile mota** taldekideen errenkadako eremu orokorrean eguneratuko da **Lan-kontratuko langilea** eta **Azpikontratuaren indarraldia** gisa ezarriko da **Baliozkoa**.

## <a name="subcontracting-a-staffed-project-team-member"></a>Proiektuko taldekide bat azpikontratatzea
Taldekide generikoak edo langilerik gabekoak bezala, proiektu batean behar den taldekideen gaitasuna ere azpikontratu batekin lotu daiteke. Proiektuko taldekide izendatu bat azpikontratatzeko, jarraitu urrats hauek:

1.  Ziurtatu izendatutako baliabidea kontratudun langile mota gisa konfiguratuta dagoela erreserba daitekeen baliabide gisa. Gainera, ziurtatu **Saltzailea** Erreserba daitekeen baliabideko eremua hautatzen ari zaren azpikontratuko saltzailearekin bat dator. 

2.  Azpikontratuak soilik hauta ditzakezu **Zirriborroa** edo **Baieztatuta** egoera. **Itxita** edo **Bertan behera utzita** ezin dira azpikontratuak hautatu. 

3.  The **Azpikontratazio lerroa** eremua ikusgai geratzen da azpikontratu bat hautatu ondoren.

4.  urtean **Azpikontratazio lerroa** eremuan, denborarako diren azpikontratazio lerroak soilik hauta ditzakezu. Ezin duzu azpikontratatutako lerroak hautatu gastuetarako edo materialetarako.

5.  Proiektuko taldekideen erregistroaren rolak bat etorri behar du azpikontratuaren lerroko rolarekin. Horrek ziurtatzen du proiektuan estimatzen den rolaren denbora azpikontratazio lerroan erosten den rol bera dela. 

Lan-kontratuko langile mota gisa eratutako proiektu-taldeko kideak izendatuak **Erreserba daitekeen baliabidea** azpikontratuaren baliozkotasun egoerarekin erakutsiko da **Ez du balio** azpikontratu batekin lotuta ez badaude. Izendatutako proiektu-taldeko kide bat azpikontratu eta azpikontratu lerro batekin lotuta dagoenean, **Langile mota** taldekideen errenkadako eremua eguneratuko da **Lan-kontratuko langilea** eta **Azpikontratuaren indarraldia** gisa ezarriko da **Baliozkoa**.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
