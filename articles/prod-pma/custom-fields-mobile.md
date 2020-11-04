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
ms.openlocfilehash: 1ea1ca002a8f68f86808831b398e452244471322
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071090"
---
# <a name="implement-custom-fields-for-the-microsoft-dynamics-365-project-timesheet-mobile-app-on-ios-and-android"></a>Ezarri eremu pertsonalizatuak Microsoft Dynamics 365 Project Timesheet mugikorretarako aplikazioa iOS eta Android

[!include [banner](../includes/banner.md)]

Gai honek luzapenak eremu pertsonalizatuak ezartzeko ohiko ereduak eskaintzen ditu. Honako gai hauek lantzen dira:

- Eremu pertsonalizatuko esparruak onartzen dituen hainbat datu mota
- Nola erakutsi irakurtzeko soilik edo editagarriak diren eremuak ordu-orriko sarreretan eta gorde erabiltzaileak emandako balioak datu-basean
- Nola erakutsi irakurtzeko soilik diren eremuak aldiz orriaren goiburuan
- Nola integratu beste negozio logika pertsonalizatu bat lehenetsitako balioak eremuetan sartzeko eta balioztapen osagarria egiteko

## <a name="audience"></a>Hartzaileak

Gai hau beren eremu pertsonalizatuak integratzen dituzten garatzaileentzat da Microsoft Dynamics 365 Project Timesheet Apple iOS eta eskuragarri dagoen mugikorretarako aplikazioa Google Android. Uste da irakurleek ezagutzen dituztela X ++ garapena eta proiektuaren denbora-orriaren funtzionalitatea.

## <a name="data-contract--tstimesheetcustomfield-x-class"></a>Datuen kontratua - TSTimesheetCustomField X ++ klasea

**TSTimesheetCustomField** class X ++ datu kontratuen klasea da, denbora-orriaren funtzionaltasunerako eremu pertsonalizatu bati buruzko informazioa adierazten duena. Eremu pertsonalizatuen objektuen zerrendak TSTimesheetDetails datuen kontratuan eta TSTimesheetEntry datuen kontratuan pasatzen dira mugikorretarako aplikazioan eremu pertsonalizatuak erakusteko.

- **TSTimesheetDetails** - Timesheet goiburuko kontratua.
- **TSTimesheetEntry** - Timesheet transakzio kontratua. Proiektuaren informazio bera duten objektu horien taldeak eta **timesheetLineRecId** balioa lerro bat osatzen dute.

### <a name="fieldbasetype-types"></a>fieldBaseType (motak)

**FieldBaseType** jabetzan **TsTimesheetCustom** objektuak aplikazioan agertzen den eremu mota zehazten du. Hurrengo **Motak** onartzen diren balioak.

| Moten balioa | Mota              | Oharrak |
|-------------|-------------------|-------|
| 0           | Katea (eta Enum) | Eremua testu-eremu gisa agertzen da. |
| 1           | Integer           | Balioa zenbaki hamartarrik gabeko zenbaki gisa erakusten da. |
| 2           | Erreala              | Balioa zenbaki hamartarrak dituen zenbaki gisa erakusten da.<p>Benetako balioa moneta gisa erakusteko aplikazioan, erabili **fieldExtenededType** jabetza. Erabil dezakezu **ZenbakiarenZenbakiak** propietatea erakusten diren hamartarren kopurua ezartzeko.</p> |
| 3           | Data              | Data formatuak erabiltzailearen arabera zehazten dira **Data, orduak eta zenbaki formatua** azpian zehazten den ezarpena **Hizkuntza eta herrialde / eskualde lehentasuna** urtean **Erabiltzailearen aukerak**. |
| 4           | Boolean           | |
| 15          | GUIDa              | |
| 16          | Int64             | |

- Bada **katea Aukerak** jabetza ez dago **TSTimesheetCustomField** objektua, testu libreko eremua eskaintzen zaio erabiltzaileari.

    **kateaLuzera** propietatea erabil daiteke erabiltzaileek sar dezaketen gehieneko kate luzera ezartzeko.

- Bada **katea Aukerak** jabetza helbidean ematen da **TSTimesheetCustomField** objektua, zerrendako elementu horiek erabiltzaileek aukera botoiak (irrati botoiak) erabiliz hautatu ditzaketen balio bakarrak dira.

    Kasu honetan, kate-eremuak zenbateko balio gisa joka dezake erabiltzailea sartzeko helburuarekin. Balioa datu-basean zenbaki gisa gordetzeko, eskuz mapatu katearen balioa enum balioarekin berriro datu basean gorde aurretik komando-katea erabiliz (ikus "Erabili komando-katea TSTimesheetEntryService klasean denbora-orriko sarrera bat gordetzeko aplikazioa datu-basera "atalean geroago gai honen adibide gisa).

### <a name="fieldextendedtype-tscustomfieldextendedtype"></a>fieldExtendedType (TSCustomFieldExtendedType)

Propietate hau erabil dezakezu benetako balioak moneta gisa formateatzeko. Ikuspegi hau **fieldBaseType** balioa da **Erreala**.

- **TSCustomFieldExtendedType:Bat ere ez** - Ez da formaturik aplikatzen.
- **TSCustomFieldExtendedType::Moneta** - Formatu balioa moneta gisa.

    Moneta formatua aktibo dagoenean, **kateaBalioa** eremuan aplikazioan erakutsi beharko litzatekeen moneta kodea gainditu daiteke. Balioa irakurtzeko soilik den balioa da.

    **benetakoBalioa** eremuak datu basean gorde behar den diru kopurua dauka.

### <a name="fieldsection-tscustomfieldsection"></a>fieldSection (TSCustomFieldSection)

Propietate hau erabil dezakezu eremu pertsonalizatuak aplikazioan non agertu behar duen zehazteko.

- **TSCustomFieldSection::Goiburua** - Eremua agertuko da **Ikusi xehetasun gehiago** ataleko aplikazioa. Eremu horiek irakurtzekoak dira bakarrik.
- **TSCustomFieldSection::Lerroa** - Eremua denbora-orriko sarreretan kutxaz kanpoko lerro-eremu guztien ondoren agertuko da. Eremu hauek editagarriak edo irakurtzeko soilik izan daitezke.

### <a name="fieldname-fieldnameshort"></a>fieldName (FieldNameShort)

Propietate honek eremua identifikatzen du aplikazioak ematen dituen balioak datu-basean gordetzen direnean.

### <a name="tablename-tablenameshort"></a>tableName (TableNameShort)

Propietate honek eremua identifikatzen du aplikazioak ematen dituen balioak datu-basean gordetzen direnean.

### <a name="iseditable-noyes"></a>isEditable (Ez Bai)

Ezarri propietate hau **Bai** zehazteko zehazteko denbora-orriko sarrera ataleko eremua erabiltzaileek editatu behar dutela. Ezarri propietatea **Ez** eremua irakurtzeko soilik egiteko.

### <a name="ismandatory-noyes"></a>Derrigorrezkoa da (Ez Bai)

Ezarri propietate hau **Bai** zehazteko zehazteko denbora-orriko sarrera ataleko eremua derrigorrezkoa izan behar luke.

### <a name="label-str"></a>Etiketa (str)

Propietate honek aplikazioaren eremuan ondoan agertzen den etiketa zehazten du.

### <a name="stringoptions-list-of-strings"></a>stringOptions (Kateen zerrenda)

Jabetza hau noiz aplikatu daiteke **fieldBaseType** ezarrita dago **Katea**. Bada **katea Aukerak** ezarrita dago, aukera-botoien bidez (irrati-botoiak) aukeratzeko dauden kateen balioak zerrendako kateek zehazten dituzte. Katerik ematen ez bada, kateen eremuan testu libreko sarrera onartzen da (ikusi "Erabili komando-katea TSTimesheetEntryService klasean aplikazioko datu-basera itzuli den denbora-orriko sarrera bat gordetzeko" atalean adibide bat lortzeko) .

### <a name="stringlength-int"></a>stringLength (int)

Propietate honek kate-eremu baten gehieneko luzera zehazten du. Aplikatu daiteke **fieldBaseType** ezarrita dago **Katea**.

### <a name="numberofdecimals-int"></a>kopuruaEzkenak (int)

Propietate honek eremu erreal baterako erakusten diren hamartarren kopurua zehazten du. Aplikatu daiteke **fieldBaseType** ezarrita dago **Erreala**.

### <a name="ordersequence-int"></a>orderSequence (int)

Propietate honek eremu pertsonalizatuak aplikazioan erakusteko ordena kontrolatzen du eremu pertsonalizatu bat baino gehiago zehazten direnean. Zenbaki txikiagoak dituzten eremuak agertzen dira lehenengo.

### <a name="booleanvalue-boolean"></a>booleanValue (boolearra)

Eremuetako **Boolearra** mota, propietate honek zerbitzariaren eta aplikazioaren arteko eremuko balio boolearra igarotzen du.

### <a name="guidvalue-guid"></a>guidValue (guid)

Eremuetako **GUID** mota, propietate honek zerbitzariaren eta aplikazioaren arteko eremuko balio globalki identifikatzaile bakarra (GUID) igarotzen du.

### <a name="int64value-int64"></a>int64Balioa (int64)

Eremuetako **Int64** mota, propietate honek zerbitzariaren eta aplikazioaren arteko eremuko balio int64 igarotzen du.

### <a name="intvalue-int"></a>intBalue (int)

Eremuetako **Int** mota, propietate honek zerbitzariaren eta aplikazioaren arteko eremuko balio int igarotzen du.

### <a name="realvalue-real"></a>benetakoBalioa (benetakoa)

Eremuetako **Erreala** mota, propietate honek zerbitzariaren eta aplikazioaren arteko eremuko balio erreala igarotzen du .

### <a name="stringvalue-str"></a>stringValue (str)

Eremuetako **Katea** mota, propietate honek zerbitzariaren eta aplikazioaren arteko eremuko balio katea igarotzen du. Eremuetako eremuetarako ere erabiltzen da **Erreala** moneta gisa formateatutako mota. Eremu horietarako, propietatea moneta kodea aplikaziora pasatzeko erabiltzen da.

### <a name="datevalue-date"></a>dateValue (data)

Eremuetako **Data** mota, propietate honek zerbitzariaren eta aplikazioaren arteko eremuko balio data igarotzen du.

## <a name="show-and-save-a-custom-field-in-the-timesheet-entry-section"></a>Erakutsi eta gorde eremu pertsonalizatua ordu-orriaren sarrera atalean

Jarraian, denbora-orriaren sarrera sortzeko mugikorretarako aplikazioaren pantaila-argazkia dago. Kutxaz kanpoko eremuak eta eremu pertsonalizatua erakusten ditu "Denbora sarrera" atalean "Proba katea" deiturikoa dagoeneko "Bigarren aukera" enum balioarekin.

![Probatu katea eremu pertsonalizatua aplikazioan](media/timesheet-entry.jpg)



Jarraian, "Probako katea" eremu pertsonalizaturako eskuragarri dauden enum aukeretako bat hautatzen duen erabiltzailearen mugikorretarako pantaila-argazkia dago.  Bi aukerak "Lehen aukera" eta "Bigarren aukera" dira botoi irudi gisa agertzen direnak. Une honetan bigarren aukera dago hautatuta.

![Aukera botoiak (irrati botoiak) Probako katea pertsonalizatutako eremurako](media/enum-option.jpg)



### <a name="extend-the-tstimesheetline-table-so-that-it-has-a-custom-field"></a>Zabaldu TSTimesheetLine taula pertsonalizatutako eremua izan dezan

Eszenatoki tipikoetan, litekeena da denbora-orriaren sarrera ataleko eremu pertsonalizatu baten datuak TSTimesheetLine taulan gordetzea. Hala ere, beste taula batzuk erabil daitezke datuak ematen diren TSTimesheetTrans erregistro batean oinarrituta berreskuratu daitezkeenean edo erregistro testuinguru zehatzik ez badute (adibidez, eremua proiektuaren parametroetan irakurtzeko soilik ezarri bada) .

Kontuan izan eremu pertsonalizatuek ez dutela zertan babeskopia datu baserik izan. Dinamikoki sor daitezke X ++ logikan oinarrituta. Ikuspegi hau erabilgarria izan daiteke irakurtzeko soilik diren eszenatokietan (ikus "Erabili komando-katea TSTimesheetDetails klasean, buildCustomFieldListForHeader metodoa denbora-orriaren xehetasunak betetzeko" atala, modu dinamikoan sortutako eremu pertsonalizatuen balioen adibidea lortzeko.)

Jarraian, pantaila-argazkia erakusten da Visual Studio Aplikazioaren Objektuen Zuhaitzaren. TSTimesheetLine taularen luzapena erakusten du TestLineString eremuak eremu pertsonalizatu gisa gehituta.

![Lerro katea](media/b6756b4a3fc5298093327a088a7710fd.png)

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-timesheet-entry-section"></a>Erabili komando katea TSTimesheetSettings klaseko buildCustomFieldList metodoan metodoa orriaren sarrera atalean eremua erakusteko

Kode honek aplikazioaren eremuko pantailako ezarpenak kontrolatzen ditu. Adibidez, kontrolatzen ditu eremu mota, etiketa, eremua derrigorrezkoa den eta eremua zein ataletan agertzen den.

Hurrengo adibidean denbora-sarreren kate-eremua erakusten da. Eremu honek bi aukera ditu, **Lehen aukera** eta **Bigarren aukera** , aukera botoien bidez (irrati botoiak) eskuragarri daudenak. Aplikazioko eremua **TestLineString** TSTimesheetLine taulan gehitzen den eremua.

Kontuan izan **TSTimesheetCustomField::newFromMetatdata()** eremu pertsonalizatuen propietateen hasiera errazteko metodoa: **fieldBaseType** , **taulaIzena** , **eremu izena** , **etiketa** , **editagarria da** , **derrigorrezkoa da** , **kateaLuzera** , eta **ZenbakiarenZenbakiak**. Parametro hauek eskuz ere ezar ditzakezu, nahi duzun moduan.

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

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforentry-method-of-the-tstimesheetentry-class-to-enter-values-in-a-timesheet-entry"></a>Erabili katearen komandoa buildCustomFieldListForEntry metodoa TSTimesheetEntry klasea sartzeko balioak lan-orduen sarrera

**buildCustomFieldListForEntry** metodoa mugikorretarako aplikazioan gordetako ordu-orrien lerroetan balioak sartzeko erabiltzen da. Parametro gisa TSTimesheetTrans erregistroa hartzen du. Erregistro horretako eremuak aplikazioko eremu pertsonalizatuko balioa betetzeko erabil daitezke.

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

### <a name="use-chain-of-command-on-the-tstimesheetentryservice-class-to-save-a-timesheet-entry-from-the-app-back-to-the-database"></a>Erabili komando-katea TSTimesheetEntryService klasean aplikazioko datu-orriko sarrera bat datu-basean gordetzeko

Eremu pertsonalizatua datu-basera ohiko erabileran gordetzeko, hainbat metodo luzatu behar dituzu:

- **timesheetLineNeedsUpdating** metodoa erabiltzen da erabiltzaileak lineako erregistroa aplikazioan aldatu duen edo ez eta datu basean gorde behar den zehazteko. Errendimendua kezka ez bada, metodo hau sinplifikatu egin daiteke, beti itzul dadin **egia**.
- **populateTimesheetLineFromEntryDuringCreate** eta **populateTimesheetLineFromEntryDuringUpdate** metodoak luza daitezke, ematen diren TSTimesheetLine datu-basearen erregistroan balioak sartu ditzaten. Ondorengo adibidean, ohartu nola datu basearen eremua eta sarrera eremua arteko mapak eskuz egiten diren X ++ kodearen bidez.
- **populateTimesheetWeekFromEntry** metodoa ere luza daiteke **TSTimesheetEntry** objektuak TSTimesheetLineweek datu basearen taulan idatzi behar du berriro.

> [!NOTE]
> Ondorengo adibideak gordetzen du **lehenAukera** edo **bigarrenAukera** erabiltzaileak datu basean hautatzen duen balioa kate gordinaren balio gisa. Datu-basearen eremua **Enum** mota, balio horiek eskuz mapatu daitezke enum balio batera eta ondoren gorde datu base taulako enum eremu batean.

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

## <a name="show-a-custom-field-in-the-timesheet-header-section"></a>Erakutsi eremu pertsonalizatua ordu-orriaren goiburuaren atalean

Jarraian, denbora-orria ikusteko erabiltzailearen mugikorretarako aplikazioaren pantaila-argazkia dago. "Informazio gehiago" botoia goiko eskuineko izkinan hautatu da "Ikusi xehetasun gehiago" aukera erakusteko.  

![Ikusi xehetasun gehiago komandoa](media/show-more.png)

Jarraian, denbora-orriaren "Gehiago" sekzioa erakutsiz mugikorretarako aplikazioaren pantaila-argazkia dago. "Orri honen erabilera-tasa (kalkulatutako eremu pertsonalizatua)" izeneko eremu pertsonalizatua gehitu da aldiz-orriaren goiburuko atalean. Irakurtzeko soilik den "0,667" balioa ezartzen da eremu pertsonalizatuan.

![Atal gehiago](media/more-section.jpg)

### <a name="extend-the-tstimesheettable-table-so-that-it-has-a-custom-field"></a>Zabaldu TSTimesheetTable taula pertsonalizatutako eremua izan dezan

Eszenatoki tipikoetan, litekeena da goiburuaren ataleko eremu pertsonalizatu baten datuak TSTimesheetHeader taulan ateratakoa. Hala ere, beste taula batzuk erabil daitezke datuak ematen diren TSTimesheetTable erregistro batean oinarrituta berreskuratu daitezkeenean edo erregistro testuinguru zehatzik ez badute (adibidez, eremua proiektuaren parametroetan irakurtzeko soilik ezarri bada) .

Kontuan izan eremu pertsonalizatuek ez dutela zertan babeskopia datu baserik izan. Dinamikoki sor daitezke X ++ logikan oinarrituta. Ondoren datorren adibideak ikuspegi hau erakusten du.

Goiburuko ataleko eremuak beti irakurtzeko soilik dira aplikazioan.

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-header-section"></a>Erabili komando katea TSTimesheetSettings klaseko buildCustomFieldList metodoan goiburuaren atalean eremua erakusteko

Kode honek aplikazioaren eremuko pantailako ezarpenak kontrolatzen ditu. Adibidez, kontrolatzen ditu eremu mota, etiketa, eremua derrigorrezkoa den eta eremua zein ataletan agertzen den.

Hurrengo adibidean aplikazioko goiburuko atalean kalkulatutako balioa erakusten da.

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

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforheader-method-of-the-tstimesheetdetails-class-to-fill-in-timesheet-details"></a>Erabili katearen komandoa buildCustomFieldListForHeader metodoa TSTimesheetDetails klasea betetzeko lan-orduen xehetasunak

**buildCustomFieldListForHeader** metodoa mugikorretarako aplikazioan ordu-orrien goiburuko xehetasunak betetzeko erabiltzen da. Parametro gisa TSTimesheetTable erregistroa hartzen du. Erregistro horretako eremuak aplikazioko eremu pertsonalizatuko balioa betetzeko erabil daitezke. Hurrengo adibidean ez da datu baseko baliorik irakurtzen. Horren ordez, X ++ logika erabiltzen du aplikazioan agertzen den balio kalkulatu bat sortzeko.


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

## <a name="other-configurabilityextensibility-opportunities"></a>Beste konfiguragarritasun / hedagarritasun aukera batzuk

### <a name="adding-additional-validation-for-the-app"></a>Aplikazioaren balioztapen gehigarria gehitzen

Datu-base mailan denbora-orrien funtzionaltasunerako dagoen logikak espero bezala funtzionatuko du. Gorde edo bidali eragiketak amaitu eta errore mezu zehatz bat erakusteko, gehitu dezakezu **bota errorea ("mezua erabiltzaileari")** kodera komando luzapen kate baten bidez. Hona hemen metodo luzagarri erabilgarrien hiru adibide:

- Bada **validateWrite** TSTimesheetLine taulan itzultzen da **faltsua** denbora-orrialde bat gordetzeko eragiketan, errore-mezu bat agertzen da mugikorretarako aplikazioan.
- Bada **validateSubmit** TSTimesheetTable taulan itzultzen da **faltsua** denbora-orrialde bat bidalketa aplikazioan, errore-mezu bat agertzen da erabiltzaileari.
- Eremuak betetzen dituen logika (adibidez, **Linearen jabetza** ) zehar **txertatu** TSTimesheetLine taulako metodoa oraindik exekutatuko da.

### <a name="hiding-and-marking-out-of-box-fields-as-read-only-via-configuration"></a>Kutxaz kanpoko eremuak ezkutatu eta markatu konfigurazioaren bidez irakurtzeko soilik

Proiektuaren parametroetatik, kutxaz kanpoko eremuak irakurtzeko soilik edo mugikorreko aplikazioan ezkutatuta egin ditzakezu. Ezarri aukerak **Mugikorreko orriak** atala **Denbora-orria** fitxategiaren fitxa **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea.

![Proiektuaren parametroak](media/5753b8ecccd1d8bb2b002dd538b3f762.png)

### <a name="changing-the-activities-that-are-available-for-selection-via-extensions"></a>Aukeratzeko dauden jarduerak luzapenen bidez aldatzea

Proiektu baterako hautatzeko dauden jarduerak webgunearen bidez betetzen dira **getActivitiesForProject()** eta **getActivityQuery()** metodoan **TsTimesheetProjectService** klasea. Komando katea erabil dezakezu jokaera hau aldatzeko, zure negozio eszenatokiarekin bat etor dadin proiektu zehatz baterako hautatzeko erabilgarri dauden jardueretarako.

### <a name="entering-a-default-project-category-on-timesheet-entries"></a>Denbora-orriaren sarreretan proiektuaren kategoria lehenetsia sartzea

Denbora-orrien sarreretan proiektuaren kategoria lehenetsia sartzea hiru mailatan gertatzen da. Komando katea erabil dezakezu portaera maila horietako guztietan edo guztietan hedatzeko nahi duzun portaera lortzeko. Ondorengo hierarkia erabiltzen da:

1. Aplikazioa proiektuaren baliabidetik kategoria lehenetsia jartzen saiatzen da. Kategoria lehenetsi hau **getCurrentUserResource** eta **getDelegatedResourcesForCurrentUser** metodoan **TSTimesheetSettingsService** klasea.
2. Kategoria lehenetsia proiektuaren baliabide mailan ematen ez bada, aplikazioa proiektuaren jardueratik ateratzen saiatuko da. Kategoria lehenetsi hau **getActivitiesForProject** metodoa **TSTimesheetProjectService** klasea.
3. Kategoria lehenetsia proiektuaren jarduera mailan ematen ez bada, lehenetsitako kategoria aterako da proiektuaren parametroetatik. Kategoria lehenetsi hau **getProjectDetailsbyRule** metodoa **TSTimesheetProjectService** klasea.
