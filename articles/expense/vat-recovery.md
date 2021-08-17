---
title: BEZaren berreskurapena Gastuen kudeaketan
description: Gai honek balio erantsiaren gaineko zergaren (BEZ) transakzioetan itzulketak nola jaso azaltzen du.
author: suvaidya
ms.date: 10/10/2020
ms.topic: article
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 64e9f4091fdf40cc702e83a165fe0a5be5043359348210bbe4afcd8a18055133
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6999346"
---
# <a name="vat-recovery-in-expense-management"></a>BEZaren berreskurapena Gastuen kudeaketan

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Balio erantsiaren gaineko Zergaren (BEZ) transakzioen itzulketak jasotzeko, enpresa edo erakunde batek informazio zehatza identifikatu, bildu, egiaztatu eta bidali behar du. Prozesu honek hainbat zeregin biltzen ditu eta, zure enpresaren tamainaren arabera, hainbat langile edo eginkizun sar ditzake.

BEZa berreskuratzeko **Gastuen kudeaketa** modulua, baldintza hauek bete behar dira:

- Zerga kodeak sortu behar dira gastu kategorietara bideratutako herrialde / eskualdeetarako.
- Zerga kode bakoitzerako salmenten gaineko zerga taldea sortu behar da.
- Salmenten zerga-kode bakoitzerako elementuen salmenten gaineko zerga-kodea sortu behar da.

Aurrebaldintzak bete ondoren, urrats hauek bete behar dira BEZaren eragiketen itzulketak eskatzeko.

1. Gastuen txostenean, sartu kreditu txartelarekin egindako transakzioei buruzko zerga informazioa, BEZaren itzulketak hautatzeko.
2. Egiaztatu zerga informazio guztia osatuta dagoela eta, ondoren, bidali gastuen txostena.
3. Nazioarteko BEZa berreskuratzeko eskubidea duten prozesuak.
4. Bidali BEZa berreskuratzeko datuak hirugarren saltzaileari nazioarteko berreskurapenen aitorpenak aurkez ditzan.
5. Barne BEZa berreskuratzeko gastuak prozesatu.

Ondorengo ataletan nola erakusten duten adibideak ematen dira Contoso langileek urrats bakoitza osatzen dute.

## <a name="enter-tax-information-about-credit-card-transactions-to-identify-eligible-vat-refunds"></a>Sartu kreditu txartelarekin egindako transakzioei buruzko zerga informazioa, BEZaren itzulketak hautatzeko

Nancy, Contoso salmenten ordezkaria Estatu Batuetan kokatua, duela gutxi Erresuma Batura egindako salmenta bidaiatik itzuli da. Bidaian, Nancyk kreditu txartel pertsonaleko zenbait gastu egin zituen otorduetarako. Nancy-k gastuen txostena sortu behar du gastuak bateratzeko.

Nancyk gastuen txostenean informazioa sartzen duenean, hautatzen du **Erresuma Batua** **Herrialdea/Eskualdea** eremuan, **Editatu gastuen txostena** orrialdean. Salmenten gaineko zergen taldeen zerrenda iragazi egiten da, Erresuma Batuari aplikatzen zaizkion taldeak soilik erakuts ditzan. Nancy-k hautatzen du **Erresuma Batua 001** salmenten gaineko zerga taldea eta ondoren hautatu **Otorduak** elementuen salmenten gaineko zergaren taldea. Ondoren, Nancy-k transakzio berri bat gehituko du ostatu hartzeko. Erresuma Batuan ostatu hartzeko salmenten gaineko zerga talde bakarra eta salmenten gaineko zerga talde bakarra dagoenez, informazio hori automatikoki betetzen da Nancyren gastuen txostenean.

Contoso politikari dagokionez, gastu guztiek bat datorren ordainagiria izan behar dute. Hori dela eta, Nancyk gastuen txostena gordetzen duenean, mezu bat jasotzen du, bere gastuen txostenean zerrendatutako transakzio bakoitzaren ordainagiria erantsi behar duela dioena. Nancy-k egiaztatzen du transakzio ordainagiri bakoitzaren irudi digitala erantsi duela bere gastuen txostenean eta, ondoren, bere txostena onartzen du. Orduan, paperezko ordainagiriak atzeko bulegoko izapidetze taldeari bidaltzen dizkio. Talde honek BEZa berreskuratzeko datuak bidaliko dizkio nazioarteko BEZaren berreskurapena itzultzen duen hirugarren saltzaileari Contoso.

## <a name="verify-tax-information-and-post-an-expense-report"></a>Egiaztatu zerga informazioa eta bidali gastuen txostena

Apirila baino lehen, ordaindu beharreko kontuen koordinatzailea Contoso, gastuen txostena bidal dezake, falta zaion zerga informazioa sartu behar du. Ireki zuren **Gastuen txostenaren xehetasunak** orrialdean eta Nancyren onartutako gastuen txostena ikusten du. Ondoren, apirilak gastuen txostena irekitzen du transakzioen xehetasunak ikusteko. Ikusten du Nancyk ez zuela transakzioetako bat salmenten gaineko zerga talde batean sartu. Informazio hau ematen ez denez, apirilak ezin du gastuen txostena argitaratu. Hori dela eta, begiratzen dio **Zerga konfigurazioak** orria Gastuak kudeatzeko atalean, eta herrialdeko/eskualdeko eta transakzio motako elementu salmenten gaineko zerga talde egokia aurkitzen du. Apirilak gastuen txostena liburu nagusian bidali dezake.

Apirilak gastuen txostena argitaratzen duenean, BEZa berreskura daitekeen lan-elementu bat sortzen da. Lan-elementu hau atzeko bulegoko izapidetze taldeko kide bati esleitzen zaio. Apirilak mezu bat jaso zuela mezu bat jaso zuen. Mezu honetan berreskuratzeko identifikatu ziren BEZaren transakzio kopurua ere agertzen da.

## <a name="process-expenses-that-are-eligible-for-international-vat-recovery"></a>Nazioarteko BEZa berreskuratzeko eskubidea duten prozesuak

Arnie, bertako kidea Contoso back-office prozesatzeko taldea, BEZa berreskuratzeko beharrezko informazio guztia gastuen txostenetan sartuta dagoela egiaztatzeaz arduratzen da. Zabaltzen du **Gastuen zerga berreskuratzea** orrialdean eta Nancyk bidalitako gastuen txostena hautatzen du. Arniek egiaztatzen du eskatutako ordainagiri guztiak erantsita daudela eta salmenten gaineko zergaren talde zuzena eta salmenten gaineko zergaren kodeak sartu direla.

Arniek Nancyren paperezko ordainagiriak jasotzen dituenean, egiaztagiri digitalen aurka egiaztatzen ditu eta, ondoren, gastuen txostenaren egoera aldatzen du **Berreskuratzeko prest**.

## <a name="send-vat-recovery-data-to-the-third-party-vendor"></a>Bidali BEZa berreskuratzeko datuak hirugarren saltzaileari

Arnie BEZa berreskuratzeko aitorpena aurkeztuko duen hirugarren saltzaileari gastuen txostenaren datuak bidaltzeko prest dagoenean, **Gastuen zerga berreskuratzea** orrialdea. Orrialdea iragazi egiten du, horrela markatuta dauden gastuen txostenak soilik erakutsi ditzan **Sendatzeko prest**. Arniek orduan hautatzen du **Fitxategia** &gt; **Esportatu Excel-era**. Gastu txostenetako BEZ informazioa a-ra esportatzen da Microsoft Excel lan orria. Arnie-k lan-orri hau hirugarren saltzaileari bidaltzen dio eta paperezko ordainagiriak mezularitza bidez bidali direla dioen mezu bat dakar.

## <a name="process-expenses-for-domestic-vat-recovery"></a>Barne BEZa berreskuratzeko gastuak prozesatu

Arniek egiaztatu behar du gastuen txostenen transakzioak BEZa berreskuratzeko modukoak direla, eta ordainagiri digitalak txostenetara erantsita daudela. Etxean berreskuratzeko hautagarriak diren gastuak prozesatzen hasteko, Arnie-k irekitzen du **Gastuen zerga berreskuratzea** orrialdean eta egiaztatzea eskatzen duen gastuen txostena hautatzen du. Egiaztagiriak langilearen ordez enpresaren izenean daudela egiaztatzen du. (BEZa berreskuratzeko, ordainagiriak enpresaren izenekoak izan behar dira.) Arniek egiaztatzen du eskatutako ordainagiri guztiak erantsita daudela eta salmenten gaineko zergaren talde zuzena eta salmenten gaineko zergaren kodeak sartu direla.

Arniek paperezko ordainagiriak jasotzen dituenean, gastuen txostenaren egoera aldatzen du **Berreskuratzeko prest**. Ondoren, aitorpena dagokion zerga agintaritzan aurkeztu dezake. Kasu honetan, Estatu Batuetako zerga agintari egokia Internal Revenue Service (IRS) da.


[!INCLUDE[footer-include](../includes/footer-banner.md)]