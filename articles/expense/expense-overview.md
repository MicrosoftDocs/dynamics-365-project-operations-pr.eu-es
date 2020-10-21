---
title: Gastuen ikuspegi orokorra
description: Gai honek Gastua funtzioari buruzko informazioa eskaintzen du Project Operations-en.
author: stsporen
manager: AnnBe
ms.date: 10/06/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 6da831fef5dba060b8019d7689645405c7ebdbed
ms.sourcegitcommit: 0874b3d89e1dc0e65a51cedb82bf8f80831ca0bb
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/06/2020
ms.locfileid: "3967351"
---
# <a name="expense-home-page"></a><span data-ttu-id="c550b-103">Gastuen etxeko orria</span><span class="sxs-lookup"><span data-stu-id="c550b-103">Expense home page</span></span>

<span data-ttu-id="c550b-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="c550b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="c550b-105">Dynamics 365 Project Operations-ek gastuak prozesatzeko gaitasuna onartzen du.</span><span class="sxs-lookup"><span data-stu-id="c550b-105">Dynamics 365 Project Operations supports the ability to process expenses.</span></span> <span data-ttu-id="c550b-106">Gastuen prozesamendua proiektuekin edo proiekturik gabe gertatzen da gidalerroen, transakzioen kategorien eta onarpenen lan-fluxu pertsonalizagarria erabiliz.</span><span class="sxs-lookup"><span data-stu-id="c550b-106">Expense processing occurs with or without projects by using a customizable workflow of policies, transaction categories, and approvals.</span></span>

<span data-ttu-id="c550b-107">Project Operations-en, Gastuetarako onartutako bi inplementazio eredu daude:</span><span class="sxs-lookup"><span data-stu-id="c550b-107">In Project Operations, there are two supported deployment models for Expense:</span></span> 

- <span data-ttu-id="c550b-108">**Osoa**: Inplementazio osoa eskuragarri dago **Baliabiden/Stockean oinarritutako eszenatokietarako proiektuen eragiketak** edo **Ekoizpen eskaeren araberako proiektuetarako eragiketak**.</span><span class="sxs-lookup"><span data-stu-id="c550b-108">**Full**: Full deployment is available for **Project Operations for resource/non-stocked based scenarios** or **Project Operations for production order based scenarios**.</span></span>
- <span data-ttu-id="c550b-109">**Oinarrizkoa**: Oinarrizko inplementazioa eskuragarri dago **Baliabidean/stockean oinarritutako eszenatokietarako proiektuen eragiketak** eta **Lite inplementazioa - aurre egiteko fakturazio proforma**.</span><span class="sxs-lookup"><span data-stu-id="c550b-109">**Basic**: Basic deployment is available for **Project Operations for resource/non-stocked based scenarios** and **Lite deployment – deal to proforma invoicing**.</span></span>

## <a name="full"></a><span data-ttu-id="c550b-110">Osoa</span><span class="sxs-lookup"><span data-stu-id="c550b-110">Full</span></span> 
<span data-ttu-id="c550b-111">Gastu osoko hedapenak gidalerroen betearazpen osoa eskaintzen du, besteak beste, politikak sortzeko gaitasuna barne.</span><span class="sxs-lookup"><span data-stu-id="c550b-111">Full Expense deployment provides a complete policy enforcement which includes the ability to create policies, such as:</span></span>

  - <span data-ttu-id="c550b-112">Gastu-kategoriaren mugak</span><span class="sxs-lookup"><span data-stu-id="c550b-112">Expense category limits</span></span>
  - <span data-ttu-id="c550b-113">Bidaia</span><span class="sxs-lookup"><span data-stu-id="c550b-113">Travel</span></span>
  - <span data-ttu-id="c550b-114">Eguneko dieta</span><span class="sxs-lookup"><span data-stu-id="c550b-114">Per diem</span></span>
  - <span data-ttu-id="c550b-115">Kreditu-txartelaren inportazioak</span><span class="sxs-lookup"><span data-stu-id="c550b-115">Credit card imports</span></span>
  - <span data-ttu-id="c550b-116">Ordainagirien karakterearen hautemate optikoa</span><span class="sxs-lookup"><span data-stu-id="c550b-116">Receipt optical character recognition</span></span>

## <a name="basic"></a><span data-ttu-id="c550b-117">Oinarrizkoa</span><span class="sxs-lookup"><span data-stu-id="c550b-117">Basic</span></span> 
<span data-ttu-id="c550b-118">Oinarrizko Gastuak hedatzeko eszenatokiak oinarrizko gastuak proiektu baten aurrean erregistratzeko aukera ematen du.</span><span class="sxs-lookup"><span data-stu-id="c550b-118">Basic Expense deployment scenario only allows you to record basic expenses against a project.</span></span> 

<span data-ttu-id="c550b-119">Informazio gehiagorako, ikusi [Gastuen sarrera (arina)](basic-expense.md)</span><span class="sxs-lookup"><span data-stu-id="c550b-119">For more information, see [Expense entry (lite)](basic-expense.md)</span></span>

## <a name="determine-your-expense-deployment"></a><span data-ttu-id="c550b-120">Zehaztu gastuen inplementazioa</span><span class="sxs-lookup"><span data-stu-id="c550b-120">Determine your Expense deployment</span></span>
<span data-ttu-id="c550b-121">Oinarrizko Gastuak kudeatzeko inplementazioa exekutatzen ari zaren jakiteko, egiaztatu URL helbidea honekin amaitzen dela **.crm.dynamics.com**.</span><span class="sxs-lookup"><span data-stu-id="c550b-121">To determine if you're running the Basic Expense management deployment, verify that the address URL ends with **.crm.dynamics.com**.</span></span> 
