---
title: Proiektuko taldekideak azpikontratatzea
description: Artikulu honek Microsoft-en proiektuko taldeko kideak nola azpikontratatu azaltzen du Dynamics 365 Project Operations.
author: rumant
ms.date: 12/03/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 649687cb9ac66e684069434a353b63155103aefb
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8916871"
---
# <a name="subcontracting-project-team-members"></a>Proiektuko taldekideak azpikontratatzea

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Microsoft-en Dynamics 365 Project Operations, langilerik gabeko edo langilerik gabeko proiektuko taldekideak azpikontratatzea aukera dezakezu.

- Langilerik gabeko proiektuko taldekideek baliabide generiko bat dute esleituta.
- Langileen taldekideek baliabide izendatua dute.

Proiektu-taldeko kide bat azpikontratu-lerro batera lotzen duzunean, taldekideak dituen zereginen esleipenak azpikontratazioari atxikitako erosketa-prezio-zerrendan oinarrituta egingo dira.  Gainean **Estimazioak** fitxan **Proiektuaren xehetasunak** orrialdea, hautatu **Eguneratu prezioak** botoia azpikontratatzeko erabakiaren ondoriozko prezio eguneratuak edo/eta kostuak ikusteko. 

## <a name="subcontracting-an-unstaffed-project-team-member"></a>Langilerik gabeko proiektuko taldekide bat azpikontratatzea
The **Taldekidearen xehetasunak** orrialdeak azpikontratazio eta azpikontratazio lerro-eremuak ditu, proiektuaren kudeatzaile bati azpikontratu batetik eskatutako gaitasuna nola atera nahiko lukeen adierazteko aukera ematen diotenak. Proiektuko taldekide bat baliabide generiko gisa azpikontratatzeko, jarraitu urrats hauek:

1.  Aukeratu azpikontratu bat **Taldekidearen xehetasuna** orrialdea.

2.  Honekin soilik hauta ditzakezu azpikontratuak **Zirriborroa** edo **Baieztatuta** egoera. **Itxita** edo **Bertan behera utzita** ezin dira azpikontratuak hautatu. 

3.  The **Azpikontratazio lerroa** eremua ikusgai geratzen da azpikontratu bat hautatu ondoren.

4.  urtean **Azpikontratazio lerroa** eremuan, denborarako diren azpikontratazio-lerroak soilik hauta ditzakezu. Ezin duzu azpikontratatutako lerroak hautatu gastuetarako edo materialetarako.

5.  Proiektuko taldekideen erregistroaren rolak bat etorri behar du azpikontratuaren lerroko rolarekin. Horrek ziurtatzen du proiektuan estimatzen den rolaren denbora azpikontratazio lerroan erosten den rol bera dela. 

Taldekide generiko bat azpikontratu eta azpikontratu lerro batekin lotuta dagoenean, **Langile mota** taldekideen errenkada generikoko eremua eguneratuko da **Lan-kontratuko langilea** eta **Azpikontratuaren Baliotasuna** moduan ezarriko da **Baliozkoa**.

## <a name="subcontracting-a-staffed-project-team-member"></a>Proiektuko taldekide bat azpikontratatzea
Taldekide generikoak edo langilerik gabekoak bezala, proiektu batean behar den taldekideen gaitasuna ere azpikontratu batekin lotu daiteke. Proiektuko taldekide izendatu bat azpikontratatzeko, jarraitu urrats hauek:

1.  Ziurtatu izendatutako baliabidea kontratudun langile mota gisa konfiguratuta dagoela erreserba daitekeen baliabide gisa. Gainera, ziurtatu **Saltzailea** Erreserba daitekeen baliabideko eremua hautatzen ari zaren azpikontratuko hornitzailearekin bat dator. 

2.  Azpikontratuak soilik hauta ditzakezu **Zirriborroa** edo **Baieztatuta** egoera. **Itxita** edo **Bertan behera utzita** ezin dira azpikontratuak hautatu. 

3.  The **Azpikontratazio lerroa** eremua ikusgai geratzen da azpikontratu bat hautatu ondoren.

4.  urtean **Azpikontratazio lerroa** eremuan, denborarako diren azpikontratazio-lerroak soilik hauta ditzakezu. Ezin duzu azpikontratatutako lerroak hautatu gastuetarako edo materialetarako.

5.  Proiektuko taldekideen erregistroaren rolak bat etorri behar du azpikontratuaren lerroko rolarekin. Horrek ziurtatzen du proiektuan estimatzen den rolaren denbora azpikontratazio lerroan erosten den rol bera dela. 

Lan-kontratuko langile mota gisa eratutako proiektu-taldekide izendatuak **Erreserba daitekeen baliabidea** azpikontratuaren baliozkotasun egoerarekin erakutsiko da **Ez du balio** azpikontratu batekin lotuta ez badaude. Izendatutako proiektu-taldeko kide bat azpikontratu eta azpikontratu lerro batekin lotuta dagoenean, **Langile mota** taldekideen errenkadako eremua eguneratuko da **Lan-kontratuko langilea** eta **Azpikontratuaren Baliotasuna** moduan ezarriko da **Baliozkoa**.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]