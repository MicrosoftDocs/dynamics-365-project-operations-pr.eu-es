---
title: Ezarri eremu pertsonalizatuak Microsoft Dynamics 365 Project Timesheet mugikorretarako aplikazioa iOS eta Android
description: Gai honek luzapenak eremu pertsonalizatuak ezartzeko ohiko ereduak eskaintzen ditu.
author: Yowelle
manager: AnnBe
ms.date: 05/29/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 10.0.3
ms.search.validFrom: 2019-05-29
ms.openlocfilehash: 5dae571fce746b49281587f5349774a7f2c4111b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5270978"
---
# <a name="implement-custom-fields-for-the-microsoft-dynamics-365-project-timesheet-mobile-app-on-ios-and-android"></a><span data-ttu-id="eabbb-103">Ezarri eremu pertsonalizatuak Microsoft Dynamics 365 Project Timesheet mugikorretarako aplikazioa iOS eta Android</span><span class="sxs-lookup"><span data-stu-id="eabbb-103">Implement custom fields for the Microsoft Dynamics 365 Project Timesheet mobile app on iOS and Android</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="eabbb-104">Gai honek luzapenak eremu pertsonalizatuak ezartzeko ohiko ereduak eskaintzen ditu.</span><span class="sxs-lookup"><span data-stu-id="eabbb-104">This topic provides common patterns for using extensions to implement custom fields.</span></span> <span data-ttu-id="eabbb-105">Honako gai hauek lantzen dira:</span><span class="sxs-lookup"><span data-stu-id="eabbb-105">The following topics are covered:</span></span>

- <span data-ttu-id="eabbb-106">Eremu pertsonalizatuko esparruak onartzen dituen hainbat datu mota</span><span class="sxs-lookup"><span data-stu-id="eabbb-106">The various data types that the custom field framework supports</span></span>
- <span data-ttu-id="eabbb-107">Nola erakutsi irakurtzeko soilik edo editagarriak diren eremuak ordu-orriko sarreretan eta gorde erabiltzaileak emandako balioak datu-basean</span><span class="sxs-lookup"><span data-stu-id="eabbb-107">How to show read-only or editable fields on timesheet entries, and save user-provided values back to the database</span></span>
- <span data-ttu-id="eabbb-108">Nola erakutsi irakurtzeko soilik diren eremuak aldiz orriaren goiburuan</span><span class="sxs-lookup"><span data-stu-id="eabbb-108">How to show read-only fields on the timesheet header</span></span>
- <span data-ttu-id="eabbb-109">Nola integratu beste negozio logika pertsonalizatu bat lehenetsitako balioak eremuetan sartzeko eta balioztapen osagarria egiteko</span><span class="sxs-lookup"><span data-stu-id="eabbb-109">How to integrate other custom business logic to enter default values in fields and do additional validation</span></span>

## <a name="audience"></a><span data-ttu-id="eabbb-110">Hartzaileak</span><span class="sxs-lookup"><span data-stu-id="eabbb-110">Audience</span></span>

<span data-ttu-id="eabbb-111">Gai hau beren eremu pertsonalizatuak integratzen dituzten garatzaileentzat da Microsoft Dynamics 365 Project Timesheet Apple iOS eta eskuragarri dagoen mugikorretarako aplikazioa Google Android.</span><span class="sxs-lookup"><span data-stu-id="eabbb-111">This topic is intended for developers who are integrating their custom fields into the Microsoft Dynamics 365 Project Timesheet mobile application that is available for Apple iOS and Google Android.</span></span> <span data-ttu-id="eabbb-112">Uste da irakurleek ezagutzen dituztela X ++ garapena eta proiektuaren denbora-orriaren funtzionalitatea.</span><span class="sxs-lookup"><span data-stu-id="eabbb-112">The assumption is that readers are familiar with X++ development and project timesheet functionality.</span></span>

## <a name="data-contract--tstimesheetcustomfield-x-class"></a><span data-ttu-id="eabbb-113">Datuen kontratua - TSTimesheetCustomField X ++ klasea</span><span class="sxs-lookup"><span data-stu-id="eabbb-113">Data contract – TSTimesheetCustomField X++ class</span></span>

<span data-ttu-id="eabbb-114">**TSTimesheetCustomField** class X ++ datu kontratuen klasea da, denbora-orriaren funtzionaltasunerako eremu pertsonalizatu bati buruzko informazioa adierazten duena.</span><span class="sxs-lookup"><span data-stu-id="eabbb-114">The **TSTimesheetCustomField** class is the X++ data contract class that represents information about a custom field for timesheet functionality.</span></span> <span data-ttu-id="eabbb-115">Eremu pertsonalizatuen objektuen zerrendak TSTimesheetDetails datuen kontratuan eta TSTimesheetEntry datuen kontratuan pasatzen dira mugikorretarako aplikazioan eremu pertsonalizatuak erakusteko.</span><span class="sxs-lookup"><span data-stu-id="eabbb-115">Lists of the custom field objects are passed on both the TSTimesheetDetails data contract and the TSTimesheetEntry data contract to show custom fields in the mobile app.</span></span>

- <span data-ttu-id="eabbb-116">**TSTimesheetDetails** - Timesheet goiburuko kontratua.</span><span class="sxs-lookup"><span data-stu-id="eabbb-116">**TSTimesheetDetails** - The timesheet header contract.</span></span>
- <span data-ttu-id="eabbb-117">**TSTimesheetEntry** - Timesheet transakzio kontratua.</span><span class="sxs-lookup"><span data-stu-id="eabbb-117">**TSTimesheetEntry** - The timesheet transaction contract.</span></span> <span data-ttu-id="eabbb-118">Proiektuaren informazio bera duten objektu horien taldeak eta **timesheetLineRecId** balioa lerro bat osatzen dute.</span><span class="sxs-lookup"><span data-stu-id="eabbb-118">Groups of these objects that have the same project information and **timesheetLineRecId** value constitute a line.</span></span>

### <a name="fieldbasetype-types"></a><span data-ttu-id="eabbb-119">fieldBaseType (motak)</span><span class="sxs-lookup"><span data-stu-id="eabbb-119">fieldBaseType (Types)</span></span>

<span data-ttu-id="eabbb-120">**FieldBaseType** jabetzan **TsTimesheetCustom** objektuak aplikazioan agertzen den eremu mota zehazten du.</span><span class="sxs-lookup"><span data-stu-id="eabbb-120">The **FieldBaseType** property on the **TsTimesheetCustom** object determines the type of the field that appears in the app.</span></span> <span data-ttu-id="eabbb-121">Hurrengo **Motak** onartzen diren balioak.</span><span class="sxs-lookup"><span data-stu-id="eabbb-121">The following **Types** values that are supported.</span></span>

| <span data-ttu-id="eabbb-122">Moten balioa</span><span class="sxs-lookup"><span data-stu-id="eabbb-122">Types value</span></span> | <span data-ttu-id="eabbb-123">Mota</span><span class="sxs-lookup"><span data-stu-id="eabbb-123">Type</span></span>              | <span data-ttu-id="eabbb-124">Oharrak</span><span class="sxs-lookup"><span data-stu-id="eabbb-124">Notes</span></span> |
|-------------|-------------------|-------|
| <span data-ttu-id="eabbb-125">0</span><span class="sxs-lookup"><span data-stu-id="eabbb-125">0</span></span>           | <span data-ttu-id="eabbb-126">Katea (eta Enum)</span><span class="sxs-lookup"><span data-stu-id="eabbb-126">String (and Enum)</span></span> | <span data-ttu-id="eabbb-127">Eremua testu-eremu gisa agertzen da.</span><span class="sxs-lookup"><span data-stu-id="eabbb-127">The field appears as a text field.</span></span> |
| <span data-ttu-id="eabbb-128">1</span><span class="sxs-lookup"><span data-stu-id="eabbb-128">1</span></span>           | <span data-ttu-id="eabbb-129">Integer</span><span class="sxs-lookup"><span data-stu-id="eabbb-129">Integer</span></span>           | <span data-ttu-id="eabbb-130">Balioa zenbaki hamartarrik gabeko zenbaki gisa erakusten da.</span><span class="sxs-lookup"><span data-stu-id="eabbb-130">The value is shown as a number without decimal places.</span></span> |
| <span data-ttu-id="eabbb-131">2</span><span class="sxs-lookup"><span data-stu-id="eabbb-131">2</span></span>           | <span data-ttu-id="eabbb-132">Erreala</span><span class="sxs-lookup"><span data-stu-id="eabbb-132">Real</span></span>              | <span data-ttu-id="eabbb-133">Balioa zenbaki hamartarrak dituen zenbaki gisa erakusten da.</span><span class="sxs-lookup"><span data-stu-id="eabbb-133">The value is shown as a number that has decimal places.</span></span><p><span data-ttu-id="eabbb-134">Benetako balioa moneta gisa erakusteko aplikazioan, erabili **fieldExtenededType** jabetza.</span><span class="sxs-lookup"><span data-stu-id="eabbb-134">To show the real value as a currency in the app, use the **fieldExtenededType** property.</span></span> <span data-ttu-id="eabbb-135">Erabil dezakezu **ZenbakiarenZenbakiak** propietatea erakusten diren hamartarren kopurua ezartzeko.</span><span class="sxs-lookup"><span data-stu-id="eabbb-135">You can use the **numberOfDecimals** property to set the number of decimal places that are shown.</span></span></p> |
| <span data-ttu-id="eabbb-136">3</span><span class="sxs-lookup"><span data-stu-id="eabbb-136">3</span></span>           | <span data-ttu-id="eabbb-137">Data</span><span class="sxs-lookup"><span data-stu-id="eabbb-137">Date</span></span>              | <span data-ttu-id="eabbb-138">Data formatuak erabiltzailearen arabera zehazten dira **Data, orduak eta zenbaki formatua** azpian zehazten den ezarpena **Hizkuntza eta herrialde / eskualde lehentasuna** urtean **Erabiltzailearen aukerak**.</span><span class="sxs-lookup"><span data-stu-id="eabbb-138">Date formats are determined by the user's **Date, times, and number format** setting that is specified under **Language and country/region preference** in **User options**.</span></span> |
| <span data-ttu-id="eabbb-139">4</span><span class="sxs-lookup"><span data-stu-id="eabbb-139">4</span></span>           | <span data-ttu-id="eabbb-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="eabbb-140">Boolean</span></span>           | |
| <span data-ttu-id="eabbb-141">15</span><span class="sxs-lookup"><span data-stu-id="eabbb-141">15</span></span>          | <span data-ttu-id="eabbb-142">GUIDa</span><span class="sxs-lookup"><span data-stu-id="eabbb-142">GUID</span></span>              | |
| <span data-ttu-id="eabbb-143">16</span><span class="sxs-lookup"><span data-stu-id="eabbb-143">16</span></span>          | <span data-ttu-id="eabbb-144">Int64</span><span class="sxs-lookup"><span data-stu-id="eabbb-144">Int64</span></span>             | |

- <span data-ttu-id="eabbb-145">Bada **katea Aukerak** jabetza ez dago **TSTimesheetCustomField** objektua, testu libreko eremua eskaintzen zaio erabiltzaileari.</span><span class="sxs-lookup"><span data-stu-id="eabbb-145">If the **stringOptions** property isn't provided on the **TSTimesheetCustomField** object, a free-text field is provided to the user.</span></span>

    <span data-ttu-id="eabbb-146">**kateaLuzera** propietatea erabil daiteke erabiltzaileek sar dezaketen gehieneko kate luzera ezartzeko.</span><span class="sxs-lookup"><span data-stu-id="eabbb-146">The **stringLength** property can be used to set the maximum string length that users can enter.</span></span>

- <span data-ttu-id="eabbb-147">Bada **katea Aukerak** jabetza helbidean ematen da **TSTimesheetCustomField** objektua, zerrendako elementu horiek erabiltzaileek aukera botoiak (irrati botoiak) erabiliz hautatu ditzaketen balio bakarrak dira.</span><span class="sxs-lookup"><span data-stu-id="eabbb-147">If the **stringOptions** property is provided on the **TSTimesheetCustomField** object, those list elements are the only values that users can select by using option buttons (radio buttons).</span></span>

    <span data-ttu-id="eabbb-148">Kasu honetan, kate-eremuak zenbateko balio gisa joka dezake erabiltzailea sartzeko helburuarekin.</span><span class="sxs-lookup"><span data-stu-id="eabbb-148">In this case, the string field can act as an enum value for the purpose of user entry.</span></span> <span data-ttu-id="eabbb-149">Balioa datu-basean zenbaki gisa gordetzeko, eskuz mapatu katearen balioa enum balioarekin berriro datu basean gorde aurretik komando-katea erabiliz (ikus "Erabili komando-katea TSTimesheetEntryService klasean denbora-orriko sarrera bat gordetzeko aplikazioa datu-basera "atalean geroago gai honen adibide gisa).</span><span class="sxs-lookup"><span data-stu-id="eabbb-149">To save the value to the database as an enum, manually map the string value back to the enum value before you save to the database by using chain of command (see the “Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database” section later in this topic for an example).</span></span>

### <a name="fieldextendedtype-tscustomfieldextendedtype"></a><span data-ttu-id="eabbb-150">fieldExtendedType (TSCustomFieldExtendedType)</span><span class="sxs-lookup"><span data-stu-id="eabbb-150">fieldExtendedType (TSCustomFieldExtendedType)</span></span>

<span data-ttu-id="eabbb-151">Propietate hau erabil dezakezu benetako balioak moneta gisa formateatzeko.</span><span class="sxs-lookup"><span data-stu-id="eabbb-151">You can use this property to format real values as currency.</span></span> <span data-ttu-id="eabbb-152">Ikuspegi hau **fieldBaseType** balioa da **Erreala**.</span><span class="sxs-lookup"><span data-stu-id="eabbb-152">This approach is applicable only when the **fieldBaseType** value is **Real**.</span></span>

- <span data-ttu-id="eabbb-153">**TSCustomFieldExtendedType:Bat ere ez** - Ez da formaturik aplikatzen.</span><span class="sxs-lookup"><span data-stu-id="eabbb-153">**TSCustomFieldExtendedType:None** – No formatting is applied.</span></span>
- <span data-ttu-id="eabbb-154">**TSCustomFieldExtendedType::Moneta** - Formatu balioa moneta gisa.</span><span class="sxs-lookup"><span data-stu-id="eabbb-154">**TSCustomFieldExtendedType::Currency** – Format the value as currency.</span></span>

    <span data-ttu-id="eabbb-155">Moneta formatua aktibo dagoenean, **kateaBalioa** eremuan aplikazioan erakutsi beharko litzatekeen moneta kodea gainditu daiteke.</span><span class="sxs-lookup"><span data-stu-id="eabbb-155">When currency formatting is active, the **stringValue** field can be used pass the currency code that should be shown in the app.</span></span> <span data-ttu-id="eabbb-156">Balioa irakurtzeko soilik den balioa da.</span><span class="sxs-lookup"><span data-stu-id="eabbb-156">The value is a read-only value.</span></span>

    <span data-ttu-id="eabbb-157">**benetakoBalioa** eremuak datu basean gorde behar den diru kopurua dauka.</span><span class="sxs-lookup"><span data-stu-id="eabbb-157">The **realValue** field contains the money amount that should be saved to the database.</span></span>

### <a name="fieldsection-tscustomfieldsection"></a><span data-ttu-id="eabbb-158">fieldSection (TSCustomFieldSection)</span><span class="sxs-lookup"><span data-stu-id="eabbb-158">fieldSection (TSCustomFieldSection)</span></span>

<span data-ttu-id="eabbb-159">Propietate hau erabil dezakezu eremu pertsonalizatuak aplikazioan non agertu behar duen zehazteko.</span><span class="sxs-lookup"><span data-stu-id="eabbb-159">You can use this property specify where the custom field should appear in the app.</span></span>

- <span data-ttu-id="eabbb-160">**TSCustomFieldSection::Goiburua** - Eremua agertuko da **Ikusi xehetasun gehiago** ataleko aplikazioa.</span><span class="sxs-lookup"><span data-stu-id="eabbb-160">**TSCustomFieldSection::Header** – The field will appear in the **View more details** section in the app.</span></span> <span data-ttu-id="eabbb-161">Eremu horiek irakurtzekoak dira bakarrik.</span><span class="sxs-lookup"><span data-stu-id="eabbb-161">These fields are always read-only.</span></span>
- <span data-ttu-id="eabbb-162">**TSCustomFieldSection::Lerroa** - Eremua denbora-orriko sarreretan kutxaz kanpoko lerro-eremu guztien ondoren agertuko da.</span><span class="sxs-lookup"><span data-stu-id="eabbb-162">**TSCustomFieldSection::Line** – The field will appear after all the out-of-box line fields on timesheet entries.</span></span> <span data-ttu-id="eabbb-163">Eremu hauek editagarriak edo irakurtzeko soilik izan daitezke.</span><span class="sxs-lookup"><span data-stu-id="eabbb-163">These fields can be either editable or read-only.</span></span>

### <a name="fieldname-fieldnameshort"></a><span data-ttu-id="eabbb-164">fieldName (FieldNameShort)</span><span class="sxs-lookup"><span data-stu-id="eabbb-164">fieldName (FieldNameShort)</span></span>

<span data-ttu-id="eabbb-165">Propietate honek eremua identifikatzen du aplikazioak ematen dituen balioak datu-basean gordetzen direnean.</span><span class="sxs-lookup"><span data-stu-id="eabbb-165">This property identifies the field when values that the app provides are saved back to the database.</span></span>

### <a name="tablename-tablenameshort"></a><span data-ttu-id="eabbb-166">tableName (TableNameShort)</span><span class="sxs-lookup"><span data-stu-id="eabbb-166">tableName (TableNameShort)</span></span>

<span data-ttu-id="eabbb-167">Propietate honek eremua identifikatzen du aplikazioak ematen dituen balioak datu-basean gordetzen direnean.</span><span class="sxs-lookup"><span data-stu-id="eabbb-167">This property identifies the field when values that the app provides are saved back to the database.</span></span>

### <a name="iseditable-noyes"></a><span data-ttu-id="eabbb-168">isEditable (Ez Bai)</span><span class="sxs-lookup"><span data-stu-id="eabbb-168">isEditable (NoYes)</span></span>

<span data-ttu-id="eabbb-169">Ezarri propietate hau **Bai** zehazteko zehazteko denbora-orriko sarrera ataleko eremua erabiltzaileek editatu behar dutela.</span><span class="sxs-lookup"><span data-stu-id="eabbb-169">Set this property to **Yes** to specify that the field in the timesheet entry section should be editable by users.</span></span> <span data-ttu-id="eabbb-170">Ezarri propietatea **Ez** eremua irakurtzeko soilik egiteko.</span><span class="sxs-lookup"><span data-stu-id="eabbb-170">Set the property to **No** to make the field read-only.</span></span>

### <a name="ismandatory-noyes"></a><span data-ttu-id="eabbb-171">Derrigorrezkoa da (Ez Bai)</span><span class="sxs-lookup"><span data-stu-id="eabbb-171">isMandatory (NoYes)</span></span>

<span data-ttu-id="eabbb-172">Ezarri propietate hau **Bai** zehazteko zehazteko denbora-orriko sarrera ataleko eremua derrigorrezkoa izan behar luke.</span><span class="sxs-lookup"><span data-stu-id="eabbb-172">Set this property to **Yes** to specify that the field in the timesheet entry section should be mandatory.</span></span>

### <a name="label-str"></a><span data-ttu-id="eabbb-173">Etiketa (str)</span><span class="sxs-lookup"><span data-stu-id="eabbb-173">label (str)</span></span>

<span data-ttu-id="eabbb-174">Propietate honek aplikazioaren eremuan ondoan agertzen den etiketa zehazten du.</span><span class="sxs-lookup"><span data-stu-id="eabbb-174">This property specifies the label that is shown next the field in the app.</span></span>

### <a name="stringoptions-list-of-strings"></a><span data-ttu-id="eabbb-175">stringOptions (Kateen zerrenda)</span><span class="sxs-lookup"><span data-stu-id="eabbb-175">stringOptions (List of Strings)</span></span>

<span data-ttu-id="eabbb-176">Jabetza hau noiz aplikatu daiteke **fieldBaseType** ezarrita dago **Katea**.</span><span class="sxs-lookup"><span data-stu-id="eabbb-176">This property is applicable only when **fieldBaseType** is set to **String**.</span></span> <span data-ttu-id="eabbb-177">Bada **katea Aukerak** ezarrita dago, aukera-botoien bidez (irrati-botoiak) aukeratzeko dauden kateen balioak zerrendako kateek zehazten dituzte.</span><span class="sxs-lookup"><span data-stu-id="eabbb-177">If **stringOptions** is set, the string values that are available for selection via option buttons (radio buttons) are specified by the strings in the list.</span></span> <span data-ttu-id="eabbb-178">Katerik ematen ez bada, kateen eremuan testu libreko sarrera onartzen da (ikusi "Erabili komando-katea TSTimesheetEntryService klasean aplikazioko datu-basera itzuli den denbora-orriko sarrera bat gordetzeko" atalean adibide bat lortzeko) .</span><span class="sxs-lookup"><span data-stu-id="eabbb-178">If no strings are provided, free-text entry in the string field is allowed (see the “Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database” section later in this topic for an example).</span></span>

### <a name="stringlength-int"></a><span data-ttu-id="eabbb-179">stringLength (int)</span><span class="sxs-lookup"><span data-stu-id="eabbb-179">stringLength (int)</span></span>

<span data-ttu-id="eabbb-180">Propietate honek kate-eremu baten gehieneko luzera zehazten du.</span><span class="sxs-lookup"><span data-stu-id="eabbb-180">This property specifies the maximum length for a string field.</span></span> <span data-ttu-id="eabbb-181">Aplikatu daiteke **fieldBaseType** ezarrita dago **Katea**.</span><span class="sxs-lookup"><span data-stu-id="eabbb-181">It's applicable only when **fieldBaseType** is set to **String**.</span></span>

### <a name="numberofdecimals-int"></a><span data-ttu-id="eabbb-182">kopuruaEzkenak (int)</span><span class="sxs-lookup"><span data-stu-id="eabbb-182">numberOfDecimals (int)</span></span>

<span data-ttu-id="eabbb-183">Propietate honek eremu erreal baterako erakusten diren hamartarren kopurua zehazten du.</span><span class="sxs-lookup"><span data-stu-id="eabbb-183">This property specifies the number of decimal places that are shown for a real field.</span></span> <span data-ttu-id="eabbb-184">Aplikatu daiteke **fieldBaseType** ezarrita dago **Erreala**.</span><span class="sxs-lookup"><span data-stu-id="eabbb-184">It's applicable only when **fieldBaseType** is set to **Real**.</span></span>

### <a name="ordersequence-int"></a><span data-ttu-id="eabbb-185">orderSequence (int)</span><span class="sxs-lookup"><span data-stu-id="eabbb-185">orderSequence (int)</span></span>

<span data-ttu-id="eabbb-186">Propietate honek eremu pertsonalizatuak aplikazioan erakusteko ordena kontrolatzen du eremu pertsonalizatu bat baino gehiago zehazten direnean.</span><span class="sxs-lookup"><span data-stu-id="eabbb-186">This property controls the order in which the custom fields are shown in the app when more than one custom field is specified.</span></span> <span data-ttu-id="eabbb-187">Zenbaki txikiagoak dituzten eremuak agertzen dira lehenengo.</span><span class="sxs-lookup"><span data-stu-id="eabbb-187">Fields that have lower numbers are shown first.</span></span>

### <a name="booleanvalue-boolean"></a><span data-ttu-id="eabbb-188">booleanValue (boolearra)</span><span class="sxs-lookup"><span data-stu-id="eabbb-188">booleanValue (boolean)</span></span>

<span data-ttu-id="eabbb-189">Eremuetako **Boolearra** mota, propietate honek zerbitzariaren eta aplikazioaren arteko eremuko balio boolearra igarotzen du.</span><span class="sxs-lookup"><span data-stu-id="eabbb-189">For fields of the **Boolean** type, this property passes the Boolean value of the field between the server and the app.</span></span>

### <a name="guidvalue-guid"></a><span data-ttu-id="eabbb-190">guidValue (guid)</span><span class="sxs-lookup"><span data-stu-id="eabbb-190">guidValue (guid)</span></span>

<span data-ttu-id="eabbb-191">Eremuetako **GUID** mota, propietate honek zerbitzariaren eta aplikazioaren arteko eremuko balio globalki identifikatzaile bakarra (GUID) igarotzen du.</span><span class="sxs-lookup"><span data-stu-id="eabbb-191">For fields of the **GUID** type, this property passes the globally unique identifier (GUID) value of the field between the server and the app.</span></span>

### <a name="int64value-int64"></a><span data-ttu-id="eabbb-192">int64Balioa (int64)</span><span class="sxs-lookup"><span data-stu-id="eabbb-192">int64Value (int64)</span></span>

<span data-ttu-id="eabbb-193">Eremuetako **Int64** mota, propietate honek zerbitzariaren eta aplikazioaren arteko eremuko balio int64 igarotzen du.</span><span class="sxs-lookup"><span data-stu-id="eabbb-193">For fields of the **Int64** type, this property passes the int64 value of the field between the server and the app.</span></span>

### <a name="intvalue-int"></a><span data-ttu-id="eabbb-194">intBalue (int)</span><span class="sxs-lookup"><span data-stu-id="eabbb-194">intValue (int)</span></span>

<span data-ttu-id="eabbb-195">Eremuetako **Int** mota, propietate honek zerbitzariaren eta aplikazioaren arteko eremuko balio int igarotzen du.</span><span class="sxs-lookup"><span data-stu-id="eabbb-195">For fields of the **Int** type, this property passes the int value of the field between the server and the app.</span></span>

### <a name="realvalue-real"></a><span data-ttu-id="eabbb-196">benetakoBalioa (benetakoa)</span><span class="sxs-lookup"><span data-stu-id="eabbb-196">realValue (real)</span></span>

<span data-ttu-id="eabbb-197">Eremuetako **Erreala** mota, propietate honek zerbitzariaren eta aplikazioaren arteko eremuko balio erreala igarotzen du .</span><span class="sxs-lookup"><span data-stu-id="eabbb-197">For fields of the **Real** type, this property passes the real value of the field between the server and the app .</span></span>

### <a name="stringvalue-str"></a><span data-ttu-id="eabbb-198">stringValue (str)</span><span class="sxs-lookup"><span data-stu-id="eabbb-198">stringValue (str)</span></span>

<span data-ttu-id="eabbb-199">Eremuetako **Katea** mota, propietate honek zerbitzariaren eta aplikazioaren arteko eremuko balio katea igarotzen du.</span><span class="sxs-lookup"><span data-stu-id="eabbb-199">For fields of the **String** type, this property passes the string value of the field between the server and the app.</span></span> <span data-ttu-id="eabbb-200">Eremuetako eremuetarako ere erabiltzen da **Erreala** moneta gisa formateatutako mota.</span><span class="sxs-lookup"><span data-stu-id="eabbb-200">It's also used for fields of the **Real** type that are formatted as currency.</span></span> <span data-ttu-id="eabbb-201">Eremu horietarako, propietatea moneta kodea aplikaziora pasatzeko erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="eabbb-201">For those fields, the property is used to pass the currency code to the app.</span></span>

### <a name="datevalue-date"></a><span data-ttu-id="eabbb-202">dateValue (data)</span><span class="sxs-lookup"><span data-stu-id="eabbb-202">dateValue (date)</span></span>

<span data-ttu-id="eabbb-203">Eremuetako **Data** mota, propietate honek zerbitzariaren eta aplikazioaren arteko eremuko balio data igarotzen du.</span><span class="sxs-lookup"><span data-stu-id="eabbb-203">For fields of the **Date** type, this property passes the date value of the field between the server and the app.</span></span>

## <a name="show-and-save-a-custom-field-in-the-timesheet-entry-section"></a><span data-ttu-id="eabbb-204">Erakutsi eta gorde eremu pertsonalizatua ordu-orriaren sarrera atalean</span><span class="sxs-lookup"><span data-stu-id="eabbb-204">Show and save a custom field in the timesheet entry section</span></span>

<span data-ttu-id="eabbb-205">Jarraian, denbora-orriaren sarrera sortzeko mugikorretarako aplikazioaren pantaila-argazkia dago.</span><span class="sxs-lookup"><span data-stu-id="eabbb-205">Below is a screenshot from the mobile app of a timesheet entry creation.</span></span> <span data-ttu-id="eabbb-206">Kutxaz kanpoko eremuak eta eremu pertsonalizatua erakusten ditu "Denbora sarrera" atalean "Proba katea" deiturikoa dagoeneko "Bigarren aukera" enum balioarekin.</span><span class="sxs-lookup"><span data-stu-id="eabbb-206">It shows the out-of-box fields and a custom field in the "Time entry" section called "Test string" with an enum value of "Second option" already set.</span></span>

![Probatu katea eremu pertsonalizatua aplikazioan](media/timesheet-entry.jpg)



<span data-ttu-id="eabbb-208">Jarraian, "Probako katea" eremu pertsonalizaturako eskuragarri dauden enum aukeretako bat hautatzen duen erabiltzailearen mugikorretarako pantaila-argazkia dago.</span><span class="sxs-lookup"><span data-stu-id="eabbb-208">Below is a screenshot from the mobile app of the user selecting one of the enum options available for the "Test string" custom field.</span></span>  <span data-ttu-id="eabbb-209">Bi aukerak "Lehen aukera" eta "Bigarren aukera" dira botoi irudi gisa agertzen direnak.</span><span class="sxs-lookup"><span data-stu-id="eabbb-209">The two options are "First option" and "Second option" shown as radio buttons.</span></span> <span data-ttu-id="eabbb-210">Une honetan bigarren aukera dago hautatuta.</span><span class="sxs-lookup"><span data-stu-id="eabbb-210">The second option is currently selected.</span></span>

![Aukera botoiak (irrati botoiak) Probako katea pertsonalizatutako eremurako](media/enum-option.jpg)



### <a name="extend-the-tstimesheetline-table-so-that-it-has-a-custom-field"></a><span data-ttu-id="eabbb-212">Zabaldu TSTimesheetLine taula pertsonalizatutako eremua izan dezan</span><span class="sxs-lookup"><span data-stu-id="eabbb-212">Extend the TSTimesheetLine table so that it has a custom field</span></span>

<span data-ttu-id="eabbb-213">Eszenatoki tipikoetan, litekeena da denbora-orriaren sarrera ataleko eremu pertsonalizatu baten datuak TSTimesheetLine taulan gordetzea.</span><span class="sxs-lookup"><span data-stu-id="eabbb-213">In typical scenarios, it's likely that the data for a custom field in the timesheet entry section will be saved to the TSTimesheetLine table.</span></span> <span data-ttu-id="eabbb-214">Hala ere, beste taula batzuk erabil daitezke datuak ematen diren TSTimesheetTrans erregistro batean oinarrituta berreskuratu daitezkeenean edo erregistro testuinguru zehatzik ez badute (adibidez, eremua proiektuaren parametroetan irakurtzeko soilik ezarri bada) .</span><span class="sxs-lookup"><span data-stu-id="eabbb-214">However, other tables can be used if the data can be retrieved based on a TSTimesheetTrans record that is provided, or if it doesn't have specific record context (for example, if the field is set as read-only in the project parameters).</span></span>

<span data-ttu-id="eabbb-215">Kontuan izan eremu pertsonalizatuek ez dutela zertan babeskopia datu baserik izan.</span><span class="sxs-lookup"><span data-stu-id="eabbb-215">Note that custom fields don't have to have any backing database records.</span></span> <span data-ttu-id="eabbb-216">Dinamikoki sor daitezke X ++ logikan oinarrituta.</span><span class="sxs-lookup"><span data-stu-id="eabbb-216">They can be dynamically generated based on X++ logic.</span></span> <span data-ttu-id="eabbb-217">Ikuspegi hau erabilgarria izan daiteke irakurtzeko soilik diren eszenatokietan (ikus "Erabili komando-katea TSTimesheetDetails klasean, buildCustomFieldListForHeader metodoa denbora-orriaren xehetasunak betetzeko" atala, modu dinamikoan sortutako eremu pertsonalizatuen balioen adibidea lortzeko.)</span><span class="sxs-lookup"><span data-stu-id="eabbb-217">This approach can be useful in read-only scenarios (see the “Use chain of command on the TSTimesheetDetails class, buildCustomFieldListForHeader method to fill in timesheet details” section for an example of dynamically generated custom field values.)</span></span>

<span data-ttu-id="eabbb-218">Jarraian, pantaila-argazkia erakusten da Visual Studio Aplikazioaren Objektuen Zuhaitzaren.</span><span class="sxs-lookup"><span data-stu-id="eabbb-218">Below is a screenshot from Visual Studio of the Application Object Tree.</span></span> <span data-ttu-id="eabbb-219">TSTimesheetLine taularen luzapena erakusten du TestLineString eremuak eremu pertsonalizatu gisa gehituta.</span><span class="sxs-lookup"><span data-stu-id="eabbb-219">It shows an extension of the TSTimesheetLine table with the TestLineString field added as a custom field.</span></span>

![Lerro katea](media/b6756b4a3fc5298093327a088a7710fd.png)

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-timesheet-entry-section"></a><span data-ttu-id="eabbb-221">Erabili komando katea TSTimesheetSettings klaseko buildCustomFieldList metodoan metodoa orriaren sarrera atalean eremua erakusteko</span><span class="sxs-lookup"><span data-stu-id="eabbb-221">Use chain of command on the buildCustomFieldList method of the TSTimesheetSettings class to show a field in the timesheet entry section</span></span>

<span data-ttu-id="eabbb-222">Kode honek aplikazioaren eremuko pantailako ezarpenak kontrolatzen ditu.</span><span class="sxs-lookup"><span data-stu-id="eabbb-222">This code controls the display settings for the field in the app.</span></span> <span data-ttu-id="eabbb-223">Adibidez, kontrolatzen ditu eremu mota, etiketa, eremua derrigorrezkoa den eta eremua zein ataletan agertzen den.</span><span class="sxs-lookup"><span data-stu-id="eabbb-223">For example, it controls the type of field, the label, whether the field is mandatory, and what section the field appears in.</span></span>

<span data-ttu-id="eabbb-224">Hurrengo adibidean denbora-sarreren kate-eremua erakusten da.</span><span class="sxs-lookup"><span data-stu-id="eabbb-224">The following example shows a string field on time entries.</span></span> <span data-ttu-id="eabbb-225">Eremu honek bi aukera ditu, **Lehen aukera** eta **Bigarren aukera**, aukera botoien bidez (irrati botoiak) eskuragarri daudenak.</span><span class="sxs-lookup"><span data-stu-id="eabbb-225">This field has two options, **First option** and **Second option**, that are available via option buttons (radio buttons).</span></span> <span data-ttu-id="eabbb-226">Aplikazioko eremua **TestLineString** TSTimesheetLine taulan gehitzen den eremua.</span><span class="sxs-lookup"><span data-stu-id="eabbb-226">The field in the app is associated with the **TestLineString** field that is added to the TSTimesheetLine table.</span></span>

<span data-ttu-id="eabbb-227">Kontuan izan **TSTimesheetCustomField::newFromMetatdata()** eremu pertsonalizatuen propietateen hasiera errazteko metodoa: **fieldBaseType**, **taulaIzena**, **eremu izena**, **etiketa**, **editagarria da**, **derrigorrezkoa da**, **kateaLuzera**, eta **ZenbakiarenZenbakiak**.</span><span class="sxs-lookup"><span data-stu-id="eabbb-227">Note the use of the **TSTimesheetCustomField::newFromMetatdata()** method to simplify the initialization of the custom field properties: **fieldBaseType**, **tableName**, **fieldname**, **label**, **isEditable**, **isMandatory**, **stringLength**, and **numberOfDecimals**.</span></span> <span data-ttu-id="eabbb-228">Parametro hauek eskuz ere ezar ditzakezu, nahi duzun moduan.</span><span class="sxs-lookup"><span data-stu-id="eabbb-228">You can also set these parameters manually, as you prefer.</span></span>

```xpp
...
[ExtensionOf(classStr(TsTimesheetSettings))]
final class TSTimesheetSettings_Extension
{
    protected List buildCustomFieldList()
    {
        List customFieldList = next buildCustomFieldList();
        TSTimesheetCustomField tsTimesheetCustomField;
        tsTimesheetCustomField =
        TSTimesheetCustomField::newFromMetadata(tableNum(TsTimesheetLine),
        fieldNum(TSTimesheetLine, TestLineString));
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Line);
        tsTimesheetCustomField.parmOrderSequence(1);
        List stringOptions = new List(Types::String);
        stringOptions.addEnd('First option');
        stringOptions.addEnd('Second option');
        tsTimesheetCustomField.parmStringOptions(stringOptions);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforentry-method-of-the-tstimesheetentry-class-to-enter-values-in-a-timesheet-entry"></a><span data-ttu-id="eabbb-229">Erabili katearen komandoa buildCustomFieldListForEntry metodoa TSTimesheetEntry klasea sartzeko balioak lan-orduen sarrera</span><span class="sxs-lookup"><span data-stu-id="eabbb-229">Use chain of command on the buildCustomFieldListForEntry method of the TSTimesheetEntry class to enter values in a timesheet entry</span></span>

<span data-ttu-id="eabbb-230">**buildCustomFieldListForEntry** metodoa mugikorretarako aplikazioan gordetako ordu-orrien lerroetan balioak sartzeko erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="eabbb-230">The **buildCustomFieldListForEntry** method is used to enter values on the saved timesheet lines in the mobile app.</span></span> <span data-ttu-id="eabbb-231">Parametro gisa TSTimesheetTrans erregistroa hartzen du.</span><span class="sxs-lookup"><span data-stu-id="eabbb-231">It takes a TSTimesheetTrans record as a parameter.</span></span> <span data-ttu-id="eabbb-232">Erregistro horretako eremuak aplikazioko eremu pertsonalizatuko balioa betetzeko erabil daitezke.</span><span class="sxs-lookup"><span data-stu-id="eabbb-232">Fields from that record can be used to fill in the custom field value in the app.</span></span>

```xpp
...
[ExtensionOf(classStr(TsTimesheetEntry))]
final class TsTimesheetEntry_Extension
{
    protected List buildCustomFieldListForEntry(TSTimesheetTrans _tsTimesheetTrans)
    {
        List customFieldList = next buildCustomFieldListForEntry(_tsTimesheetTrans);
        TSTimesheetLine tsTimesheetLine = _tsTimesheetTrans.timesheetLine();
        TSTimesheetCustomField tsTimesheetCustomField;
        tsTimesheetCustomField =
        TSTimesheetCustomField::newFromMetadata(tableNum(TsTimesheetLine),
        fieldNum(TSTimesheetLine, TestLineString));
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Line);
        tsTimesheetCustomField.parmOrderSequence(1);
        tsTimesheetCustomField.parmStringValue(tsTimesheetLine.TestLineString);
        List stringOptions = new List(Types::String);
        stringOptions.addEnd('First option');
        stringOptions.addEnd('second option;);
        tsTimesheetCustomField.parmStringOptions(stringOptions);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-tstimesheetentryservice-class-to-save-a-timesheet-entry-from-the-app-back-to-the-database"></a><span data-ttu-id="eabbb-233">Erabili komando-katea TSTimesheetEntryService klasean aplikazioko datu-orriko sarrera bat datu-basean gordetzeko</span><span class="sxs-lookup"><span data-stu-id="eabbb-233">Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database</span></span>

<span data-ttu-id="eabbb-234">Eremu pertsonalizatua datu-basera ohiko erabileran gordetzeko, hainbat metodo luzatu behar dituzu:</span><span class="sxs-lookup"><span data-stu-id="eabbb-234">To save a custom field back to the database in typical usage, you must extend multiple methods:</span></span>

- <span data-ttu-id="eabbb-235">**timesheetLineNeedsUpdating** metodoa erabiltzen da erabiltzaileak lineako erregistroa aplikazioan aldatu duen edo ez eta datu basean gorde behar den zehazteko.</span><span class="sxs-lookup"><span data-stu-id="eabbb-235">The **timesheetLineNeedsUpdating** method is used to determine whether the line record has been changed by the user in the app and must be saved to the database.</span></span> <span data-ttu-id="eabbb-236">Errendimendua kezka ez bada, metodo hau sinplifikatu egin daiteke, beti itzul dadin **egia**.</span><span class="sxs-lookup"><span data-stu-id="eabbb-236">If performance isn't a concern, this method can be simplified so that it always returns **true**.</span></span>
- <span data-ttu-id="eabbb-237">**populateTimesheetLineFromEntryDuringCreate** eta **populateTimesheetLineFromEntryDuringUpdate** metodoak luza daitezke, ematen diren TSTimesheetLine datu-basearen erregistroan balioak sartu ditzaten.</span><span class="sxs-lookup"><span data-stu-id="eabbb-237">The **populateTimesheetLineFromEntryDuringCreate** and **populateTimesheetLineFromEntryDuringUpdate** methods can be extended so that they enter values in the TSTimesheetLine database record from the TSTimesheetEntry data contract record that is provided.</span></span> <span data-ttu-id="eabbb-238">Ondorengo adibidean, ohartu nola datu basearen eremua eta sarrera eremua arteko mapak eskuz egiten diren X ++ kodearen bidez.</span><span class="sxs-lookup"><span data-stu-id="eabbb-238">In the example that follows, notice how the mapping between the database field and the entry field is manually done via X++ code.</span></span>
- <span data-ttu-id="eabbb-239">**populateTimesheetWeekFromEntry** metodoa ere luza daiteke **TSTimesheetEntry** objektuak TSTimesheetLineweek datu basearen taulan idatzi behar du berriro.</span><span class="sxs-lookup"><span data-stu-id="eabbb-239">The **populateTimesheetWeekFromEntry** method can also be extended if the custom field that is mapped to the **TSTimesheetEntry** object must write back to the TSTimesheetLineweek database table.</span></span>

> [!NOTE]
> <span data-ttu-id="eabbb-240">Ondorengo adibideak gordetzen du **lehenAukera** edo **bigarrenAukera** erabiltzaileak datu basean hautatzen duen balioa kate gordinaren balio gisa.</span><span class="sxs-lookup"><span data-stu-id="eabbb-240">The following example saves the **firstOption** or **secondOption** value that the user selects to the database as a raw string value.</span></span> <span data-ttu-id="eabbb-241">Datu-basearen eremua **Enum** mota, balio horiek eskuz mapatu daitezke enum balio batera eta ondoren gorde datu base taulako enum eremu batean.</span><span class="sxs-lookup"><span data-stu-id="eabbb-241">If the database field is a field of the **Enum** type, those values can be manually mapped to an enum value and then saved to an enum field on the database table.</span></span>

```xpp
...
[ExtensionOf(classStr(TSTimesheetEntryService))]
final class TSTimesheetEntryService_Extension
{
    protected boolean timesheetLineNeedsUpdating(TSTimesheetLine _tsTimesheetLine,
    TsTimesheetEntry _tsTimesheetEntry)
    {
        boolean ret = next timesheetLineNeedsUpdating(_tsTimesheetLine,
        _tsTimesheetEntry);
        if (!ret)
        {
            */ Loop through custom fields to see if value needs updating*/
            ListEnumerator enumerator =  _tsTimesheetEntry.parmCustomFields().getEnumerator();
            while (enumerator.moveNext())
            {
                TSTimesheetCustomField customField = enumerator.current();
                if (customField.parmFieldName() == fieldId2Name(tableNum(TsTimesheetLine),
                fieldNum(TSTimesheetLine, TestLineString)))
                {
                    */ If Custom field value for TestLineString field has changed, We need to update the timesheet line.*/
                    if (_tsTimesheetLine.TestLineString != customField.parmStringValue())
                    {
                        ret = true;
                    }
                }
            }
        }
        return ret;
    }
    protected void populateTimesheetLineFromEntryDuringCreate(TSTimesheetLine
    _tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
    {
        next populateTimesheetLineFromEntryDuringCreate(_tsTimesheetLine,
        _tsTimesheetEntry);
        this.populateTimesheetLineFromCustomFields(_tsTimesheetLine,
        _tsTimesheetEntry);
        }
        protected void populateTimesheetLineFromEntryDuringUpdate(TSTimesheetLine
        \_tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
        {
            next populateTimesheetLineFromEntryDuringUpdate(_tsTimesheetLine,
            _tsTimesheetEntry);
            this.populateTimesheetLineFromCustomFields(_tsTimesheetLine,
            _tsTimesheetEntry);
        }
        private void populateTimesheetLineFromCustomFields(TSTimesheetLine
        _tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
        {
            ListEnumerator enumerator =
            _tsTimesheetEntry.parmCustomFields().getEnumerator();
            while (enumerator.moveNext())
            {
                TSTimesheetCustomField customField = enumerator.current();
                if (customField.parmFieldName() == fieldId2Name(tableNum(TsTimesheetLine),
                fieldNum(TSTimesheetLine, TestLineString)))
                {
                    _tsTimesheetLine.TestLineString = customField.parmStringValue();
                }
            }
        }
    }
...
```

## <a name="show-a-custom-field-in-the-timesheet-header-section"></a><span data-ttu-id="eabbb-242">Erakutsi eremu pertsonalizatua ordu-orriaren goiburuaren atalean</span><span class="sxs-lookup"><span data-stu-id="eabbb-242">Show a custom field in the timesheet header section</span></span>

<span data-ttu-id="eabbb-243">Jarraian, denbora-orria ikusteko erabiltzailearen mugikorretarako aplikazioaren pantaila-argazkia dago.</span><span class="sxs-lookup"><span data-stu-id="eabbb-243">Below is a screenshot from the mobile app of a user viewing a timesheet.</span></span> <span data-ttu-id="eabbb-244">"Informazio gehiago" botoia goiko eskuineko izkinan hautatu da "Ikusi xehetasun gehiago" aukera erakusteko.</span><span class="sxs-lookup"><span data-stu-id="eabbb-244">The "More information" button has been selected in the upper-right corner to show the "View more details" option.</span></span>  

![Ikusi xehetasun gehiago komandoa](media/show-more.png)

<span data-ttu-id="eabbb-246">Jarraian, denbora-orriaren "Gehiago" sekzioa erakutsiz mugikorretarako aplikazioaren pantaila-argazkia dago.</span><span class="sxs-lookup"><span data-stu-id="eabbb-246">Below is a screenshot from the mobile app showing the “More” section of a timesheet.</span></span> <span data-ttu-id="eabbb-247">"Orri honen erabilera-tasa (kalkulatutako eremu pertsonalizatua)" izeneko eremu pertsonalizatua gehitu da aldiz-orriaren goiburuko atalean.</span><span class="sxs-lookup"><span data-stu-id="eabbb-247">A custom field called “Utilization rate of this timesheet (computed custom field)” has been added to the timesheet header section.</span></span> <span data-ttu-id="eabbb-248">Irakurtzeko soilik den "0,667" balioa ezartzen da eremu pertsonalizatuan.</span><span class="sxs-lookup"><span data-stu-id="eabbb-248">A read-only value of "0.667" is set on the custom field.</span></span>

![Atal gehiago](media/more-section.jpg)

### <a name="extend-the-tstimesheettable-table-so-that-it-has-a-custom-field"></a><span data-ttu-id="eabbb-250">Zabaldu TSTimesheetTable taula pertsonalizatutako eremua izan dezan</span><span class="sxs-lookup"><span data-stu-id="eabbb-250">Extend the TSTimesheetTable table so that it has a custom field</span></span>

<span data-ttu-id="eabbb-251">Eszenatoki tipikoetan, litekeena da goiburuaren ataleko eremu pertsonalizatu baten datuak TSTimesheetHeader taulan ateratakoa.</span><span class="sxs-lookup"><span data-stu-id="eabbb-251">In typical scenarios, it's likely that the data for a custom field in the header section will be pulled from the TSTimesheetHeader table.</span></span> <span data-ttu-id="eabbb-252">Hala ere, beste taula batzuk erabil daitezke datuak ematen diren TSTimesheetTable erregistro batean oinarrituta berreskuratu daitezkeenean edo erregistro testuinguru zehatzik ez badute (adibidez, eremua proiektuaren parametroetan irakurtzeko soilik ezarri bada) .</span><span class="sxs-lookup"><span data-stu-id="eabbb-252">However, other tables can be used if the data can be retrieved based on a TSTimesheetTable record that is provided, or if it doesn't have specific record context (for example, if the field is set as read-only in the project parameters).</span></span>

<span data-ttu-id="eabbb-253">Kontuan izan eremu pertsonalizatuek ez dutela zertan babeskopia datu baserik izan.</span><span class="sxs-lookup"><span data-stu-id="eabbb-253">Note that custom fields don't have to have any backing database records.</span></span> <span data-ttu-id="eabbb-254">Dinamikoki sor daitezke X ++ logikan oinarrituta.</span><span class="sxs-lookup"><span data-stu-id="eabbb-254">They can be dynamically generated based on X++ logic.</span></span> <span data-ttu-id="eabbb-255">Ondoren datorren adibideak ikuspegi hau erakusten du.</span><span class="sxs-lookup"><span data-stu-id="eabbb-255">The example that follows shows this approach.</span></span>

<span data-ttu-id="eabbb-256">Goiburuko ataleko eremuak beti irakurtzeko soilik dira aplikazioan.</span><span class="sxs-lookup"><span data-stu-id="eabbb-256">Fields in the header section are always read-only in the app.</span></span>

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-header-section"></a><span data-ttu-id="eabbb-257">Erabili komando katea TSTimesheetSettings klaseko buildCustomFieldList metodoan goiburuaren atalean eremua erakusteko</span><span class="sxs-lookup"><span data-stu-id="eabbb-257">Use chain of command on the buildCustomFieldList method of the TSTimesheetSettings class to show a field in the header section</span></span>

<span data-ttu-id="eabbb-258">Kode honek aplikazioaren eremuko pantailako ezarpenak kontrolatzen ditu.</span><span class="sxs-lookup"><span data-stu-id="eabbb-258">This code controls the display settings for the field in the app.</span></span> <span data-ttu-id="eabbb-259">Adibidez, kontrolatzen ditu eremu mota, etiketa, eremua derrigorrezkoa den eta eremua zein ataletan agertzen den.</span><span class="sxs-lookup"><span data-stu-id="eabbb-259">For example, it controls the type of field, the label, whether the field is mandatory, and what section the field appears in.</span></span>

<span data-ttu-id="eabbb-260">Hurrengo adibidean aplikazioko goiburuko atalean kalkulatutako balioa erakusten da.</span><span class="sxs-lookup"><span data-stu-id="eabbb-260">The following example shows a computed value in the header section in the app.</span></span>

```xpp
...
[ExtensionOf(classStr(TsTimesheetSettings))]
final class TSTimesheetSettings_Extension
{
    protected List buildCustomFieldList()
    {
        List customFieldList = next buildCustomFieldList();
        TSTimesheetCustomField tsTimesheetCustomField;

        */ Computed utilization rate*/
        tsTimesheetCustomField = new TSTimesheetCustomField();
        tsTimesheetCustomField.parmFieldBaseType(Types::Real);
        tsTimesheetCustomField.parmLabel("Utilization rate of this timesheet (computed
        custom field)");
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Header);
        tsTimesheetCustomField.parmOrderSequence(2);
        tsTimesheetCustomField.parmNumberOfDecimals(3);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforheader-method-of-the-tstimesheetdetails-class-to-fill-in-timesheet-details"></a><span data-ttu-id="eabbb-261">Erabili katearen komandoa buildCustomFieldListForHeader metodoa TSTimesheetDetails klasea betetzeko lan-orduen xehetasunak</span><span class="sxs-lookup"><span data-stu-id="eabbb-261">Use chain of command on the buildCustomFieldListForHeader method of the TSTimesheetDetails class to fill in timesheet details</span></span>

<span data-ttu-id="eabbb-262">**buildCustomFieldListForHeader** metodoa mugikorretarako aplikazioan ordu-orrien goiburuko xehetasunak betetzeko erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="eabbb-262">The **buildCustomFieldListForHeader** method is used to fill in the timesheet header details in the mobile app.</span></span> <span data-ttu-id="eabbb-263">Parametro gisa TSTimesheetTable erregistroa hartzen du.</span><span class="sxs-lookup"><span data-stu-id="eabbb-263">It takes a TSTimesheetTable record as a parameter.</span></span> <span data-ttu-id="eabbb-264">Erregistro horretako eremuak aplikazioko eremu pertsonalizatuko balioa betetzeko erabil daitezke.</span><span class="sxs-lookup"><span data-stu-id="eabbb-264">Fields from that record can be used to fill in the custom field value in the app.</span></span> <span data-ttu-id="eabbb-265">Hurrengo adibidean ez da datu baseko baliorik irakurtzen.</span><span class="sxs-lookup"><span data-stu-id="eabbb-265">The following example doesn't read any values from the database.</span></span> <span data-ttu-id="eabbb-266">Horren ordez, X ++ logika erabiltzen du aplikazioan agertzen den balio kalkulatu bat sortzeko.</span><span class="sxs-lookup"><span data-stu-id="eabbb-266">Instead, it uses X++ logic to generate a computed value that is then shown in the app.</span></span>


```xpp
...
[ExtensionOf(classStr(TSTimesheetDetails))]
final class TSTimesheetDetails_Extension
{
    protected List buildCustomFieldListForHeader(TSTimesheetTable
    _tsTimesheetTable)
    {
        List customFieldList = next buildCustomFieldListForHeader(_tsTimesheetTable);
        TSTimesheetCustomField tsTimesheetCustomField;

        */ Computed utilization rate*/
        tsTimesheetCustomField = new TSTimesheetCustomField();
        tsTimesheetCustomField.parmFieldBaseType(Types::Real);
        tsTimesheetCustomField.parmLabel("Utilization rate of this timesheet (computed
        custom field)");
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Header);
        tsTimesheetCustomField.parmOrderSequence(2);
        tsTimesheetCustomField.parmNumberOfDecimals(3);
        real utilizationRate = 0;
        if (_tsTimesheetTable.totalHours() != 0)
        {
            utilizationRate = _tsTimesheetTable.totalHoursBillable() /
            _tsTimesheetTable.totalHours();
        }
        tsTimesheetCustomField.parmRealValue(utilizationRate);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

## <a name="other-configurabilityextensibility-opportunities"></a><span data-ttu-id="eabbb-267">Beste konfiguragarritasun / hedagarritasun aukera batzuk</span><span class="sxs-lookup"><span data-stu-id="eabbb-267">Other configurability/extensibility opportunities</span></span>

### <a name="adding-additional-validation-for-the-app"></a><span data-ttu-id="eabbb-268">Aplikazioaren balioztapen gehigarria gehitzen</span><span class="sxs-lookup"><span data-stu-id="eabbb-268">Adding additional validation for the app</span></span>

<span data-ttu-id="eabbb-269">Datu-base mailan denbora-orrien funtzionaltasunerako dagoen logikak espero bezala funtzionatuko du.</span><span class="sxs-lookup"><span data-stu-id="eabbb-269">Existing logic for timesheet functionality at the database level will still work as expected.</span></span> <span data-ttu-id="eabbb-270">Gorde edo bidali eragiketak amaitu eta errore mezu zehatz bat erakusteko, gehitu dezakezu **bota errorea ("mezua erabiltzaileari")** kodera komando luzapen kate baten bidez.</span><span class="sxs-lookup"><span data-stu-id="eabbb-270">To interrupt the completion of save or submit operations and show a specific error message, you can add **throw error("message to user")** to the code via a chain of command extension.</span></span> <span data-ttu-id="eabbb-271">Hona hemen metodo luzagarri erabilgarrien hiru adibide:</span><span class="sxs-lookup"><span data-stu-id="eabbb-271">Here are three examples of useful extensible methods:</span></span>

- <span data-ttu-id="eabbb-272">Bada **validateWrite** TSTimesheetLine taulan itzultzen da **faltsua** denbora-orrialde bat gordetzeko eragiketan, errore-mezu bat agertzen da mugikorretarako aplikazioan.</span><span class="sxs-lookup"><span data-stu-id="eabbb-272">If **validateWrite** on the TSTimesheetLine table returns **false** during a save operation for a timesheet line, an error message is shown in the mobile app.</span></span>
- <span data-ttu-id="eabbb-273">Bada **validateSubmit** TSTimesheetTable taulan itzultzen da **faltsua** denbora-orrialde bat bidalketa aplikazioan, errore-mezu bat agertzen da erabiltzaileari.</span><span class="sxs-lookup"><span data-stu-id="eabbb-273">If **validateSubmit** on the TSTimesheetTable table returns **false** during timesheet submission in the app, an error message is shown to the user.</span></span>
- <span data-ttu-id="eabbb-274">Eremuak betetzen dituen logika (adibidez, **Linearen jabetza**) zehar **txertatu** TSTimesheetLine taulako metodoa oraindik exekutatuko da.</span><span class="sxs-lookup"><span data-stu-id="eabbb-274">Logic that fills in fields (for example, **Line Property**) during the **insert** method on the TSTimesheetLine table will still run.</span></span>

### <a name="hiding-and-marking-out-of-box-fields-as-read-only-via-configuration"></a><span data-ttu-id="eabbb-275">Kutxaz kanpoko eremuak ezkutatu eta markatu konfigurazioaren bidez irakurtzeko soilik</span><span class="sxs-lookup"><span data-stu-id="eabbb-275">Hiding and marking out-of-box fields as read-only via configuration</span></span>

<span data-ttu-id="eabbb-276">Proiektuaren parametroetatik, kutxaz kanpoko eremuak irakurtzeko soilik edo mugikorreko aplikazioan ezkutatuta egin ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="eabbb-276">From the project parameters, you can make out-of-box fields read-only or hidden in the mobile app.</span></span> <span data-ttu-id="eabbb-277">Ezarri aukerak **Mugikorreko orriak** atala **Denbora-orria** fitxategiaren fitxa **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="eabbb-277">Set the options in the **Mobile timesheets** section on the **Timesheet** tab of the **Project management and accounting parameters** page.</span></span>

![Proiektuaren parametroak](media/5753b8ecccd1d8bb2b002dd538b3f762.png)

### <a name="changing-the-activities-that-are-available-for-selection-via-extensions"></a><span data-ttu-id="eabbb-279">Aukeratzeko dauden jarduerak luzapenen bidez aldatzea</span><span class="sxs-lookup"><span data-stu-id="eabbb-279">Changing the activities that are available for selection via extensions</span></span>

<span data-ttu-id="eabbb-280">Proiektu baterako hautatzeko dauden jarduerak webgunearen bidez betetzen dira **getActivitiesForProject()** eta **getActivityQuery()** metodoan **TsTimesheetProjectService** klasea.</span><span class="sxs-lookup"><span data-stu-id="eabbb-280">The activities that are available for selection for a project are filled in via the **getActivitiesForProject()** and **getActivityQuery()** methods in the **TsTimesheetProjectService** class.</span></span> <span data-ttu-id="eabbb-281">Komando katea erabil dezakezu jokaera hau aldatzeko, zure negozio eszenatokiarekin bat etor dadin proiektu zehatz baterako hautatzeko erabilgarri dauden jardueretarako.</span><span class="sxs-lookup"><span data-stu-id="eabbb-281">You can use chain of command to change this behavior to match your business scenario for the activities that are available for selection for a specific project.</span></span>

### <a name="entering-a-default-project-category-on-timesheet-entries"></a><span data-ttu-id="eabbb-282">Denbora-orriaren sarreretan proiektuaren kategoria lehenetsia sartzea</span><span class="sxs-lookup"><span data-stu-id="eabbb-282">Entering a default project category on timesheet entries</span></span>

<span data-ttu-id="eabbb-283">Denbora-orrien sarreretan proiektuaren kategoria lehenetsia sartzea hiru mailatan gertatzen da.</span><span class="sxs-lookup"><span data-stu-id="eabbb-283">Entry of a default project category on timesheet entries occurs at three levels.</span></span> <span data-ttu-id="eabbb-284">Komando katea erabil dezakezu portaera maila horietako guztietan edo guztietan hedatzeko nahi duzun portaera lortzeko.</span><span class="sxs-lookup"><span data-stu-id="eabbb-284">You can use chain of command to extend the behavior at any or all of these levels to achieve the desired behavior.</span></span> <span data-ttu-id="eabbb-285">Ondorengo hierarkia erabiltzen da:</span><span class="sxs-lookup"><span data-stu-id="eabbb-285">The following hierarchy is used:</span></span>

1. <span data-ttu-id="eabbb-286">Aplikazioa proiektuaren baliabidetik kategoria lehenetsia jartzen saiatzen da.</span><span class="sxs-lookup"><span data-stu-id="eabbb-286">The app tries to put the default category from the project resource.</span></span> <span data-ttu-id="eabbb-287">Kategoria lehenetsi hau **getCurrentUserResource** eta **getDelegatedResourcesForCurrentUser** metodoan **TSTimesheetSettingsService** klasea.</span><span class="sxs-lookup"><span data-stu-id="eabbb-287">This default category is set in the **getCurrentUserResource** and **getDelegatedResourcesForCurrentUser** methods in the **TSTimesheetSettingsService** class.</span></span>
2. <span data-ttu-id="eabbb-288">Kategoria lehenetsia proiektuaren baliabide mailan ematen ez bada, aplikazioa proiektuaren jardueratik ateratzen saiatuko da.</span><span class="sxs-lookup"><span data-stu-id="eabbb-288">If the default category isn't provided at the project resource level, the app tries to pull it from the project activity.</span></span> <span data-ttu-id="eabbb-289">Kategoria lehenetsi hau **getActivitiesForProject** metodoa **TSTimesheetProjectService** klasea.</span><span class="sxs-lookup"><span data-stu-id="eabbb-289">This default category is set in the **getActivitiesForProject** method in the **TSTimesheetProjectService** class.</span></span>
3. <span data-ttu-id="eabbb-290">Kategoria lehenetsia proiektuaren jarduera mailan ematen ez bada, lehenetsitako kategoria aterako da proiektuaren parametroetatik.</span><span class="sxs-lookup"><span data-stu-id="eabbb-290">If the default category isn't provided at the project activity level, the default category it taken from the project parameters.</span></span> <span data-ttu-id="eabbb-291">Kategoria lehenetsi hau **getProjectDetailsbyRule** metodoa **TSTimesheetProjectService** klasea.</span><span class="sxs-lookup"><span data-stu-id="eabbb-291">This default category is set in the **getProjectDetailsbyRule** method in the **TSTimesheetProjectService** class.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]