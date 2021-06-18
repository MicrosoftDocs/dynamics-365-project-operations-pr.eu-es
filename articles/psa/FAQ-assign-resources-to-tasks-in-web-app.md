---
title: Nola esleitzen da baliabide erreserbagarria zeregin bati web aplikazioan
description: Baliabide erreserbagarriak esleitzeko moduen ikuspegi orokorra.
author: JohnPBurrows
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 32a04ddef901515cd77262b5ae6be2458cb6b00c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993268"
---
# <a name="how-do-i-assign-a-bookable-resource-to-a-task-in-the-web-app-project-service-app-v2x"></a>Nola eslei daiteke baliabide erreserbagarri bat zeregin bati web-aplikazioan (Project Service aplikazioa v2.x)?

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1.x-2.x](../includes/cc-applies-to-psa-app-1x-2x.md)]

Baliabide bat bi modutan eslei daiteke Project Service-n. Baliabide taldearen kide gisa erreserbatutako eta ondoren, zeregin bat esleitu. Bestela, duzu sor dezakezu funtzio-zeregin bidez orokorra taldearen kide zereginekin lan, talde bat sortu eta, ondoren, egin named baliabidearekin backing eskakizunak.

Kontutan izan dela nahi duzun baliabidea bookable zeregin bat esleitu, bookable baliabide taldeko kide izan behar bookings nahikoa erabilgarri. Egoera-erreserbatu Commit Mota Disko Liburua eta Committed Egoera izan behar du. Baliabidearen erreserba nahikoa ez badaude, Project Service-k esleipena kendu eta errore-mezu hau bistaratzen du:

*Ezin da esleitu baliabidea zereginean - Baliabide hauek ez dute nahikoa ordu erreserbatuta proiektuan*

## <a name="book-a-resource-as-a-team-member-and-then-assign-the-resource-to-a-task"></a>Erreserbatu baliabidea taldearen kide gisa eta esleitu baliabidea zereginari

Metodo honekin proiektua taldeari baliabide bat gehitu aurkitzea esleitu zereginak, baliabideak antolaketan proiektua. Hemen da hori egiteko modua:
1.  Saretan taldearen kide, gehitu taldeko kide berria hautatuta **Berria**.
2.  Taldearen Kide Sortze Bizkorren pantailan, hautatu baliabide bookable izena eta funtzio bat ezarri.
3.  Hautatu **Noiztik** eta **Noiz arte** datak.

    > [!div class="mx-imgBorder"] 
    > ![Taldekidea gehitzeko pantaila-argazkia](media/FAQ-Resources-to-Tasks2-1.png "Taldekidea gehitzeko pantaila-argazkia")
 
4.  Hautatu booking baliabidea-kopuruan metodoak ondorengo aukeretako bat:
    - **Gaitasun osoa** aukerarekin baliabidearen ahalmena osoa zehaztutako liburu batetik eta data.
    - **Ehunekoaren gaitasuna** aukerak baliabidearen ahalmenaren ehuneko batean erreserbatzen du baliabidea zehaztutako daten artean.
    - **Orduak berdin banatuta** aukerak epe jakin batean ordu, zehaztutako, igaro uniformeki egunaren ordua banatzen baliabidea books batetik eta data.
    - **Aurreikusitako orduaren arabera** ordu jakin baterako erreserbatzen du baliabidea, egunean ordu jakin batzuk zehaztutako datetan.

    Ez hautatu **Bat ere ez** baliabidea taldean gehitzen duelako, baina ez du sortzen edozein bookings absorb baliabidearen ahalmena.
5.  Hautatu **Gorde**.

    Kontuan hartu erreserbatu-orduak azal-ahalegina ordu eta baliabide hau esleitu zeregin data-barruti nahikoa izan behar. Horiek ez lerrokatzea aplikazioan, ezin diozu baliabidea zeregina.

6.  Lan egin diren kanpaina-xehatzea egitura (WBS) zereginaren, sakatu baliabidea gelaxka goitibeherako. Orduan: 

    1. Hautatu **Gehitu**.
    2. Hautatu ataleko goitibeherako **Baliabideak** eta gaineko gehitu taldeko kide hautatzeko.
    3. Hautatu **Ados**. Taldeko kide orain den esleitutako zeregina.

    > [!div class="mx-imgBorder"] 
    > ![WBSekin baliabideak gehitzeko pantaila-argazkia](media/FAQ-Resources-to-Tasks2-2.png "WBSekin baliabideak gehitzeko pantaila-argazkia")
 
Taldearen kide saretan, ikusiko duzu baliabideen agregatuen esleitutako Esleitutako Ordu atalean ordu. Izango da, baliabide-booked ordu berdina edo txikiagoa. 

> [!div class="mx-imgBorder"] 
> ![Baliabide bati esleitutako orduen pantaila-argazkia](media/FAQ-Resources-to-Tasks2-3.png "Baliabide bati esleitutako orduen pantaila-argazkia")
 
Baliabidea esleitzen saiatzen ari zara zeregina abiarazten baliabideak bookings amaiera-data ondoren, baliabidea ez agertuko-barrako goitibeheran.

Kontutan izan ditzakezu esleitzea baliabide beren booked ordu baino gehiago ordu baliabidea esleitu gabeko ahalmena gelditzen diren zenbait badu. Kasu honetan, baliabide soilik partzialki esleituko bookings beren gehienez. Esleitu gabeko zeregin ordu gainerako horiek lan diren kanpaina-xehatzea egitura Unstaffed Ordu zutabe gehituz ikus dezakezu.

Baliabideak ordu booked beren esleitzen baduzu (beren booked ordu berdina da ordu esleitutako beren), eslei diezazkiekezu are gehiago zereginak saiatzean hurrengo errore-mezua ikusiko duzu:

*Ezin da esleitu baliabidea zereginean - Baliabide hauek ez dute nahikoa ordu erreserbatuta proiektuan.*

Gainera, lehenetsia proiektua kudeatzailea taldearen kide proiektuan sortzean taldeari gehitutako bookings edozein gabe gehituko da eta ezin zaizkie objektuak esleitu zeregin guztiak. Horiek ez erakutsi, baliabide-barrako goitibeheran zereginetarako.

Baliabide hau esleitu nahi badituzu, talde batetik ezaba eta, ondoren, berriro gehitzeko bat Ere ez guztirako baldintza kopuruak metodo bat beharko duzu. Xede proiektuaren lehenespenez proiektua approver gutxienez da daitezen da duten ari taldera gehitu, proiektuan sortzen denean arrazoia.

## <a name="create-a-generic-team-member-through-role-assignment-on-tasks"></a>Funtzio-zeregin bidez orokorra taldearen kide zereginekin lan sortu

Metodo hori assures baliabide-dituzte zereginak bookings nahikoa. Lehenik eta behin, sortu leku-marka edo ultimately zereginak lantzeko zereginak funtzio esleituz ondoren talde bat sortzen du nahi duzun baliabidea named ezaugarri deskribatzen duen baliabide orokorra. Hemen da hori egiteko modua:

1. Lan egin diren kanpaina-xehatzea egitura, hautatu zeregin bat.
2. Hautatu **Esleitu Funtzioa** baliabide gelaxka goitibeherako ikonoa.
3. Hautatu **Funtzioa** goitibeherako eta orokorra baliabide funtzioa hautatzeko.
4. Hautatu **Ados**.

    > [!div class="mx-imgBorder"] 
    > ![WBS erabiliz baliabidea gehitzeko pantaila-argazkia](media/FAQ-Resources-to-Tasks2-4.png "WBS erabiliz baliabidea gehitzeko pantaila-argazkia")
 
Administrazio-funtzioak, WBS zereginak osatu dituzunean, hautatu **Sortu proiektu-taldea**. Project Service-k orokorra taldekideak oinarrituta-funtzioak, resourcing erakundearen unitateak eta proiektua egutegi zeregina esleipenetan aggregating arabera kopurua gutxieneko sortzen du.

> [!div class="mx-imgBorder"] 
> ![Proiektuaren taldea sortzeko pantaila-argazkia](media/FAQ-Resources-to-Tasks2-5.png "Proiektuaren taldea sortzeko pantaila-argazkia")
 
Taldeko Kide saretan, ikusiko duzu baliabide-funtzioak eta posizio izen Orokorra Baliabide mota. Baliabideak bi ditu-funtzio bat behar diren, Sortu Taldearen eginbidea bi taldekideak sortzen du eta apart ezarri posizioaren izena erabiltzen.

> [!div class="mx-imgBorder"] 
> ![Bi baliabide generiko gehitzeko pantaila-argazkia](media/FAQ-Resources-to-Tasks2-6.png "Bi baliabide generiko gehitzeko pantaila-argazkia")
 
Baliabide Eskakizun atalean esteka hautatuta backing baliabide eskakizun orokorra taldearen kide ireki dezakezu.

> [!div class="mx-imgBorder"] 
> ![Ordezko baliabide-eskakizunak irekitzearen pantaila-argazkia](media/FAQ-Resources-to-Tasks2-7.png "Ordezko baliabide-eskakizunak irekitzearen pantaila-argazkia")

Hautatu **Erreserbatu** orokorra baliabidea, eta, ondoren, erabil dezakezu antolaketa board bilaketa eta erreserbatutako benetako baliabide. Baliabide kudeatzailea arabera betetze-eskakizun hautatuta bidali dezakezu ere **Eskatzeko Bidali**.

Baliabidea orokorra baliabide named beteta dagoenean, orokorra baliabide-taldetik kendu eta orokorra baliabide esleitutako zeregina orokorra baliabide baliabide eskakizun beteta baliabidea named esleitzen zaizkio.
 



[!INCLUDE[footer-include](../includes/footer-banner.md)]