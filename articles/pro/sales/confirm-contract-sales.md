---
title: Berretsi proiektu-kontratua
description: Gai honek Project Operations-en kontratuak berresteari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 24da0887c0266d51bddcbbf8efd6f2644b6d0f4f
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4128268"
---
# <a name="confirm-a-project-contract"></a>Berretsi proiektu-kontratua

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations proiektuaren kontratua aktiboa izan daiteke **Baieztatuta**, edo itxi arrazoiarekin **Galdua**. Proiektuaren kontratua berresten duzunean, egoera **Zirriborroa** egoeratik **Aktiboa** egoerara eguneratzen da eta egoeraren arrazoia **Baieztatuta** da. Ezin da kontratu aktibo edo itxi bat editatu edo berriro ireki. 

### <a name="financial-impact-of-confirming-a-project-contract"></a>Proiektuaren kontratua berrestearen finantza-eragina

Proiektu-kontratu bat berretsi eta gero, aplikazioak kostuak birkalkultzen ditu kostu zaharrenak alderantzikatuz eta kostu erreal berriak sortuz. Kostu erreal berriak orduan lotutako proiektuaren kontratu lerroaren Fakturazio metodoan oinarrituta prozesatzen da. Kostuen benetako denbora eta materialaren kontratu lerroa aipatzen bada, aplikazioak automatikoki berriro sortzen ditu fakturatu gabeko salmenten benetako datuak. Kostuen prezioak Prezio Finkoaren kontratu lerroa aipatzen badu, aplikazioak kostuaren errealitatea berriro prozesatzeari uzten dio.

Ez gainditzeko mugak, kargagarritasuna konfiguratzea eta prezioei eta kostuei buruzko datuak ebaluatu eta gero berresten dira baieztapen prozesuaren barruan.

## <a name="close-a-project-contract-as-lost"></a>Itxi proiektu-kontratu bat galdutako gisa

Proiektuaren kontratua galdu gisa ixten duzunean, kontratuaren egoera eguneratu egingo da **Itxita** eta egoeraren arrazoia **Galduta** da. Proiektuaren kontratua irakurtzeko soilik bihurtzen da. Aldaketak amaitu aurretik berrespen elkarrizketa-koadroa ematen da, ezin baituzu itxitako proiektuaren kontratua berriro ireki.

Galdutako itxita dagoen proiektuaren kontratuak bere lerroetan proiektu bat aipatzen badu, proiektu hori itxita dagoela ere markatuko da. Egun horretatik aurrera edozein baliabide erreserba bertan behera geratzen da. Proiektuaren kontratuan fakturatu gabeko salmenten fakturak aurrez fakturan ez badaude, atzera botako dira.

> [!NOTE]
> Dynamics 365 Project Operations-en, proiektuaren kontratua galdutako moduan ixteak ez du eragingo lotutako aukeraren egoera horretan. Aukera irekita egongo da eta eskuz itxi behar da.
