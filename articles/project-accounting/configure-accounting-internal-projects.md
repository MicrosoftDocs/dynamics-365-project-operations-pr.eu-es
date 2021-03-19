---
title: Konfiguratu barne-proiektuen kontabilitatea
description: Gai honek Project Operations-en barne-proiektuetarako kontabilitate-praktikak ezartzeko moduari buruzko informazioa eskaintzen du.
author: sigitac
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 9f1cc75b12fec81d726e46f8d970dcfe030f6b29
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287583"
---
# <a name="configure-accounting-for-internal-projects"></a><span data-ttu-id="ea942-103">Konfiguratu barne-proiektuen kontabilitatea</span><span class="sxs-lookup"><span data-stu-id="ea942-103">Configure accounting for internal projects</span></span>

<span data-ttu-id="ea942-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="ea942-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="ea942-105">Barne-proiektuek enpresei bezero bati fakturatzen ez zaizkion jarduerei lotutako kostuak jarraitzea ahalbidetzen dute.</span><span class="sxs-lookup"><span data-stu-id="ea942-105">Internal projects allow companies track cost related to activities that aren't being billed to a customer.</span></span> <span data-ttu-id="ea942-106">Barne-proiektuen adibideak hauek dira:</span><span class="sxs-lookup"><span data-stu-id="ea942-106">Examples of internal projects include:</span></span>

- <span data-ttu-id="ea942-107">Produktu bat garatzea, hala nola mugikorretarako aplikazio bat, eta garapenarekin lotutako kostuen jarraipena egitea.</span><span class="sxs-lookup"><span data-stu-id="ea942-107">Developing a product, such as a mobile app, and tracking the cost associated with the development.</span></span>
- <span data-ttu-id="ea942-108">Salmentaren aurreko denbora eta gastuak kudeatzea.</span><span class="sxs-lookup"><span data-stu-id="ea942-108">Managing pre-sale time and expense.</span></span> <span data-ttu-id="ea942-109">Salmentaren aurreko barne proiektu hau fakturatzeko proiektu bihur daiteke gero, aurrekontua irabaziz gero.</span><span class="sxs-lookup"><span data-stu-id="ea942-109">This pre-sale internal project can be converted later to a billable project if quote is won.</span></span>

<span data-ttu-id="ea942-110">Urtean kontratuarekin loturarik ez duen edozein proiektu Dynamics 365 Project Operations barne gisa tratatzen da.</span><span class="sxs-lookup"><span data-stu-id="ea942-110">Any project not associated with a contract in Dynamics 365 Project Operations is treated as internal.</span></span> <span data-ttu-id="ea942-111">Proiektuaren kostua eta diru-sarreren profilak ez dira erabiltzen proiektuaren kontabilitate-arauak zehazteko.</span><span class="sxs-lookup"><span data-stu-id="ea942-111">Project cost and revenue profiles aren't used to determine accounting rules for the project.</span></span> <span data-ttu-id="ea942-112">Barne-proiektuaren kostua irabazien eta galeren printzipioak erabiliz argitaratzen da beti.</span><span class="sxs-lookup"><span data-stu-id="ea942-112">Internal project cost is always posted using profit and loss principles.</span></span> <span data-ttu-id="ea942-113">Argitaratzeko liburu nagusiko kontuak **Liburu nagusian argitaratzeko konfigurazioa** orrialdean definitzen dira.</span><span class="sxs-lookup"><span data-stu-id="ea942-113">Ledger accounts for postings are defined on the **Ledger posting setup** page.</span></span>

- <span data-ttu-id="ea942-114">Denborazko transakzioak **Kostua** kontua zordunduta eta **Nominen esleipena** kontuan zordunduta argitaratzen dira.</span><span class="sxs-lookup"><span data-stu-id="ea942-114">Time transactions are posted by debiting the **Cost** account and crediting the **Payroll allocation** account.</span></span>
- <span data-ttu-id="ea942-115">Gastuen transakzioak **Kostua** kontua zordunduta eta **Gastuetarako lehenetsitako kontua** zordunduta argitaratzen dira.</span><span class="sxs-lookup"><span data-stu-id="ea942-115">Expense transactions are posted by debiting the **Cost** account and crediting the **Offset account for expense**.</span></span>

<span data-ttu-id="ea942-116">Transakzioak proiektuan argitaratu ondoren, proiektua proiektuko kontratu batekin lotzen bada, sistemak metatutako transakzio guztiak alderantzikatzen ditu eta fakturagarriak diren transakzio berriak sortzen ditu.</span><span class="sxs-lookup"><span data-stu-id="ea942-116">After transactions are posted to the project, if the project is associated with a project contract, the system reverses all accumulated transactions and creates new billable transactions.</span></span> <span data-ttu-id="ea942-117">Fakturagarriak diren eragiketek Proiektuaren kostu eta diru-sarreren profilean zehaztutako kontabilitate arauak jarraitzen dituzte.</span><span class="sxs-lookup"><span data-stu-id="ea942-117">The billable transactions follow the accounting rules defined in respective Project cost and revenue profile.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]