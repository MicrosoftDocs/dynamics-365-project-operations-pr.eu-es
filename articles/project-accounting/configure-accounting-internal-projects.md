---
title: Konfiguratu barne-proiektuen kontabilitatea
description: Gai honek Project Operations-en barne-proiektuetarako kontabilitate-praktikak ezartzeko moduari buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 10/09/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: ad8b974ef75cb0a4e43af0aa254cec1bbcab154a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012841"
---
# <a name="configure-accounting-for-internal-projects"></a><span data-ttu-id="5ef8d-103">Konfiguratu barne-proiektuen kontabilitatea</span><span class="sxs-lookup"><span data-stu-id="5ef8d-103">Configure accounting for internal projects</span></span>

<span data-ttu-id="5ef8d-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="5ef8d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="5ef8d-105">Barne-proiektuek enpresei bezero bati fakturatzen ez zaizkion jarduerei lotutako kostuak jarraitzea ahalbidetzen dute.</span><span class="sxs-lookup"><span data-stu-id="5ef8d-105">Internal projects allow companies track cost related to activities that aren't being billed to a customer.</span></span> <span data-ttu-id="5ef8d-106">Barne-proiektuen adibideak hauek dira:</span><span class="sxs-lookup"><span data-stu-id="5ef8d-106">Examples of internal projects include:</span></span>

- <span data-ttu-id="5ef8d-107">Produktu bat garatzea, hala nola mugikorretarako aplikazio bat, eta garapenarekin lotutako kostuen jarraipena egitea.</span><span class="sxs-lookup"><span data-stu-id="5ef8d-107">Developing a product, such as a mobile app, and tracking the cost associated with the development.</span></span>
- <span data-ttu-id="5ef8d-108">Salmentaren aurreko denbora eta gastuak kudeatzea.</span><span class="sxs-lookup"><span data-stu-id="5ef8d-108">Managing pre-sale time and expense.</span></span> <span data-ttu-id="5ef8d-109">Salmentaren aurreko barne proiektu hau fakturatzeko proiektu bihur daiteke gero, aurrekontua irabaziz gero.</span><span class="sxs-lookup"><span data-stu-id="5ef8d-109">This pre-sale internal project can be converted later to a billable project if quote is won.</span></span>

<span data-ttu-id="5ef8d-110">Urtean kontratuarekin loturarik ez duen edozein proiektu Dynamics 365 Project Operations barne gisa tratatzen da.</span><span class="sxs-lookup"><span data-stu-id="5ef8d-110">Any project not associated with a contract in Dynamics 365 Project Operations is treated as internal.</span></span> <span data-ttu-id="5ef8d-111">Proiektuaren kostua eta diru-sarreren profilak ez dira erabiltzen proiektuaren kontabilitate-arauak zehazteko.</span><span class="sxs-lookup"><span data-stu-id="5ef8d-111">Project cost and revenue profiles aren't used to determine accounting rules for the project.</span></span> <span data-ttu-id="5ef8d-112">Barne-proiektuaren kostua irabazien eta galeren printzipioak erabiliz argitaratzen da beti.</span><span class="sxs-lookup"><span data-stu-id="5ef8d-112">Internal project cost is always posted using profit and loss principles.</span></span> <span data-ttu-id="5ef8d-113">Argitaratzeko liburu nagusiko kontuak **Liburu nagusian argitaratzeko konfigurazioa** orrialdean definitzen dira.</span><span class="sxs-lookup"><span data-stu-id="5ef8d-113">Ledger accounts for postings are defined on the **Ledger posting setup** page.</span></span>

- <span data-ttu-id="5ef8d-114">Denborazko transakzioak **Kostua** kontua zordunduta eta **Nominen esleipena** kontuan zordunduta argitaratzen dira.</span><span class="sxs-lookup"><span data-stu-id="5ef8d-114">Time transactions are posted by debiting the **Cost** account and crediting the **Payroll allocation** account.</span></span>
- <span data-ttu-id="5ef8d-115">Gastuen transakzioak **Kostua** kontua zordunduta eta **Gastuetarako lehenetsitako kontua** zordunduta argitaratzen dira.</span><span class="sxs-lookup"><span data-stu-id="5ef8d-115">Expense transactions are posted by debiting the **Cost** account and crediting the **Offset account for expense**.</span></span>
- <span data-ttu-id="5ef8d-116">Artikuluen transakzioak zordunketa bidez argitaratzen dira **Kostua** kontua eta kreditua **Kostua - Elementua** kontua.</span><span class="sxs-lookup"><span data-stu-id="5ef8d-116">Item transactions are posted by debiting the **Cost** account and crediting the **Cost - Item** account.</span></span>

<span data-ttu-id="5ef8d-117">Transakzioak proiektuan argitaratu ondoren, proiektua proiektuko kontratu batekin lotzen bada, sistemak metatutako transakzio guztiak alderantzikatzen ditu eta fakturagarriak diren transakzio berriak sortzen ditu.</span><span class="sxs-lookup"><span data-stu-id="5ef8d-117">After transactions are posted to the project, if the project is associated with a project contract, the system reverses all accumulated transactions and creates new billable transactions.</span></span> <span data-ttu-id="5ef8d-118">Fakturagarriak diren eragiketek Proiektuaren kostu eta diru-sarreren profilean zehaztutako kontabilitate arauak jarraitzen dituzte.</span><span class="sxs-lookup"><span data-stu-id="5ef8d-118">The billable transactions follow the accounting rules defined in respective Project cost and revenue profile.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]
