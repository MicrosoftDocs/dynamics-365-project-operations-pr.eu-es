---
title: Berreskuratu onartutako denbora edo gastu-sarrerak
description: Gai honek aldez aurretik onartutako denbora edo gastu-transakzioa berreskuratzeari buruzko informazioa eskaintzen du.
author: rumant
ms.custom: ''
ms.author: rumant
ms.date: 03/08/2019
ms.topic: article
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 71f75c1c516ca6e652baf311aa14e0c3fd4ba81e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998171"
---
# <a name="recall-approved-time-or-expense-entries"></a>Berreskuratu onartutako denbora edo gastu-sarrerak

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Proiektuko taldekide batek edo denbora- edo gastu-sarrera bat bidaltzen duen beste pertsona batek denbora- edo gastu-sarrera hori berreskuratu dezake onartu ondoren. Onartutako denbora- edo gastu-sarrera berreskuratzeko prozesuak bi urrats ditu:

1. Igorleak berreskurapena eskatzen du.
2. Onartzaile batek berreskurapena onartzen du.

## <a name="request-a-recall"></a>Eskatu berreskurapena

Jarraitu urrats hauei onartutako denbora- edo gastu-sarrera berreskuratzeko.

1. Denbora-sarrerak lortzeko, joan **Proiektuak** \> **Nire lana** \> **Denbora-sarrera** atalera.

    –edo–

    Gastu-sarrerak lortzeko, joan **Proiektuak** \> **Nire lana** \> **Gastuak** atalera.

2. Denbora-sarrerak aukeratzeko, hautatu proiektu eta zeregin baten konbinazio zehatz baterako denbora-sarrera guztiak. Bestela, saretan, hautatu proiektu zehatz baterako data zehatz baten denboraren gelaxka indibidualak.

    –edo–

    Gastu-sarreretarako, hautatu berreskuratu nahi den gastu-sarreraren errenkada.

3. Hautatu **Berreskuratu**. Berresteko elkarrizketa-koadroa agertzen da. Hautatutako denbora- eta gastu-sarrerak dagoeneko onartuak baziren, berreskurapenaren zergatia idazteko eskatuko zaizu.
4. Idatzi berreskurapenerako arrazoia eta, ondoren, hautatu **Ados** eragiketa berresteko. Sistemak sarrerak berreskurapena onartzeko eskaera bidaltzen dio onartu dituen pertsonari.

> [!NOTE]
> Onartutako denbora- eta gastu-sarrerak berreskuratu daitezkeen arren, onartutako denbora edo gastua bezeroari fakturatu bazaio, ezin da sortu berreskuratze eskaerarik. Berreskuratze eskaera bat sortzen saiatzen den erabiltzaile batek denbora edo gastua ezin direla berreskuratu adierazten duen mezu bat jasoko du, jada fakturatu delako.

## <a name="approve-or-reject-a-recall-request"></a>Onartu edo baztertu berreskuratze eskaera

Jarraitu urrats hauei berreskuratze eskaera onartu edo arbuiatzeko.

1. Joan **Proiektuak** \> **Nire lana** \> **Onartutakoak** atalera.
2. **Onartutakoak** zerrenda-orrian, aldatu ikuspegia **Berreskuratu onartzeko eskaerak** egoerara. Bidalitako berreskuratze eskaeren zerrenda aurkezten da.
3. Hautatu sarrera bat edo gehiago eta, ondoren, hautatu **Onartu** edo **Baztertu**.
4. **Onartu** aukeratu baduzu, onarpenaren eragina azaltzen duen abisu-mezu bat jasoko duzu. Sakatu **Ados** eragiketa berresteko. Berreskuratze eskaera onartu da.

    –edo–

    **Baztertu** aukeratu baduzu, berreskuratze eskaera baztertu egingo da.

> [!NOTE]
> Berreskuratze eskaera bat egiten denean, berreskuratzea onartzen denean, sistemak denbora- edo gastu-sarreretan egondako fakturazio-jarduerak egiaztatzen ditu. Sarrera bat fakturatuta badago edo faktura zirriborro batean badago, onartzaileak denbora edo gastua berreskurapenerako onartu ezin direla dioen errore mezua jasoko du, dagoeneko fakturatuta zegoelako.

## <a name="impact-of-a-recall-request"></a>Berreskuratze eskaera baten eragina

Onarpena bat berreskuratzen denean, eragiketa-eragina eta finantza-eragina daude.

### <a name="operational-impact"></a>Eragile operazionala

Berreskuratze eskaera onartzen bada, onarpen-erregistroa **Baztertuta** gisa markatzen da. Sarreraren egoera aldatu egingo da **Itzulia** edo **Baztertuta** egoerara, denbora-sarrera edo gastu-sarrera den kontuan hartuta.

Proiektuko taldekideak sarrerak ikusi, sarrerak editatu eta berriro bidali edo sarrerak ezabatu ditzake.

Berreskuratze eskaera baztertzen bada, sarreraren egoera **Onartuta** gisa mantenduko da eta ez proiektuko taldekideak ,ez proiektuaren onartzaileak ezin du editatu sarrera.

### <a name="financial-impact"></a>Eragin ekonomikoa

Berreskuratze eskaera onartzen bada, kostuari eta salmentei dagozkien datu errealak era honetara eguneratzen dira:

- **Doikuntzaren egoera** eremua **Doituta** eremura eguneratzen da.
- **Fakturazio-egoera** eremua **Bertan behera utzita** eremura eguneratzen da.

Ondoren, itzulera-sarrerak Datu errealak taulan sortzen dira. Itzulera-sarrerak sortzeko, sistemak eremuko balioak baino gehiago kopiatzen ditu jatorrizko datu errealetatik. Kopiatzen ez diren balio bakarrak kantitatearen balioak dira. Horren ordez itzuli egiten dira balio horiek. Itzulitako datu errealak hauetarako sortzen dira: **Kostua** eta **Fakturatu gabeko salmentak**. Itzulitako datu errealetako **Egokitzearen egoera** eremua **Egokiezina** disa ezartzen da, eta **Fakturazio-egoera** eremua **Bertan behera utzita** gisa dago ezarrita. Aldaketa horiek direla eta, proiektuan erregistratutako gastuak eta diru-sarreren lanak ez dute gehiago azalduko datu erreal horiek adierazten dutena.

Berreskuratze eskaera baztertzen bada, ez dago eragin ekonomikorik proiektuan.

## <a name="changes-to-time-entry-records"></a>Denora-sarreraren erregistroen aldaketak

Hurrengo irudian, berreskuratzen direnean onartutako denbora-sarreretan gertatzen diren aldaketak erakusten dira.

![Denbora-sarreraren egoera trantsizioak](media/TimeEntryStateTransitions.png)

## <a name="changes-to-expense-entry-records"></a>Gastu-sarreraren erregistroen aldaketak

Hurrengo irudian, berreskuratzen direnean onartutako gastu-sarreretan gertatzen diren aldaketak erakusten dira.

![Gastu-sarreraren egoera trantsizioak](media/ExpenseEntryStateTransitions.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]