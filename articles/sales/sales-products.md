---
title: Produktuak
description: Gai honek zure erakundeak eskaintzen dituen produktuei eta prezioei buruz bezeroei informazioa emateko erabil dezakezun produktuen katalogoari buruzko informazioa eskaintzen du.
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
ms.openlocfilehash: 28397fd49ad4cdb2c820ef4b6f198f410995ba0f
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898696"
---
# <a name="products"></a><span data-ttu-id="df4b1-103">Produktuak</span><span class="sxs-lookup"><span data-stu-id="df4b1-103">Products</span></span>

<span data-ttu-id="df4b1-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="df4b1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="df4b1-105">Produktuak zure erakundearen berariazko backbone dira.</span><span class="sxs-lookup"><span data-stu-id="df4b1-105">Products are the backbone of your business.</span></span> <span data-ttu-id="df4b1-106">Dynamics 365 Sales Professional-eko produktuen katalogoa produktuei eta beren prezio-informazioari leku da.</span><span class="sxs-lookup"><span data-stu-id="df4b1-106">The product catalog in Dynamics 365 Sales Professional is a collection of products and pricing information.</span></span> <span data-ttu-id="df4b1-107">Egin salmenta-agenteak zure produktuen katalogoa sortu beren salmentak areagotzeari bizkorrago.</span><span class="sxs-lookup"><span data-stu-id="df4b1-107">Make it easier for your sales reps to increase their sales by creating a product catalog quickly.</span></span>

## <a name="add-a-product"></a><span data-ttu-id="df4b1-108">Gehitu produktua</span><span class="sxs-lookup"><span data-stu-id="df4b1-108">Add a product</span></span>

1.  <span data-ttu-id="df4b1-109">Ziurtatu Salmenta-kudeatzaile profesionala edo Sistemaren administratzailearen funtzioa edo antzeko baimenak dituzula Dynamics 365 Sales Professional-en produktuak gehitu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="df4b1-109">Make sure you have the Sales Manager Professional or a System Administrator role so you can add products in Dynamics 365 Sales Professional.</span></span>
2.  <span data-ttu-id="df4b1-110">Gunearen mapako **Konfigurazioa** atalean, hautatu **Produktuak**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-110">In the site map, under **Setup**, select **Products**.</span></span>
3.  <span data-ttu-id="df4b1-111">Aukeratu **Gehitu produktua** eta bete informazio hau:</span><span class="sxs-lookup"><span data-stu-id="df4b1-111">Select **Add Product** and fill in the following information:</span></span>

    -  <span data-ttu-id="df4b1-112">**Izena**</span><span class="sxs-lookup"><span data-stu-id="df4b1-112">**Name**</span></span>
    -  <span data-ttu-id="df4b1-113">**Produktuaren IDa**</span><span class="sxs-lookup"><span data-stu-id="df4b1-113">**Product ID**</span></span>
    -  <span data-ttu-id="df4b1-114">**Bazkidea**: hautatu produkturako produktu-familia nagusia.</span><span class="sxs-lookup"><span data-stu-id="df4b1-114">**Parent**: Select a parent product family for the product.</span></span> <span data-ttu-id="df4b1-115">Produktu-familiaren bigarren mailako produktu multzo bat sortzen ari bazara, produktu-familia nagusiaren izena hemen beteta dago.</span><span class="sxs-lookup"><span data-stu-id="df4b1-115">If you're creating a child product in a product family, the name of the parent product family is populated here.</span></span> <span data-ttu-id="df4b1-116">Hori ezin da aldatu erregistroa gorde ondoren.</span><span class="sxs-lookup"><span data-stu-id="df4b1-116">This can't be changed after the record is saved.</span></span>
    -  <span data-ttu-id="df4b1-117">**Baliozkoa data honetatik**/**Baliozkoa data honetara arte**: zehaztu produktua baliozkoa izango den denbora tartea; horretarako, hautatu **Baliozkoa data honetatik** and **Baliozkoa data honetara arte** datak.</span><span class="sxs-lookup"><span data-stu-id="df4b1-117">**Valid From**/**Valid To**: Define the period the product is valid for by selecting a **Valid From** and **Valid To** date.</span></span>
    -  <span data-ttu-id="df4b1-118">**Salmenta-unitatea**: Hautatu salmenta-unitatea.</span><span class="sxs-lookup"><span data-stu-id="df4b1-118">**Unit Group**: Select a unit group.</span></span> <span data-ttu-id="df4b1-119">Salmenta-unitateko unitate hainbat saltzeko produktuak eta elementuak banakako modua zehazten leku gehienez zatitu taldekatzen diren da.</span><span class="sxs-lookup"><span data-stu-id="df4b1-119">A unit group is a collection of various units a product is sold in and defines how individual items are grouped into larger quantities.</span></span> <span data-ttu-id="df4b1-120">Adibidez, haziak gehitzen ari bazara produktu gisa, "Haziak" izena duen salmenta-talde bat sortu behar duzu eta bere unitate nagusia "Pakete"gisa zehaztu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="df4b1-120">For example, if you're adding seeds as a product, you might have created a unit group called "Seeds" and defined its primary unit as "packet."</span></span>
    -  <span data-ttu-id="df4b1-121">**Lehenetsitako unitatea**: hautatu produktua gehien salduko duen unitatea.</span><span class="sxs-lookup"><span data-stu-id="df4b1-121">**Default Unit**: Select the most common unit in which the product will be sold.</span></span> <span data-ttu-id="df4b1-122">Unitateak produktuak saltzen dituzun kantitateak edo neurketak dira.</span><span class="sxs-lookup"><span data-stu-id="df4b1-122">Units are the quantities or measurements that you sell your products in.</span></span> <span data-ttu-id="df4b1-123">Adibidez, haziak gehitu badituzu produktu gisa, paketetan, kaxetan edo paletetan sal ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="df4b1-123">For example, if you're adding seeds as a product, you can sell it in packets, boxes, or pallets.</span></span> <span data-ttu-id="df4b1-124">Produktuaren unitate bakoitzaren horien da.</span><span class="sxs-lookup"><span data-stu-id="df4b1-124">Each of these becomes a unit of the product.</span></span> <span data-ttu-id="df4b1-125">Seeds gehienak saltzen packets atalean, hautatu duzun unitate gisa.</span><span class="sxs-lookup"><span data-stu-id="df4b1-125">If seeds are mostly sold in packets, select that as the unit.</span></span>
    -  <span data-ttu-id="df4b1-126">**Lehenetsitako prezio-zerrenda**: produktua berria bada, eremu hau irakurtzeko soilik izango da.</span><span class="sxs-lookup"><span data-stu-id="df4b1-126">**Default Price List**: If this is a new product, this field is read-only.</span></span> <span data-ttu-id="df4b1-127">Prezio-zerrenda lehenetsia hautatu ahal izateko, aurrena dagozkion beharrezko eremu guztiak bete eta, ondoren, erregistroa gorde behar duzu.</span><span class="sxs-lookup"><span data-stu-id="df4b1-127">Before you can select a default price list, you must complete all the required fields and then save the record.</span></span> <span data-ttu-id="df4b1-128">Lehenetsitako prezio-zerrenda beharrezkoa ez den arren, produktuaren erregistroa gordetzen duzunean, komeni da produktu bakoitzarentzat lehenetsitako prezio-zerrenda bat ezartzea.</span><span class="sxs-lookup"><span data-stu-id="df4b1-128">Although the default price list is not required, after you save the product record, it is a good idea to set a default price list for each product.</span></span> <span data-ttu-id="df4b1-129">Ondoren, bezero baten erregistroak prezio-zerrendarik ez badu, Sales aplikazioak lehenetsitako prezio-zerrenda erabil dezake eskaintzak, eskaerak eta fakturak sortzeko.</span><span class="sxs-lookup"><span data-stu-id="df4b1-129">Then, if a customer record does not contain a price list, Sales can use the default price list for generating quotes, orders, and invoices.</span></span>
    -  <span data-ttu-id="df4b1-130">**Onartutako hamartarrak**: sartu 0 eta 5 arteko zenbaki oso bat.</span><span class="sxs-lookup"><span data-stu-id="df4b1-130">**Decimals Supported**: Enter a whole number between 0 and 5.</span></span> <span data-ttu-id="df4b1-131">Produktua ezin bada zatikietan zatitu, 0 idatzi.</span><span class="sxs-lookup"><span data-stu-id="df4b1-131">If the product can't be divided into fractional quantities, enter 0.</span></span> <span data-ttu-id="df4b1-132">Zehaztasun maila **Kopurua** eremuan eskaintza, eskaera edo faktura-produktu erregistroan balioztatutako balioa da eremu honetan produktuak erlazionatutako prezio-zerrendarik ez badu.</span><span class="sxs-lookup"><span data-stu-id="df4b1-132">The precision of the **Quantity** field in the quote, order, or invoice product record is validated against the value in this field if the product does not have an associated price list.</span></span>
    -  <span data-ttu-id="df4b1-133">**Gaia**: erlazionatu produktua gai batekin.</span><span class="sxs-lookup"><span data-stu-id="df4b1-133">**Subject**: Associate this product with a subject.</span></span> <span data-ttu-id="df4b1-134">Gaiak produktuak sailkatzeko eta txostenak iragazteko erabil ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="df4b1-134">You can use subjects to categorize your products and to filter reports.</span></span>

4.  <span data-ttu-id="df4b1-135">Sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-135">Select **Save**.</span></span>
5.  <span data-ttu-id="df4b1-136">**Xehetasun gehiago** fitxan, **Prezio-zerrendako elementuak** atalean, hautatu **Komando gehiago**, eta hautatu **Gehitu prezioen zerrenda berria**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-136">On the **Additional Details** tab, in the **Price List Items** section, select **More commands**, and then select **Add New Price List Item**.</span></span>
7.  <span data-ttu-id="df4b1-137">**Xehetasun gehiago** fitxan, **Produktuen erlazioa** atalean, hautatu **Komando gehiago** ikonoa, eta hautatu **Gehitu produktu berrien erlazioa**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-137">On the **Additional Details** tab, in the **Product Relationship** section, select the **More commands** icon, and then select **Add New Product Relationship.**</span></span>
8.  <span data-ttu-id="df4b1-138">Aplikazioan, **Produktu-erlazio Berria** inprimakian, idatzi honako xehetasunak eta komando-barran, hautatu **Gorde eta itxi**:</span><span class="sxs-lookup"><span data-stu-id="df4b1-138">In the **New Product Relationship** form, enter the following details, and on the command bar, select **Save and Close**:</span></span>

    -   <span data-ttu-id="df4b1-139">**Erlazionatutako produktua**: Hautatu kudeatzen ari zaren eta lehendik dagoen produktu-erregistroan erlazionatutako produktu gisa gehitu nahi duzun produktua.</span><span class="sxs-lookup"><span data-stu-id="df4b1-139">**Related Product**: Select a product that you want to add as a related product to the existing product record you're working on.</span></span>
    -   <span data-ttu-id="df4b1-140">**Salmenten erlazio mota**: Gehitu produktu bat gidatua, salmenta gurutzatua, accessory gisa edo ordezko produktu nahi duzun hautatu.</span><span class="sxs-lookup"><span data-stu-id="df4b1-140">**Sales Relation Type**: Select whether you want to add the product as an up-sell, cross-sell, accessory, or substitute product.</span></span>
    -   <span data-ttu-id="df4b1-141">**Zuzenketa**: Hautatu produktuak arteko erlazioa izango noranzko bakarrekoa edo noranzko bikoa den ala ez.</span><span class="sxs-lookup"><span data-stu-id="df4b1-141">**Direction**:Select whether the relationship between the products will be unidirectional or bidirectional.</span></span> <span data-ttu-id="df4b1-142">Hautatzean Noranzko Bakarrekoa, aukeran hautatu duzun produktu **Erlazionatutako produktua** aukera gomendio gisa erakutsiko da lehendik dagoen produkturako baina ez alderantziz.</span><span class="sxs-lookup"><span data-stu-id="df4b1-142">When you select unidirectional, the product that you select in **Related Product** will be shown as a recommendation for the existing product but not vice versa.</span></span>

9.  <span data-ttu-id="df4b1-143">Produktuen inprimakian, hautatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-143">On the Product form, select **Save**.</span></span>

## <a name="import-products"></a><span data-ttu-id="df4b1-144">Inportatu produktuak</span><span class="sxs-lookup"><span data-stu-id="df4b1-144">Import products</span></span>

<span data-ttu-id="df4b1-145">Inportazio txantiloiak erabil ditzakezu produktu solteak bidaltzeko Dynamics 365 Sales-era.</span><span class="sxs-lookup"><span data-stu-id="df4b1-145">You can use import templates to bring bulk product data into Dynamics 365 Sales.</span></span>

## <a name="revise-a-product"></a><span data-ttu-id="df4b1-146">Berrikusi produktuak</span><span class="sxs-lookup"><span data-stu-id="df4b1-146">Revise a product</span></span>

<span data-ttu-id="df4b1-147">Mantendu bizkor guztietatik beharren produktuak propietateak eta argitaratu berriro informazioa horrela, zure agente salmenta-inbentarioa azken aldaketak ikus ditzakezu eguneratu produktu-inbentarioa.</span><span class="sxs-lookup"><span data-stu-id="df4b1-147">Keep the product inventory updated by quickly revising properties for the products, as required, and republishing the information so that your sales agents can see the latest changes to the inventory.</span></span>

1.  <span data-ttu-id="df4b1-148">Ziurtatu ondorengo segurtasun-funtzio edo baimen baliokideetako bat duzula: Sistemaren administratzailea, Sistemaren pertsonalizatzailea, Salmenten arduraduna, Salmenten zuzendariordea, Marketineko zuzendariordea edo Zuzendari nagusia.</span><span class="sxs-lookup"><span data-stu-id="df4b1-148">Make sure that you have one of the following security roles or equivalent permissions: System Administrator, System Customizer, Sales Manager, Vice President of Sales, Vice President of Marketing, or CEO-Business Manager.</span></span>
2.  <span data-ttu-id="df4b1-149">Gunearen mapan, hautatu **Produktuak**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-149">In the site map, select **Products**.</span></span>
3.  <span data-ttu-id="df4b1-150">Ireki aldatu nahi duzun produktu, multzo edo familia aktibo bat eta, komando-barran, hautatu **Berrikusi**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-150">Open an active product that you want to change, and on the command bar, select **Revise**.</span></span>
4.  <span data-ttu-id="df4b1-151">**Berretsi berrikustea** elkarrizketa-koadroan, hautatu **Berretsi**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-151">In the **Confirm Revise** dialog box, select **Confirm**.</span></span> <span data-ttu-id="df4b1-152">Honek produktu egoera aldatzen **Atalean Berrikuspenaren**</span><span class="sxs-lookup"><span data-stu-id="df4b1-152">This will change the product status to **Under Revision**.</span></span>
5.  <span data-ttu-id="df4b1-153">Aldaketak egin ondoren, komando-barran, hautatu **Argitaratu**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-153">After you're done making changes, on the command bar, select **Publish**.</span></span>

    > [!TIP]
    > <span data-ttu-id="df4b1-154">Aldaketak berreskuratzeko eta produktuaren azken bertsio aktiboarekin jarraitzeko, hautatu **Itzuli**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-154">To revert the changes and continue with the last active version of the product, select **Revert**.</span></span> <span data-ttu-id="df4b1-155">Produktuaren egoera babeskopia aldaketak hau **Aktibo**</span><span class="sxs-lookup"><span data-stu-id="df4b1-155">This changes the status of the product back to **Active**.</span></span>

## <a name="clone-a-product"></a><span data-ttu-id="df4b1-156">Produktuak klonatu</span><span class="sxs-lookup"><span data-stu-id="df4b1-156">Clone a product</span></span> 

<span data-ttu-id="df4b1-157">Produktu berri bat sortzen ari bazara, denbora aurrezteko lehendik dagoen bat kopia dezakezu.</span><span class="sxs-lookup"><span data-stu-id="df4b1-157">When you're creating a new product, save time by cloning an existing one.</span></span> <span data-ttu-id="df4b1-158">Sortzen du jatorrizko kopia xehetasunekin guztiak izan ezik, izena eta ida.</span><span class="sxs-lookup"><span data-stu-id="df4b1-158">This creates a copy of the original record with all the details except for the name and ID.</span></span>

1.  <span data-ttu-id="df4b1-159">Ziurtatu ondorengo segurtasun-funtzio edo baimen baliokideetako bat duzula: Sistemaren administratzailea, Sistemaren pertsonalizatzailea, Salmenten arduraduna, Salmenten zuzendariordea, Marketineko zuzendariordea edo Zuzendari nagusia.</span><span class="sxs-lookup"><span data-stu-id="df4b1-159">Make sure that you have one of the following security roles or equivalent permissions: System Administrator, System Customizer, Sales Manager, Vice President of Sales, Vice President of Marketing, or CEO-Business Manager.</span></span>
2.  <span data-ttu-id="df4b1-160">Gunearen mapan, hautatu **Produktuak**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-160">In the site map, select **Products**.</span></span>
3.  <span data-ttu-id="df4b1-161">Hautatu klonatu nahi duzun produktu bat eta, komando-barran, hautatu **Klonatu**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-161">Select a product record that you want to clone, and on the command bar, select **Clone**.</span></span> <span data-ttu-id="df4b1-162">Berresteko elkarrizketa-koadroa agertzen da.</span><span class="sxs-lookup"><span data-stu-id="df4b1-162">A confirmation dialog box appears.</span></span>
4.  <span data-ttu-id="df4b1-163">Hautatu **Berretsi**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-163">Select **Confirm**.</span></span>

<span data-ttu-id="df4b1-164">Produktu-erregistro berri bat irekiko bera izan ezik, izena eta ida. jatorrizko duzuna gisa xehetasunekin</span><span class="sxs-lookup"><span data-stu-id="df4b1-164">A new product record opens with the same details as the original one except for the name and ID.</span></span>

## <a name="retire-a-product"></a><span data-ttu-id="df4b1-165">Erretiratu produktuak</span><span class="sxs-lookup"><span data-stu-id="df4b1-165">Retire a product</span></span> 

<span data-ttu-id="df4b1-166">Erakundeak ez badu gehiago saltzen produktu bat, ken ezazu saltzaileek erabilgarri eduki ez dezaten.</span><span class="sxs-lookup"><span data-stu-id="df4b1-166">If your organization doesn't sell a product anymore, retire it so that the product is no longer available to your sales agents.</span></span>

1.  <span data-ttu-id="df4b1-167">Ziurtatu Sistemaren administratzailearen edo Sales Professional kudeatzailearen funtzioa edo antzeko baimenak dituzula.</span><span class="sxs-lookup"><span data-stu-id="df4b1-167">Make sure that you have the System Administrator or Sales Professional Manager role or equivalent permissions.</span></span>
2.  <span data-ttu-id="df4b1-168">Gunearen mapan, hautatu **Produktuak**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-168">In the site map, select **Products**.</span></span>
3.  <span data-ttu-id="df4b1-169">Ireki kendu nahi duzun produktua, multzo edo familia aktibo bat eta, komando-barran, hautatu **Kendu**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-169">Open an active product that you want to retire, and on the command bar, select **Retire**.</span></span>
4.  <span data-ttu-id="df4b1-170">**Berretsi erretiratzea** elkarrizketa-koadroan, hautatu **Berretsi**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-170">In the **Confirm Retire** dialog box, select **Confirm**.</span></span>


## <a name="delete-a-product"></a><span data-ttu-id="df4b1-171">Ezabatu produktu bat</span><span class="sxs-lookup"><span data-stu-id="df4b1-171">Delete a product</span></span>

<span data-ttu-id="df4b1-172">Horrela, produktu bat saltzen gelditzeko, ezaba ezazu.</span><span class="sxs-lookup"><span data-stu-id="df4b1-172">To stop selling a product, delete it.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="df4b1-173">Ezin duzu eskuratu ezabatutako erregistro bat.</span><span class="sxs-lookup"><span data-stu-id="df4b1-173">You can't recover a deleted record.</span></span>

1.  <span data-ttu-id="df4b1-174">Ziurtatu Sistemaren administratzailearen edo Sales Professional kudeatzailearen funtzioa edo antzeko baimenak dituzula.</span><span class="sxs-lookup"><span data-stu-id="df4b1-174">Make sure that you have the System Administrator or Sales Professional Manager role or equivalent permissions.</span></span>
2.  <span data-ttu-id="df4b1-175">Gunearen mapan, hautatu **Produktuak**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-175">In the site map, select **Products**.</span></span>
3.  <span data-ttu-id="df4b1-176">Hautatu ezabatu nahi duzun produktu bat eta, komando-barran, hautatu **Ezabatu**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-176">Select a product record you want to delete, and on the command bar, select **Delete**.</span></span>
4.  <span data-ttu-id="df4b1-177">**Berretsi ezabatzea** elkarrizketa-koadroan, hautatu **Jarraitu**.</span><span class="sxs-lookup"><span data-stu-id="df4b1-177">In the **Confirm Deletion** dialog box, select **Continue**.</span></span>
 
 ## <a name="quantity-factors-for-products"></a><span data-ttu-id="df4b1-178">Produktuen kantitate faktoreak</span><span class="sxs-lookup"><span data-stu-id="df4b1-178">Quantity factors for products</span></span>

<span data-ttu-id="df4b1-179">Kantitate faktoreak erabiltzen ditu harpidedun oinarritutako produktuen salmenta sustatzeko.</span><span class="sxs-lookup"><span data-stu-id="df4b1-179">Quantity factors support the sale of subscription-based products.</span></span> <span data-ttu-id="df4b1-180">Harpidetzetan oinarritutako produktuetarako, aurrekontuan edo proiektuaren kontratuaren lerroan erabiltzaile-hilabete kopurua adierazten da.</span><span class="sxs-lookup"><span data-stu-id="df4b1-180">For subscription-based products, the quantity on the quote or project contract line is expressed as the number of user months.</span></span>

<span data-ttu-id="df4b1-181">Normalean, harpidedun softwarearen prezioa katalogoan gordetzen da erabiltzaile bakoitzeko prezio gisa.</span><span class="sxs-lookup"><span data-stu-id="df4b1-181">Usually, the price of subscription software is stored in the catalog as the price per user per month.</span></span> <span data-ttu-id="df4b1-182">Hala ere, beste denbora deskribapen batzuk erabil ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="df4b1-182">However, you can use other time descriptions instead.</span></span> <span data-ttu-id="df4b1-183">Salmenta prozesuan, aurrekontuen lerroko prezioa erabiltzaile bakoitzeko, salmentako IT agentearen bidez negoziatu eta deskontatu zen hileko prezioa izan ohi da.</span><span class="sxs-lookup"><span data-stu-id="df4b1-183">During the sales process, the price on the quote line is usually the per-user, per-month price that was negotiated and discounted by the IT sales agent.</span></span> <span data-ttu-id="df4b1-184">Akordio bakoitzak erabiltzaile kopurua eta harpidetza hilabete desberdinak ditu.</span><span class="sxs-lookup"><span data-stu-id="df4b1-184">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="df4b1-185">Aurrekontuen lerroaren zenbatekoa kalkulatzeko erabiltzen den kantitatea erabiltzaile kopurua eta harpidetza hilabeteen produktua da.</span><span class="sxs-lookup"><span data-stu-id="df4b1-185">The quantity that is used to compute the amount of the quote line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="df4b1-186">Kopuru-faktoreek produktuaren atributuetan oinarritzen dira.</span><span class="sxs-lookup"><span data-stu-id="df4b1-186">Quantity factors rely on product attributes.</span></span> <span data-ttu-id="df4b1-187">Produktu baterako propietate espezifikoak konfiguratzen dituzunean, propietate horien edo propietate guztien azpimultzoa uzten dizu kantitate faktore gisa.</span><span class="sxs-lookup"><span data-stu-id="df4b1-187">When you configure specific properties for a product, you can flag a subset of those properties, or all the properties, as quantity factors.</span></span>

<span data-ttu-id="df4b1-188">Sistemak balioztatzen du zenbakizko datu mota bat duten zenbakizko propietateak edo produktuaren propietateak kantitate faktore gisa markatzen direla.</span><span class="sxs-lookup"><span data-stu-id="df4b1-188">The system validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="df4b1-189">Kantitate-faktoreak konfiguratutako produktu bat aurrekontu-lerrora gehitzen denean, **Kopurua** aurrekontuen lerroan irakurtzeko soilik eremu bihurtzen da.</span><span class="sxs-lookup"><span data-stu-id="df4b1-189">When a product that quantity factors are configured for is added to a quote line, the **Quantity** field on the quote line becomes a read-only field.</span></span> <span data-ttu-id="df4b1-190">Kantitate faktoreak diren produktuaren propietateen balioak sartu ondoren, aurrekontuen lerroaren kantitatea kalkulatzen du.</span><span class="sxs-lookup"><span data-stu-id="df4b1-190">After you enter values for product properties that are quantity factors, the quantity of the quote line is calculated.</span></span>

<span data-ttu-id="df4b1-191">Adibidez, propietate hauek badaude:</span><span class="sxs-lookup"><span data-stu-id="df4b1-191">For example, if there are the following properties:</span></span> 

- <span data-ttu-id="df4b1-192">**Erabiltzaile kop**: erabiltzaile kopurua</span><span class="sxs-lookup"><span data-stu-id="df4b1-192">**No of users**: The number of users</span></span> 
- <span data-ttu-id="df4b1-193">**Hilabete kop**: harpidetza-hilabete kopurua</span><span class="sxs-lookup"><span data-stu-id="df4b1-193">**No of Months**: The number of subscription months</span></span>
- <span data-ttu-id="df4b1-194">**SKU produktua**</span><span class="sxs-lookup"><span data-stu-id="df4b1-194">**Product SKU**</span></span> 

<span data-ttu-id="df4b1-195">**Erabiltzaile kop** eta **Hilabete kop** propietateak kantitate faktore gisa markatu daitezke produktuaren lerroko propietateak editatzean.</span><span class="sxs-lookup"><span data-stu-id="df4b1-195">The **No of Users** and **No of Months** properties can be flagged as quantity factors by editing the properties of the product line.</span></span> 