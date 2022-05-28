---
title: Kudeatu diru-sarreren kalkuluak
description: Gai honek proiektuko diru-sarreren aurreikuspenekin lan egiteko moduari buruzko informazioa ematen du.
author: sigitac
ms.date: 11/04/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 6f91a0eb6fa0d13ebe8dfb6e837dae0bbff3eb5e
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8595851"
---
# <a name="manage-revenue-estimates"></a>Kudeatu diru-sarreren kalkuluak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Diru sarreren kalkuluak sortu, kalkulatu, argitaratu, alderantzikatu edo ezabatu ditzakezu. Hori eskuz edo aldian aldiko prozesua erabiliz egin dezakezu. Gai honek proiektuko diru-sarreren aurreikuspenekin lan egiteko moduari buruzko informazioa ematen du.

### <a name="manage-revenue-estimates-manually"></a>Kudeatu diru-sarreren kalkuluak eskuz

Prezio finkoko diru-sarreren aurrekontuaren proiektuan edo **Aurrekontuen kontsulta** orrialdea (**Proiektuen kudeaketa eta kontabilitatea** > **Txostenak eta kontsultak** > **Kontsultak eta txostenak kalkulatzen ditu**), hautatu **Aurrekontuak**.

### <a name="manage-revenue-estimates-using-a-periodic-process"></a>Kudeatu diru-sarreren kalkuluak aldian aldiko prozesu baten bidez

Joan **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkakoa** > **Aurrekontuak** eta hautatu dagokion prozesua.

## <a name="create-a-revenue-estimate"></a>Sortu diru-sarreren aurrekontua

Diru-sarreren kalkuluak egiteko, egin urrats hauek. 

1. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkakoa** > **Aurrekontuak** aukerara.
2. Hautatu **Berria**. **Sorkuntza kalkulatu** orrian, hautatu parametro hauek:

   - **Garai kodea**: Kode honek kalkuluak zenbat aldiz argitaratzen diren zehazten du.
   - **Aurreikusitako data**: Aurrekontua prozesatzen den eguna.
   - **Etengabea**: Hautatu kontrol lauki hau kalkuluak sortzeko aurreko aldian kalkuluak egin badira edo estimazioa sortu den lehen kalkulua bada. Aukeratzen ez bada, estimazioak aurreko aldian argitaratu ez badira ere sortzen dira.
   - **Metodoa osatzeko kostua**: Definitu gainerako proiektuaren lana nola kalkulatu. Informazio gehiagorako, ikusi [Metodoak osatzeko kostua](cost-complete-methods.md).
   - **Osatze metodoa**: Aukeratu osatze metodo bat aukera hauetatik:
     - **Automatikoa**: Osatze ehunekoa automatikoki kalkulatzen da eta kalkuluan sartutako kostu lerroetan oinarritzen da. Kostuen txantiloiak sartzen diren kostu lerroak definitzen ditu.
     - **Eskuzkoa**: Osatze-ehunekoa azken kalkuluaren amaierako ehunekoa da. Aurrekontua sortu ondoren, aldatu dezakezu **Eskuzko kalkulua** **Aurrekontuak** orrialdean.
     - **Kostuen txantiloitik**: Metodo automatikoen eta eskuzkoen konbinazioa. Aukera hau automatikoki edo eskuz ezartzen da, kostu txantiloiaren balio lehenetsiaren arabera.
   - **Iragarpen eredua**: Aukeratu aurrekontuaren eredu bat.
   - **Inprimatu aurrekontuen zerrenda**: Sortu eta erakutsi aurrekontuen zerrenda. Zerrendan uneko funtzioaren egoera dago. Aurrekontuaren inguruko oharrak inprimatu ditzakezu txostenean. Ondorengo baldintzek ohartarazpenak estimazio zerrendan agertzea eragiten dute:
     - 100 ehuneko baino gehiagoko osaketa ehunekoa.
     - Ehuneko zero baino gutxiagoko osaketa ehunekoa.
     - Kopuru negatiboa **Osatzeko** zutabea.
     - Kontratuaren zenbatekoari dagokion aurrekontua.
     - Erantsitako kostuen aurrekonturik gabeko aurrekontua.
   - **Erakutsi Infolog**: Aukeratu aukera hau lana exekutatzean prozesatu ziren aurrekontu proiektuen inguruko informazioa jasotzen duen mezua jasotzeko.


## <a name="post-wip-or-accruals"></a>Bidali WIP edo metaketak

Estimazioak ebaluatu ondoren, mantendu, gutxitu edo handitu egiten dira. WIP mezua bidal dezakezu **Bukatutako kontratua** ebaluazio-printzipioa, edo metatu sortzapenekin lan egiten duzunean **Osatutako ehunekoa** ebaluazio printzipioa.
  
Aurreikusitako aldiaren egoera aldatu egiten da **Sortu** **Argitaratua** aukerara.

## <a name="reverse-wip-or-accruals"></a>Alderantzikatu WIP edo metaketak

Erabili alderantzizko aukera dagoeneko argitaratutako WIP edo metaketak kreditatzeko, eta ondoren sortu epealdirako estimazioak.

> [!NOTE]
> Beste aldi batzuen artean dagoen aldia alderantzikatzeko, alderantzikatu beharrezko estimazio aldiak eta berriro bidali. Ondorengo aldi guztiak aurreko aldiko kalkuluen araberakoak direnez, ez ezazu aldirik saltatu.

## <a name="eliminate-the-estimate-project-and-finish-the-project"></a>Ezabatu aurrekontuaren proiektua eta amaitu proiektua

Aurrekontuaren prozesuaren azken urratsa aurrekontuaren proiektua ezabatzea eta prezio finkoaren proiektua amaitzea da amaitzearen ehunekoa ehuneko 100era iristen denean.

Honako hau gertatzen da kanporaketa exekutatzean:

- Bukatutako kontratua duen prezio finkoarentzako, WIP balioak balantze kontuetatik atera eta irabazien eta galeren kontuetara garbitzen dira.
- Ehuneko osatua duen prezio finkoaren proiektuan, metaketa irabazien eta galeren kontuetatik kentzen da.

Estimazioak egoera aldatzen du **Ezabatuta**.

> [!NOTE]
> Kasu berezietan, ehunekoa ehuneko 100etik haratago hedatu daiteke. Hori gertatzen denean, murriztu osatze portzentajea erabiliz **Ezarri kostua zero metodoa osatzeko** ehuneko 100era iristeko.

## <a name="reverse-elimination"></a>Alderantzizko kanporaketa

1. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkakoa** > **Aurreikuspenak** > **Alderantzikazko konfigurazioa**. 
2. Ekintza panelean, **Prozesua** fitxan,**Mantendu** taldean, hautatu **Estimazioa**. 
3. Hautatu **Alderantzizko kanporaketa**.

Erabili orrialde hau aurrez zehaztutako data batekin eta aurrekontuaren egoerarekin ezabatze guztiak alderantzikatzeko **Ezabatuta**. Transakzioaren egoera aldatu egiten da eremu egokiak hautatu ondoren.

Honek ere automatikoki aldatzen du proiektuaren egoera **Prozesuan** proiektuaren etapa amaituta badago. Proiektuaren aldiaren aurrekontuaren egoera berriro aldatzen da **Argitaratua**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]