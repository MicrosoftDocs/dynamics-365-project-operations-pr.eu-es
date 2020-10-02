---
title: Zuzendutako fakturak
description: Gai honek zuzendutako fakturak egiteari buruzko informazioa ematen du.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
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
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: e14da1c07d5b697de6caf1b9041c30581ecff102
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898066"
---
# <a name="corrected-invoices"></a><span data-ttu-id="89cde-103">Zuzendutako fakturak</span><span class="sxs-lookup"><span data-stu-id="89cde-103">Corrected invoices</span></span>

<span data-ttu-id="89cde-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="89cde-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="89cde-105">Berretsitako fakturak editatu daitezke.</span><span class="sxs-lookup"><span data-stu-id="89cde-105">Confirmed invoices can be edited.</span></span> <span data-ttu-id="89cde-106">Berretsitako faktura editatzen duzunean, zuzendutako fakturaren zirriborro berria sortzen da.</span><span class="sxs-lookup"><span data-stu-id="89cde-106">When you edit a confirmed invoice, a draft of the corrected invoice is created.</span></span> <span data-ttu-id="89cde-107">Jatorrizko fakturatik transakzio eta kantitate guztiak berraztertu nahi dituzulako hipotesiarekin, zuzendutako faktura honek jatorrizko fakturaren transakzio guztiak barne hartzen ditu, eta bertan dauden kantitate guztiak zero (0) dira.</span><span class="sxs-lookup"><span data-stu-id="89cde-107">Because the assumption is that you want to reverse all the transactions and quantities from the original invoice, the corrected invoice includes all the transactions from the original invoice, and all the quantities on it are zero (0).</span></span>

<span data-ttu-id="89cde-108">Transakzioren bat zuzentzen ez bada, faktura zuzentzailearen zirriborrotik kendu dezakezu.</span><span class="sxs-lookup"><span data-stu-id="89cde-108">When transactions don't require correction, you can remove them from the draft corrective invoice.</span></span> <span data-ttu-id="89cde-109">Kantitate partziala soilik alderantzikatzeko edo itzultzeko, editatu dezakezu Kopurua eremuan, lerroaren xehetasunean.</span><span class="sxs-lookup"><span data-stu-id="89cde-109">To reverse or return only a partial quantity, you can edit the Quantity field on the line detail.</span></span> <span data-ttu-id="89cde-110">Fakturen lerroaren xehetasuna irekitzen baduzu, fakturaren jatorrizko kantitatea ikus dezakezu.</span><span class="sxs-lookup"><span data-stu-id="89cde-110">If you open the invoice line detail, you can see the original invoice quantity.</span></span> <span data-ttu-id="89cde-111">Uneko fakturaren kantitatea editatu ahal izango duzu, fakturaren jatorrizko kantitatea baino gutxiago edo gehiago izan dadin.</span><span class="sxs-lookup"><span data-stu-id="89cde-111">You can then edit the current invoice quantity so that it's less than or more than the original invoice quantity.</span></span>

<span data-ttu-id="89cde-112">Faktura zuzentzailea baieztatzen duzunean, fakturatutako jatorrizko salmenten benetakoa alderantzikatu egiten da eta fakturatutako salmenta erreal berria sortzen da.</span><span class="sxs-lookup"><span data-stu-id="89cde-112">When you confirm a corrective invoice, the original billed sales actual is reversed, and a new billed sales actual is created.</span></span> <span data-ttu-id="89cde-113">Kantitatea murriztuko balitz, aldaketak fakturatu gabeko salmenta berriak ere sortuko ditu.</span><span class="sxs-lookup"><span data-stu-id="89cde-113">If the quantity was reduced, the difference will cause a new unbilled sales actual to be created too.</span></span> <span data-ttu-id="89cde-114">Adibidez, fakturatutako jatorrizko salmenta zortzi orduz izan bazenuen eta zuzendutako fakturaren linearen xehetasunak sei orduko kantitatera murriztu badu, jatorrizko fakturatutako salmenta-lerroa alderantzikatuko da eta bi berri sortuko dira:</span><span class="sxs-lookup"><span data-stu-id="89cde-114">For example, if the original billed sale was for eight hours, and the corrected invoice line detail has a reduced quantity of six hours, the original billed sales line is revered and two new actuals are created:</span></span>

- <span data-ttu-id="89cde-115">Fakturatutako salmentak sei orduz fakturatu dira.</span><span class="sxs-lookup"><span data-stu-id="89cde-115">A billed sales actual for six hours.</span></span>
- <span data-ttu-id="89cde-116">Bete gabeko salmentak benetako gainerako bi orduetan.</span><span class="sxs-lookup"><span data-stu-id="89cde-116">An unbilled sales actual for the remaining two hours.</span></span> <span data-ttu-id="89cde-117">Transakzio hau beranduago fakturatu daiteke edo kargagabea izan daiteke, bezeroarekin izandako negoziazioen arabera.</span><span class="sxs-lookup"><span data-stu-id="89cde-117">This transaction can either be billed later or marked as non-chargeable, depending on the negotiations with the customer.</span></span>
