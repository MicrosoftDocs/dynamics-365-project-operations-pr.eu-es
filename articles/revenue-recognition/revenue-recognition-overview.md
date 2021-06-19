---
title: Diru sarreren ezagutzaren ikuspegi orokorra
description: Gai honek diru-sarreren ezagutzari buruzko informazioa eskaintzen du Project Operations-en.
author: sigitac
ms.date: 11/16/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: f5f962572c6ec0298d2d91d33f83e4120a498a6f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6013741"
---
# <a name="revenue-recognition-overview"></a>Diru sarreren ezagutzaren ikuspegi orokorra

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Dynamics 365 Project Operations-en, diru-sarrerak ezagutzeko printzipioak aldatu egiten dira proiektu bat edo proiektuaren zati bat hautatutako fakturazio metodoaren arabera. Gai honek diru-sarreren ezagutzari buruzko informazioa eskaintzen du Project Operations-en.

## <a name="transactions-accounted-using-time-and-material-billing-method"></a>Denboraren eta materialen fakturazio-metodoa erabiliz kontabilizatutako transakzioak

- Kostuen eta diru-sarreren aitorpena lotuta daude. Transakzio kostua eta fakturatu gabeko salmentak [Project Operations Integration aldizkaria](../project-accounting/project-operations-integration-journal.md).
- Proiektuaren kostua eta diru-sarreren profilak fakturatu gabeko salmenten transakzioak liburu nagusian kontabilizatzen diren zehazten du. **Diru sarrerak lortu** hautatuta badago, sistemak **WIP salmenten balioa** eta **Sarreren irabazien salmenten balioa** kontuak argitaratzean. Hau metodo honen adibidea da.  

  | Transakzio mota | Zordunketa / Kreditua | Kopurua |
  | --- | --- | --- |
  | WIP-salmenten balioa | Zordunketa | 100 |
  | Metatutako diru-sarrerak-salmenten balioa | Kreditua | 100 |

- Diru-sarrera ez da ezagutu fakturazioan. Sistemak **Fakturatutako diru-sarrerak** kontua argitaratzean. Hau metodo honen adibidea da.  

  | Transakzio mota | Zordunketa / Kreditua | Kopurua |
  | --- | --- | --- |
  | Bezeroen saldoa | Zordunketa | 120 |
  | Salmenten zerga-ordaingarria | Kreditua | 20 |
  | Fakturatutako diru-sarrerak | Kreditua | 100 |

- Sarrerak fakturatu gabeko salmentak argitaratzen direnean metatzen badira, sistemak fakturatutakoan itzuliko ditu sortutako diru sarrerak.

  | Transakzio mota | Zordunketa / Kreditua | Kopurua |
  | --- | --- | --- |
  | WIP-salmenten balioa | Kreditua | 100 |
  | Metatutako diru-sarrerak-salmenten balioa | Zordunketa | 100 |

## <a name="transactions-accounted-using-the-fixed-price-billing-method"></a>Prezio finkoko fakturazio-metodoa erabiliz kontabilizatutako transakzioak

- Kostuen eta diru-sarreren aitorpena bereizita daude. Transakzio kostua [Project Operations Integration aldizkaria](../project-accounting/project-operations-integration-journal.md). Fakturatu gabeko salmenta transakzioak ez dira sortzen.
- Diru-sarrerak fakturatzerakoan antzeman daitezke proiektuaren kostua eta diru-sarreren profila badituzte **Proiektua amaitzeko kalkuluetarako erabilitako printzipioa** ezarri **WIP ez**. Erabili metodo hau epe laburreko proiektu sinpleetarako.
- Diru-sarrerak prezio finkoko diru-sarreren kalkuluen bidez aitortu daitezke **Bukatutako kontratua** edo **Osatutako ehunekoen sarreren aitorpena** metodoa.

## <a name="additional-resources"></a>Baliabide gehigarriak
[Konfiguratu proiektu fakturagarrien kontabilitatearen artikulua](../project-accounting/configure-accounting-billable-projects.md)

[Prezio finkoko diru-sarrerak kalkulatzeko proiektuak](rev-rec-percentage-completion-method.md)

[Kudeatu diru-sarreren kalkuluak](rev-rec-completed-contract-method.md)

[Metodoak osatzeko kostua](cost-complete-methods.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]