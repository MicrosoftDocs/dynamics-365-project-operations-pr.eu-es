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
ms.openlocfilehash: d807d3631f40a93ec7dbd918b64c287fd4875c79
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5273813"
---
# <a name="confirm-a-project-contract"></a><span data-ttu-id="604ca-103">Berretsi proiektu-kontratua</span><span class="sxs-lookup"><span data-stu-id="604ca-103">Confirm a project contract</span></span>

<span data-ttu-id="604ca-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="604ca-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="604ca-105">Dynamics 365 Project Operations-eko proiektu-kontratu bat **Baieztatuta** arrazoiarekin aktibo egon daiteke, **Galduta** arrazoiarekin itxi egin daiteke.</span><span class="sxs-lookup"><span data-stu-id="604ca-105">A project contract in Dynamics 365 Project Operations can be active with a reason of **Confirmed**, or closed with a reason of **Lost**.</span></span> <span data-ttu-id="604ca-106">Proiektuaren kontratua berresten duzunean, egoera **Zirriborroa** egoeratik **Aktiboa** egoerara eguneratzen da eta egoeraren arrazoia **Baieztatuta** da.</span><span class="sxs-lookup"><span data-stu-id="604ca-106">When you confirm a project contract, the status updates from **Draft** to **Active** and the status reason is **Confirmed**.</span></span> <span data-ttu-id="604ca-107">Ezin da kontratu aktibo edo itxi bat editatu edo berriro ireki.</span><span class="sxs-lookup"><span data-stu-id="604ca-107">An active or closed contract can't be edited or reopened.</span></span> 

### <a name="financial-impact-of-confirming-a-project-contract"></a><span data-ttu-id="604ca-108">Proiektuaren kontratua berrestearen finantza-eragina</span><span class="sxs-lookup"><span data-stu-id="604ca-108">Financial impact of confirming a project contract</span></span>

<span data-ttu-id="604ca-109">Proiektu-kontratu bat berretsi eta gero, aplikazioak kostuak birkalkultzen ditu kostu zaharrenak alderantzikatuz eta kostu erreal berriak sortuz.</span><span class="sxs-lookup"><span data-stu-id="604ca-109">After a project contract is confirmed, the application recalculates the costs by reversing the older cost actuals and creating new cost actuals.</span></span> <span data-ttu-id="604ca-110">Kostu erreal berriak orduan lotutako proiektuaren kontratu lerroaren Fakturazio metodoan oinarrituta prozesatzen da.</span><span class="sxs-lookup"><span data-stu-id="604ca-110">The new cost actuals are then processed based on the billing method of the associated project contract line.</span></span> <span data-ttu-id="604ca-111">Kostuen benetako denbora eta materialaren kontratu lerroa aipatzen bada, aplikazioak automatikoki berriro sortzen ditu fakturatu gabeko salmenten benetako datuak.</span><span class="sxs-lookup"><span data-stu-id="604ca-111">If the cost actuals reference a Time and Material contract line, the application automatically re-creates corresponding unbilled sales actuals.</span></span> <span data-ttu-id="604ca-112">Kostuen prezioak Prezio Finkoaren kontratu lerroa aipatzen badu, aplikazioak kostuaren errealitatea berriro prozesatzeari uzten dio.</span><span class="sxs-lookup"><span data-stu-id="604ca-112">If the cost actuals reference a Fixed Price contract line, the application stops reprocessing the cost actuals.</span></span>

<span data-ttu-id="604ca-113">Ez gainditzeko mugak, kargagarritasuna konfiguratzea eta prezioei eta kostuei buruzko datuak ebaluatu eta gero berresten dira baieztapen prozesuaren barruan.</span><span class="sxs-lookup"><span data-stu-id="604ca-113">Not-to-exceed limits, chargeability setup, and pricing and costing on the actuals is evaluated and then updated as part of the confirmations process.</span></span>

## <a name="close-a-project-contract-as-lost"></a><span data-ttu-id="604ca-114">Itxi proiektu-kontratu bat galdutako gisa</span><span class="sxs-lookup"><span data-stu-id="604ca-114">Close a project contract as lost</span></span>

<span data-ttu-id="604ca-115">Proiektuaren kontratua galdu gisa ixten duzunean, kontratuaren egoera eguneratu egingo da **Itxita** eta egoeraren arrazoia **Galduta** da.</span><span class="sxs-lookup"><span data-stu-id="604ca-115">When you close a project contract as lost, the contract status is updated to **Closed** and the status reason is **Lost**.</span></span> <span data-ttu-id="604ca-116">Proiektuaren kontratua irakurtzeko soilik bihurtzen da.</span><span class="sxs-lookup"><span data-stu-id="604ca-116">The project contract becomes read-only.</span></span> <span data-ttu-id="604ca-117">Aldaketak amaitu aurretik berrespen elkarrizketa-koadroa ematen da, ezin baituzu itxitako proiektuaren kontratua berriro ireki.</span><span class="sxs-lookup"><span data-stu-id="604ca-117">A confirmation dialog is provided before the changes are complete because you can't reopen a closed project contract.</span></span>

<span data-ttu-id="604ca-118">Galdutako itxita dagoen proiektuaren kontratuak bere lerroetan proiektu bat aipatzen badu, proiektu hori itxita dagoela ere markatuko da.</span><span class="sxs-lookup"><span data-stu-id="604ca-118">If the project contract that is closed as lost references a project on its lines, that project is also marked as closed.</span></span> <span data-ttu-id="604ca-119">Egun horretatik aurrera edozein baliabide erreserba bertan behera geratzen da.</span><span class="sxs-lookup"><span data-stu-id="604ca-119">Any resource bookings from that day forward are canceled.</span></span> <span data-ttu-id="604ca-120">Proiektuaren kontratuan fakturatu gabeko salmenten fakturak aurrez fakturan ez badaude, atzera botako dira.</span><span class="sxs-lookup"><span data-stu-id="604ca-120">Any unbilled sales actuals on the project contract that aren't already on an invoice, will be reversed.</span></span>

> [!NOTE]
> <span data-ttu-id="604ca-121">Dynamics 365 Project Operations-en, proiektuaren kontratua galdutako moduan ixteak ez du lotutako aukeraren egoeran eragingo.</span><span class="sxs-lookup"><span data-stu-id="604ca-121">In Dynamics 365 Project Operations, closing a project contract as lost will not impact that status of the associated opportunity.</span></span> <span data-ttu-id="604ca-122">Aukera irekita egongo da eta eskuz itxi behar da.</span><span class="sxs-lookup"><span data-stu-id="604ca-122">The opportunity will remain open and must be manually closed.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]