---
title: Zehaztu gaitasunak eta trebetasunak
description: Gai honek baliabideak baloratzeko trebetasun-ereduen konfigurazioari buruzko informazioa ematen du.
author: ruhercul
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 9376e0b268a3ab682716da604ceecfa1e878da68
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897616"
---
# <a name="define-skills-and-proficiencies"></a><span data-ttu-id="b4786-103">Zehaztu gaitasunak eta trebetasunak</span><span class="sxs-lookup"><span data-stu-id="b4786-103">Define skills and proficiencies</span></span>

<span data-ttu-id="b4786-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="b4786-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b4786-105">Gaitasunak Dynamics 365 Project Operations aplikazioaren eta, aurkezten bada, Dynamics 365 Field Service aplikazioaren artean partekatzen diren baliabideen ezaugarriak dira.</span><span class="sxs-lookup"><span data-stu-id="b4786-105">Skills are resource characteristics that are shared between Dynamics 365 Project Operations and if present, Dynamics 365 Field Service.</span></span> 

- <span data-ttu-id="b4786-106">Gaitasunen biltegia Project Operations-en mantentzeko, joan **Baliabideak** \> **Baliabideen gaitasunak** atalera.</span><span class="sxs-lookup"><span data-stu-id="b4786-106">To maintain the repository of skills in Project Operations, go to **Resources** \> **Resource Skills**.</span></span> 

## <a name="use-proficiency-models-to-rate-resources"></a><span data-ttu-id="b4786-107">Erabili gaitasun ereduak baliabideak baloratzeko</span><span class="sxs-lookup"><span data-stu-id="b4786-107">Use proficiency models to rate resources</span></span>

<span data-ttu-id="b4786-108">Baliabideetarako trebetasunak gaitasun ereduen arabera sailkatzen dira.</span><span class="sxs-lookup"><span data-stu-id="b4786-108">Skills for resources are rated by proficiency models.</span></span> <span data-ttu-id="b4786-109">Banakako balorazioak gaitasun ereduan daude.</span><span class="sxs-lookup"><span data-stu-id="b4786-109">The individual ratings are in a proficiency model.</span></span> 

1. <span data-ttu-id="b4786-110">Gaitasun eredua sortzeko, joan **Baliabideak** \> **Gaitasun ereduak** atalera eta, ondoren, hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="b4786-110">To create a proficiency model, go to **Resources** \> **Proficiency Models**, and then select **New**.</span></span>
2. <span data-ttu-id="b4786-111">Ebaluazio-eredu berrian, zehaztu gutxieneko balorazioaren balioa, gehienezko balorazioaren balioa eta kalifikatzen den entitatea.</span><span class="sxs-lookup"><span data-stu-id="b4786-111">In the new rating model, specify the minimum rating value, the maximum rating value, and the entity that is being rated.</span></span>
3. <span data-ttu-id="b4786-112">**Balorazioaren balioak** azpi-saretaren, balorazioaren balio desberdinak definitu ditzakezu, gutxieneko baliotik gehienekora.</span><span class="sxs-lookup"><span data-stu-id="b4786-112">In the **Rating Values** sub-grid, you can define the different rating values, from the minimum to the maximum.</span></span>


<span data-ttu-id="b4786-113">Balorazioaren balio horiek **Baliabide-eskakizunak**, **Antolaketa-panela** eta **Antolaketa-laguntzailea** iragazkietan erakusten dira.</span><span class="sxs-lookup"><span data-stu-id="b4786-113">These rating values are shown on the **Resource Requirements**, **Schedule Board**, and **Schedule Assistant** filters.</span></span>
