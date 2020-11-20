---
title: Zuzendutako fakturak
description: Gai honek zuzendutako fakturak egiteari buruzko informazioa ematen du.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 1ebfec053a59bbadd261d4333f6737cf16292e81
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122373"
---
# <a name="corrected-invoices"></a><span data-ttu-id="395ff-103">Zuzendutako fakturak</span><span class="sxs-lookup"><span data-stu-id="395ff-103">Corrected invoices</span></span>

<span data-ttu-id="395ff-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="395ff-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="395ff-105">Berretsitako fakturak editatu daitezke.</span><span class="sxs-lookup"><span data-stu-id="395ff-105">Confirmed invoices can be edited.</span></span> <span data-ttu-id="395ff-106">Berretsitako faktura editatzen duzunean, zuzendutako fakturaren zirriborro berria sortzen da.</span><span class="sxs-lookup"><span data-stu-id="395ff-106">When you edit a confirmed invoice, a draft of the corrected invoice is created.</span></span> <span data-ttu-id="395ff-107">Jatorrizko fakturatik transakzio eta kantitate guztiak berraztertu nahi dituzulako hipotesiarekin, zuzendutako faktura honek jatorrizko fakturaren transakzio guztiak barne hartzen ditu, eta bertan dauden kantitate guztiak zero (0) dira.</span><span class="sxs-lookup"><span data-stu-id="395ff-107">Because the assumption is that you want to reverse all the transactions and quantities from the original invoice, the corrected invoice includes all the transactions from the original invoice, and all the quantities on it are zero (0).</span></span>

<span data-ttu-id="395ff-108">Transakzioren bat zuzentzen ez bada, faktura zuzentzailearen zirriborrotik kendu dezakezu.</span><span class="sxs-lookup"><span data-stu-id="395ff-108">When transactions don't require correction, you can remove them from the draft corrective invoice.</span></span> <span data-ttu-id="395ff-109">Kantitate partziala soilik alderantzikatzeko edo itzultzeko, editatu dezakezu Kopurua eremuan, lerroaren xehetasunean.</span><span class="sxs-lookup"><span data-stu-id="395ff-109">To reverse or return only a partial quantity, you can edit the Quantity field on the line detail.</span></span> <span data-ttu-id="395ff-110">Fakturen lerroaren xehetasuna irekitzen baduzu, fakturaren jatorrizko kantitatea ikus dezakezu.</span><span class="sxs-lookup"><span data-stu-id="395ff-110">If you open the invoice line detail, you can see the original invoice quantity.</span></span> <span data-ttu-id="395ff-111">Uneko fakturaren kantitatea editatu ahal izango duzu, fakturaren jatorrizko kantitatea baino gutxiago edo gehiago izan dadin.</span><span class="sxs-lookup"><span data-stu-id="395ff-111">You can then edit the current invoice quantity so that it's less than or more than the original invoice quantity.</span></span>

<span data-ttu-id="395ff-112">Faktura zuzentzailea baieztatzen duzunean, fakturatutako jatorrizko salmenten benetakoa alderantzikatu egiten da eta fakturatutako salmenta erreal berria sortzen da.</span><span class="sxs-lookup"><span data-stu-id="395ff-112">When you confirm a corrective invoice, the original billed sales actual is reversed, and a new billed sales actual is created.</span></span> <span data-ttu-id="395ff-113">Kantitatea murriztuko balitz, aldaketak fakturatu gabeko salmenta berriak ere sortuko ditu.</span><span class="sxs-lookup"><span data-stu-id="395ff-113">If the quantity was reduced, the difference will cause a new unbilled sales actual to be created too.</span></span> <span data-ttu-id="395ff-114">Adibidez, fakturatutako jatorrizko salmenta zortzi orduz izan bazenuen eta zuzendutako fakturaren linearen xehetasunak sei orduko kantitatera murriztu badu, jatorrizko fakturatutako salmenta-lerroa alderantzikatuko da eta bi berri sortuko dira:</span><span class="sxs-lookup"><span data-stu-id="395ff-114">For example, if the original billed sale was for eight hours, and the corrected invoice line detail has a reduced quantity of six hours, the original billed sales line is revered and two new actuals are created:</span></span>

- <span data-ttu-id="395ff-115">Fakturatutako salmentak sei orduz fakturatu dira.</span><span class="sxs-lookup"><span data-stu-id="395ff-115">A billed sales actual for six hours.</span></span>
- <span data-ttu-id="395ff-116">Bete gabeko salmentak benetako gainerako bi orduetan.</span><span class="sxs-lookup"><span data-stu-id="395ff-116">An unbilled sales actual for the remaining two hours.</span></span> <span data-ttu-id="395ff-117">Transakzio hau beranduago fakturatu daiteke edo kargagabea izan daiteke, bezeroarekin izandako negoziazioen arabera.</span><span class="sxs-lookup"><span data-stu-id="395ff-117">This transaction can either be billed later or marked as non-chargeable, depending on the negotiations with the customer.</span></span>
