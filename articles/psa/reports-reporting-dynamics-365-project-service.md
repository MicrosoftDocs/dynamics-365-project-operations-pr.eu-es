---
title: Txostenaren orri nagusia
description: Gai honek txostenari buruzko informazioa ematen du Dynamics 365 Project Service Automation aplikazioan.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 78c62f69c6529669789a461f1ded8e3ea5f8219e
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5283263"
---
# <a name="reporting-home-page"></a><span data-ttu-id="a7473-103">Etxeko orria salatzen</span><span class="sxs-lookup"><span data-stu-id="a7473-103">Reporting home page</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="a7473-104">Microsoft Dynamics 365 Project Service Automation aplikazioak negozioaren eragiketak modu eraginkorrean kudeatzen laguntzen die proiektuan oinarritutako erakundeei.</span><span class="sxs-lookup"><span data-stu-id="a7473-104">Microsoft Dynamics 365 Project Service Automation lets project-based organizations efficiently manage the operations of their business.</span></span> <span data-ttu-id="a7473-105">Edozein proiektutan, taldekideek abagunea eta eskaria kudeatu behar dute eta lana planifikatu behar dute, proiektuei baliabideak eman, lana planaren arabera kudeatu, lanaren faktura egin eta, ondoren, lana burutu beharko dute proiektua osatzeko.</span><span class="sxs-lookup"><span data-stu-id="a7473-105">On any project, team members must manage the opportunity, quote and plan the work, resource the projects, manage the work according to the plan, bill for the work, and then do the work to complete the project.</span></span> <span data-ttu-id="a7473-106">Eragiketen berri emateko gaitasuna funtsezkoa da erakundearen osasuna zehazteko eta beharrezkoa den edozein ekintza zuzentzaile hartzeko.</span><span class="sxs-lookup"><span data-stu-id="a7473-106">The ability to report on operations is key to determining the health of the organization and taking any corrective action that's required.</span></span> <span data-ttu-id="a7473-107">PSA-k Microsoft Dynamics 365-eko berri emateko metodoak eta teknologiak erabiltzen ditu txosten guztietan.</span><span class="sxs-lookup"><span data-stu-id="a7473-107">PSA uses Microsoft Dynamics 365 reporting methods and technologies for all its reporting.</span></span> <span data-ttu-id="a7473-108">Jakinarazteko aukerei buruzko informazio gehiago eskuratzeko, ikusi [Txostena idazteko gida Dynamics 365 Customer Engagement (on-premises), 9. bertsioa](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/reporting-analytics-with-dynamics-365).</span><span class="sxs-lookup"><span data-stu-id="a7473-108">For more information about the options for reporting, see the [Report writing guide for Dynamics 365 Customer Engagement (on-premises), version 9](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/reporting-analytics-with-dynamics-365).</span></span>

## <a name="report-wizard"></a><span data-ttu-id="a7473-109">Txostenentzako morroia</span><span class="sxs-lookup"><span data-stu-id="a7473-109">Report Wizard</span></span>

<span data-ttu-id="a7473-110">Txostenentzako morroiari esker, garatzaile ez direnek txosten errazak sor ditzakete.</span><span class="sxs-lookup"><span data-stu-id="a7473-110">The Report Wizard lets non-developers create simple reports.</span></span> <span data-ttu-id="a7473-111">Aplikazioa lehendik dagoen plataforma batean eraikita dagoenez, egoera [Sortu edo editatu txostena txostenentzako morroia erabiliz](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/basics/create-edit-copy-report-wizard) atalean dokumentatzen den esperientziaren berdina da.</span><span class="sxs-lookup"><span data-stu-id="a7473-111">Because the app is built on an existing platform, the experience is the same as the experience that is documented in [Create or edit a report using the Report Wizard](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/basics/create-edit-copy-report-wizard).</span></span> <span data-ttu-id="a7473-112">Hala ere, Project Service Automation-en berariazko entitateak erabiliko dituzu.</span><span class="sxs-lookup"><span data-stu-id="a7473-112">However, you will use the Project Service Automation-specific entities.</span></span>

## <a name="custom-sql-server-reporting-services-reports"></a><span data-ttu-id="a7473-113">SQL Server Reporting Services-en txosten pertsonalizatuak</span><span class="sxs-lookup"><span data-stu-id="a7473-113">Custom SQL Server Reporting Services reports</span></span>

<span data-ttu-id="a7473-114">Zure negozioak txostenentzako morroia erabiliz sortu ezin daitekeen txosten zehatz bat behar badu, txosten pertsonalizatua sor dezakezu.</span><span class="sxs-lookup"><span data-stu-id="a7473-114">If your business requires a specific report that can't be created by using the Report Wizard, you can create a custom report.</span></span> <span data-ttu-id="a7473-115">Microsoft Visual Studio izan behar duzu instalatuta, dagokion Microsoft SQL Server Data Tools-ekin eta txostena sortzeko baimenekin batera.</span><span class="sxs-lookup"><span data-stu-id="a7473-115">You must have Microsoft Visual Studio installed, together with the appropriate Microsoft SQL Server Data Tools and Report Authoring Extensions.</span></span> <span data-ttu-id="a7473-116">Tresna eta bertsioei buruzko informazio gehiago lortzeko, ikusi [Txostena idazteko ingurunea SQL Server Data Tools erabiliz](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/report-writing-environment-using-sql-server-data-tools).</span><span class="sxs-lookup"><span data-stu-id="a7473-116">For more information about tools and versions, see [Report writing environment using SQL Server Data Tools](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/report-writing-environment-using-sql-server-data-tools).</span></span> <span data-ttu-id="a7473-117">Txosten pertsonalizatua sortzeari buruzko informazioa lortzeko, ikusi [Sortu txosten berria SQL Server Data Tools erabiliz](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/create-a-new-report-using-sql-server-data-tools).</span><span class="sxs-lookup"><span data-stu-id="a7473-117">For information about how to create a custom report, see [Create a new report using SQL Server Data Tools](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/create-a-new-report-using-sql-server-data-tools).</span></span>

## <a name="power-bi-insights-apps"></a><span data-ttu-id="a7473-118">Power BI Insights aplikazioak</span><span class="sxs-lookup"><span data-stu-id="a7473-118">Power BI insights apps</span></span>

<span data-ttu-id="a7473-119">Elkarrekin, Microsoft Power BI eta Dynamics 365 aplikazioek zure datuekin lan egiteko modu indartsua ematen dizu, Insights aplikazioen inprimakian.</span><span class="sxs-lookup"><span data-stu-id="a7473-119">Together, Microsoft Power BI and Dynamics 365 give you a powerful way to work with your data, in the form of insights apps.</span></span> <span data-ttu-id="a7473-120">Insights aplikazioen erabilgarritasunari buruzko informazio gehiago lortzeko, ikusi [Power BI Insights aplikazioen orrialdea](https://powerbi.microsoft.com/power-bi-insights-apps/).</span><span class="sxs-lookup"><span data-stu-id="a7473-120">For information about the availability of insights apps, see the [Power BI insights apps page](https://powerbi.microsoft.com/power-bi-insights-apps/).</span></span>


## <a name="additional-resources"></a><span data-ttu-id="a7473-121">Baliabide gehigarriak</span><span class="sxs-lookup"><span data-stu-id="a7473-121">Additional resources</span></span>
<span data-ttu-id="a7473-122">PSA-n txostenak egiteari buruzko informazio gehiago lortzeko, ikusi gai hauek:</span><span class="sxs-lookup"><span data-stu-id="a7473-122">For more information about reporting in PSA, see the following topics:</span></span>

- [<span data-ttu-id="a7473-123">Project Service-ren datu ereduarekin lan egitea</span><span class="sxs-lookup"><span data-stu-id="a7473-123">Working with the Project Service data model</span></span>](reports-working-project-service-data-model.md)
- [<span data-ttu-id="a7473-124">Aginte-panelak</span><span class="sxs-lookup"><span data-stu-id="a7473-124">Dashboards</span></span>](reports-dashboards.md)



[!INCLUDE[footer-include](../includes/footer-banner.md)]