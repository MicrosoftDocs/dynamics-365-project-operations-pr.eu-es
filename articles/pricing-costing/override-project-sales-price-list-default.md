---
title: Gainidatzi proiektuaren salmenten prezio-zerrendak
description: Gai honek salmenta prezioen zerrenda pertsonalizatuak sortzeari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 10/22/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: db2ff6acaad6ab4cbcc98d3d5b06b36ed23b758f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5995066"
---
# <a name="override-project-sales-price-lists"></a><span data-ttu-id="47521-103">Gainidatzi proiektuaren salmenten prezio-zerrendak</span><span class="sxs-lookup"><span data-stu-id="47521-103">Override project sales price lists</span></span>

<span data-ttu-id="47521-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="47521-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

## <a name="customer-specific-project-price-lists"></a><span data-ttu-id="47521-105">Bezeroarentzako proiektuaren prezioen zerrendak</span><span class="sxs-lookup"><span data-stu-id="47521-105">Customer-specific project price lists</span></span>

<span data-ttu-id="47521-106">Bezeroen berariazko prezioen akordioak proiektuaren prezioen zerrenda gisa konfigura daitezke Dynamics 365 Project Operations-eko kontu erregistro batean.</span><span class="sxs-lookup"><span data-stu-id="47521-106">Customer-specific price agreements can be set up as project price lists on an account record in Dynamics 365 Project Operations.</span></span>

<span data-ttu-id="47521-107">Bezeroaren proiektuaren prezioen zerrenda konfiguratzeko, **Salmentak** eremuan, nabigatu kontuaren erregistroa.</span><span class="sxs-lookup"><span data-stu-id="47521-107">To set up a customer-specific project price list, in the **Sales** area, navigate to the account record.</span></span>

1. <span data-ttu-id="47521-108">Ireki **Kontuak** zerrenda orria.</span><span class="sxs-lookup"><span data-stu-id="47521-108">Open the **Accounts** list page.</span></span>
2. <span data-ttu-id="47521-109">Aurkitu eta egin klik bikoitza bezeroaren erregistroan fitxategia irekitzeko **Kontua** xehetasunen orria.</span><span class="sxs-lookup"><span data-stu-id="47521-109">Locate and double-click a customer record to open the **Account** details page.</span></span>
3. <span data-ttu-id="47521-110">**Proiektuaren prezio-zerrendak** fitxan, hautatu **+ Proiektuaren prezio-zerrenda berria**.</span><span class="sxs-lookup"><span data-stu-id="47521-110">On the **Project Price lists** tab, select **+ New Project Price List**.</span></span>
4. <span data-ttu-id="47521-111">**Proiektuaren prezio-zerrenda berrian** orrialdean, hautatu goitibeherako prezioen zerrenda.</span><span class="sxs-lookup"><span data-stu-id="47521-111">On the **New Project Price List** page, select a price list from the drop-down.</span></span> <span data-ttu-id="47521-112">Testuingurua ezarrita duten prezioen zerrendak soilik **Salmentak** eta zeinen moneta bat datorren kontuaren moneta barne.</span><span class="sxs-lookup"><span data-stu-id="47521-112">Only price lists that have the context set to **Sales** and whose currency matches the account currency are included.</span></span>
5. <span data-ttu-id="47521-113">Elkarketaren izena, eta ondoren egin klik **Gorde** botoian.</span><span class="sxs-lookup"><span data-stu-id="47521-113">Name the association, and then select **Save**.</span></span> <span data-ttu-id="47521-114">Bezeroarentzako proiektuaren prezioen zerrenda sortzen da.</span><span class="sxs-lookup"><span data-stu-id="47521-114">A customer-specific project price list is created.</span></span> <span data-ttu-id="47521-115">Prezio zerrenda hau proiektu honen aurrekontuak edo bezero honentzat sortutako kontratuetan proiektuaren prezio lehenetsiak erabiliko dira, aurrekontuaren edo proiektuaren kontratuaren sortutako data prezioen zerrendaren eraginkortasun dataren barruan kokatzen bada.</span><span class="sxs-lookup"><span data-stu-id="47521-115">This price list will be used to default project prices on project quotes or contracts created for this customer where the created date of the quote or project contract falls within the date effectivity of the price list.</span></span>

## <a name="custom-pricing-on-project-quotes"></a><span data-ttu-id="47521-116">Prezio pertsonalizatuak proiektuaren aurrekontuetan</span><span class="sxs-lookup"><span data-stu-id="47521-116">Custom pricing on project quotes</span></span>

<span data-ttu-id="47521-117">Proiektuen aurrekontuetan, bezeroaren edo proiektuaren parametroen arabera lehenetsitako prezio zerrenda lehenetsi batekin hasten den proiektuaren prezioak izan ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="47521-117">On project quotes, you can have project pricing that starts with a default standard price list that defaults from the customer or from the project parameters.</span></span>

<span data-ttu-id="47521-118">Aurrekontu jakin batean proiektuarekin lotutako lanaren prezio pertsonalizatuak behar dituzunean, proiektuaren prezioen zerrendekin lotutako erakundetik lor dezakezu.</span><span class="sxs-lookup"><span data-stu-id="47521-118">When you need custom pricing for project-related work on a particular quote, you can get that from the project price lists associated entity.</span></span>

<span data-ttu-id="47521-119">Osatu urrats hauek aurrekontuaren araberako proiektuaren prezioak konfiguratzeko.</span><span class="sxs-lookup"><span data-stu-id="47521-119">Complete the following steps to set up quote-specific project pricing.</span></span>

1. <span data-ttu-id="47521-120">Ireki proiektuaren eskaintza eta hautatu **Proiektuen prezioen zerrendak** fitxa.</span><span class="sxs-lookup"><span data-stu-id="47521-120">Open the project quote and select the **Project Price Lists** tab.</span></span>
2. <span data-ttu-id="47521-121">Azpisaretan, sakatu **Sortu prezio pertsonalizatuak**.</span><span class="sxs-lookup"><span data-stu-id="47521-121">In the subgrid, select **Create custom pricing**.</span></span>

<span data-ttu-id="47521-122">Aurrekontuari erantsitako proiektuen prezio zerrenda guztiak prezio zerrenda berrietara kopiatzen dira.</span><span class="sxs-lookup"><span data-stu-id="47521-122">All the project price lists that are attached to the quote are copied to new price lists.</span></span> <span data-ttu-id="47521-123">Prezio zerrenda berrien izenek aurrekontuaren izena islatzen dute prezio zerrenda hauek sortu zireneko data-ordu zigiluarekin.</span><span class="sxs-lookup"><span data-stu-id="47521-123">The names of the new price lists reflect the name of quote with a date-time stamp for when these price lists were created.</span></span>

<span data-ttu-id="47521-124">Prezio zerrenda horietako bakoitza erabil dezakezu eta eskulanaren (rolaren prezioa) eta gastuen (kategoriaren prezioa) prezioen eguneratzeak egin ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="47521-124">You can use each of those price lists and make updates to labor (role price) and expense (category price) prices.</span></span> <span data-ttu-id="47521-125">Prezio hauek proiektuaren eskaintza honi soilik aplikatuko zaizkio.</span><span class="sxs-lookup"><span data-stu-id="47521-125">These prices will only be applicable to this project quote.</span></span>

## <a name="price-lists-on-a-project-contract"></a><span data-ttu-id="47521-126">Proiektu-kontratuko prezio-zerrendak</span><span class="sxs-lookup"><span data-stu-id="47521-126">Price lists on a project contract</span></span>

<span data-ttu-id="47521-127">Proiektuaren kontratu batean, proiektuaren prezioak beti lehenetsitako prezioen zerrenda pertsonalizatu gisa kontratuaren izenarekin eta sortutako data-ordu zigilua izenarekin erantsita daude.</span><span class="sxs-lookup"><span data-stu-id="47521-127">On a project contract, project pricing always defaults as a custom price list with the name of contract and the created date time stamp appended to the name.</span></span> <span data-ttu-id="47521-128">Egia da kontratua aurrekontua irabazi zenean sortu zen edo kontratua hutsetik sortu zen.</span><span class="sxs-lookup"><span data-stu-id="47521-128">This is true whether the contract was created when the quote was won or if the contract was created from scratch.</span></span> <span data-ttu-id="47521-129">Behar izanez gero, elkarte hau pertsonalizatutako prezioen zerrendara ken dezakezu eta horren ordez prezio zerrenda estandarra proiektuaren kontratuarekin lotu.</span><span class="sxs-lookup"><span data-stu-id="47521-129">If needed, you can remove this association to the custom price list and associate a standard price list to the project contract instead.</span></span>

<span data-ttu-id="47521-130">Prezio zerrenda estandar bat aurrekontuan edo kontratuan proiektuaren prezio zerrendekin lotzen duzunean, prezio zerrendako prezioetan egindako aldaketek eragina izango dute prezio zerrenda erabiltzen duten aurrekontu eta kontratu guztietan.</span><span class="sxs-lookup"><span data-stu-id="47521-130">When you associate a standard price list to the project price lists on quote or contract, any changes made to the prices in the price list will impact all quotes and contracts that use the price list.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]