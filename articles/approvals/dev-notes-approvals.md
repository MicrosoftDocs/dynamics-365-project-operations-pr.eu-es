---
title: Onespenetarako garatzaileen oharrak
description: Gai honek garatzailearen informazio osagarriarekin lan egiteari buruzko informazioa eskaintzen du.
author: stsporen
ms.date: 11/09/2020
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: a89ea669a262c145b9f391fddc19e79a425fabb5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996776"
---
# <a name="developer-notes-for-approvals"></a><span data-ttu-id="17392-103">Onespenetarako garatzaileen oharrak</span><span class="sxs-lookup"><span data-stu-id="17392-103">Developer notes for Approvals</span></span>

<span data-ttu-id="17392-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="17392-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="17392-105">Dynamics 365 Project Operations-ek onarpen-etapetan erregistroaren trantsizio zuzena ziurtatzen duen balioztatze-logika dakar.</span><span class="sxs-lookup"><span data-stu-id="17392-105">Dynamics 365 Project Operations includes validation logic that ensures correct record transition through the approval stages.</span></span> <span data-ttu-id="17392-106">Erregistro trantsizio zuzenak ziurtatzen ditu:</span><span class="sxs-lookup"><span data-stu-id="17392-106">Correct record transitions ensure:</span></span> 

  - <span data-ttu-id="17392-107">Laguntzeko errenkada guztiak erlazionatutako tauletan sortzen dira, hala nola aldizkarietan eta egunkarietan.</span><span class="sxs-lookup"><span data-stu-id="17392-107">All supporting rows are created in related tables, such as journals and actuals.</span></span>
  - <span data-ttu-id="17392-108">Onartzailea a gisa markatuta dago **Proiektuaren onartzailea** proiektuan aurrera egin aurretik.</span><span class="sxs-lookup"><span data-stu-id="17392-108">The approver is marked as a **Project Approver** in the project before proceeding.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]