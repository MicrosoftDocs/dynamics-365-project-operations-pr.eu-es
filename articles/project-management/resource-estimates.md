---
title: Proiektuetako baliabideen denboraren aurreikuspen ekonomikoak
description: Gai honek denborarako finantza kalkuluak nola kalkulatzen diren jakiteko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 03/19/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 91156c5cf79af8c66c12b84a6d2b17aa7fe09ed1
ms.sourcegitcommit: 386921f44f1e9a8a828b140206d52945de07aee7
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/22/2021
ms.locfileid: "5701811"
---
# <a name="financial-estimates-for-resource-time-on-projects"></a>Proiektuetako baliabideen denboraren aurreikuspen ekonomikoak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Denborari buruzko finantza kalkuluak hiru faktoreren arabera kalkulatzen dira: 

- Proiektuaren planeko hosto-nodo zeregin bakoitzari esleitutako taldekide generiko edo izendatutako mota. 
- Lan mota edo konplexutasuna.
- Baliabidea zereginean esleitzeko ahaleginaren hedapena. 

Lehenengo bi faktoreek baliabide baten esleipenaren kostu unitarioan edo fakturan duten tasan eragina dute. Baliabideen esleipenaren unitate-kostua edo faktura-tasa esleitutako baliabidearen atributuek zehazten dute. Atributu horien artean, baliabideari dagokion antolakuntza-unitatea eta baliabidearen eginkizun estandarra daude. Zure negozioari dagozkion atributu pertsonalizatuak ere gehi ditzakezu baliabidearentzat, adibidez, titulu estandarra edo esperientzia maila, eta lagundu beharreko unitateko kostuan edo fakturazio tasan eragina izan dezakete.
Baliabidearen atributuez gain, lanaren atributuek, hala nola zereginak, zereginaren faktura unitarioan edo kostu tasan ere eragina izan dezakete. Adibidez, zenbait zeregin konplexuagoak direnean, baliabideak zeregin zehatz horiei esleitzeak kostu unitario edo fakturazio tasa handiagoa eragiten du hain konplexuak ez diren zereginak baino.   

Hirugarren faktoreak ordu kopuru hori ematen du tasa horretan. Zeregin batek bi prezio-aldi estaltzen dituen kasuetan, litekeena da zeregin horretarako baliabideen esleipenaren lehen zatia zereginaren bigarren zatiaren aldean kostua eta prezioa izatea. Baliabideen esleipen bakoitzaren ahaleginaren estimazioa eguneko ahaleginaren banaketa egunerokoarekin gordetako balio konplexua da.

Lanaren eta baliabideen atributu pertsonalizatuak prezioen eta kostuen dimentsio gisa konfiguratzeko moduari buruzko argibide zehatzak lortzeko, ikusi [Prezioen dimentsioen ikuspegi orokorra](../pricing-costing/pricing-dimensions-overview.md).

Baliabideen esleipen bakoitzaren finantza-estimazioa honela kalkulatzen da **tasa/orduko lanaren ordu kopuruarekin biderkatuta.**  Ahaleginaren estimazioaren antzera, baliabideen esleipen bakoitzaren kostuen eta diru-sarreren finantza-estimazioa eguneko diru-zenbatekoaren eguneroko banaketarekin gordetako balio konplexua da. 

## <a name="summarizing-financial-estimates-for-time"></a>Denborarako finantza estimazioak laburbilduz
Hosto-nodo baten zereginaren denboraren finantza-estimazioa zeregin horretarako baliabide-esleipen guztien finantza-estimazioen batura da.

Laburpen-zeregin edo zeregin nagusi baten zereginaren denboraren finantza-estimazioa ber bigarren mailako zeregin guztietan. Hau da proiektuaren eskulanaren kostua. 

![Baliabideen aurreikuspenak](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a>Kostuaren prezioei eta kostuaren moneta lehenetsia

Kostuaren prezio lehenetsia proiektuaren kontratazio unitateari atxikitako prezio zerrendetatik dator. Proiektuaren kostu moneta proiektuan kontratatzeko unitatearen moneta da beti. Baliabideak esleitzerakoan, kostuaren finantza-estimazioa proiektuaren kostuaren monetan gordetzen da. Batzuetan, kostu-tasa prezioen zerrendan ezarrita dagoen moneta proiektuaren kostuaren moneta ezberdina da. Kasu horietan, aplikazioak kostuaren prezioa finkatutako moneta bihurtzen du proiektuaren monetara. **Aurrekontuak** saretan, kostuen kalkulu guztiak proiektuaren kostu monetan bistaratzen dira eta laburbiltzen dira. 

## <a name="default-bill-rate-and-sales-currency"></a>Fakturazio-tasa eta salmenten moneta lehenetsia

Salmenta-prezio lehenetsia erlazionatutako proiektuaren kontratuari atxikitako proiektuen prezioen zerrendetatik dator, tratua irabazten bada edo lotutako proiektuaren aurrekontutik tratua salmenta aurreko fasean badago. Proiektuaren salmenten moneta proiektuaren eskaintzaren edo proiektuaren kontraturen moneta da beti. Baliabideak esleitzerakoan, salmenten finantza-estimazioa proiektuaren salmenten monetan gordetzen da. Kostua ez bezala, prezioen zerrendan ezarritako salmenta-prezioa ezin da inoiz proiektuaren salmenta-monetatik desberdina izan. Ez dago eszenatokirik moneta bihurtzeko beharrezkoa denik. **Aurrekontuak** saretan, salmenten kalkulu guztiak proiektuaren salmenta monetan bistaratzen dira eta laburbiltzen dira. 

[!INCLUDE[footer-include](../includes/footer-banner.md)]
