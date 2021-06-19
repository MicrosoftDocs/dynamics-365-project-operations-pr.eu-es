---
title: Berretsi proiektu-kontratua
description: Gai honek Project Operations-en kontratuak berresteari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 10/13/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b5eabcad028a8282f552f3571b170d9b933a7b88
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003661"
---
# <a name="confirm-a-project-contract"></a>Berretsi proiektu-kontratua

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations-eko proiektu-kontratu bat **Baieztatuta** arrazoiarekin aktibo egon daiteke, **Galduta** arrazoiarekin itxi egin daiteke. Proiektuaren kontratua berresten duzunean, egoera **Zirriborroa** egoeratik **Aktiboa** egoerara eguneratzen da eta egoeraren arrazoia **Baieztatuta** da. Ezin da kontratu aktibo edo itxi bat editatu edo berriro ireki. 

### <a name="financial-impact-of-confirming-a-project-contract"></a>Proiektuaren kontratua berrestearen finantza-eragina

Proiektu-kontratu bat berretsi eta gero, aplikazioak kostuak birkalkultzen ditu kostu zaharrenak alderantzikatuz eta kostu erreal berriak sortuz. Kostu erreal berriak orduan lotutako proiektuaren kontratu lerroaren Fakturazio metodoan oinarrituta prozesatzen da. Kostuen benetako denbora eta materialaren kontratu lerroa aipatzen bada, aplikazioak automatikoki berriro sortzen ditu fakturatu gabeko salmenten benetako datuak. Kostuen prezioak Prezio Finkoaren kontratu lerroa aipatzen badu, aplikazioak kostuaren errealitatea berriro prozesatzeari uzten dio.

Ez gainditzeko mugak, kargagarritasuna konfiguratzea eta prezioei eta kostuei buruzko datuak ebaluatu eta gero berresten dira baieztapen prozesuaren barruan.

## <a name="close-a-project-contract-as-lost"></a>Itxi proiektu-kontratu bat galdutako gisa

Proiektuaren kontratua galdu gisa ixten duzunean, kontratuaren egoera eguneratu egingo da **Itxita** eta egoeraren arrazoia **Galduta** da. Proiektuaren kontratua irakurtzeko soilik bihurtzen da. Aldaketak amaitu aurretik berrespen elkarrizketa-koadroa ematen da, ezin baituzu itxitako proiektuaren kontratua berriro ireki.

Galdutako itxita dagoen proiektuaren kontratuak bere lerroetan proiektu bat aipatzen badu, proiektu hori itxita dagoela ere markatuko da. Egun horretatik aurrera edozein baliabide erreserba bertan behera geratzen da. Proiektuaren kontratuan fakturatu gabeko salmenten fakturak aurrez fakturan ez badaude, atzera botako dira.

> [!NOTE]
> Dynamics 365 Project Operations-en, proiektuaren kontratua galdutako moduan ixteak ez du lotutako aukeraren egoeran eragingo. Aukera irekita egongo da eta eskuz itxi behar da.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]